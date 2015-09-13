# Html5-multiply-sounds-manager
Lightweight javascript class(solution) to enable multiply html5 audio sound to be run in the same time.

Should work in modern html5 browsers including Iphone and Ipad Safari.

See it in action: 
http://kena23.cz/examples/Html5-multiply-sounds-manager/demo/


# USAGE

in html file include jquery.js and sound-manager.js

&lt;script&gt;

  //sounds can be turned on/off any time
  soundsManager.on = false; //turn sounds off
  soundsManager.on = true;  //turn sounds on

&lt;/script&gt;


add html audio tag with someName id attribut, smsound class and preload auto attributtes

 &lt;audio id="someName" class="smsound" preload="auto"&gt;

    <source src="sounds/Vinyl.ogg" type="audio/ogg">

    <source src="soundst/Vinyl.mp3" type="audio/mpeg">

    <source src="sounds/Vinyl.aac" type="audio/aac">

&lt;/audio&gt;

when document ready you can call

&lt;script&gt;

 $(function(){

     //can be called as many times as you wish in the same time 

     soundsManager.play('someName');

 });

&lt;/script&gt;




# LICENSE
MIT license


