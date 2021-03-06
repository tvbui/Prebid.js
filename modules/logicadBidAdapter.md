# Overview
```
Module Name: Logicad for Publishers
Module Type: Bidder Adapter
Maintainer: prebid@so-netmedia.jp
```

# Description
Module that connects to Logicad's demand sources.
Currently module supports only banner mediaType.

# Test Parameters
```
var adUnits = [
  // Banner adUnit
  {
    code: 'test-code',
    sizes: [[300, 250], [300, 600]],
    mediaTypes: {
      banner: {
        sizes: [[300, 250], [300, 600]]
      }
    },
    bids: [{
      bidder: 'logicad',
      params: {
        tid: 'lfp-test-banner',
        page: 'url'
      }
    }]
  },
  // Native adUnit
  {
    code: 'test-native-code',
    sizes: [[1, 1]],
    mediaTypes: {
      native: {
        title: {
          required: true
        },
        image: {
          required: true
        },
        sponsoredBy: {
          required: true
        }
      }
    },
    bids: [{
      bidder: 'logicad',
      params: {
        tid: 'lfp-test-native',
        page: 'url'
      }
    }]
  }
];
```
