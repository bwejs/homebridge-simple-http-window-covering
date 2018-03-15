# homebridge-simple-http-window-covering

This Plugin is to Control a Window-Covering, that has only URL's for Open and Close.
When Running both URL's should stop the Covering.

HomeBridge: https://github.com/nfarina/homebridge

# Installation

1. Install homebridge using: npm install -g homebridge
2. Install homebridge-openwebif-switch using: npm install -g git+https://github.com/bwejs/homebridge-simple-http-window-covering.git
3. Update your configuration file. See sample-config.json in this repository for a sample.

# Configuration

 <pre>
"accessories": [
        {
            "accessory": "HTTP-Window-Covering",
            "name": "Covering",
            "open-URL": "http://192.168.1.1/open",
            "close-URL": "http://192.168.1.1/close",
  		      "valueMapping": {"closed" : 0 , "kind of closed": 30, "open" : 100},
        }
    ]
</pre>
optional settings written in italic font
