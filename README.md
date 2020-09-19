# Hand.js library
HandJs library is a library for hand posture detection via a webcam.
More info: https://hand-js.com/

The library is **locked** against the localhost domain. If you want to use it on your page please contact: contact@hand-js.com


### Documentaion

The following code demonstrates the usage of the library. For complete sample, please take a look **Sample.html**.

    var handJS = new HandJS(action => 
    {
        if (action === 'HandDetected') 
           console.log('Hand detected :-)');
        else
           console.log('Hand lost :-(');
    });

    handJS.start()
          .catch(/* handle error */);
