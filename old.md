<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="2575.4">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 13.0px 'Helvetica Neue'}
    p.p2 {margin: 0.0px 0.0px 0.0px 0.0px; font: 13.0px 'Helvetica Neue'; min-height: 15.0px}
  </style>
</head>
<body>
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html lang="en"&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;meta charset="UTF-8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;title&gt;Retro Soundboard&lt;/title&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;style&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>* {</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-sizing: border-box;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin: 0;</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 0;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>body {</p>
<p class="p1"><span class="Apple-converted-space">      </span>height: 100vh;</p>
<p class="p1"><span class="Apple-converted-space">      </span>display: flex;</p>
<p class="p1"><span class="Apple-converted-space">      </span>justify-content: center;</p>
<p class="p1"><span class="Apple-converted-space">      </span>align-items: center;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: radial-gradient(circle, #2e2e2e 0%, #1b1b1b 100%);</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-family: 'Courier New', Courier, monospace;</p>
<p class="p1"><span class="Apple-converted-space">      </span>color: #fff;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.soundboard {</p>
<p class="p1"><span class="Apple-converted-space">      </span>display: grid;</p>
<p class="p1"><span class="Apple-converted-space">      </span>grid-template-columns: repeat(3, 1fr);</p>
<p class="p1"><span class="Apple-converted-space">      </span>gap: 30px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>max-width: 700px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>text-align: center;</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 40px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background-color: #333;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: 8px solid #111;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 16px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-shadow:</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 0 25px rgba(255, 0, 0, 0.5),</p>
<p class="p1"><span class="Apple-converted-space">        </span>inset 0 0 20px #000;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.button-group {</p>
<p class="p1"><span class="Apple-converted-space">      </span>display: flex;</p>
<p class="p1"><span class="Apple-converted-space">      </span>flex-direction: column;</p>
<p class="p1"><span class="Apple-converted-space">      </span>align-items: center;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.sound-button {</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 20px 40px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-size: 1.2rem;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-weight: bold;</p>
<p class="p1"><span class="Apple-converted-space">      </span>color: #fff;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: linear-gradient(to bottom, #c00, #800);</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: 4px solid #000;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 10px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>cursor: pointer;</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-shadow:</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 8px 0 #400,</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 12px 20px rgba(0, 0, 0, 0.6);</p>
<p class="p1"><span class="Apple-converted-space">      </span>transition: all 0.2s ease;</p>
<p class="p1"><span class="Apple-converted-space">      </span>width: 160px;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.sound-button:active {</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-shadow:</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 4px 0 #400,</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 6px 10px rgba(0, 0, 0, 0.6);</p>
<p class="p1"><span class="Apple-converted-space">      </span>transform: translateY(4px);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.sound-button:hover {</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: linear-gradient(to bottom, #f00, #900);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.upload-button {</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 7px 12px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-size: 0.85rem;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: linear-gradient(to bottom, #888, #444);</p>
<p class="p1"><span class="Apple-converted-space">      </span>color: #fff;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-weight: bold;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: 3px solid #111;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 6px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>cursor: pointer;</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-shadow:</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 4px 0 #111,</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 6px 10px rgba(0, 0, 0, 0.5);</p>
<p class="p1"><span class="Apple-converted-space">      </span>transition: all 0.2s ease;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin-bottom: 10px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>width: 70%;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.upload-button:active {</p>
<p class="p1"><span class="Apple-converted-space">      </span>box-shadow:</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 2px 0 #111,</p>
<p class="p1"><span class="Apple-converted-space">        </span>0 3px 5px rgba(0, 0, 0, 0.5);</p>
<p class="p1"><span class="Apple-converted-space">      </span>transform: translateY(2px);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.upload-button:hover {</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: linear-gradient(to bottom, #bbb, #666);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>input[type="file"] {</p>
<p class="p1"><span class="Apple-converted-space">      </span>display: none;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/style&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p1">&lt;body&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div class="soundboard"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- Create 9 button groups --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-1"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-1"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-1"&gt;Play Sound 1&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-2"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-2"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-2"&gt;Play Sound 2&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-3"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-3"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-3"&gt;Play Sound 3&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-4"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-4"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-4"&gt;Play Sound 4&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-5"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-5"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-5"&gt;Play Sound 5&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-6"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-6"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-6"&gt;Play Sound 6&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-7"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-7"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-7"&gt;Play Sound 7&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-8"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-8"&gt;Play Sound 8&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="button-group"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;label class="upload-button" for="file-9"&gt;Upload Sound&lt;/label&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;input type="file" accept="audio/mp3" id="file-9"&gt;</p>
<p class="p1"><span class="Apple-converted-space">      </span>&lt;button class="sound-button" id="play-sound-9"&gt;Play Sound 9&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;script&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>const sounds = {};</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>for (let i = 1; i &lt;= 9; i++) {</p>
<p class="p1"><span class="Apple-converted-space">      </span>const fileInput = document.getElementById(`file-${i}`);</p>
<p class="p1"><span class="Apple-converted-space">      </span>const playButton = document.getElementById(`play-sound-${i}`);</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>fileInput.addEventListener('change', (event) =&gt; {</p>
<p class="p1"><span class="Apple-converted-space">        </span>const file = event.target.files[0];</p>
<p class="p1"><span class="Apple-converted-space">        </span>if (file &amp;&amp; file.type === 'audio/mpeg') {</p>
<p class="p1"><span class="Apple-converted-space">          </span>const fileURL = URL.createObjectURL(file);</p>
<p class="p1"><span class="Apple-converted-space">          </span>sounds[i] = new Audio(fileURL);</p>
<p class="p1"><span class="Apple-converted-space">          </span>alert(`Sound ${i} uploaded successfully!`);</p>
<p class="p1"><span class="Apple-converted-space">        </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">          </span>alert('Please upload a valid MP3 file.');</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">      </span>});</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>playButton.addEventListener('click', () =&gt; {</p>
<p class="p1"><span class="Apple-converted-space">        </span>const sound = sounds[i];</p>
<p class="p1"><span class="Apple-converted-space">        </span>if (sound) {</p>
<p class="p1"><span class="Apple-converted-space">          </span>sound.onloadedmetadata = () =&gt; {</p>
<p class="p1"><span class="Apple-converted-space">            </span>if (sound.duration &gt;= 1 &amp;&amp; sound.duration &lt;= 60) {</p>
<p class="p1"><span class="Apple-converted-space">              </span>sound.play();</p>
<p class="p1"><span class="Apple-converted-space">            </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">              </span>alert('Audio file must be between 1 and 60 seconds long.');</p>
<p class="p1"><span class="Apple-converted-space">            </span>}</p>
<p class="p1"><span class="Apple-converted-space">          </span>};</p>
<p class="p1"><span class="Apple-converted-space">          </span>sound.load();</p>
<p class="p1"><span class="Apple-converted-space">        </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">          </span>alert(`Please upload a sound for button ${i} first.`);</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">      </span>});</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/script&gt;</p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
