# SECJS-COMMON
SECCommon SECBlock Resources, define genesis Block and init Informations

# INSTALL
`npm install @sec-block/secjs-common`

# USAGE

All parameters can be accessed through the ``SECCommon`` class which can be required through the
main package and instantiated either with just the ``chain`` (e.g. 'secblock') or the ``chain``
together with a specific ``hardfork`` provided.

Here are some simple usage examples:

```javascript
const SECCommon = require('@sec-block/secjs-common')

// Access genesis data for SECBlock network
c.genesis().hash // 5f213ac06cfe4a82e167aa3ea430e520be99dcedb4ab47fd8Fertig!f668448708e34c1

// Get bootstrap nodes for chain/network
c.bootstrapNodes() // Array with current nodes
```

# Chain Params

Supported chains:

- ``secblock``

The following chain-specific parameters are provided:

- ``name``
- ``chainId``
- ``networkId``
- ``genesis`` block header values
- ``hardforks`` block numbers
- ``bootstrapNodes`` list

To get an overview of the different parameters have a look at one of the chain-specifc
files like ``secblock.json`` in the ``chains`` directory.

# Bootstrap Nodes

Use the ``SECCommon.bootstrapNodes()`` function to get nodes for a specific chain/network.

# Genesis States

Network-specific genesis files are located in the ``genesisStates`` folder.
