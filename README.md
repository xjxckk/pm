### ProtonMail Custom Theme
![ProtonMail Custom Theme](https://jxck.cf/wp-content/uploads/pm.jpg)
### How to use:
* Open ProtonMail
* Go to Settings
* Go to Appearance
* [Copy the CSS](https://raw.githubusercontent.com/xjxckk/pm/master/pm.css) and paste it under Custom Theme


### CSS:
```
@charset "UTF-8";
:root{
    --theme1:#667cbd;
    --theme2:#5f5f60;
    --theme3:#f0f0f0;
    --theme4:#bcbdbf;
    --theme5:#797a7c;
    --theme6:#9397cd;
    --theme7:#fefefe;
    --red:#cc9393;
    --red-light:#ec6446;
    --yellow:#dfdf19;
    --yellow-light:#e7d360;
    --green:#a6cc93;
    --green-light:#89bc70;
    --blue:#bce8f1;
    --blue-light:#93b9cc;
    --white:hsla(0,0%,100%,.8);
    --black:#333;
	--logo:url(https://vgy.me/chQYqf.png); /* assets/img/logo.svg */
    --image:url(https://vgy.me/yRZJ0U.jpg);
	--image-white:url(https://vgy.me/VKAM2a.jpg);
}

@import url(//fonts.googleapis.com/css?family=Roboto);

html{
    background:var(--image) no-repeat center center fixed;
    -webkit-background-size:cover;
    -moz-background-size:cover;
    -o-background-size:cover;
    background-size:cover
}
/* White BG */
body #conversation-list-rows .conversation, body #conversation-list-rows .conversation.read, .pm_toolbar, #pm_settings, #conversation-view .message .summary, #conversation-view .message .summary .summary-right, #conversation-view .message .details .recipients-summary, #conversation-view .message .details .recipients-details, #conversation-view .message .details .action-row, .messageExtra-container>[class*=-container], #conversation-view .message .frame, #conversationHeader h1, .alert {
	box-shadow: 0 1px 2px rgba(0,0,0, 0.15),
				0 2px 3px rgba(0,0,0, 0.3);
	border-radius: 2px;
	transition: box-shadow 0.25s ease-in-out;
	background: var(--image-white) no-repeat left top fixed !important;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
	opacity: 0.75;
	font-family: Roboto;
}
#conversation-view .message .summary .summary-right, #conversation-view .message .details .recipients-summary, #conversation-view .message .summary, #conversation-view .message .details .recipients-details{
	box-shadow: none;
	border-radius: 0;
	border: 0;
	margin: 0;
}
/* Buttons */
.sidebarApp-container .sidebar-btn-compose:hover, .tooltip, .pm_buttons a:focus,.pm_buttons a:hover, .pm_buttons.primary a:focus,.pm_buttons.primary a:hover, .pm_buttons .pm_buttons-child:focus,.pm_buttons .pm_buttons-child:hover{
	background: var(--image-white) no-repeat center center scroll !important;
	box-shadow: 0 1px 2px rgba(0,0,0, 0.15),
				0 2px 3px rgba(0,0,0, 0.3);
	border-radius: 2px;
	transition: box-shadow 0.25s ease-in-out;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
}
.customCheckbox-input:checked+.customCheckbox-mask {
	background-color: var(--black);
}
.pm_button.primary {
	background-color: var(--black) !important;
	border-color: var(--black);
}
.pm_button.primary:active {
	background-color: var(--black) !important;
	border-color: var(--black);
}
.pm_badge.primary {
	background-color: var(--black);
	border-color: var(--black);
}
.customRadio-input:checked+.customRadio-mask:after {
	color: var(--black);
	background-color: var(--black);
}
.customRadio-input:checked + .customRadio-mask {
	background-color: var(--black);
	color: rgba(20, 20, 20, .25);
}
/* Scrollbar */
::-webkit-scrollbar-thumb  {
	background-color: hsla(0,0%,100%,.25);
	-webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
	box-shadow: 0 1px 2px rgba(0,0,0, 0.15),
				0 2px 3px rgba(0,0,0, 0.3);
	border-radius: 20px;
	transition: box-shadow 0.25s ease-in-out;
}

::-webkit-scrollbar {
	width: 5px;
}
/* Logo */
.headerSecuredDesktop-logo:before {
	background: var(--logo) no-repeat bottom;
	background-size: 35px;
}
.alert.alert-info {
	color: var(--black);
	opacity: 1;
	box-shadow: 0 0 2px rgba(0,0,0, 0.15),
				0 0 3px rgba(0,0,0, 0.3);
}
p a {
    color: var(--black);
}
body #pm_main::before{
    position:absolute;
    top:0;
    left:0;
    z-index:-1;
    height:100%;
    content:"";
	font-family: Roboto;
}
body #pm_main{
    position:relative;
    border-top-left-radius:15px;
	background: none;
	width: calc(100% - 200px) !important;
	float: right;
}
#pm_main{
    color: var(--black);
}
body,body #body,body header,body header a.logo,body section.sidebar,#ptSidebar{
    background:transparent!important
}
.conversation.marked:before{
	background: none;
}
body #conversation-list-rows .conversation .fa-star-o{
	opacity: 1;
}
body #conversation-list-rows .conversation .fa-star{
	color: var(--black);
}
.pm_buttons {
	color: var(--black);
	border: 1px solid rgba(20, 20, 20, .25);
}
.navigation>li.active, .navigation>li:hover{
	border-color: var(--white);
}
/* Unread */
body #conversation-list-rows .conversation{
	color: black;
	font-weight: bold;
	margin-bottom: 5px;
	border-bottom: 0;
	width: calc(100% - 5px);
	opacity: 1;
}
body #conversation-list-rows .conversation .subject h4{
	color: black;
}
/* Read */
body #conversation-list-rows .conversation.read {
	color: var(--black);
	margin-bottom: 5px;
	border-bottom: 0;
}
body #conversation-list-rows .conversation .subject h4 .subject-text{
	font-weight: bold;
}
body #conversation-list-rows .conversation.read .subject h4{
	font-weight: bold;
}
.pm_toolbar {
	border-top-left-radius: 2px;
	border-bottom:0;
	margin-bottom: 5px;
	opacity: 0.75;
}
.tooltip {
	opacity: 1;
	color: var(--black);
}
.navigation-upgrade-item {
	display: none !important;
}
.navigationReport {
	display: none !important;
}
html.protonmail .text-purple {
	color: var(--black) !important;
}
/* Folders / Labels */
.fa.fa-folder.menuLabel-icon {
	color: hsla(0,0%,100%,.5) !important;
}
/* Storage left / Version */
.sidebarApp-container .footer {
    display: none;
}
.sidebarApp-menu {
	margin: 2px -20px 10px -25px;
}
.sidebarApp-item .navigationItem-item,.sidebarApp-item .sidebarApp-link,.sidebarApp-menu .menuLabel-link{
    font-weight:600
}
/* Active item / Current Page */
.menuLabel-item.active .menuLabel-link,.sidebarApp-item.active .navigationItem-item,.sidebarApp-item.active .sidebarApp-link{
    background-color:var(--white);
	color: var(--black);
	letter-spacing: 1px;
}
.active .navigationItem-title:hover{
	color: black;
	font-weight: 700;
}
.sidebarApp-item.active .navigationItem-icon {
	color: var(--black);
}
.sidebarApp-item.active i {
	color: var(--black);
}
.active .navigationItem-aside .navigationItem-counter {
	color: #4c4c4c;
}
.fa.fa-repeat.refresh.navigationItem-btn-refresh {
	color: var(--black);
}
/* Conversation */
#conversation-view .message{
	border: 0;
	margin: 0;
}
#conversation-view .message .summary{
	border: 0;
	margin: 0;
}
#conversation-view .message .summary .time {
	background: none;
}
#conversation-view .message .summary .status {
	background: none;
}
#conversation-view .message .details{
	padding: 0;
	background: none;
	border-bottom: 0;
}
#conversation-view .message .details .recipients-summary, #conversation-view .message .details .recipients-details {
	padding-left: 10px;
}
#conversation-view .message .toggleDetails {
	color: var(--black);
	margin-left: 10px;
}
.allMessageLabels-container {
	padding: 0;
}
#conversation-view .message .details .action-row{
	margin-bottom: 5px;
	border-top-left-radius: 0;
	border-top-right-radius: 0;
	box-shadow: none;
}
.action-row .pull-right {
	padding-right: 20px;
}
.messageExtra-container>[class*=-container] {
	padding-left: 10px;
}
#conversation-view .message .frame{
	border: 0;
	margin: 0;
	opacity: 1;
}
#conversation-view header {
	border-bottom: 0;
	padding: 0;
}
#conversationHeader h1 {
	border-radius: 5px;
	padding: 14px !important;
	margin-bottom: 5px !important;
}
.alert {
	margin-bottom: 5px !important;
 }
#conversation-view header h1 .starButton {
	right: 0;
}
.pm_button,.pm_form .pm_select{
    background-color:var(--white)
}
.pm_button.link{
    color:var(--black)!important
}
/* Compose */
body section.sidebar a.compose{
    box-shadow:0 2px 4px 0 rgba(0,0,0,0.16),0 2px 10px 0 rgba(0,0,0,0.12)!important
}
.sidebarApp-container .sidebar-btn-compose{
    color: var(--white);
	border: 3px solid var(--white);
	background: none;
	height: 45px;
}
.sidebarApp-container .sidebar-btn-compose:hover{
    color: var(--black);
	background-attachment: scroll !important;
	background-position: center center !important;
}
.composerHeader-container{
    color:var(--black)!important
}
```
