# Agar.io
* {
    font-family: sans-serif;
    font-size: 14px;
}

html, body {
    background-color: #222;
}

html, body, canvas {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
}

div {
    -webkit-user-select: none; /* webkit (safari, chrome) browsers */
    -moz-user-select: none; /* mozilla browsers */
    -khtml-user-select: none; /* webkit (konqueror) browsers */
    -ms-user-select: none; /* IE10+ */
}

#split {
    position: absolute;
    bottom: 10px;
    left: 10px;
    width: 100px;
    height: 100px;
    padding: 5px;
}

#feed {
    position: absolute;
    bottom: 10px;
    right: 10px;
    width: 100px;
    height: 100px;
    padding: 5px;
}

#status {
    position: absolute;
    padding: 10px;
    background: rgba(0, 0, 0, 0.4);
    color: #FFF;
    font-size: 16.1px;
    top: 10px;
    right: 10px;
    font-weight: bold;
    text-align: center;
}

#status .title {
    font-size: 25px;
}

#status .me {
    color: #FF8888;
    font-size: 16.1px;
}

.chatbox {
    position: absolute;
    width: 300px;
    height: 320px;
    background: rgba(255, 255, 255, 0.7);
    bottom: 5px;
    left: 5px;
    border-radius: 5px;
    pointer-events: none;
}

.chatbox .chat-list {
    padding: 5px;
    margin: 0;
    list-style: none;
    box-sizing: border-box;
    height: 285px;
    overflow: hidden;
}

.chatbox .chat-list li {
    padding: 2px;
    margin: 3px;
}

.chatbox .chat-list li.me b {
    color: #ea6153;
}

.chatbox .chat-list li.friend b {
    color: #2ecc71;
}

.chatbox .chat-list li.system {
    color: #9b59b6;
    font-style: italic;
}

.chatbox .chat-list li.system:before {
    content: "» ";
}

.chatbox .chat-input {
    pointer-events: all;
    box-sizing: border-box;
    width: 100%;
    padding: 8px;
    background: transparent;
    border: none;
    border-top: 1px solid #DDD;
    outline: none;
}

#startMenu {
    position: relative;
    margin: auto;
    margin-top: 100px;
    width: 350px;
    padding: 20px;
    border-radius: 5px;
    -moz-border-radius: 5px;
    -webkit-border-radius: 5px;
    background-color: white;
    box-sizing: border-box;
}

#startMenu p {
    padding: 0;
    text-align: center;
    font-size: x-large;
    font-weight: bold;
}

#playerNameInput {
    width: 100%;
    text-align: center;
    padding: 10px;
    border: solid 1px #dcdcdc;
    transition: box-shadow 0.3s, border 0.3s;
    box-sizing: border-box;
    border-radius: 5px;
    -moz-border-radius: 5px;
    -webkit-border-radius: 5px;
    margin-bottom: 10px;
    outline: none;
}

#playerNameInput:focus, #playerNameInput.focus {
    border: solid 1px #CCCCCC;
    box-shadow: 0 0 3px 1px #DDDDDD;
}

#startButton, #spectateButton {
    position: relative;
    margin: auto;
    margin-top: 10px;
    width: 100%;
    height: 40px;
    box-sizing: border-box;
    font-size: large;
    color: white;
    text-align: center;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.25);
    background: #2ecc71;
    border: 0;
    border-bottom: 2px solid #28be68;
    cursor: pointer;
    -webkit-box-shadow: inset 0 -2px #28be68;
    box-shadow: inset 0 -2px #28be68;
    border-radius: 5px;
    -moz-border-radius: 5px;
    -webkit-border-radius: 5px;
    margin-bottom: 10px;
}

#spectateButton:active, #spectateButton:hover,
#startButton:active, #startButton:hover {
    top: 1px;
    background: #55D88B;
    outline: none;
    -webkit-box-shadow: none;
    box-shadow: none;
}

#settingsButton {
    position: relative;
    margin: auto;
    margin-top: 10px;
    width: 100%;
    height: 40px;
    box-sizing: border-box;
    font-size: large;
    color: white;
    text-align: center;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.25);
    background: #2ecc71;
    border: 0;
    border-bottom: 2px solid #28be68;
    cursor: pointer;
    -webkit-box-shadow: inset 0 -2px #28be68;
    box-shadow: inset 0 -2px #28be68;
    border-radius: 5px;
    -moz-border-radius: 5px;
    -webkit-border-radius: 5px;
    margin-bottom: 10px;
}

#settingsButton:active, #settingsButton:hover {
    top: 1px;
    background: #55D88B;
    outline: none;
    -webkit-box-shadow: none;
    box-shadow: none;
}

#settings, #startMenuWrapper {
    -webkit-transition: max-height 1s;
    -moz-transition: max-height 1s;
    -ms-transition: max-height 1s;
    -o-transition: max-height 1s;
    transition: max-height 1s;
    overflow: hidden;
}

#settings {
    max-height: 0;
}

#startMenu h3 {
    padding-bottom: 0;
    margin-bottom: 0;
}

#startMenu ul {
    margin: 10px;
    padding: 10px;
    margin-top: 0;
}

#startMenu .input-error {
    color: red;
    opacity: 0;
    font-size : 12px;
}

#startMenuWrapper {
    z-index: 2;
}

#gameAreaWrapper {
    position: absolute !important;
    top: 0;
    left: 0;
    opacity: 0;
}

@media only screen  and (min-width : 1224px) {
#mobile {
display: none;
	}
}

@media only screen  and (max-width : 1224px) {
#chatbox {
display: none;
        }
}
