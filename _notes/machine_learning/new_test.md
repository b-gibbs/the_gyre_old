---
title: Style Testing
layout: default
excerpt: CSS testing
permalink: /notes/machine_learning/style_test_full
sidebar:
  nav: "notes_machine_learning"
toc: true
toc_label: "Topics"
---





<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<title>style_testing</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>

<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.2.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.2.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.2.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.2.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.2.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.2.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2);
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1);
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1);
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
@media (max-width: 991px) {
  #ipython_notebook {
    margin-left: 10px;
  }
}
[dir="rtl"] #ipython_notebook {
  float: right !important;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#login_widget {
  float: right;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  text-align: center;
  vertical-align: middle;
  display: inline;
  opacity: 0;
  z-index: 2;
  width: 12ex;
  margin-right: -12ex;
}
.alternate_upload .btn-upload {
  height: 22px;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
[dir="rtl"] #tabs li {
  float: right;
}
ul#tabs {
  margin-bottom: 4px;
}
[dir="rtl"] ul#tabs {
  margin-right: 0px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons {
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-right {
  padding-top: 1px;
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-left {
  float: right !important;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: baseline;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
#tree-selector {
  padding-right: 0px;
}
[dir="rtl"] #tree-selector a {
  float: right;
}
#button-select-all {
  min-width: 50px;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
[dir="rtl"] #new-menu {
  text-align: right;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
[dir="rtl"] #running .col-sm-8 {
  float: right !important;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI colors. */
.ansibold {
  font-weight: bold;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  border-left-width: 1px;
  padding-left: 5px;
  background: linear-gradient(to right, transparent -40px, transparent 1px, transparent 1px, transparent 100%);
}
div.cell.jupyter-soft-selected {
  border-left-color: #90CAF9;
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected {
  border-color: #ababab;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 5px, transparent 5px, transparent 100%);
}
@media print {
  div.cell.selected {
    border-color: transparent;
  }
}
div.cell.selected.jupyter-soft-selected {
  border-left-width: 0;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 7px, #E3F2FD 7px, #E3F2FD 100%);
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #66BB6A -40px, #66BB6A 5px, transparent 5px, transparent 100%);
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  padding: 0.4em;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. We need the 0 value because of how we size */
  /* .CodeMirror-lines */
  padding: 0;
  border: 0;
  border-radius: 0;
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul {
  list-style: disc;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ul ul {
  list-style: square;
  margin: 0em 2em;
}
.rendered_html ul ul ul {
  list-style: circle;
  margin: 0em 2em;
}
.rendered_html ol {
  list-style: decimal;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
  margin: 0em 2em;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  background-color: #fff;
  color: #000;
  font-size: 100%;
  padding: 0px;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: 1px solid black;
  border-collapse: collapse;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  border: 1px solid black;
  border-collapse: collapse;
  margin: 1em 2em;
}
.rendered_html td,
.rendered_html th {
  text-align: left;
  vertical-align: middle;
  padding: 4px;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget {
  float: right !important;
  float: right;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  margin-top: 6px;
}
span.save_widget span.filename {
  height: 1em;
  line-height: 1em;
  padding: 3px;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  display: none;
}
.command-shortcut:before {
  content: "(command)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    
/* Temporary definitions which will become obsolete with Notebook release 5.0 */
.ansi-black-fg { color: #3E424D; }
.ansi-black-bg { background-color: #3E424D; }
.ansi-black-intense-fg { color: #282C36; }
.ansi-black-intense-bg { background-color: #282C36; }
.ansi-red-fg { color: #E75C58; }
.ansi-red-bg { background-color: #E75C58; }
.ansi-red-intense-fg { color: #B22B31; }
.ansi-red-intense-bg { background-color: #B22B31; }
.ansi-green-fg { color: #00A250; }
.ansi-green-bg { background-color: #00A250; }
.ansi-green-intense-fg { color: #007427; }
.ansi-green-intense-bg { background-color: #007427; }
.ansi-yellow-fg { color: #DDB62B; }
.ansi-yellow-bg { background-color: #DDB62B; }
.ansi-yellow-intense-fg { color: #B27D12; }
.ansi-yellow-intense-bg { background-color: #B27D12; }
.ansi-blue-fg { color: #208FFB; }
.ansi-blue-bg { background-color: #208FFB; }
.ansi-blue-intense-fg { color: #0065CA; }
.ansi-blue-intense-bg { background-color: #0065CA; }
.ansi-magenta-fg { color: #D160C4; }
.ansi-magenta-bg { background-color: #D160C4; }
.ansi-magenta-intense-fg { color: #A03196; }
.ansi-magenta-intense-bg { background-color: #A03196; }
.ansi-cyan-fg { color: #60C6C8; }
.ansi-cyan-bg { background-color: #60C6C8; }
.ansi-cyan-intense-fg { color: #258F8F; }
.ansi-cyan-intense-bg { background-color: #258F8F; }
.ansi-white-fg { color: #C5C1B4; }
.ansi-white-bg { background-color: #C5C1B4; }
.ansi-white-intense-fg { color: #A1A6B2; }
.ansi-white-intense-bg { background-color: #A1A6B2; }

.ansi-bold { font-weight: bold; }

    </style>
<style type="text/css">
    
    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<p>title: Style Testing
layout: jupyter
excerpt: CSS testing</p>
<h2 id="permalink:-/notes/machine_learning/style_test_full">permalink: /notes/machine_learning/style_test_full<a class="anchor-link" href="#permalink:-/notes/machine_learning/style_test_full">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="o">%</span><span class="k">matplotlib</span> inline

<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">scipy</span> <span class="k">as</span> <span class="nn">sp</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>

<span class="kn">from</span> <span class="nn">matplotlib</span> <span class="k">import</span> <span class="n">rcParams</span>
<span class="kn">import</span> <span class="nn">matplotlib.cm</span> <span class="k">as</span> <span class="nn">cm</span>
<span class="kn">import</span> <span class="nn">matplotlib</span> <span class="k">as</span> <span class="nn">mpl</span>
<span class="kn">from</span> <span class="nn">cycler</span> <span class="k">import</span> <span class="n">cycler</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#svg.fonttype: path</span>

<span class="n">blue</span> <span class="o">=</span> <span class="s1">&#39;#3498DB&#39;</span>
<span class="n">gray</span> <span class="o">=</span> <span class="s1">&#39;#95A5A6&#39;</span>
<span class="n">red</span> <span class="o">=</span> <span class="s1">&#39;#E74C3C&#39;</span>
<span class="n">dark_gray</span> <span class="o">=</span> <span class="s1">&#39;#34495E&#39;</span>
<span class="n">green</span> <span class="o">=</span> <span class="s1">&#39;#2ECC71&#39;</span>
<span class="n">purple</span> <span class="o">=</span> <span class="s1">&#39;#9B59B6&#39;</span>
<span class="n">flatui</span> <span class="o">=</span> <span class="p">[</span><span class="n">blue</span><span class="p">,</span> <span class="n">gray</span><span class="p">,</span> <span class="n">red</span><span class="p">,</span> <span class="n">dark_gray</span><span class="p">,</span> <span class="n">green</span><span class="p">,</span> <span class="n">purple</span><span class="p">]</span>

<span class="c1">#rcParams[&#39;axes.prop_cycle&#39;] = cycler(&#39;color&#39;, [blue, gray, red, dark_gray, green, purple])</span>

<span class="c1"># Patches</span>
<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;patch&#39;</span><span class="p">,</span> 
       <span class="n">linewidth</span><span class="o">=</span><span class="mf">0.5</span><span class="p">,</span> 
       <span class="n">facecolor</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">,</span> 
       <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> 
       <span class="n">force_edgecolor</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> 
       <span class="n">antialiased</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>    
  
<span class="c1"># Figure</span>
<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;figure&#39;</span><span class="p">,</span> 
       <span class="n">figsize</span><span class="o">=</span> <span class="p">(</span><span class="mi">10</span><span class="p">,</span> <span class="mi">6</span><span class="p">),</span>
       <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> 
       <span class="n">edgecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span> 
       <span class="n">titlesize</span><span class="o">=</span><span class="s1">&#39;large&#39;</span><span class="p">)</span>

<span class="c1"># Grid</span>
<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;grid&#39;</span><span class="p">,</span> 
       <span class="n">color</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">,</span>
       <span class="n">alpha</span><span class="o">=</span><span class="mf">0.5</span><span class="p">,</span> 
       <span class="n">linewidth</span><span class="o">=</span><span class="mf">0.5</span><span class="p">,</span> 
       <span class="n">linestyle</span><span class="o">=</span><span class="s1">&#39;-&#39;</span><span class="p">)</span>

<span class="c1"># Axes</span>
<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;axes&#39;</span><span class="p">,</span> 
       <span class="n">facecolor</span><span class="o">=</span><span class="s1">&#39;w&#39;</span><span class="p">,</span>
       <span class="n">edgecolor</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">,</span>
       <span class="n">linewidth</span><span class="o">=</span><span class="mf">0.5</span><span class="p">,</span>
       <span class="n">grid</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
       <span class="n">titlesize</span><span class="o">=</span><span class="s1">&#39;large&#39;</span><span class="p">,</span>
       <span class="n">labelsize</span><span class="o">=</span><span class="s1">&#39;large&#39;</span><span class="p">,</span>
       <span class="n">labelcolor</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">,</span>
       <span class="n">axisbelow</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;axes.spines&#39;</span><span class="p">,</span>
       <span class="n">right</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
       <span class="n">top</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>

<span class="c1"># Ticks</span>
<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;xtick&#39;</span><span class="p">,</span> 
       <span class="n">direction</span><span class="o">=</span><span class="s1">&#39;out&#39;</span><span class="p">,</span>
       <span class="n">color</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;xtick.major&#39;</span><span class="p">,</span> 
       <span class="n">size</span><span class="o">=</span><span class="mf">0.0</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;xtick.minor&#39;</span><span class="p">,</span> 
       <span class="n">size</span><span class="o">=</span><span class="mf">0.0</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;ytick&#39;</span><span class="p">,</span> 
       <span class="n">direction</span><span class="o">=</span><span class="s1">&#39;out&#39;</span><span class="p">,</span>
       <span class="n">color</span><span class="o">=</span><span class="n">dark_gray</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;ytick.major&#39;</span><span class="p">,</span> 
       <span class="n">size</span><span class="o">=</span><span class="mf">0.0</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;ytick.minor&#39;</span><span class="p">,</span> 
       <span class="n">size</span><span class="o">=</span><span class="mf">0.0</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;legend&#39;</span><span class="p">,</span> 
       <span class="n">frameon</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
       <span class="n">numpoints</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span>
       <span class="n">scatterpoints</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>

<span class="n">mpl</span><span class="o">.</span><span class="n">rc</span><span class="p">(</span><span class="s1">&#39;font&#39;</span><span class="p">,</span> 
       <span class="n">size</span><span class="o">=</span><span class="mi">14</span><span class="p">,</span>
       <span class="n">weight</span><span class="o">=</span><span class="s1">&#39;bold&#39;</span><span class="p">,</span>
       <span class="n">family</span><span class="o">=</span><span class="s1">&#39;sans-serif&#39;</span><span class="p">)</span>

<span class="n">pd</span><span class="o">.</span><span class="n">set_option</span><span class="p">(</span><span class="s1">&#39;display.width&#39;</span><span class="p">,</span> <span class="mi">500</span><span class="p">)</span>
<span class="n">pd</span><span class="o">.</span><span class="n">set_option</span><span class="p">(</span><span class="s1">&#39;display.max_columns&#39;</span><span class="p">,</span> <span class="mi">100</span><span class="p">)</span>
<span class="n">pd</span><span class="o">.</span><span class="n">set_option</span><span class="p">(</span><span class="s1">&#39;display.notebook_repr_html&#39;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">scipy.stats</span> <span class="k">as</span> <span class="nn">stats</span>
<span class="kn">import</span> <span class="nn">sklearn</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Load and return the boston house-prices dataset (regression).</span>
<span class="kn">from</span> <span class="nn">sklearn.datasets</span> <span class="k">import</span> <span class="n">load_boston</span>

<span class="n">boston</span> <span class="o">=</span> <span class="n">load_boston</span><span class="p">()</span>
<span class="n">bos</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">boston</span><span class="o">.</span><span class="n">data</span><span class="p">)</span>
<span class="n">bos</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">boston</span><span class="o">.</span><span class="n">feature_names</span>
<span class="n">bos</span><span class="p">[</span><span class="s1">&#39;PRICE&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">boston</span><span class="o">.</span><span class="n">target</span>

<span class="n">bos</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[4]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>CRIM</th>
      <th>ZN</th>
      <th>INDUS</th>
      <th>CHAS</th>
      <th>NOX</th>
      <th>RM</th>
      <th>AGE</th>
      <th>DIS</th>
      <th>RAD</th>
      <th>TAX</th>
      <th>PTRATIO</th>
      <th>B</th>
      <th>LSTAT</th>
      <th>PRICE</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0.00632</td>
      <td>18.0</td>
      <td>2.31</td>
      <td>0.0</td>
      <td>0.538</td>
      <td>6.575</td>
      <td>65.2</td>
      <td>4.0900</td>
      <td>1.0</td>
      <td>296.0</td>
      <td>15.3</td>
      <td>396.90</td>
      <td>4.98</td>
      <td>24.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>0.02731</td>
      <td>0.0</td>
      <td>7.07</td>
      <td>0.0</td>
      <td>0.469</td>
      <td>6.421</td>
      <td>78.9</td>
      <td>4.9671</td>
      <td>2.0</td>
      <td>242.0</td>
      <td>17.8</td>
      <td>396.90</td>
      <td>9.14</td>
      <td>21.6</td>
    </tr>
    <tr>
      <th>2</th>
      <td>0.02729</td>
      <td>0.0</td>
      <td>7.07</td>
      <td>0.0</td>
      <td>0.469</td>
      <td>7.185</td>
      <td>61.1</td>
      <td>4.9671</td>
      <td>2.0</td>
      <td>242.0</td>
      <td>17.8</td>
      <td>392.83</td>
      <td>4.03</td>
      <td>34.7</td>
    </tr>
    <tr>
      <th>3</th>
      <td>0.03237</td>
      <td>0.0</td>
      <td>2.18</td>
      <td>0.0</td>
      <td>0.458</td>
      <td>6.998</td>
      <td>45.8</td>
      <td>6.0622</td>
      <td>3.0</td>
      <td>222.0</td>
      <td>18.7</td>
      <td>394.63</td>
      <td>2.94</td>
      <td>33.4</td>
    </tr>
    <tr>
      <th>4</th>
      <td>0.06905</td>
      <td>0.0</td>
      <td>2.18</td>
      <td>0.0</td>
      <td>0.458</td>
      <td>7.147</td>
      <td>54.2</td>
      <td>6.0622</td>
      <td>3.0</td>
      <td>222.0</td>
      <td>18.7</td>
      <td>396.90</td>
      <td>5.33</td>
      <td>36.2</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">bos</span><span class="o">.</span><span class="n">DIS</span><span class="p">,</span> <span class="n">bos</span><span class="o">.</span><span class="n">PRICE</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.3</span><span class="p">,</span> <span class="n">s</span><span class="o">=</span><span class="mi">60</span><span class="p">);</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">hist</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">bos</span><span class="o">.</span><span class="n">CRIM</span><span class="p">))</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Crime Rate per Capita&quot;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Crime rate per capita&quot;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Frequency&quot;</span><span class="p">);</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABsgAAARNCAYAAAD/38WlAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAewgAAHsIBbtB1PgAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMi4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvhp/UCwAAIABJREFUeJzs3WecVdW9P/4vDB2EoWosgAIKKHZBiqBiQLDGiDUxduNNlFhJbFw1GiVqjCY3P8UES6JGUYMRUOxiB6WDUoQovXcGmJnzf3D/zvVwZoY5M8MUz/v9es2DvfZea33n7HM2ej6z96qRSCQSAQAAAAAAABmiZmUXAAAAAAAAABVJQAYAAAAAAEBGEZABAAAAAACQUQRkAAAAAAAAZBQBGQAAAAAAABlFQAYAAAAAAEBGEZABAAAAAACQUQRkAAAAAAAAZBQBGQAAAAAAABlFQAYAAAAAAEBGEZABAAAAAACQUQRkAAAAAAAAZBQBGQAAAAAAABlFQAYAAAAAAEBGEZABAAAAAACQUQRkAAAAAAAAZBQBGQAAAAAAABlFQAYAAAAAAEBGEZABAAAAAACQUWpVdgEAAFCe8vLyYubMmTF37txYtGhRbNy4MfLz8yM7Ozuys7Nj7733jsMPPzwaNWpUqXUee+yx8e677xZsDx06NP77v/+78goCqCJWrlwZ06ZNiwULFsTq1atjy5Yt0aBBg8jOzo5mzZpFly5dol27dpVdZpX1xhtvxA9/+MOC7aysrMjNza3EigAAqiYBGQAA1V5OTk4899xz8fzzz8fbb78dmzZtKvb4mjVrRseOHWPAgAFx/vnnx2GHHVZBlVLVPf7443HRRReV6Ng6depEkyZNokmTJnHAAQfE4YcfHn379o3evXtHjRo1dnGl8P0yderUeOqpp2LUqFExZ86cnR7frFmz6N69e5x99tnxox/9qNL/6AEAgOpHQAYAQLWVm5sbDz/8cPzud7+LFStWlLhffn5+zJw5M2bOnBn3339/dOnSJW6//fb40Y9+tAur5ftm27ZtsWLFilixYkXMnTs3Ro8eHXfeeWe0a9cubr755hIHbZXtxRdfjKlTpxZsH3744XHqqadWYkVkkunTp8f1118fr732Wlr9Vq9eHaNHj47Ro0dHgwYN4uKLL45bb701WrVqtYsq/X77/PPP4+WXXy7YbtasWVx99dWVWBEAwK4nIAMAoFr68ssv46yzzkr6Yr+0pk2bFmeccUYcffTR8fbbb0e9evXKoUIy1bx58+Liiy+OkSNHxsiRI6N+/fqVXVKxXnzxxfjHP/5RsH3JJZcIyNjl8vPz46677orbb7898vLyyjTW5s2b409/+lM8/vjjMXz48DjnnHPKqcrM8fnnn8ftt99esN2uXTsBGQDwvScgAwCg2nn33XfjlFNOiQ0bNqTs23PPPePEE0+Mfv36Rfv27aNly5bRrFmzyMnJiSVLlsQXX3wR7733XvzrX/+KhQsXJvX9+OOPIycnR0BGknPPPTdat26d0r5169ZYuXJlTJ48OaZPn56yf8yYMTFo0KB4+eWXo2bNmhVRKlQL27Zti3POOSdeeumllH21atWKnj17xoknnhg9evSIVq1aRcuWLaN27dqxdu3amD9/fkyYMCHGjRsXb731VlK4tnHjxpg4caKADACAEhGQAQBQrXz00UcxYMCA2LJlS1L7HnvsEUOHDo1LL700atVK/c/cRo0aRYsWLaJLly4xaNCgeOihh2LMmDFx5513xieffFJR5Rd45513KnxOSufyyy+PY489tthjZs2aFTfeeGO88sorSe2jR4+OJ598Mi688MJdVyBUI/n5+XHWWWfFqFGjUvb9+Mc/jnvuuSfat29faN/GjRtH69ato0+fPnH99dfHkiVL4g9/+EP86U9/Svk3IZOdcMIJkUgkKrsMAIAqz58xAgBQbSxZsiROP/30lC9CjznmmJg1a1b8/Oc/LzQcK0yNGjXipJNOio8++ihGjBgRjRs33hUlkyE6deoU//73v+OSSy5J2ffdx5ZBprv55ptTwrE6derEc889FyNHjiwyHCvMD37wgxg2bFjMmjUr+vfvX96lAgDwPScgAwCg2rjiiiti+fLlSW39+vWLcePGRXZ2dqnGrFGjRlx44YUxadKkOPDAA8ujTDLYQw89FLvvvntS24IFC2LatGmVVBFUHR999FEMGzYsqa127doxevToGDRoUKnHbdOmTYwdOzbuuusujzMFAKDE/JcjAADVwrhx4+Lf//53UlvLli3j73//e7msGbbffvvFBx98EA0bNizzWGSuBg0axLnnnpvS/u6771ZCNVC1XHPNNZGfn5/UNnTo0DjhhBPKPHaNGjXipptuihtuuKHMYwEAkBmsQQYAQLXw29/+NqXt4YcfjpYtW5bbHE2aNCnzGF9//XV89tln8Z///Cc2btwY9erVi86dO8fAgQPLocKdW7FiRXz44Ycxf/782LhxY+y2225xwAEHRK9evaJRo0Y77Z9IJGLy5MkxefLkWL58edSsWTP22GOP6Nq1axxwwAHlWmt+fn58/vnn8dVXX8WKFSti3bp10bRp02jZsmUcccQRse+++5brfBXlqKOOSmlbvHhxqcfbtGlTfPnll/Hll1/GypUrY8OGDVGnTp1o1qxZ7LHHHtGtW7do3rx5WUre5fLz8+Ozzz6L+fPnp5zrI488Mtq2bVvZJRZq1apV8dFHH8W8efNi48aN0axZs9hrr72iZ8+eu+Q1nzNnTkyfPj1WrFgRq1atioYNG0bLli3jgAMOiMMOOyxq1KhR7nNG/O/nfurUqTF9+vRYsmRJ5OTkROPGjaN3795x6KGHlssc48aNS1nv8dBDD40hQ4aUy/jfSvffhCVLlsQXX3wRX331Vaxbty62bNkSjRs3jqZNm0aHDh3i8MMPj9q1a5drjTuaN29eTJw4MRYuXBjbtm2L3XffPdq0aRO9evWKunXr7tK5K8LWrVtj9uzZ8eWXX8bSpUtjw4YNkZWVFc2aNYuWLVvGUUcdFXvuuWdllwkAZKIEAABUcTNnzkxERNJPmzZtEnl5eRVWw/z581NqmD9/fiKRSCTy8/MTjz/+eOLQQw9NOSYiEoccckjKeH369Ek6ZujQoTutoU2bNkl9RowYUbDvk08+SZx44omJmjVrFlpDo0aNEtdee21i3bp1hY6dk5OTuO+++xL77LNPof0jItGlS5fEuHHjSvPyJfn8888T5557bqJZs2ZFzhURiQ4dOiR+97vfJTZv3lzmOUtqxIgRKXW8/fbbaY3x2muvpYxx+eWXpzXGxIkTE7/+9a8TXbt2TdSqVavY16lGjRqJAw88MPHnP/+5xK/V+eefX+yYO/sZP358ieb57LPPEuecc85Oz/X++++fuPfeeyv0XPfs2TOphjvvvLNg34QJExIDBw5MZGVlFVpvrVq1Ev3790988sknZa5j0aJFiV/96leJtm3bFvsatWrVKvGLX/wisXjx4rTGHz58eNI47dq1K9i3fv36xG233Zb4wQ9+UOic1113XZl/v2+dccYZKeM/8cQT5TZ+SW3evDnx/PPPJy644IJE69atd/per1+/fuLUU09NvPvuu2nPtX379mI/O//85z+L/HcjIhKNGzdOXHTRRYlFixalNe/rr7+eNE5WVlahx+343kj357ufmR3NmjUrcccddyR69+6dqFu37k7H2m+//RJ33313Ys2aNWn9rgAAZeERiwAAVHkjR45MabvsssuqxFozK1eujOOOOy4uvPDCmDx5cqXUcMcdd0T37t3j1VdfTXl82bc2btwYDzzwQBx99NHxzTffJO2bO3duHHXUUXH99den7PuuadOmRb9+/eLuu+8uVZ2rV6+Os88+O4444oh45plnYvXq1cUeP2fOnPjNb34T7dq1i7feeqtUc1aGLVu2pLSlcwdKz54948gjj4x77rknPv3008jNzS32+EQiETNmzIhf/OIXsf/++8enn36ads3lbeXKlTFo0KA48sgj49lnn93puZ49e3YMGTIkOnToUOmPoxw2bFgcffTRMWbMmMjLyyv0mNzc3Hjttdeie/fucf3110cikUh7nry8vLjllluiffv28eCDD8aCBQuKPX758uXx5z//Odq1axcPPfRQ2vPtaMKECdGpU6e44447YsmSJWUerzhbtmyJsWPHJrU1bdq0TOuOlcakSZOiVatWMWjQoHjyySfj66+/3mmfLVu2xMsvvxx9+vSJM888MzZu3FjmOnJycuKss86Ks88+u9h/N9avXx8jRoyIzp07x9NPP13meSvK+eefH506dYrbbrst3nvvvdi6detO+3z11Vdx0003xX777RdjxoypgCoBAKxBBgBANTBu3LiUttNOO60SKkm2fv366Nu3b6V+of+b3/wmhg4dWmQwtqNZs2bFSSedFDk5ORHxv4/26t27d0ybNq3Ec958883xxBNPpFXn7Nmzo1u3bvHcc8+lHSYsWbIkTjzxxPj73/+eVr/KMn/+/JS23XffvcT9Fy1aVOq5Fy5cGL1794433nij1GOU1axZs6Jbt24xcuTItM/1okWLol+/fvHss8/uouqKN2zYsBgyZEiRwdiO8vPz4/77749LL700rd91/fr1cfLJJ8ddd91VaKBanC1btsTgwYPj6quvTqvfd02aNCn69u1bpvdaOt57772U37Nfv35Rv379Cpn/W+vWrStTwPXCCy9Ez549Y9OmTaUeIz8/PwYNGhTPP/98ifusW7cufvrTn8aI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T2oryxfT5Wnr1q2xePHiGD16dPzsZz+LHj16xNKlS5OO6d69e9xwww0VUk/Xrl3jlFNOKdjevHlzvP322xUyd15eXvz+979Parv22mvjxBNPLPEYHTp0SHkvVvS5PvLII+Paa68t0bEDBgyIn/70p0lto0aNisWLFxfZ5957701aq+zoo49OeX8Xp169ejF8+PCktqeffjrlkZY706JFi3jooYfS6lMWVf06XhJDhw6N2rVrF2yPGTOmxGs/7ujqq6+Oo48+ukTH3n777Sl/APGXv/ylVPNWdW3bto1LL720YDuRSMTo0aMrsSIA4PtOQAYAQJVWWADTpEmTSqgk1SGHHBJ9+vSptPn32GOPOOecc0p8fGF3K/zyl78s8V/57/i75uXlxfTp04s8/q233orZs2cXbNeuXTt+85vflLDa/3PppZcm3YE1Y8aMpDXVdrXjjjsuatSokfJTr1692GuvveLkk0+OJ598MrZv357U74QTTohXXnklrbvHyqp79+5J2x999FGFzPv666/HvHnzCrbr1KmTcudLSVx22WVJIcSUKVNi+fLl5VJjSdxwww3F3km5ox1/x9zc3HjuuecKPXbDhg0pd8Tdeuutad0pGPG/d9t99zxv3749aQ26kvjZz35WodfRwq7jjRs3rrD5y0Pz5s2T/shg3bp1MWvWrLTHycrKiuuvv77Ex9etWzcGDx6c1DZz5syYPHly2nNXB5V1DQMAMlPJ73cHAACSnHrqqZU6/3HHHZfWI6z233//lLZ+/fqVuP/ee+8d9evXT/qye+XKlUUe/9ZbbyVtH3fccdG8efMSz/et+vXrx5FHHpn0+L7x48fHWWedlfZYFeHII4+MX/3qV3HeeeelHX4U5ZtvvompU6fG119/HevXr48NGzZEbm5uynFTpkxJ2p45c2a5zL8zO57rE044IenRmCXVqFGjOPzww+OTTz4paHv//ffjjDPOKHONO9OgQYO0P9MHHnhgdOnSJaZNm1bQ9vHHHxd67Pjx45NC1MaNG6f1+fuu3r17JwUH48ePj0GDBpW4f2VfuyKi3D4bZbV9+/aYNWtWTJ8+PVauXBnr16+PTZs2Jd3p961169Ylbc+cOTMOPPDAtObr06dP/OAHP0irz7nnnhtXX311Uk0ff/xxHHrooWmNU5mWLVsWU6dOja+++qrgGrZt27aU4xYs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OzvlLrKvvvoqnnzyyWL77bjGUJ06ddKad8yYMbF48eK0+kRE1K1bN2l7xyChJHY8119//XXSWmzVwebNm+Pll19Oq8+MGTNi2rRpSW1HH310ocf27ds3atZM/l/wxx57LL0iq7ETTzwxZS2ySZMmlftjJleuXJnSVti6X+l+vsrrXL377rspQdLOPPvssyl/XFDU+6y0yuM6UNZr2IwZM0oVIAIAlJaADACAamHAgAExcODApLbly5fHT37yk1Ld9bGj+fPnR69evQr9IpXS6d+/f+yzzz5Jbb/+9a9L9cVrdfOrX/0qGjdunNT229+WRaubAAAgAElEQVT+tti7yJo3b560/cUXX5R4vtzc3Pjv//7vtGr81m677Za0XVjAsDMDBw6MPffcM6ltyJAh1S5w/v3vf5/Wo1vvvffepO1atWrFWWedVeixLVq0iNNPPz2p7cEHH4z//Oc/6RdaDdWoUSP+8Ic/pISEd9xxR7zxxhtlHj+RSMTvfve7GDZsWMq+HT9bEel9viZOnBgvvfRSmer7Vl5eXtx3330lPn7r1q3xxz/+Mamtc+fOceihh5ZLPd/a8TqwatWqtO/4Lcs1LCLi5ptvTut4AICyEpABAFBtPProo9GiRYuktnHjxkX//v1j3bp1pRozkUjE448/HoceemhMnz69PMrk/1e3bt2ULzynTp0aF110UZnWj1u2bFlZS9vlmjZtGldffXVS2/z58+Pxxx8vss+BBx6YtD127NgS3xH2m9/8JiZOnJh2nRH/u27ad02aNCntL8br1asXN910U8o4l1xySZnO9fLly0vdtzQmTpwYDzzwQImOHTt2bMracqeddlpKUPhdt99+e9Kj7DZv3hwnn3xyrFmzpnQFR/X4PHyrV69ecd111yW1bdu2LU466aQyPTL366+/joEDB8ZNN91U6PutYcOG0aZNm6S2kt4RtmrVqvjJT35Sro+CfOihh0p8p9TQoUNj7ty5SW1XXnlludXyrR2vA5s3b0474NrxGvb555/HpEmTStT3z3/+c4waNSqt+QAAykpABgBAtbHXXnvFSy+9FPXq1Utqf++996JTp07x6KOPlvhLzEQiEWPGjIkePXrERRddFOvXr98VJWe8iy++OHr16pXU9vTTT0ffvn3TWn9p48aN8cwzz0T37t1TvmCvqq655pqUuzLuuuuuIu+qGjBgQNL25s2bY9CgQbF27doi58jJyYnBgwendUfKjnZ87N3SpUtT7lgpicsuuyy6d++e1PbUU0/FD3/4w1iwYEGJx9mwYUP84x//iG7dusWNN96Ydh1ldeONN8af/vSnYo8ZO3ZsnHnmmUltdevWjTvuuKPYfgcddFBce+21SW3Tp0+Pww8/PN57770S15ibmxtvvvlm/PjHP46ePXuWuF9V8Lvf/S5OOumkpLZt27bFoEGD4qyzzkoJg4qzZMmS+PWvfx2dOnXa6eNbd/x8jRo1qtC7zb5r9uzZceyxx8aXX35Z4ppKIjc3NwYOHFjselv5+fnx29/+NuUuxQ4dOsQll1xSrvVE/G+4Vb9+/aS2oUOHpnUXaL9+/SIrK6tgO5FIxNlnnx0LFy4ssk9eXl7cc889cdVVV6VfNABAGdWq7AIAACAdvXr1itGjR8dpp50WGzduLGhfsmRJXHHFFXH77bfHgAEDon///tG+ffto2bJlNG3aNHJycmLp0qUxc+bMGD9+fPzrX/+Kb775phJ/k8xQu3btePHFF6Nr165JIck777wTHTp0iNNOOy0GDhwYXbt2jVatWkWjRo1i48aNsXbt2pg7d25MmTIlPvjgg3jzzTdj69atERHRrl27Svpt0tOsWbO46qqr4u677y5oW7BgQTz++ONx2WWXpRzfrVu36NOnT7z77rsFbR9++GFBqNKvX7/YZ599Ytu2bbFw4cJ47bXX4pFHHil4XbOysuKCCy6IESNGpFVn9+7do3Xr1vH1118XtF1zzTXx6KOPRrdu3aJ58+ZRq1by/zpeeeWVKXfk1KlTJ1566aXo2rVr0lhvvfVWtG/fPn70ox/FgAED4qijjko513PmzCk412+99VbBue7UqVNav0tZnHzyyTF27NjIy8uLq666Kv75z3/G5ZdfHj169IiWLVvG2rVrY/LkyfHkk0/GCy+8kNL/tttui86dO+90nmHDhsWsWbNizJgxBW0LFiyIPn36RI8ePeLMM8+MHj16xN577x1NmjSJnJycWLduXXzzzTcxZcqUmDBhQowdOzZWr14dEZFyHqq6rKysGDlyZJx11lnx73//O2nf888/Hy+99FL06tUrTjzxxOjRo0fsvvvu0bJly6hVq1asW7cuvvrqq5gwYUKMGzcu3nzzzRL/UcR1110Xjz32WNJjTocMGRKvv/56XHnllXHUUUdF06ZNY/Xq1TFr1qx44YUX4oknnih4JOzBBx8cdevWjQkTJpTp9z/ttNNi1KhRsWbNmujTp0+cd955cf7558dBBx0UTZo0iWXLlsX48ePjL3/5S8pdoTVr1oy//e1vKUFWeahVq1acccYZ8Y9//KOg7fnnn4/33nsv+vTpE3vuuWfKOmX9+/eP4447rmB7zz33jPPPPz9pvcU5c+bEwQcfHIMHD45TTjkl9t1330gkErF48eJ466234rHHHktax+/SSy/NqLX5AIBKlgAAgGpoxowZiYMOOigREeX2c/zxxydycnIKnW/+/Pkpx8+fP7/U9ffp0ydprKFDh+60T5s2bZL6jBgxIq05R4wYkdS/TZs2addd2hoWLFiQOPLII8vlPJ1//vlp111SO75GEZF4++23Sz3eypUrE40aNUp53bdt21bo8V988UUiOzu7VK/Lww8/nBg+fHhSW7t27UpU5xNPPJHWXOPHjy9yrPnz5ycOO+ywcjnXP/vZz0rzspdIz549k+a68847E7///e9LVedFF12UyMvLK/HcmzZtSpx//vnl8hrt7HNc2vfErpabm5u49dZbE1lZWeXyOkREIjs7O/HCCy8UOec999xTqnF33333xNy5cwt9zxRn+/btKWO9++67iVNOOSXtGmrUqJH461//WqLX9vXXX0/qm5WVVaJ+M2fOTDRs2LDENRX2+y9btizRunXrUr3O1113XalrBwAoDY9YBACgWurcuXN8/vnnMWzYsGjevHmZxuratWu8+uqr8eabb6b8hTzlo02bNvH+++/HNddck/KIzHRkZ2dHt27dyrGyXat58+bxy1/+MqntP//5T5F3eR1wwAHxyiuvxO67717iOerVqxePPfZYyjzpuOCCC+KBBx4ol/d/27Zt48MPP4zBgweXabymTZtW+Lm+/vrrY9iwYUmPiStOzZo149prr43HHnssatYs+f9eN2jQIP7+97/H//t//y9atWpV2nKjdu3acfzxx5e6f2XKysqKO+64Iz777LM44YQTyjRW48aN48Ybb4yvvvoqzjjjjCKPGzJkSNx8881J68DtTOfOnWP8+PHldudqzZo147nnnouzzjqrxH0aN24cTz31VFx88cXlUkNROnXqFKNGjSp2Hb2dadWqVbz22mvRoUOHEvf59r1QlkfFAgCUhoAMAIBqq3bt2nHDDTfEN998EyNGjIgBAwZEgwYNdtovKysrDjrooBgyZEhMnz49Pvnkk+jfv38FVJzZ6tatGw888EDMnz+/YN2gkmjbtm1ccsklMXLkyFi6dGm1W6vmuuuui0aNGiW13XXXXQWPbttRz549Y9KkSfFf//VfxT5KrUGDBnHhhRfGjBkzymVNomuuuSYWLFgQDzzwQJx++unRoUOHyM7Ojtq1a6c9Vr169eLBBx+M+fPnx5AhQ6Jjx44l6rfvvvvGpZdeGi+88EIsWbIkrrzyyrTnLqsbbrghPv744xgwYECRoVetWrWiX79+8dFHH8X999+fVjj2XVdccUUsWLAgHn744Tj66KNTHmVZmObNm8eZZ54ZjzzySCxZsiT+9re/lWruquKQQw6J119/PSZPnhzXXHNNiYOo5s2bx6mnnhrPPPNMLF26NO69995o2rTpTvv99re/jTfeeCN69+5d7HH77bdf3H///TFp0qS0wp6SqFevXvzzn/+MZ599Ng4++OAij9ttt93iwgsvjFmzZsX5559frjUUpW/fvjFnzpx46qmn4vzzz49DDjkkWrRokVbY3bFjx5gwYULcdNNNkZ2dXeRxderUiR//+McxceLEuPXWW8ujfACAtNRIJBKJyi4CAADKS15eXsyYMSPmzJkTixYtik2bNkV+fn5kZ2dH06ZNo3Xr1nHYYYdFw4YNK7tUImLZsmUxceLEWLFiRaxatSpycnKiUaNGkZ2dHfvtt1906tQpWrRoUdllVpqcnJz48MMPY/bs2bF69eqoWbNmNG/ePDp27Bhdu3atVnc8Ll26ND777LNCz3W7du2iU6dOZb4bNB29evWKDz74oGD7zjvvjFtuuSXpmJUrV8ZHH30U8+bNi02bNkXTpk1jzz33jF69eu2S9+XGjRvj008/jcWLF8eqVatiw4YN0aBBg2jcuHG0bt06OnbsGPvss09ad0BVR8uXL49p06bFggULYvXq1ZGTkxMNGjSIpk2bRvPmzaNLly6x3377lXmeJUuWxPvvvx+LFy+ODRs2RP369WOvvfaKww47LA444IAyj5+bm5sSMI8fPz569eqV1DZv3ryYMGFCfPPNN7F9+/Zo1apVtGnTJo455pgy3XFbFeTm5sann34aM2bMiFWrVkUikYjs7OzYf//9o1u3bil/PAAAUJEEZAAAAGSckgRk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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">regplot</span><span class="p">(</span><span class="n">y</span><span class="o">=</span><span class="s2">&quot;PRICE&quot;</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="s2">&quot;RM&quot;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">bos</span><span class="p">,</span> <span class="n">fit_reg</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
            <span class="n">scatter_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;color&#39;</span><span class="p">:</span> <span class="s1">&#39;C0&#39;</span><span class="p">,</span> <span class="s1">&#39;alpha&#39;</span><span class="p">:</span><span class="mf">0.3</span><span class="p">,</span> <span class="s1">&#39;s&#39;</span><span class="p">:</span><span class="mi">60</span><span class="p">},</span> 
            <span class="n">line_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;color&#39;</span><span class="p">:</span> <span class="s1">&#39;C1&#39;</span><span class="p">})</span>

<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Number of Rooms&#39;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Median Home Value ($1,000s)&#39;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Number of Rooms vs. Median Home Value&#39;</span><span class="p">);</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABtAAAARNCAYAAADLpgS5AAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAewgAAHsIBbtB1PgAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMi4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvhp/UCwAAIABJREFUeJzs3XdUFNf/N/D3AirSFAwoYgE1ttijYolobLHFgsaGgiUmJho1MZYUNcYkamJUNCZGvzas0Z8l9lhiIYKAJWoUCwoKiPTeyzx/eODZ2dlddpZdmu/XOXsOc5lbdnZ2ZnY+c+9VCIIggIiIiIiIiIiIiIiIiIgAACZl3QAiIiIiIiIiIiIiIiKi8oQBNCIiIiIiIiIiIiIiIiIlDKARERERERERERERERERKWEAjYiIiIiIiIiIiIiIiEgJA2hEREREREREREREREREShhAIyIiIiIiIiIiIiIiIlLCABoRERERERERERERERGREgbQiIiIiIiIiIiIiIiIiJQwgEZERERERERERERERESkhAE0IiIiIiIiIiIiIiIiIiUMoBEREREREREREREREREpYQCNiIiIiIiIiIiIiIiISAkDaERERERERERERERERERKGEAjIiIiIiIiIiIiIiIiUsIAGhEREREREREREREREZESBtCIiIiIiIiIiIiIiIiIlDCARkRERERERERERERERKSEATQiIiIiIiIiIiIiIiIiJQygERERERERERERERERESlhAI2IiIiIiIiIiIiIiIhICQNoREREVOlMmjQJCoWi6DVp0qSybhIZWX5+Pg4dOgQvLy+88cYbqFWrFszMzLgfEBFVAKdPnxYdr83NzYvNs3HjRlGe5s2bl0JLiYjks7KyEh2vjh8/XtZNIiIiHTGARkREpMX27dtFP3YKX1ZWVoiOjtarzLS0NEl527dvN2zDiV4h//33H1q3bo2RI0fCx8cH9+7dQ0JCAvLz841WZ69evdQeG9S9rK2t4eTkhHbt2sHLywve3t4IDw83WtuIyLjq1Kmj9rtuampqkO929+7dNR5Prl69aoB3QKRZVlaWZL+bPn16icvt0qULA56vqH/++UeyT33yyScGr8ff319Sz2effWbweoiI6NXCABoREZEe0tPTsWzZsrJuBtErLywsDD179kRwcHBZN0Wj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bRrS09N1zuPj4wNPT89SG5I3MzNT9rlZ2cWLF9GpU6cS79dLly7FnDlzdDquKOdRHfruVXH48GH06dMHjx49kpVPEATs3LkTvXr1QkxMTInqHzVqFNLS0nRaPzExEUOHDsXjx48BvBzysX///jh69KjOdR46dAizZ8+W1c7k5GQMGjQIK1askH1dkJGRgZkzZ+Kzzz6TlU8f48ePlwyLun37dtnl/N///R9SU1NFaZrOScoSEhJk/R5QtWPHDvTu3btS/+a7efMmOnfujJMnT8rOGxoail69euH48eNGaBkRUeljAI2IiKgEVqxYIVoODw/Hhg0byqg1pWPBggW4ePEigJc3ZpctW4agoCBER0cjISEB169fx8KFCyU/jDdv3ozLly/j/v37mDBhQtFNoyFDhmDfvn148uQJkpOTER4ejgMHDqBTp06i/JmZmZg+fbpebX727BkmT55cdIOuVatW+OWXX4rmXAsPD8eZM2cwdepUyfwvZ8+exccff6xzXe+//z62bNkiSrO0tMT06dNx5MgRPHnyBElJSYiJiUFQUBB++OEH1K1bV7T+kSNHMG/ePL3e68SJExEREQEAsLOzw1dffQVfX19EREQgKSkJ9+/fx65du9C1a1e9ytckMjISAwcORGxsrCjdyckJ3333XdH8b9HR0QgMDMTXX3+NWrVqidYNCwvDgAEDkJSUpLaOwYMHY8GCBUWvVq1aif7fqlUr0f+VX2+99ZZB329JRUZGSgIRDg4OqF+/vs5lfP7559i1a5coTaFQYPTo0fjzzz8RGhqK5ORkPHr0CLt370afPn0kZSxduhS//fabTvUlJSVhwIABePr0qSi9Vq1a+PrrrxEQEIAXL14gLi4ON27cwHfffQcnJyfRujExMRg4cGDRPipHTk4ORo4cWbSPvfnmm/j9998RHByMxMREREVF4ezZsxg5cqQonyAImDFjBlJTU7F582asX78ewMv5LGfOnInz588jIiICycnJePDgAdatWycJZN6+fRs///xzsW387LPPJO/tzTffxLp164q2T2pqKuLj4xEWFoYLFy5g/fr1cHd3N+pccao3FAvn55JLdZ6uZs2aoXv37pL1cnJyMHXqVNGDAAqFAsOGDcPOnTtx+/ZtxMXFIS0tDTExMXj48CGOHz+OH374Ab169arQ88FNmjRJtKy6zVQdO3YM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E1q0aAFnZ2eDnIsyMjKK5v2MjY1FtWrV0KBBA7i6upaoV5whxcfHF80Hl5ycjGrVqsHR0RFt2rRB69ateR1VjkVHRyMgIAAxMTGIi4tD1apV4eDggIYNG6JLly6lHpgtz9LS0hAQEICoqCjEx8cjNTUVFhYWsLGxQYMGDdCiRYsyCw6VB+Hh4bhy5QpevHiBtLQ0WFhYoH79+mjfvr3sXo/GlpSUhMuXLyMiIgKJiYkwNzdHw4YN0bVr11LpHRcZGYkbN24gLi4O8fHxouuaJk2aoEWLFrC1tTV6O4iIShMDaERERERERERERERERERKKtcjzkREREREREREREREREQlxAAaERERERERERERERERkRIG0IiIiIiIiIiIiIiIiIiUMIBGREREREREREREREREpIQBNCIiIiIiIiIiIiIiIiIlDKARERERERERERERERERKWEAjYiIiIiIiIiIiIiIiEgJA2hEREREREREREREREREShhAIyIiIiIiIiIiIiIiIlLCABoRERERERERERERERGREgbQiIiIiIiIiIiIiIiIiJQwgEZERERERERERERERESkhAE0qlCysrJxPyQMWVnZZd0UIiIiIiIiIiIiIiKqpBhAowolLCIKE2ctQVhEVFk3hahUxCUkYdOuw4hLSCrrphBRBcHjBhHJxeMGEcnBYwYRycXjBhHJVV6OGwygERERERERERERERERESlhAI2IiIiIiIiIiIiIiIhICQNoREREREREREREREREREoYQCMiIiIiIiIiIiIiIiJSwgAaERERERERERERERERkRIG0IiIiIiIiIiIiIiIiIiUMIBGREREREREREREREREpIQBNCIiIiIiIiIiIiIiIiIlDKARERERERERERERERERKWEAjYiIiIiIiIiIiIiIiEgJA2hEREREREREREREREREShhAIyIiIiIiIiIiIiIiIlLCABoRERERERERERERERGREgbQiIiIiIiIiIiIiIiIiJQwgEZERERERERERERERESkhAE0IiIiIiIiIiIiIiIiIiUMoBEREREREREREREREREpYQCNiIiIiIiIiIiIiIiISAkDaERERERERERERERERERKGEAjIiIiIiIiIiIiIiIiUsIAGhEREREREREREREREZESBtCIiIiIiIiIiIiIiIiIlDCARkRERERERERERERERKSEATQiIiIiIiIiIiIiIiIiJQygERERERERERERERERESlhAI2IiIiIiIiIiIiIiIhICQNoREREREREREREREREREoYQCMiIiIiIiIiIiIiIiJSwgAaERERERERERERERERkRIG0IiIiIiIiIiIiIiIiIiUMIBGREREREREREREREREpIQBNCIiIiIiIiIiIiIiIiIlDKARERERERERERERERERKWEAjYiIiIiIiIiIiIiIiEgJA2hEREREREREREREREREShhAIyIiIiIiIiIiIiIiIlLCABoRERERERERERERERGREgbQiIiIiIiIiIiIiIiIiJQwgEZERERERERERERERESkhAE0IiIiIiIiIiIiIiIiIiVmZd0AqhziEpIQ/CgM8YlJSExOhaVFdbxmWwMN6zuiccN6Zd08IiIiIiIiIiIiIiIinTGAVgkMnTQXUTFxJS7n+wUfoX/PLjqvLwgCjp65jD/PXMZ/9x9DEAS169WvWxv93FzhOWoQLC2ql7idREREREREREREREREyEkHMpMA6zqAialBi2YAjfQS+uw5lq39H+7cf1zsuuHPo7F131EcP+uLBTO94ObavhRaSERERERERERERERElVJOJpCVBORmAlAYpQoG0Ei2J88iMX3BciQmp8rKFxOfiPnL1uHbeR/K6ulGRET0qisoEJCUmYvUrFykZ+ejQBBgolDAspoprM2roGb1KjAxMc7FIhEZFr/PpYvb+9XEz710FAgCEtJzuJ1fQfyOGV5x29SmmhlSsvN02ub6fD6FeZIzchCdko3U7Fxk5xagWhUTWFWrgjo1qqFG9aoG/2y5L2lmjG3D7W18mrZx9SomKABgogAycwq47UsqNxvISgRyMgCh4GWawrA9zwoxgEayxCcm46MvVsoOnhXKLyjA4lWbULOGNTq3e8PArSMiIqpcsnLzEZ6QgcikTOTlCygQBGTm5kMQAIUCqF7FFCYKBcxMFXCqWR317SzKuslEpIE+32fzKsb5Efgq4PZ+NfFzLx3ZeQWIzQKuhibBwiKH2/kVwu+Y4RW3Tc1MFIhPy0HS/2PvzqMkS+/yzn/vvXEjbmwZkZGVtXZVd/Xe6m61pG5AQlibBY0AIQkQskBGsg1jMzY2Y3vGGI/NwTNjmzkew9iYOZbhWBIWYDYZjJGEQQsgCYS6W91q9VKt3jIrKzOrKiNjvfsyf0RmqpZcKyNyfT7n6Bx1Rtw33njf+2ZlxpPv+/Mi6kWbRiVPkmarjvlkpUAGXO4FW/rdYbrp8tJCn9mWz+VegBcNPvSPkhTbNDFNg6JtcaRS4HjN4eyR8rbnVvfS2kYxNhrv0VtrjIM4pdUP6QUxaTYI0MqFHI1ynnzO1NhvVRwOdpwFfciSHXlJBWgHWGO8tqXnF/L5DZ/zc7/4qzQX26s+VnQKPPym13L29EkWWh3+4DN/xtylheuelyQJ/+rnP8yv/X//F3nb3lIfRUREDouZlse5+S5BlNDshyy6Ef7SLznLDAMc22K8ZONHCedbHpOF1WuSisjuudH1fOexKqfqqiG8VRrvw0nzvjNmWh5fmmrTDA3mOj5RN9E4HxJaY8O30Zh2/YimG2IaBgYZGZBm0CgVqDqDj3SXx9wgww0TMKBk58hgw/l5/HwLMAjjhGfnurS8kI4X4UXpSkgHgxCvmLcYKw52yVzuBduaW91LaxvF2Gi8R2+tMe54Mc1+QJKmeFFCnA7Wk5OzyFkGjXKesaKtsd+AAZBE4LUh6O5YcLZMAdoB9smP/tuhtvflr57jE5/+wqqPNcZr/Ief+cfcctOJla/98Hvfwd/7p/+ax7567rrnT1+Y56O//Qn+2nvePtQ+ioiI7HdpmvHUbIe5ts9CP+RCyyPLMmpFm8lKAcc2sQyDJMvwo5SuHzHX9pnvBJysF1nMIuY8gyxTkCay27a7npMkY7Efcu/JMQxDR7psRON9OGned8aV43y5FzLvGYx3Q040ChrnA05rbPg2GtN8zmCu5RPECQXL5GJ3sCvMyVkcG3PI5wbHvp2sF/HChK9d7DHX8fGiwYfKxZzF8XqBO45WKdrWdfMz2/L4ykwb2zJp9gehWc4yiOKMfM7kxFieUj5HzjJIkox+FNPxYhb7IT0/otkPOTtZIY7TLc1tlsEz8z38LNC9dI1RrDOt3dFba4zHHJsgTsjnDKqOTbMfYBomTm4QgmdkjDmDHWimYVCwDI39GqolBzNsQ7sFabwrfVCAJpv2W7//qTUf+3t//T1XhWcw2JH2z/7+j/B9/9NPkCTXJ8O//fuf5gPf/12H/huBiIjIlZ6a7TDb8phquiy6ERPlPMdrDrZlXvfcUh4a5TxRkjLb9pluutjEdCJ49mKfyYnxXXgHIrJsu+u550crYfh9p7Z2usRhpPE+nDTvO+PKcb7Q9ilaGXceLdOola97rsb5YNEaG76NxnRqwaUbxLSXdoOdrBcZc3K0/ZieH2N5ULBMLvcCjMygkDMp5ExaXoSRwXjRxrEsekHMRLmw8rrL85OkGRe7AU/MtgiihELOpFSwOdMoMV6yscyr57ZOnuNj2VLYFuJHKV+b7+IGMd90tgFsbm7nfYMjnYBWGOpeusYo1pnW7uitNcYX2h5pktHxInpBQr2UX1lbSTpYSy0vIkpT8paJadjcc2JMY3+lNMWKupTCy2RuE3LVXeuKAjTZlL7r8ZnPP7LqY+Wiw1vf8I2rPnbTiaM8eP/dfPHLX73usblLCzzyxDM89MA9Q+2riIjIfjXT8phr+0w1XdpexC0TJeqljY9Yti2TM40SY06OZ2aaLIYGF7shMy1PRz+I7JJhrOeppstU08UwDMbLea3ndWi8DyfN+864dpxP1x06ecit8iHslTTO+5/W2PBtNKYLvYCmG3KpF+AGCUerBcqFwce3kxWLkm1xqRdAL6AbxICBF8UEUcodkxUALvWCwXMMg0ohZKJ8dfsdP6YfDo7wi9MMI8mYsC0KOfO68GyZZRpMVguU8haXugGmAXMdn6/MtDc1t3OdgG4E51s+iZHTvXSFUawzQGt3xNaat4V+yGI/4lIvoB9evYbh+rV0iQDDGOwq1dgz2KoadMBvkfWb+G4Pdvl0nfV/2hFZ8qXHn8YPwlUfu/+e29etZbZeQPbHf/7otvsmIiJyEPhRwrn57uAHbjfiTGNzv+RcqV7Kc1PdwY9h0Y04N9/Fj3b2fHARGd56PtMosehGLPRDred1aLwPJ837zlhtnMeKW6tlrnHen7TGhm+jMY2SlAttn64f0Q8SJq/54B2gXMgxWSnQ9mLOL3qcb7l0vGjlucuP94KErh9zoeURJulV7bfckPmOT6WQo2jnyJkmWTbYFZOk6brvoVzIMVktkGRQtE1evNxnruOvO7d+lPD8ZZd+DB0/1r10hVGss6/OtPnqTFtrd4TWmrcwSbnQ8uj6Mb0gYbJy/RpetryW+kFC14+40PaJkvTwjn2WDeqbtc9D/zLE0a4HZ8sUoMmmPPP8S2s+dvvZ0+tee/staz/+7PNTN9olERGRA2W66RJECRdaHo1yfsu/5CwbK9qUchlznYAgSphuukPuqYhsZFjruV7K0yjnudDytJ7XofE+nDTvO0PjfHhp7odvozG91A2IkoRmP6SyFIatplzIgQFtL6TthhgYVz23XMhRcXI0+4P2LneDq9o/v+hSsAzCJGWsZDNWtOkGMUma0vY2rjFULuSoFHL4UYpjWzwz21l3bqebLmGc0IkM6kVb99IVRrHOZhZdzi+6WrsjtNa8XV5ZwwEVZ+01vGx5LTX7IVGScGlprR66sQ970LkAvUsQB3smOFumIxwPsJ/61/+BZ55/mcsLLfqeT6XkUK2UOXvmJPfffTtv/uYHueX0yU219ezzL6/52LEjjXWvPTa59uPPvagATUREJE0zZloezX5IlmWcqDnbaq9qs/JXpI7tcdtkBdNUzVGRnTDs9Xyi5tByQ63nNWi8DyfN+87QOB9emvvh22hM06Wf3bt+TJYN6lGtJcsyLAOCeLBbzDAYfOBsfH1MGyWbfhDT9WNsK+TYWGGphlmMGyY4tglJRjVvAQZBlOBGCTk/YrxkYxjrz0+jnKcfxNiWScePuNwLcGzrurldft+LbgTAseqNhTnLDtK9NIp1ttgPeXnBBQOqhZzW7gisNW9ZlrGwvIYZrMHNWF5LXT8mb4UcrzmYhnE4xj50wW9B5EO2/u7X3aQdaAfY73/q87zw8gydXp8kSWh3+5yfvcif/PmX+YUP/ybf/7d+kh/7p/+al6YvbNjW+dmLaz7WqI+te+16j3d7Lq1Ob8PXFxEROchaXkScZCy6EbWivWph562wDBhzciy6g3ZbXjSknorIRoa9nm3LpFa0tZ7XoPE+nDTvO0PjfHhp7odvozHtBzFxmtHzE0oFC2udD8r9KAW+/rhhGHjx1R8+W6ZJOW/RCxKSNONiLyROM5puRD5nESYZhZyJaZqYpkHBNvHDlCQDP974uDjLNCgVLLwwoWhbzLb9Ved2+X23vBjHyjasnbiRg3QvjWKd2TmTthfT9mLyOVNrdwTWmrdeOFhrvSChnLfWrCd4reW11PMT4jSjHwx2gR7osY986M5Cd24Qou3h8AwUoB1qWZbxZ498hff93Z/i9//oc+s+t9/31nys6Kz/1wxFp7Du473+Ad+GKiIisoGuH5GkKX6UUHW2VldkLeVCDj9KSLOMrn+AftgW2eNGsZ4rWs9r0ngfTpr3naFxPrw098O30Zh6S2MTpSlF21q3rTBJydIMg0F4lmUZ4Sqhl2NbRElKlmW0+gFpluGFEbYJSZpRsL7+OnnLJMmypbY292F20baI0pRCzqTrxavO7fL7DuKUwpA+hT4o99Io1lnOhCBOCOKE3CYDnI0clPEelrXmzQtj0iwlSlKK9tYO/VteS1mW4V1R7+zAjX0cQG9+cFxj0N/zwdkyHeEoBEHIT//sf6RUdHjTNz+46nP67toBWn6Dbwp5e/1/BNZrey2tdpfLzdaWrxPZb5qLbVzPp7nY3u2uiMgIzVzqc7nl4no+Udmkk934D8fdXp8gjIgDH9eHS4smFSuhbByAH7hF9oFhrudlcZTgev7I1vN+/nljP463bJ/mfWesNc7LP2t0e/0tt6lx3h+0xoZvozFdaPt0+gFBEJIWDDx/7V1gXTfEDWPSNMUA3CAkb2bkjas/jE7ilCAIafcNOsbglEc3iLFNiKKExDYIw8HrpGlGFMW4gbFqW6tJl9r3c4PQ7dJi97q5XX7fnueTxjf2feNaB+VeGsU6c/0ANwgB6Hs+nd72Q7SDMt7Dsta8LXS+vobjgoHnb1xPcFl6xVp1zBTHGKzLgzD2hgFGmmCEbQh6ZMnmx6Xd6eL5Ae1Od3OvZeUYH7/Rnq5NAdoBVsjbOE6BvusRb7D9Ok0zfvpnf5FX3XcX9bHKdY/7S998V2NZ6/9lTC63/uOeH6z7+Go+9bkv8cTTX9vydSL7jev5PP3ciwCUits7u1pE9q45z+CyDwuBQXM6I7eN33OCMGL6wjxxCu00z6WpjOcdeLK4twrxihxUw1zPy+IULvrGyNbzfv55Yz+Ot2yf5n1nrDXOyz9rwOBzh63QOO8PWmPDt9GYLobQCQ26kUH38qDG2Vp6MbixgZsMQjG/C4s5uJS7ekyTDNqhQftSNjjxMYOLgYEFBCl4na8fTZYC/Rj6bVjMZVzaxCfGy+03cxlxBunCzHVzu/y+5/opfvMijzyx9e8b1zoo99Io1tll32DGHdw8Rnue+SH8WHdQxntY1pq3xdCgE7KpNXytK9fqXD5jaqlU4H4eezuXw8lbFPEh6BIFPmm6tR1nnh/w/MvngY1PuAMoOEXeeebeG+rvehSgHRCWZfHq++7ida+5j1e+4g5uP3uaSqkIQJqmPP/yef77H32OX//dPySKV096e32XD/36f+PHf/i91z3mFPL0PX/V6+INkuO1Xm/ZZhbAtd7y+oe4/ezpLV8nst8s/yX4d7zlm2mM13a5NyIyKucu9nnxsssLCy63HilteGzLepb/qvPee+7kog+3TpQ4e6TEnUfLw+quiKxjmOt5mRclvHDZHdl63s8/b+zH8Zbt07zvjLXGeflnjQdfeTfVytbGSeO8P2iNDd9GYzrT8pnvBsx3Ao6PFcivk6Ys9ENaXszlXogBTFTy1Is2E+Wrg6kgTpnvBBwbK2As7UAzLrnYJvSChHrJxl6qtRalGS03ol6yV21rNWGcMtcJGC/bhHHKN5ypXze3y+/7q+ebLOaTG/q+ca2Dci+NYp29sOCSXRjs1rn3RJVbj5S23eZBGe9hWWveZto+851gZc0VtpCILq+lY2MFjlULnKoPks/9OvYmGUbYhaBDFkfAjQV/yzvP3vi6V1Mbq274fMMaTdSlAO0A+Ft/9Xt47YP306iPrfq4aZrccfYMP/7DZ/jWN3wTf/sn/+81j038wz/54qoBWrlUXDNAi6L1d7eF0foBWnkp6NuKeq3KkUZ9y9eJ7EelokNjvKZ7XuQA62c2vcRizk2x8w5j5fy22ivkbXIFh5IBk+NVTk1WOdLYHz9si+x3w17PAFEvoFRMR7qe9+vPG/t1vGV7NO87Y71xLuRtqpUyY1v8IFzjvD9ojQ3fRmPqZxZ+atIKMsycTXGdmljVzCJMA0w3BsOgVMhTLeUpOle3GfsRhUJGrVzEsU38KKXUCSEzsFMDy8yRzw8+/E/CGNvO1mxrNcvtO3kbJ2+sOrfL77u44NLO3dj3jWsdlHtpFOus1E8oOwEZUC462x5rODjjPSxrzZufWfjJYA3ncnmKzuZjlyvX6kStyFhlEKDtu7FPUwg64HcgF0POAba3DbLoFKiNVWnUVs89rmJsP4RezZDKN8pu+o6//Po1w7Nr3Xvnrfydv/buNR+fv9Tk5fNz1329XF475Nqohpm7weOVGwjQREREDpKqY2MaBo5tDa04cD+IcWwL0zCGVpRaRDY2ivXc03pek8b7cNK87wyN8+GluR++jca0aFsYhoFtmngb/KF63jIxDIMMyLIMwzDIr1I+xY8S7KXn1ssFDMOgmLeJ0gzLNAiSr79OmKRYhrHU1uY+LvaiBNs0CeKUajG36twuv+9CziTY2ultazoo99Io1lmcQt6yKOQs4i0el7eWgzLew7LWvBXzucEatky8DTaTXGt5LRmGcdVOxH0z9lk2CM0656G/AMmN7zrbixSgHULf/uZvxjLXnvq5SwvXfe2mE0fXfH6z3Vn39ZqttR+vVkrUaxtvwRQRETnI6kWbnGUwXrJpexFRsr1fdpIMOn7MeGnQbr24h3/YFjlghr2eoySl7UVaz2vQeB9OmvedoXE+vDT3w7fRmJYLOXKmQcWxcIOEJF37w2fHNrnyw+ksyyheE3olaUo/TKgULCzT4GglT840aJRswjghbxkEcUqapqRpRhClOHkTywBnlTDuWkma4QYJxbyFFyWcqDmrzu3y+64Xc/iJQax7acUo1lkUp9SKOWrFHGGcau2OwFrzVskP1lqlYNEPE5JNBpjLa6niWORMg3JhsHNt34x90IPODPQvQRxykIKzZQrQDqFKqbhuaLV8vuiV7rrt5jWfP3+pue7rrff4HWfPrHutiIjIYWCaBqfqRRrlPIZhMNte/djkzepGYBgGjXKeU/UiprmFCsYisi3DXs+zbV/reR0a78NJ874zNM6Hl+Z++DYaU3NpfKpODsOAZj9csy3DMEgyKORMCjmTLAOMq8e06UYYQNXJMVHOY5kmjXKesWKOUt4iXQroumFCN4jBgJJtUXFsDGPj+Wn2Qwxj8CH/mGNzpFJYdW6X3/d4afDh/3x37fe1GQfpXhrFOjNNg5snSpxplDBNc0ttpllG14+42PWZbrq8vNDnsekWbS8ib5mcqDn7eryHZa15MwyDieU1zGANbsbyWqo6ORrlPObS+tvz93rYh/YM9C5C5A92oR1QCtAOKd8P1nysULj+zN27b7tlzec//9L0uq/13ItrP37XbQrQREREAE43ShRsi5P1Is1+SMu9sV8uO16EGxscHytQsC1ON7ZfOFpEtmZY67nlhjT7ISfrRa3ndWi8DyfN+87QOB9emvvh22hMJ6sFbMuiUc7TC2L6werHwPWDGDKoFfPUSnkysque2w9ien5Mozxo70i1cFX7N42XCJKMvGXScSM6XkS1kMMyTWrFjes29YN46Wg5Ez9KuPvE2Lpze7pRIp+zGLMzWl6ke+kKo1hnp8ZL3DRe2nSbUZJyoeXx1IUOz1/qM7PocaHt8fzFHi9d6pMB04seU02X5+a7+BscMXoYrDVvR1bWcIGev/YaXra8lhrlPLZlMbm0Vvf0vR560JmF7jxEHmRDOpt1D9t8NTvZk5bPOt6KZ59/mb639l8gHBmvXfe1hx64B6eQxw+u/6b7lWeeJwhDCvnVi13+xeNPrflab/im12yixyIiIgefY1vceaxKkmT0/IippgtAvbT5YtItN+R8y8fJwXjJ5s5jVRx7NIV0RWRtw1rPU02X8ZLNRDmv9bwOjffhpHnfGauNc6OwtTY0zvuT1tjwbTSmtmVysuaQpBlelHCpO/jj9+Uj3WDwgfulXkCtmFsaSwMvileeC3CpF1ApWFSdHCfrRfKWeV37x8YcppsuXhSv1ElrLO1UW08/GLyWZYAXpdx6pMzxMWfduXVsi9uOlCjnYMzJ6V66wijW2T0nxwB4+kJnwzYXegEX2j5RktD1Y3p+QpSmeGFCx48o5Eya/ZCibXGpG5CkGedbHnceq3KqXhzCCOxP683byXqRJM3wo8FahavX8LLltVQuWFQdm5M1B9sy9+69HgXgL0LoHorQ7EoK0Pa5H/yxf8bffN+7eONrNxdEpWnKv//Qb6z5uFPIc/vZ09d9vVwq8sbXPcgnP/OF6x5zPZ//8cdf5Lve+i3XPfby+Tm+/NVnV32t45MTPPjKuzfVbxERkcPgVL3IYj8kyzKmmi4vzZjbpAAAIABJREFULbg0/JgTSz9MryVKUmbbPs1+SNXJMZ7POFrNH+pfakR22zDW83jJ5kyjxPGao/W8AY334aR53xnXjvN0s0srZMNaRhrn/U9rbPg2GtOJSoF+kJBlGZcIuNgNqIQJtWKOtj/YWVYpWExWCoxX8hiZwUI/YC71ee5SDzI4PlYYPF4efAB/pYlKgbYXUc5bGAbkTIO8ZeBFCX6cUkrTVUO0JM1o9kM6Xkicgm0ZnKwXuf9UbVNze3ysQNWGm+oOrdDQvXSFUa2z9dpMs4zzTY+mG9L1I5r9kCwb1NeLU7BMgzPjg2MKi4UcNcdmru0z3wkGAVGSsdgPuffk2JY3dhwU683beNkeHGnYW1rDUUKjZGOZ5spa6gUx5aW13CjlGSvaTDXdvXevxyH4LQj6kB3O3YcK0Pa5516Y4h/+8/+X226+iXc8/Ebe9ubXrVnfrNXu8i9//kN84ZGvrNne6x585Zo7yb7vO9+yaoAG8O/+069z3923cctNJ1a+5no+//xn/+PKucrX+p7vePOh/SYrIiKylnuX/mLQMAwqTsiFlkfLDakVbSqFHMW8hWUYJFmGFyb0gpi2F2EYBqcbJewsom3DXUfLu/xORGS763minOd4zVlpR9an8T6cNO8748pxJol4NjE4d7HPidjUOB9wWmPDt9GYTlRswjghTFKSNGO27fHC5QQnZ3F0zGGsaFN2chypFOj7EW1vEICEcUKWwcVOgGnCeDlPL4iwTfOq+en6EaZp8Mqb6kuhWETOMriw6HG5GzDmDObVtkziJMONYjpeRJRk2JZBKZ/j7GSF+0+OcaJe3PTcHnMyjo0VqGW27qVrjGKdrddm24tww5jFfkQ3iCnkzMGRnHGKAZyoFQd/mFkeBDkGxkpgN9106fkR2VLNq/tOXX+S2WGx1hiPFW1My2CsOAjNmv2Ay90A0xjUmrMtk4lygVLBwjIN0izl6dnO3rrXkwi8NgTdQxucLVOAdkA8//J5/s0HP8rP/eKvcPstp3nlPXcwOVGnUi7S7bk8+/wUn3/kCYJVjmBcZpoGf+O9373m46+6904eftPrVg3Rmottfujv/hTf/ubXccvpkzQX23ziM19g/lJz1bZOnzzGD7zr4a2/URERkQPOMAzuO1VjvJzn3HyXWjFHsx+y6Ea0PO+q2ryGMTg+4njNoVHOU7AtJgt5Lhe3fsSziAzfdtfzYT8eZ6s03oeT5n1nXDnOfdflWHGw292PU43zAac1NnybHdMwTgmTlPFyngYZGRAmCWGco+1GTDc9ekGEZZrUizls0yAzoJCzCOOMx6ZbGEDVsRlzctg5E8e2BqHXqRq9IAYMwjjh2bkuLW8Qps12fJI0W+lHzjQo5i3Gy3nqRZu7jlc5US9ueW4NA+4+ViEwC7qXrjGKdbZWmy8vuMwsBT1+lFIr2mRAkg3KAFSdHLY1qO915Q5G2zI50yitHMM51XQxDIPx8uE9+WS9ecsyCONsEFgbkGYpYTJYTwYGHX8QXDu2RZBke+deTxPw2+B3IF2/htthoQDtgEnTjHMvTHHuhaktX/uD73obd91287rP+V9+5L38xeNP0VxsX/eY5wd87OOf2fB1LMviJ/7O+9fc6SYiIiKDIyEmynmmmy6O7XG06pBmg3oIWTb4xaloW5iGQc4yOFUvcrpRotft7nbXReQaN7qe90S9g31I4304ad53xql6Ec7UePLLGcfHHEqlksb5kNAaG77NjGnONFjohbS8iHrRplHJc6kbMNv2KeZNTMOmHySD8KMy+JzNDRLiNCNnGis7izLgZL3IZKVw1fwATDddJqsFZls+l3sBXpSQZhlRkmKbJqZpULQtjlQKHK85nD1S3tbcHsZ7KU0zWl5E14/oB4PxNQ1jpf5VvWhjmsZIxubKNk2jz3wnoFHOE8YpZxp5yoUc+aU6eJZpMFHOc6RaWKmdd63lWmovLbhUnJBz810myvl9PT/btd68BXFKa+nIxjQD0xjURGuU8+Rz5t6519MUgs7guMYkAVY/Ue4wUoAmALzj4TfyY3/9+zd83sR4jV/4F/8bP/oT/4rF9tY/oDNNg5/+Bz/CN77q3hvppoiIyKHi2BZ3HKty22RlU79wAfR2uc8isrobWc9y4zTeh5PmfWcUciaTDrz2bJ2cU9Y4HyJaY8O32TEdK+Ro+RGPTS3CUq2qy92YnGVwdrLMsWph5Zi/OM1YcEMWegHNXogXJlTHbLIso5S3+KazDawrwpErX7/thsx3ArpBRBClFGyTSsHmeK1ArZgf2twelnvJjxKmm4MdX3GSbToMG/bYLLeZphkdP6LlhpydKHO0VsDEoGCbFPM5KnlrUyeZ1Et5Gn7MhZZHrZhjuulyx7HVSwodFhvNW9E2SRkEaF6Y7p17PcuWgrM2xBEKzq6nAG2fu+PsaZ57cfqGr69WSvz4D7+X7/62N2z6mttuvon/8DM/yT//2V/kyWef3/R1kxN1/tHffj9vfO1rbqSrIiIih5ZpGjTKeRpl7d4W2e+0nneWxvtw0rzvDNPQOB9WWmPDt5kxnWv7kA1qKKUp3HG0wvGag33NTqECgx0uZ8ZLK3Wrmv1BkNYPYp6e615Xt+rK1z87WRnFW1zVQb6XZloe5+a7BFGycqyfvxSeLVs+jnG8ZONHCedb3srxfcMemzTNmO34hPHg2MZ7Toxdd+9sxYmaQ8sNafZDHNvjtsnKvg47h2Xf3NNZBmEPvBYkIVfdmHIVBWj73K/8+/+TF6Zm+KM//Qu+9PjTfPXZ5wnCaN1rDMPg9ltu4rve+i1851u/hVp16/8wnj1zkl/6f/53/tv/+BN+55Of5clnX1gpHnmtU8cnefiNr+WH3v2dlEuH80xcERERERERERGRGzHT8phr+0w1XdpexC0TpZWj9NajulU7L00znprtMNf2WeiHXGh5ZFlGrWgzWSng2CaWYZBkGX6U0vUj5to+852Ak/UiSZKx2A+59+TYUOtat7yIOMlYdCNqRXtb4RkM7q1a0WbRjThadWh50d4PjWQg7IHXhjiALN3t3ux5CtAOgFvPnOLWHzjFj/zAO4mimPOzF5m6MMflhRau5xNGEcWiQ6VU5PjRCV5xx1kq5dK2X9c0Td7x8Bt5x8Nv5NLCIk9/7SUWFtu02l3KJYeJ8To333SC22+5aQjvUkRERERERERE5HDxo4Rz810WlnYxbTY8u5LqVu2cp2Y7zLY8ppoui27ERDm/6k5BgFIeGuX8yk7B6aZLz49WNilcu1NwO7p+RJKm+FHCZKUwlDYrhRwtzyPNMrq+ArQ9L3QHNc4iX8HZFihAO2BsO8fZMyc5e+bkjr7u5MQ4kxPjO/qaIiIiIiIiIiIiB9l00yWIEi60PBrl/JbDs2WqWzV6e3mnYD9I8OOUbKmG3jAU8xZZBl6U0A+SobQpIxD54C9C6Ck4uwHDWS0iIiIiIiIiIiIiMjRpmjHT8mj2Q7Is40TN2VZ7J2oOWZbR7IfMtDzSVHWPhuXanYJnGje2U/BMo8SiG7HQH+wU9KPhBFNplq2UubKGdDTkcjvZUm0+2WPiAHrz0LkAQV/h2Q1SgCYiIiIiIiIiIiKyx4yyblWcZLS8aEg9laHuFCznudDyCKKE6aY7lP6ZhsFybpYMKexabscwBu3LHpFE0LsE7QvgdxWcbZMCNBEREREREREREZE95sq6VVXHHkqblUIOP0pW6lbJ9u2HnYLlgkXRtjAM8KPhBCpemGAYULQtygXV09t1SQz9BWjPgN+GTMdqDoMCNBEREREREREREZE9RnWr9of9sFOw6tiYhoFjW0MLTntBjGNbmIYxtIBXbkCagNuEznnwFiGNd7tHB4oCNBEREREREREREZE9RnWr9of9sFOwXrTJWQbjJZu2FxEl29uFFiUpbS9ivDRot15UgLbj0hS8FrSnwV0c7ECToVOAJiIiIiIiIiIiIrLHqG7V/rAfdgqapsGpepFGOY9hGMy2/W21N9v2MQyDRjnPqXoR09S9tGOybHBEY+f84MjGJAYUho+KAjQRERERERERERGRPUZ1q/aH/bJT8HSjRMG2OFkv0uyHtNzwhtppuSHNfsjJepGCbXG6URpK/2QTgi60z0P/MsQhCs5GL7fbHRARERERERERERGRq11bt6pRzm+7TdWtGr79slPQsS3uPFYlSTJ6fsRU0wWgXtr8fdVyQ6aaLuMlm4lynjuPVXFsBbEjF/bAa0McQDacMF02RwGaiIiIiIiIiIiIyB5zZd2qubZPlKTY1o0fKLZct+p4zVHdqiG6dqfgFvKoNY1qp+CpepHFfkiWZUw1XV5acGn4MSdqzrr3VpSkzLZ9mv2Q8ZLNmUaJ4zWHU/Xi0Pomqwhd8FsQ+QrOdokCNBEREREREREREZE9ZrlulR8lzHcCZts+Z7ZxXJ7qVo3GftspeO/JMQAMw6DihFxoebTckFrRplLIUcxbWIZBkmV4YUIviGl7EYZhcLpRYqKc53jNWWlHRiDywV+E0FNwtssUoImIiIiIiIiIiIjsQacbJc63PE7Wi0w3Xcac3JaO3Fu2XLdquQ6W6lYNz37bKWgYBvedqjFeznNuvkutmKPZD1l0I1qex5WnUBrG4OjH4zWHRjlPYekYSO08G5E4GOw4C/oKzvYIBWgiIiIiIiIiIiIie5DqVu19+3Wn4Kl6kYlynummi2N7HK06pFmGFyVkGStHSJqGQc4avMfTjZLunVGIQ/DbEPQgS3a7N/tTOppxU4AmIiIiIiIiIiIiskepbtXet193Cjq2xR3Hqtw2WaHlRXT9iH6QkGYZpmFQLlhUHZt60daRn6OQxEvBWRfSeLd7sz/FATzze/DYL8Pfe3zozStAExEREREREREREdnDVLdqb9vvOwVNc7DjbRj122QT0mQpOOsMQjTZuqALX/kNeOLXwF0Y2csoQBMRERERERERERHZw1S3au/TTkHZUJoOQjO/BUkCZBteItfoXYLHfwWe/C2I+iN/OQVoIiIiIiIiIiIiIvuA6lbtbdopKKvKsqXgrA1xhIKzG7D4Ejz2EXjm9yGNduxlFaCJiIiIiIiIiIjIoZWm2b6q/6S6VXuXdgrKVbIMwh54LUhCrroBZFOsy0/D534TXvg0uxE8KkATERERERERERGRQ8ePEqabLjMtjzjJ9t1OLtWt2ru0U1AGwVkb4gCydLd7s79kGfaFL/Km+Q9Sm3phV7uiAE1EREREREREREQOlZmWx7n5LkGUrOwQ8pfCjWXLO4TGSzZ+lHC+5WmHkGyadgoeUqE7qHEW+QrOtiqN4Wt/CI9+hOrlZ6lu5dqcM5IuKUATERERERERERGRQyFNM56a7TDX9lnoD2pUZVlGrWgzWSng2OZKjSo/Sun6EXNtn/lOwMl6kSTJWOyH3HtyDMNQ6CEb007BQyLywV+E0FNwtlWxD0//Ljz2n6Ezs7VrnRq88q/AK987kq4pQBMREREREREREZFD4anZDrMtj6mmy6IbMVHOc7zmYFvmdc8t5aFRzhMlKbNtn+mmS8+PyJa2qd13qrbT3ReRvSYOBjvOgr6Cs63yO/CVX4cnfg28xa1dWz0Br3ofvOIdYBfBGM3xpwrQRERERERERERE5MCbaXnMtX2mmi5tL+KWiRL10sa7gmzL5EyjxJiTY6rpMtV0MQyD8XJexzmKHFZxCH4bgh5kyW73Zn/pzcOXPwpf/W2IvK1dO3E7vOb9cPu3gmWPpn9XUIAmIiIiIiIiIiIiB5ofJZyb77KwVO9ss+HZlZaf/9KCS8UJOTffZaKcx7FHs/NBRPagJF4KzrqDml2yec0X4dEPw7mPb33sTr5mEJzd/PpBgcodogBNREREREREREREDrTppksQJVxoeTTK+S2HZ8vqpTwNP+ZCy6NWzDHddLnjWHXIvRWRPSdNloKzziBEk82bfXwQnL342S1fGp7+FvLf9MNw/P4RdGxjCtBERERERERERETkwErTjJmWR7MfkmUZJ2rOtto7UXNouSHNfohje9w2WcE0d25HhIjsoDQdhGZ+C5IEyHa7R/tDlsHLfwqPfAhmv7y1a80cwdm38kfuK3jtm95OozY2ki5uhgI0ERERERERERERObBaXkScZCy6EbWijW2Z22rPtkxqRZtFN+Jo1aHlRTTKN7ajTUT2qCxbCs7aEEcoONukJILn/mCw46z5/NautUtw77vgVT9IPynS/eyfj6aPW6AATURERERERERERA6UNM1oeRFdP+JrF3u8eKnHdNPl5kaJrh9RLuQwt1FHp1LI0fI80iyj6ytAEzkwsgzCHngtSMLBf8vGIg+e+hh8+aPQndvatcVxeOC9cN+7wVnabdbuDL+PN0ABmoiIiIiIiIiIiBwIfpQw3XSZaXnESUaaZXztYo/ZtkezF1IpWPTDhJxp0CjnmawWbmhHWjFvkWXgRQn9IBnBOxGRHRf2wGtDHECW7nZv9gdvEZ74dXjiv0DQ3tq1Y6fg1X8V7nk75LZ3tO6oKEATERERERERERGRfW+m5XFuvksQJTT7IYtuhB8lXOz6NHsRi26IaULRzlFxLMIkYaEfcrLmMFEpbOm1rKXda1kGqXaoiOxvoTuocRb5Cs42qzMLX/5leOq/DgLHrThyF7zm/XD7XwZzb0dUe7t3IiIiIiIiIiIiIutI04ynZjvMtX0W+iEXWh5ZllEr2kxWCpRsi6LtYxgwXs6TpBmL/YiWOzh6MUkz+kHC6UYRY5PHOiZLoZlhsK2jIEVkF0U++IsQegrONuvyc/DYR+DcJyHb4u7bm75hEJydfu3gm+c+oABNRERERERERERE9q2nZjvMtjymmi6LbsREOc/xmrNyNGOcpvSCmHzOpGBZVMo5knJGsx9yuRfiRQnZUiB2ZqK0qdf0wgTDgKJtUS5YI3tvIjICcTDYcRb0FZxtRpbBhcfg0Q/By5/b4sUG3PaWQXB27N5R9G6k9kyA5vsB5+cuMTt/mcuLLTw/IAhCcjkLp1CgWi5x4ugEJ44d4eiRxm53V0RERERERERERHbZTMtjru0z1XRpexG3TJSol/JXPaeYz2EYBrZl4kUxFSeHZRpMVguU8haXugGXCDAMg3LB2tRxjr0gxrEtTMOg6tijensiMkxxCH4bgt7Wd08dRlkKL34WHvkwzH9la9eaNtz9XYMaZ+M3j6Z/O2DXArRWu8vnv/QEX3riab567gVePj9Htsm0t1opc88dZ7n/rtt43UP3c99dt216e7WIiIiIiIiIiIjsf36UcG6+y8JSvbPVwjOASt7CMg0qBYtFN6KRpljmYHdauTD4ePRiN6BrR1xoG4wV7ZXda6uJkpS2F3G85pCzDOpFBWgie1oSLwVnXUjj3e7N3pdE8OzH4bEPw+JLW7s2X4b7vg8eeC+UJ0fSvZ20owFap9vnD/74z/j4pz7PV599gYzB1uit1tnsdPt88bEn+eJjT/JLv/Y7jFUqvPn1D/Idb3k9r7r3zhH0XERERERERERERPaS6aZLECVcaHk0yvlVwzMAwzCYKOeJkoSWG9F0Iyav2GVWLuSohAnNfki5MNiRdrJeXPN1Z9s+hmHQKOc5VS9imvrDfpE9KU2WgrPOIEST9YV9+Opvw5d/BfoXt3ZtaQIe+AG473uhUB1N/3bBjgRoz3ztJT76sU/w6c99iSge3KhXhmY3unlsuY12t8fvfPKz/M4nP8up40d5z3d/K9/9bW+g6Gy83VpERERERERERET2lzTNmGl5NPshWZZxouas+/wj1QIL/ZBGucDlXkDJtlZ2nwE0ynn6QUzXj8lbIcdrDuYqH1q23JBmP+R0o0TBtjjd2FzNtK1K04yWF9H1I/pBQpplmEtHTFYdm3rRVnAnspY0HYRmfguSBNjiDp7Dxl2Ax38NnvyNwS69raidhlf/ENz9nZA7eHnMSAO0R7/yDB/86Md47Mlnga8HXobx9dAsy1bfgZbP2zh5mzhO8MOINF39eMcr/x3LMjg/e5F/88GP8sH//DHe/fa38r7vfRuV0tp/MSIiIiIiIiIiIiL7S8uLiJOMRTeitsGRiwB5y+RkvUiSZvhRzKVeAHz9CEfLNCgVLHp+Qq2Y0Q/i62qbtdyQqabLeMlmopznzmNVHNsa6vvyo4TppstMyyNOMtIsw4sSsmzwOWhxqe5azjI4VS9yulEaeh9E9q0sWwrO2hBHKDjbQPs8PPbL8PR/gyTY2rVHXwGveT/c+mYwD+73oJEEaM8+/zI//6Hf4IuPPQmw8g3eMK4OzE4cneAVd97Knbee4bZbbuLYkQbHjjSo167f4heEIZcWFrl4eZGpmTmee3Ga516Y4qnnXiSMBrvargzlun2X//Rffpff/L0/5Ie+7zt57zsfxrZ3reSbiIiIiIiIiIiIDEnXj0jSFD9KrjqOcT0T5Ty9IBp8eNgLuNgNqEQJjZKNZZoUbQs3HOxo86JkJUCLkpTZtk+zHzJesjnTKHG85nBqnWMeb8RMy+PcfJcgGhwnuehG+Evh2TLDAMe2GC/Z+FHC+ZbHnceqQ++LyL4TdMFrQRJuvWbUYXPpGXj0w/C1P4Rs9Y1Lazr9TfDgB+DUN9z40YL7yFATpU63zy985Df5r5/4LFmWrgRnMLhn7VyOb3z1vbzpda/hoQdewanjmy8iV8jnuenEMW46cYzX3H/3ytfDKOKJp77GFx55gk997kvMzF0Cvv66nZ7Lv//wb/CxT3yGf/i33sfrv+GBob1fERERERERERER2Xn9IMGPB58/Ovb6u8+udGb5yEXDwLFjmv2AfhBTzg92doVxihvEtN0IyzDoBTFtL8IwDE43SkyU8xyvOdx7cmxo7yVNM56a7TDX9lnoh1xoeWRZRq1oM1kp4NgmlmGQZBl+lNL1I+baPvOdQa22JMlY7Ifce3IM4xB8oC1ylbAHXhviYOth0GGSZTDzF/DIh2H6z7Z2rWHC7W8dHNV49J7R9G+PGmqA9r0/8o/o9HrXBWf33X0b7/r2N/GW1z9EecjHKeZtm4ceuIeHHriHH/vr7+HZ51/md//gj/nEp79At++u9GNm7hJ//6d/ln/wN9/H97/9rUPtg4iIiIiIiIiIiOycNMtWNplYWwiNDAxubpSpFAZBVblg0vVjekGCF0VLNdWgHyW4UYJjWxyvOTTKeQq2NZLdXk/NdphteUw1XRbdaCWkW+1YylJ+UK9teVfcdNOl50dkS4Nx36naUPsmsmeF7qDGWeQrOFtPmsALn4FHPwQXn9ratVYB7nk7vPp9g1pnh9BQA7R2t7cSWJmmycNveh3v+563cfstNw3zZdZ1120387/+6F/l7/6N9/DxT32e//zbn2BqZu6qPoqIiIiIiIiIiMj+ZRrGyueQyQ0c1zZRzlN1clzuBthWSK04qI2WpnBsrMCJWpHbj1ZGXm9spuUx1/aZarq0vYhbJkrUS/kNr7MtkzONEmNOjqmmy1TTxTAMxst5HecoB1vkg78IoafgbD1JCM/8Hjz6y9Ce2tq1hSrc92544K9AaWI0/dsnhl4UzDRN3vnwm3j/u7+T40d3b3AL+Tzv/PY38Y6H38gf/elf8MGPfoyXpmd3rT8iIiIiIiIiIiIyHOWCRdG2MAzwo5RNZE7XyVsmJ+tFTtQcemHCbMulFyScaZS59UiZ249VqDo29aKNaQ7/aEQ/Sjg332Vhqd7ZZsOzKy0//6UFl4oTcm6+y0Q5P/SgT2TXxcFgx1nQV3C2nqALT/4WPP4r4C5s7dryJLzqB+He74F8eTT922eGGqD95dc/xP/8gXdz+uSxYTa7LYZh8Na/9I285fUP8bt/8MeofKCIiIiIiIiIiMj+VnVsTMPAsS26fkSjfAMJ2hLDMKgWcjRzFqcbJc4eKfPqm8e31eZmTDddgijhQsujUc5vOTxbVi/lafgxF1oetWKO6abLHceqQ+6tyC6JQ/DbEPQgS3a7N3tX//IgNHvyNyHsb+3a+s3wmvfDXW8Da7Tf9/aboQZo//In/84wmxsq0zR557e/abe7ISIiIiIiIiIiIttUL9rkLIPxks1c2ydK0lVrhm1WlKS0vYjjNYecZVAv2kPs7fXSNGOm5S3VXMs4UXO21d6JmkPLDWn2Qxzb47bJykh2zYnsmCReCs66kMa73Zu9qzUFj35kcFxjGm3t2mP3wYMfgLNvBOPGv38eZEM/wlFERERERERERERklExzUJfMjxLmOwGzbZ8zjdINtzfb9jEMg8ZSDbFRh08tLyJOMhbdiFrR3lb4B4OaaLWizaIbcbTq0PK2tytPRitNM1peRNeP6AcJaZZhGgblgjXSY0P3hTRZCs46gxBNVjf/FDz6IXj+U7DVc/dufv1gx9nJ17BSTFJWpQBNRERERERERERE9p3TjRLnWx4n60Wmmy5jTu6GjkFc3rl1ulGiYA+OcRy1rh+RpCl+lDBZKQylzUohR8vzSLNs28daymj4UcJ002Wm5REnGWmW4UUJWTbIMYq2hWkY5KxBQHy6UTo89eyybBCc+e2l4EzFmK6TZTD95/Doh+H8F7d2rWHBHd82CM6O3DGa/h1ACtBERERERERERERk33FsizuPVUmSjJ4fMdV0AbYUorXckKmmy3jJZqKc585j1R0JLPpBgh+nZBk49nCOTivmLbIMvCihH6hW1F4z0/I4N98liBKa/ZBFN8JfCs+WGcbgvh4v2fhRwvmWx53HqpyqF3ev4zsh6ILXGtQ7U3B2vTQe7DR79ENw6dmtXZsrwD3vhFe/D8ZOjqR7B5kCNBEREREREREREdmXTtWLLC7VEZtqury04NLwY07UnHWPRYySlNm2T7MfMl6yOdMocbzm7FhQkWbZSnBiDekIteV2smzQvuwNaZrx1GyHubbPQj/kQssjyzJqRZvJSgHHNrEMgyTL8KOUrh8x1/aZ7wScrBdJkozFfsi9J8ddq90AAAAgAElEQVQwDtpxe2F/KTgLIEt3uzd7T+wPaps9+hHozGzt2sIYvPI9g/8Vx0fTv0Ng3wZocRyTZWDb+/YtiIiIiIiIiIiIyDbde3IMAMMwqDiDgKLlhtSKNpVCjmLeWgkovDChF8S0vQjDMDjdKDFRznO85qy0sxNMw1gpPZQMKexabscwBu3L3vDUbIfZlsdU02XRjVbut9UC3lIeGuX8SsA73XTp+RHZ0tzed6q2090fjcgHbxEiT8HZaoIufOU34PFfBa+5tWsrx+BVPwiveBfkR38c7UG3r9Kn87MX+dCv/x6f/9LjLCy2ARivjfGG176aH3zX27j5puO73EMRERERERERERHZSYZhcN+pGuPlPOfmu9SKuZUj8lqet+oRecdrDo1ynsLSMZA7fUReuWBRtC0MA/wo5QZKt13HC5OVOlrlwiGpm7XHzbQ85to+U02Xthdxy0RpU0eM2pbJmUaJMSfHVNNlquliGAbj5fz+Ps4xDsBvQdBXcLaa3kV4/Ffgyd+CyN3atY1bB/XN7ngYLHs0/TuEdiVA+9qL0/zcL/7qyn+/9sH7ed/3vG3da/7kz7/MP/mZXyAIw6v+0Wu2OvzOJz/Lxz/1ef7xj32A73jL60fVbREREREREREREdmjTtWLTJTzTDddHNvjaNUhzTK8pTpTy+GSaRjkLINT9SKnG6UdqXl2rapjYxoGjm3R9SMa5e0naL0gxll6f1VHH6DvNj9KODffZWEpzN1seHal5ee/tOBScULOzXeZKOd35Z7dliQeHNUYdCFTfb7rLL4Ij/4yPPvfB/XOtuLEA/CaD8At3wLGcOopytftSoD28U9/ni9++Slg8A/XB77/7es+/6Xzs/yTn/kF/CBcueZKWQZBGPF//NwvUR+r8s0PvXIk/RYREREREREREZG9y7Et7jhW5bbJCi0voutH9IOENMswDYNywaLq2NSLNqa5e8cc1os2OctgvGQz1/aJknTdmm0biZKUthdxvOaQswzqRQVou2266RJECRdaHo1yfsvh2bJ6KU/Dj7nQ8qgVc0w3Xe44Vh1yb0ckTcBvQ9AZhGhytbmvwKMfghc+C2zxKNdb3gAPvh9OvGoUPZMluxKgfeGRr6z8/8mJcR564J51n/9vf+nX8INwJTi79ljglfOCk5R/8e/+E7/5wZ/BKQxh37OIiIiIiIiIiIjsO6Zp0Cjnh7KzaxRMc7ADzo8S5jsBs22fM40br1c02/YxjMF7PlUv7mo4KJCmGTMtj2Y/JMsyTtScbbV3oubQckOa/RDH9rhtsrK35zjLBsGZ314KzoZT5+9AyDKY+jw88mG48MjWrjUtuOPbB0c1Ttw2mv7JVXY8QPP8gBdenlkJvV7/0APrPv/FqQv86RcfxzC+Hpw9/KbX8t3f+gZKJYdHn3iGX/rV38ELAgAuLSzy2x//ND/wzodH+TZEREREREREREREbtjpRonzLY+T9SLTTZcxJ3dDu5SWg5XTjRIF2+L0NoI4GY6WFxEnGYtuRK1ob2t3IQxqotWKNotuxNGqQ8sbzrGfQ5dlg2Ma/TbEIQrOrpDG8NwfwKMfgYXntnatXYRXvAte9QNQPTGa/smqdjxAe3HqAmmWrQRo999z+7rP/8RnvrDy/w0Dvuutf4l/+uN/Y+Vr9955K/fdfRs/+hP/CoyMLINPfOrzCtBERERERERERERkz3JsizuPVUmSjJ4fMdV0AbYUorXckKmmy3jJZqKc585j1f1XH+sA6voRSZriRwmTlcJQ2qwUcrQ8jzTLhlY3b6iCHvgtiIPrj5A7zCIPnv5deOyXoTu7tWudOrzyPXD/90OxPpr+ybp2PECbvXgZYKVw561nTq37/D/+s0dXdp9ZlsmP/tD3XvecV993F29+/UP80Z/+BQDPvvAy7W6PWrUy/DcgIiIiIiIiIiJyAKVptqfrhh1Ep+pFFpeO+Ztqury04NLwY07UnHV3LUVJymzbp9kPGS/ZnGmUOF77/9m78/A2zvPe+99nBjMYbAQJiuImypJlyZu8yXE2Z98XN3EWp9nt9rxd3nOa5mR5c9qkp02b0zTpljZN99MmduIsthMnjZ3VceOsbmLJtmxLtmRrISUukghiITCDGczM+wdISLRIiqAAcbs/19WrIYHnwQMTBHXND/d9W/S3x87h6cVcShUfpxoQhmAZZ1d9Ni1m6oQh2J5PqeI3Zc+mcEu1ijPPgTBY6tMsH3YOHrkNdn+lFiw2ItUHV70TLn5drfpMLJlzHqCNT8x8sXR1zp2c5gqTHBg8CtTCtmdcfjHrMrPf/yWnBGgA+w8MnXG2mhBCCCGEEEIIIYQQa53j+QxlyxzN2VT9kCAMsT2//gH4mKGjKUVEr83tGsjEpcqpiS7tawNAKUXSchnO2eTKLumYQTIaIWbq6ErhhyG26zNZqZK3PZRSDGTidCZMetJWfR+x9IIwrBdh6ao5ofP0PmFY23/JuXYtGPJsCc5OVRyFh26FPXfW/ts0onMr7Hg3bH0FaOc8uhGzOOc/BcdxZ3ydiM+doO7eu7/+hxrgufPMS9t2/nnAyfseHT0mAZoQQgghhBBCCCGEEPM4mrPZN1ak4vlkSy4TZQ9nKjybplSt3WBH3MDxfI7kbLZ1p6TaqUmUUmzvT9ORMNk3ViQdi9R/FjnbnvVn0ZO2yCRMolNtIOVnsbxoStWvU/tNCrum91Gqtv+S8SrgTIBbluDsVONPwa6bYf93IGiwQrDvarj6Rtj43JMBh1gWznmAVvUX/uJ57IkDwMl2j1dt3zbnfTs7Zn7ColRuMN0VQgghhBBCCCGEEGKNCIKQPSMFRvMO46Va1VMYhqRjBl3JKJah1aueHC+g6HiM5h3GChX62mP4fshEyeXSvjaUXPBtiv72GJ0Jk6FsmWjEJmZGKFU8CnYVPwjRNUVbLEIiWmunuaFDqgGXq0RUJ2boKAWOF9DAWLs52a5frwhNRJfgZ151a60aK5MQLqMWkktt5CHYeTMc+lGDCxWc/yLYcSP0XNaCg4lmOOcBWsyyZnw9WSoTj1mz3nf3nv0n10WjXLjlvDn31fWZbxpOxZ3jnkIIIYQQQgghhBBCrG17RgqM5GwGs2Umyl69DeBsc7fiJmQSZn3u1lC2zKTjEU5VxGzvT5/r4696IWGtqoCnh5MKwrB2u1i2UpaBphSWoVN0PDKJs0/QJitVrKl2qinLaMIpF8iv1oIzpyDB2bQwgEM/gV2fg5GHG1urReDC18KOd0HH5pYcTzTPOQ/Q2lLxGV8fHT3O+nWZ0+7nVFweeeKpesXiRVs3zftplslSecbXVrQJsb4QQgghhBBCCCGEEKvM0ZzNaN5hMFsmb3ts6ozTvoASGUPX2JiJ02ZFGMyWGcyWUUrRkTClhWATLKSdpu35WIaO7fm41UDaaS5T7TGDiK7oiBuM5h08P5g1nF4ozw/I2x49aYuIrmiPnYMALfCnKs4KtRBNgO/B/u/Crlsg+1Rja404bH8TXPF2SK5vzflE053zAG3Thl7gZCvPnbsf56rtF552v5/v3I3revX7XXnp6fc5Va5QnPF1MhGf455CCCGEEEIIIYQQQqxNjuezb6zI+FRAs9Dw7FTT9z80XiZpuewbK9KZMKWV4CJJO83VR9MU/e0xHM9nrFBhJO+wMbP469UjeQelFJmpsFrTWvhzDoJaaObkwPdBqh1r8972fB0e+gJMjjW2NpaBK94G298MVtuZ7y+WlXMeoG3ZNIARiVD1q4Qh/Mf3fsS73vxqoubMP9S33/UD4OT8s2uuvGTefZ88dGTG/XvXr2vNExBCCCGEEEIIIYQQYoUaypapeD7DOZtMwpw3PAvCkFKliu35VLyAIAzRlCJqaMQMnY64wXDOJh2LMJQts7U7dQ6fyeoh7TRXp4FMnCM5m772GEPZMm1WpOGwGiBXdsmWXAYycaKGzsBZBHHzCsOp4CwPVQ8JzgB7AnZ/BXbfBpV8Y2vb+mHHu+Gi6yAy+wgrsfyd8wDNipo89xmXcd/9D6IUjJ0Y58Of+Af+4L2/Tke6jSAI+OxXvskDD+9F1Vr60tmRZscsVWqnevzJwzO+3rihp5VPQwghhBBCCCGEEEKIFSUIQo7mbLIllzAM6U3PflHX8wOOFytkSy7VICQMQ1w/qH9w3dS1qUqnkImyx1jBwDJ0tnQlW1sZswpJO83VyzJ0tnWn8P2QScdjMFsbQdRIiJYruwxmy3TEDToTJtu6U62p9KwUwc6B7zKjZ+haVRiGB78Ae78O1Upja7suhB03wZaX1OadiRVtSX6CN/zKy7jv/geB2u/jT37xEK991/voXd9JfrJEcbJUv00peMOrX3zG8uOf79xdD9za0210zzJXTQghhBBCCCGEEEKItSpne1T9WuiVjhmzVjiNT1YYzjt4vk/RqTLp+HhBMOOaulJgaBpJS8f1fHYfyWNFdHK2RybReIXNWiXtNFe//vYYE1OB9WC2zKHxMhmnSu8cFYbTpisMsyWXjrjBxkycnrTV/HDULdWCs2oFwqC5e69EJ/bDrpth//cg9Btbu+GZsONGGHjWyflVYsVbkgDtmVdeysue/0zu+fEv6qFX1fcZGjlWv8/097s6O3jHG141736Hj4xyaGgEpWrrLrtwS6ufghBCCCGEEEIIIYQQK0rR8fCDAMfz6UpGZ9wWhCFHsjbZskvR8aaq1CAe1WkzTMyIhqYUQRjiVgNsz2ei5GF7tRlJg9kyOw9nednF3TKHa4Eaaac5n/a4ScapSjvNZerSvtrcK6UUSas24y5XdknHDJLRCDFTr8+4s12fyUqVvO2hlGIgE6+39JzepylcuzbjzLMlOAtDGN5VC84O/7TBxapWabbjJuiefwSVWJmWrIbwj97//5ArFOutGp8uDKEtGeeTH3kP8dj8PULvuufHM74+07w0IYQQQgghhBBCCCHWmlLFx6nWqsksY2b1y5GszXipwvHJCqWKT8qK0BE30WdpyRiN6KQsAz8RMlawGczatRAoafLYcEHmcC3AQttpLlRv2qrPyrIMW9ppLiNKKbb3p+lImOwbK5KORchOVR3mbPu06k7L0OlJW2QSJtGpNpBNqzzzKuBMgFuW4CwM4OB9sPNmGHuksbWaARf/Clz1Lmjf2JrziWVhyQK0qGny93/6Ib76rXu589s/ZP/BofptiXiMFz77Kn7znW+gr7tr3n0qrsud3/khcLLl47XXXNHKowshhBBCCCGEEEIIseIEYVi/WK+f8on28ckK2bLL8ckK5YrP+lSURPTMlw11TbE+ZZG3q5Rcn5Gcw2jeIR0zSEQjFB2PUsUnCEM0pUhEa8Fbe8xY8+HOQtppNsLQNdIxg4myx/qUJe00l6H+9hidCZOhbBnLsFmfsgjCENvz69e1Y4aOphQRXdHfHmMgE29OO86qW6s4q5Qab0242vgePPEtePAWmDjU2FozAdvfDFe8DRLz5xbiHGvRn5QlnWKnlOLNr30pb37tSynbDtlcnkgkQlemA32BfzQmSzYf+K131L82IhE29K5v1ZGFEEIIIYQQQgghhFiRNKXqnaD8qSTN8wOG80497FpoeDbND0MsQ6c9HiFve+wdybNnJM/W9Sl0TZ2bcGAFmq+d5mIloxFytk0QhhQdCdCWI8vQ2dqdYktXkpzttT5k9qu1GWeVogRnbgke+xo8dCuUjje2Nt4JV74DLn0jRKU96vKhQGkQTYCZBK35f0+WNEA7VTxmnbFV42w6O9K8+sXPbcGJhBBCCCGEEEIIIYRYPRJRnZihoxQ4XkDchOPFCp7vky25JKORhsIzALcaoBTomobjuTw+WqQ9bjJR9khGI7O2p+uIGziez5Gc3dz2dCvIfO00Fytm6oQh2J5PqbLGw5JlTtMUmYTZupAz8MHJQ6VQC9HWsvI4PPxlePT2WpDYiPRG2PFuuOi1oEsgvWwoDXSjFmaaSdBbF3MtmwBNCCGEEEIIIYQQQgjROinLQFMKy9ApOh7tcYNsyaXoVAlDFnUx33arlCq19TFTY3C8TNn16WmzuLA7RdzU0ZXCD0McL6DoeIzmHcYKFfraY/h+yETJ5dK+NpRaO20d52qneTam9wnD2v5iDQqCWmjm5MD3gTX8OsgfgQc/D3v/A3y3sbXrL4UdN8L5L2pJVZNYjKlqMzNWC86MOJyDvxkSoAkhhBBCCCGEEEIIsQa0xwwiuqIjbjCad2gre1SDkEnHJx7V0RtsGecHASOFCrqqtSQkjNAeN7EMjc5klGhEI26evPwYN2shnecHjOQdhrJlJh2PcCrs2d6fburzXc5ma6d5tqb3Uaq2v1h+giBsTevGMJwKzvJQ9VjTwdnxx2HXzfDkPRAGja3d+JxacNb/jHMSzogzU5oGEbNWaRZN1SrPziEJ0IQQQgghhBBCCCGEWAM0rTZ7zPF8xgoVDmfLBGGIFwS0GY1Xnx2ZsHE8H0NTGBGN9W0WQRgyXnIJwxDb80lZp1/sNHSNjZk4bVaEwWyZwWwZpRQdCXPNtHOcrZ3m2bJdvz5rLhGVqpnlxPF8hrJljuZsqn5IMPX7cdbzAcMQ3MnanDPfhbVaeRiGcPSXsPNmGLq/sbVKgwteXmvV2HVRa84nGqb0CFZbJyS6Id2zZIGmBGhCCCGEEEIIIYQQQqwRA5k4R3I2fe0xHhycQFeKMAQz0tgcroLtMlpwiGgKLwi5oDNBIhqhUq2FAq4fUPHmr/5on0qNDo2XSVou+8aKdCbMhQUHK9zT22k2YxbWZKWKNRXEzBZciqVxNGezb6xIxavNGpwoezhT4dm0Rc0HdCfBzkO10nil1WoR+HDgP2sVZ8f2NLZWj8Ilr4Mr3wnpDa05n2iMUrWWmWYboWonFw7hR2JLWg24JAHa/oOD7Nl3kKcOH2F49ATHsxMUiiXKToWqV0XTNOKxKDHLIh6L0tXZwaaBPjYP9HHBpg1csHlgKY4thBBCCCGEEEIIIcSKZhk627pT+H5IMqozmLXxg7Chln+lSpXD2TKmpnCDkJ42i7apwEZrcA5Xe9wk41QZztmkYxGGsmW2dqcW9+RWkKe30/T8AENvLMQ8lecH5G2PnrRFRFe0xyRAW2pBELJnpMBo3mG85DKcswnDkHTMoCsZxTK0xc0HdMu1GWees3aDs2oFnrgbdn0e8oONrY2m4LK3wOVvhXimNecTjVEaGNbUbLMEaBpBJUel0uDsuhY4ZwHag48+wd33/IQf/+IhcoXijNtm+1uaL04Cp4SLP99Zv617XScvePZVvPwFz+KKS7a26shCCCGEEEIIIYQQQqw6/e0xJkoufekY45MuQxM2x4oVetqi6NrcIY4fBGTLHkXbIwzBiGhoYciGjpNVMsEi5nD1pi1yZZdsycUybLZ0JRc3B2oFeXo7zZG8w8ZMfNH7jeQdlFJkptpgrvb/fivBnpECIzmbwWyZibJHZ8KkJ23NGpQuaD6g54AzAa69doOzShEe/So8/EUojze2NrEernw7XPpGMBOtOZ9ogAJdB2NqtpkRXeoDzarlAdpDj+3jb//vl9mz/wAwe1h2pr+lT18zenyc2++6h9vvuodrrriE/3HTDVy8dXOTTiyEEEIIIYQQQgghxOp2aV8bI3mb8ZJLwalStD08PyBh6liGjhk5WR3jVgMcz6fk+iggFTNQSlF2q/S2WTNCN7caoBSYukbUWFhFlaFrpGMGE2WP9SmLnN2clobL3antNIeyZdqsSL2tZSOmw8eBTJyooTNwFkGcaI6jOZvRvMNgtkze9tjUGV/Qz/bp8wFHCw6JSMCx0TzrjeraDc5Kx+HhL8Gjd4Bbamxtxya46ka48NWgS2XmklMaRKK10MxMwjwf2lgOWhag+X7A3/7bl/jKf3wfOBmCzRaWnamae741v3hoD7983x/z1te9gt/9b29FP4tSZyGEEEIIIYQQQggh1gKlFFeflyFb8hgtOGhTM5gmKz4l1z1tPpOha3TEDVJWhFLFx0waqBLEjZmXF23Px9A0lFLEGphlloxGyNk2QRg2bSbYcndqO81Jx2MwWwZoKETLlV0Gs2U64gadCZNt3ak1MUNuOXM8n31jRcan5p0tNDw7VWcyStIIyY4fp3Tc40BBkR5oJxpZYz/b3CDsugUevwsCr7G13ZfB1TfC5hfWQhuxhKZnmyWmqs2spT7QgrUkQKv6Pr//8c/wo/968LTg7OlhWVsyTndXJ4l4jGjUxDINwhAqnkel4lIq24wdH6cwWZ6x7tT9whC+/B/f4+jocT75kfdIiCaEEEIIIYQQQgghxBm0xwy626JcvqGdfWNF2mIG6ZhJGIa4fkAYUq8mU0qha4rOhIlT9TlerBCGHkbk5Cff/SCkXPHpSBhENEUiuvBLjzFTJwxrAVyp4s973yAIydkeRcejVPEJwtoMt0RUJ2UZtMeMFdPCcLqdZhiGDGbLHBovk3Gq9M7R6m/adKu/bMmlI26wMROnJ23R3x6bc404N4ayZSqez3DOJpMwGwrPdE1hqgCzWiDhFylVJzky6bKlK8FI3mFT5xppPTi2B3Z9Dp66FzjzLMUZzrsWdtwEfVedufWdaC2lQcSsVZpFU7UQbYVpSYD2N//6Je67/0FgZtAV0XWuveZyrrrsIq68ZBvnb+zDshbW29JxKhwYHOahPft48JHH+ekvd1P1/Rn7//gXD/Kpf/0iH/ztd7biaQkhhBBCCCGEEEIIsWqcOocrW3JpsyJkklFst0rFCwgI0VBEDY2YGSFp6iilOJwt1T8kr59ygTpbclEKUlaETMJc8Ay0U/cJw5Nz1J7O8XyGsmWO5myqfkgQhtieXw/6YoaOphQRvfa8BjLxFVGNdWlfG1CrCkxaLsM5m1zZJR0zSEYjxEy93k7Tdn0mK1XytodSioFMvD5ba3ofsXSCIORoziY7FYr2phdWaaMpMDUwq0VUJU+1Wpt/ti5pkLcr5G2PsUJtTl4jv1crShjC0P2w62Y48svG1iodtr4CdtwI67a25nxigVQtOIsmasGZubJbyjY9QHvk8Se5/a57ZgRbpmlw0w3X8abXvpiO9OLeyC0ryiXbNnPJts28/fpXMpEvcMfd93Lz7XfjeR5K1R7rjrt+wKte9By2X7Slic9KCCGEEEIIIYQQQojV5+lzuNIxg/Wp+S/6a6j6tT8/DIkApUqVyUqVdUkTQ9fpSi3sQ/PT/KnQTClmDQiO5mz2jRWpTIV9E2UPZyo8m6am2lB2xA0cz+dIzmZbd2rZV2Uppdjen6YjYbJvrEg6Fqk/x5xtz/oce9IWmYRJdKoN5HJ/jmtFzvao+iETZY90zJi3ihBqwZmhQdSfRJWL+F5lRoBs6BopyyBvV+lMhBScKu2xVTbHK6jWKs12fQ6OP9HY2kgULrkernwntPW15HhigZRWmzE3PdtMb9n0sHOq6c/ic7fdVf/URxjCht71fOqj7+e8DT1NfZyOdBu/8fbrefkLnsX7/uivGR47DkBIyOduu4u//MP3NvXxhBBCCCGEEEIIIYRYbRYzhytqaFNtHcGrhlT9KseLlXoLxb4ztB+cje369SqyRPRk1VgQhOwZKTCadxgv1aqzwjAkHTPoSkaxDK1eneV4AUXHYzTvMFao0Ncew/dDJkoul/a1oZZ55U5/e4zOhMlQtoxl2KxPWaumym6tKDoefhDgeD5dyblDZKXA1BRmUEK3C1S9CkEQzHrfuKFTdDyCMKRU8VZPgFZ1YO834cHPQ+FoY2ujabj8V+Hyt0CsozXnEwuwuqrNZtPUAG2ybPOzB3bXw7NkIsanP/YBNvR2N/NhZti0oZe//ZMPcNP7/phSufaJjJ89sJvJsk0yLp+8EEIIIYQQQgghhBBiPo3O4YqZEZRSaEoxnC9j6LXQqysZJRM36ZwnOJjLZKWKNRUOpayTAcGekQIjOZvBbJmJsldvVzjbueImZBJmfT7YULbMpFNrhQewvT/d8LnONcvQ2dqdYktXctXMeVtLShUfp1qbH2gZp79GFbWqMjOwidgTVL0K7hzB2TRraj6gUw2w3fnvuyI4BXj0Dnj4S2BnG1ub7Iar3gmXvAEMufa/ZE6dbbaKqs1m09Rn9ujjT+L7AUrVUvQ3vvrFLQ3Ppm3s7+ENr34xn7/jWwD4gc8je5/kOVdf1vLHFkIIIYQQQgghhBBipWtkDlfF8xmfrEyFO1W2dVu0x00ycZOBTOMXtT0/IG979KQtIrqqV9gczdmM5h0Gs2Xytsemzvi8lXHTDF1jYyZOmxVhMFtmMFtGKUVHwlwxrQ41TZFJmGQSZ36+YvkIwnDW+YAKiOiKaOCgV/IEroPr+wvac7q+cL75gCvC5DF46FZ47GvglRtbm9lSm2+29RW1NoFiCSjQ9FqV2SqtNptNUwO0waNjAPWS4pc+75pmbj+vlz//mXz+jm/V+y8PDY9JgCaEEEIIIYQQQgghxAI0PIfL1Olrj5Ere/hhyEBHbFGVZwAjeQelaoFRf3sMTVM4ns++sSLjU2dYaHh2qun7Hxovk7Rc9o0V6UyY0vJQtIymZs4HBDB0hRm6RCp5QreMt8DgbNr0veeaD7jsTRyEXZ+HJ+6uzTtrRN9VteDsvOfBSnzuq8Gp1WbRVC1EW0OaGqCVyvaMr/t6upq5/bx6u9fNexYhhBBCCCGEEEIIIcT8FjqHqxqEPHlsku42i3Klir7IdoK5sku25DKQiRM1dAYytaqGoWyZiucznLPJJMyGw7Np7XGTjFNlOGeTjkUYypbZ2p1a1F5CnEkiqhMzdJSCIICE7hNx84RuCa/aYHg0xZmaD2hFNGJmY7MFl9ToI7Drc3DgPqDByrnNL6wFZ71XtOJk4owU6DoY07PNVkblbis0NUCL6DPTR9upkE4lm/kQc7KdyoyvdW0FvZkIIYQQQgghhBBCCLFMLHQO12Ub0jwxUuTweInBbK0lWyNBV67sMrCkpLcAACAASURBVJgt0xE36EyYbOtOYRk6QRByNGeTnZrL1pu2zur59KatelBnGTZbupIyP0y0RMoyMHWNnqSObh8nElYXHZxNK3s+ZkSf+t1b5u0LwxAGfwY7b4bhnY2t1XTY9hrY8W7InN+a84n5KQ0iUYhOzTZbY9Vms2lqgNbR3jbj66cOHaGnq7OZDzGnpw4dAU62j8x0LP+hoEIIIYQQQgghhBBCLFdnmsOVSZjkyx5hGDKYLXNovEzGqdKbtjD0uT/c7vkBI3mHbMmlI26wMROnJ23V55PlbI+qHzJR9kjHjHn3WghD10jHDCbKHutTFjnbk9lioiXaTWgL87jBcY5mS7StS5zV69fzA4qOR1cqiq4p2qzTL+cHYUjBqVKqeNhuUA+6Y6ZGImrQZkVa3/oxqML+78GuW2B8f2NrjRhc8ka48u2Q6mnN+cQ8pqvNkrXgzDi7DyysNk0N0C7YtAE42Y70jrt+wLXXnJsyy9vv+sGsZxFCCCGEEEIIIYQQQrTGpX21D9QrpUhaLsM5m1zZJR0zSEYjxEwdXSn8MMR2fSYrVfK2h1KKgUyczoRJT9qq7wNQdDz8IMDxfLoWOVft6ZLRCDnbJghDio4EaKLJAh/sPFqlQEazmZwq3DledOlrX3wgcbzoopQiHTPobrNmBGGVqs9I3mGs4OAHIUEY4lSDeoGJFdHQlELXFN1tFr1pi2ikyRVFng17vgEPfQGKI42tjXXA5W+Fy24AS4phzjml1cIyMwlmQqrN5tDUAO3CLefR0d5GLl8gDOFnO3fz1bvv5U2vfUkzH+Y0t9/1A372wG6UqlWgtafbuOiCTS19TCGEEEIIIYQQQggh1jqlFNv703QkTPaNFUnHImRLLhNlj5xtE4an3rfWHrInbZFJmEQNnW3dqXrl2bRSxa8HAZbRnDEtMVMnDMH2fEoVvyl7CkEQgJOHSh58HwjpTUcZLdTmB47mbZJRnbZY460XC7ZH3nbpSccwI/qMVqZjRYeDJ0q4VZ+87ZG3q7hV/7TfNzOik45FqFR9RgsOm9cl6E41ocLIzsEjt8Hur4CTa2xtqg+uehdc/Cu16jNx7ihVC8rMVC04M5rzAYXVrKkBmlKK17/iBXzutrvqYdZf/NMXODY+wW+8/fVEIk19OKrVKv9669e5+Y5v1R9PKbj+FS9o6uMIIYQQQgghhBBCCCHm1t8eozNhMpQtYxm18CAIQ2zPr1+zixm1OU4RXdHfHmMgE8cyTq96CMKwHgToTWo9N71PGNb2F+KshOHJ4KxaBU6+pqIRnc3rEgRBSNmtMpy3ARoK0Qq2x3Depi1m0BE32LwuQTSiE4QhTx6b5MRkhYmyx7GiQxiGpCyDTNwkamjogA9UvICSW+V4scKJSbf2OxmE5MseW7uTKBbxu1UcgYduhcfuhKrT2Np122DHjXDBy0Brbk4gzmC62iyaAiMBWnM+mLAWNP2V+q43vZpvfPc+coUiSkEQBHzutm/yvfvu542veTGvfenzyDxtVlqjsrkCd9/zE7727f9keOx4/Y8w1KrP3vXm1zThmQghhBBCCCGEEEIIIRbKMnS2dqfY0pUkZ3sUHY9Sxa/PZEpEdVKWQXvMQNPmvnivKVW/1uc3Keya3kcpWj8PSqxeYQjuZK0Cq+pyanB2qu6UVZ8POAwczdlMVny6UuYZ5wMeL7rkbZe2mEFf2mJdMlqvGnvy2CTHiw7DeYeC7dEeM1k3x54xQ6c9buD5UY4XXUbzNmW3Sjj1u7CtO7Xw5z3+ZG2+2f7v1NpVNqL/athxE2x8zsmL+KL1pNqsKZoeoKWSCf7kg7/Fe//orwnDoF4ZdnT0OJ/57G185rO3cd6GXq64ZCubB/roWb+O7q4MiXgMyzQxTQOloFLxcFyXUtlm7HiW0WMnODg0zMN79jN4ZJSQk59EmX4MXdf4kw/8JslEvNlPSwghhBBCCCGEEGLFCoLwrAINIRqhaYpMwlz0nLFEVCdm6CgFjhcQb8K4Mtv161VwiajM+hGLUA/OKrCAYHdrdxKodW2LmxGOFR0KjkvKMogbOpap16vFHNen7PkUndp8wJ50jI64wbpktL7PWNHhxGSF4bxD0fHob48tqKrN0DX62i2SUZ3hvM3w1JnScePM7RyHH4RdN8OhH5/xcWZScP6LahVnPZc1uFacFaXXwjKpNmuKltRKPmvHdv70f/2//NFf/jNetVoPlqffVw4NjXD4SINDBZm5BzBjX9OI8Mcf/C2etWP7WZxcCCGEEEIIIYQQYvVwPJ+hbJmjOZuqHy66pZ4Q51LKMtCUwjJ0io636CDuVJOVKtbU6z1lNT6PSqxhbrk258tzIAwWvEyh2NadIh03OHiiRMrS6/PKio4367yyrlSUdMzAnGoDOR1wVao+B0+UmCh7FOyFh2enmr7/0ZxN3Ixw8ESJ9phBNPK09/wwqAVmO2+G0Ycbegy0CFz0Wrjq3dCxqbG1YvGUqv23N1MQTUBEqs2apWXNRl/6vGvY0Luej/7Vv/DU4aMoNbNCc7HV17PtcdGW8/jIe3+dC7ect/gDCyGEEEIIIYQQQqwiR3M2+8aKVDyfbMllouzhTIVn05Sqtd3riBs4ns+RnM227hT97bGlO7hY89pjBhFd0RE3GM07eH4wb9u7M/H8gLzt0ZO2iOiK9gaDB7FGeQ44E+DaDQVnT9edsmiPGYzkHcYKDp2J2ocZnGpQ/zCDFdHQlELXFN1tFr1pa0awNZJ3cKs+x4oO6ZjZcHg2rS1mMFmp7ZOydEbyDps6E7UbfQ/2fQcevAWyBxrb2EjA9jfBFW+HZNeiziYWQelgWlNtGhPSIrMFWjqt78It5/GFv/sY3/z+j7j1zu9w+Mho/bbF/ixP/Ufe5o19/Mbbr+dlz3/mWZ5UCCGEEEIIIYQQYnUIgpA9IwVG8w7jJZfhnE0YhqRjBl3JKJahoSuFH4Y4XkDR8RjNO4wVKvS1x/D9kImSy6V9bSi5GCeWgKbVKiIdz2esUGEk77Axs/iRLSN5B6VqbSX722PSrlTMr1qpVZxVSmcVnJ0qGtHZ1JlgYyZOwalSqnjYblBvpxszNRJRgzYrctqMviAMGSs45O3aTLWu1NlVZHalTAqOS972GCs4bEyCtvfr8NCtMDnW2GbxTrj8rXDZDbWWgaL1lAb6KbPNIk3ocSvm1NIADWpzya5/1Yu4/lUv4tHHn+K++3fxwMN72X9wENerNrRXzIqyZdMGrn3G5bzwOVdzwaYNLTq1EEIIIYQQQgghxMq0Z6TASM5mMFtmouzRmTDpSVuzVvDETcgkTDw/YCTvMJQtM+nULtICbO9Pn+vjCwHAQCbOkZxNX3uMoWyZNitC+yKGoeXKLtmSy0AmTtTQGTiLIE6sclUXnDxUJiH0W/IQmqpVQDZSBVlwqvhBSN6ukrKMs6rGhNpMtJRl4BTG6Tv6ffj+XeAWGtskvaHWpvGi66Rd4DmhasGZGYNoslbxJx9wOSdaHqCdavtFW9h+0RYAqr7P0NExjo4e43g2R7FYomQ7VH0fXdOIWVFiVpR4zKKrs4PNA330rO88l8cVQgghhBBCCCGEWFGO5mxG8w6D2TJ522NTZ3xBoYOha2zMxGmzIgxmywxmyyil6Jiq2BHiXLMMnW3dKXw/ZNLxGMyWARoK0XJll8FsmY64QWfCZFt3Smb8idP51angrAhBYwUf50Kp4uEHAW7VJ7OIEPnpouVRrjl8GxtGvk8kdBtb3HUR7LgRtrwUNPldajmlgR6pVZpJtdmSOKcB2owH1nU2b+xj88a+pTqCEEIIIYQQQgghxKrheD77xoqMT807W2h4dqrp+x8aL5O0XPaNFelMmBI6iCXR3x5jouQShiGD2TKHxstknCq9c1RUTpuuqMyWXDriBhszcXrSloTBYqbAnwrOCrUQbZmy3YCKHxKGEDUWX30WLzxF/4HbWDf6I1SjrSk3PBOuvqn2/6XyqcWk2mw5WbIATQghhBBCCCGEEEI0z1C2TMXzGc7ZZBLmotrdQS1EyzhVhnM26ViEoWyZrd0y20YsjUv72gBQSpG0ajP9cmWXdMwgGY0QM/X6TD/b9ZmsVMnbHkopBjLxegvT6X2EIAhqoZmTA98HwqU+0byCsBaeATT8UYYwpC27m/4Dt9Fx4oHG1ioNtrwEdtwE6y9u9JFFo5QGulGrNIsma/9bLDkJ0IQQQgghhBBCCCFWuCAIOZqzyU5V6/SmrbParzdt1WdHWYbNlq4kmiafgBfnnlKK7f1pOhIm+8aKpGMRslNVljnbrgcLtfvWWj/2pC0yCZPoVBtIqTwTAIThVHCWh6rHcg/OpmlK1QuQFjyZLQzIjP2c/gNfIZV/orEH1M3abLOr3gXtGxtbKxo0VW0WjdeCMyMu1WbLjARoQgghhBBCCCGEECtczvao+iETZY90zJi3vd1CGLpGOmYwUfZYn7LI2R6ZhMxeEUunvz1GZ8JkKFvGMmzWpyyCMMT2fMKwds05ZuhoShHRFf3tMQYycWk/KmrBmTsJdg58lxmp6woQMzWsiIZSUPECYvO8ppXv0jV8L30HbydeOtLYA5kJ2H4DXPE2SKw7y1OLeU1Xm0VTteBMl5hmuZKfjBBCCCGEEEIIIcQKV3Q8/CDA8Xy6ktGm7JmMRsjZNkEYUnQkQBNLzzJ0tnan2NKVJGd7FB2PUsUnCEM0pUhEdVKWQXvMkIpJUeNOgp2HagUanfu1TCSiBppSmBGdklulPX56az/dK9E99C16D91JtDLe0P5BfB3ale+A7W+shTmiRRRoOphT1WZmfKkPJBZgWQRojlMhP1nCth28ahVN04hbFrGYRTwWxTSk36cQQgghhBBCCCHEXEoVH6caEIZgGWdXfTYtZuqEIdieT6my4MZhQrScpikyCVNCXTE3t1Rr1eg5KzY4m9ZmRdA1RToW4XixgudH61XGRmWC3kN30jN4F5FqqaF9J2P9HLvgLWy69gaINOeDF2IWSoOIORWaSbXZSnPOf1pPHT7CLx/aw559B3nq8BGGx05Qtu1516SSCTYP9LFpoJcLNg1w7TVXsKF3/Tk6sRBCCCGEEEIIIcTyFoRhvSuZ3qT5KdP7hGFtfyGEWPbcMji5VRGcTdOUorvNolL1OTHpcrzocr4xTt/BO1h/9PtogdfQftnkVh7qej2RrS9iY2cbmoRnLTBdbZaYCs5kDuNKdU4CtFxhkjvu+gHfuvenHB09Vv/+Qv/tVSiW2L13P7v37gfgr//lVract4GXv+BZvOVXXkYiLi9AIYQQQgghhBBCrF2aUkznZn6Twq7pfZSq7S+EEMuW54AzAa69aoKzU/WmLUYLDhdwhP69X2Fz7r9QNPY8J9Y9g/39b+QRLqCnPU6nYdKbtlp04jVKabVqPjNRm2+myQzGla6lAVrV97nl9ru5+fa7cSqV0wKzRv/tder6Jw8d4anDR/jind/lprdcx6++/uVEdHlBCiGEEEIIIYQQYu1JRHViho5S4HgB8SZ0trNdH6UgZugkonLNRQixDHmVqeCsvCqDMwDCkOjITq7a9W9ERx5obCkaJ3pfwNHz38KosZHhvE2bZdARN9i8LkE0Iu/tZ0+BroMh1WarUcsCtBPZHP/fxz7Nnv0H6sHX0wOzRj8QNdv6fHGST//7l7nnx7/gL/7377Iu0774Q4tFOzp6nCcPDjE+kSdfnKQtmaCzI80Fmzewobd7qY8nhBBCCCGEEEKsainLQFMKy9ApOl5TZkNNVqpYho6mFClL5tMLIZaRaqU246xSgnCVzmgMfDhwL+y8GY7vpZFGi75mcmzDKxne/GYmo+s5XnTJ52zaYgZ9aYt1ySjdKak+OyvT1WbRqdlmUm22KrUkQMvmCvzWhz7OkdFjhOHJ4OvUwCwes9jY30NPVyc96zMk4jGipknUNAkJcV2PiutSKtuMHssyenycwaOjlG2nvsep+z627wC/9aGP869/+Qdk2tta8bRWtJ89sJv3/uFfzXufb3z2L+nr7lrwnp5X5Svf/D7fuvdn7D8wOOf9tm4e4NUveS5vfd0rMAwZkiiEEEIIIYQQQjRbe8wgois64gajeQfPDzB0bdH7eX5A3vboSVtEdEV7TAI0IcQyUHWngrPJ1RucVSvw+F3w4OchP9TQUi+S5OjAdQwOvI4iKcquT7EwiVKKnnSMjrjBumSUrd3JFh1+lVNTs82MZC04MySEXO1akmZ85BP/wNDIMZSqvaamg7Otmwe47mXPZ8dlF7Lt/I2oBns4hmHIvgOD7HrkCe6658fsPzg04zGGRo7xkU/+I//4Z/+rBc9q5XKcCp/8h1uauufuvU/ysb/5vxwaGjnjffcfHGL/v32Fb3z3R/zv//nfuOKSrU09ixBCCCGEEEIIsdZpmqK/PYbj+YwVKozkHTZm4ovebyTvoJQikzDpb4+haTIDTQixhHwP7DxUiqs3OKsU4dE74OEvQXm8oaUlo5NH11/H45mXUtVjUAClHMyITlcqSjpmYEZ0Nq9LSOXZYiitFpaZ09Vmi/+AilhZmh6gffeHP2fnI4/PqA7btKGX33/PTVy1/cKz2lspxYVbzuPCLefxtutfwa5HHufPPvM5Dh8ZrYdoux7Zy/fuu59XvPDZTXg2q8O/3Pp1hkePN22/nY88zv/8w7/CqbgNrTt8ZITf+cif8zd/8gGuvuyipp1HCCGEEEIIIYQQMJCJcyRn09ceYyhbps2K0L6IYWi5sku25DKQiRM1dAbOIogTQoiz4lfBKUClAEF1qU/TGpPH4eEvwqNfBa/U0FK37TyGNt/AsZ4X4asI/dWg3hHOimhoSqFriu42i960JTPPGjFdbWamaqGZ0UgTTbFaND1A++LXvzvj6+c+43L+/A/eg2k0v9R/x2UX8cXP/B8++LG/5ec7H6mHaF/42nckQJuy78DgaT+Ts/HU4SO8/6Ofajg8m+ZUXN7/0U/x2U/9Iedv7G/auYQQQgghhBBCiLXOMnS2dafw/ZBJx2MwWwZoKETLlV0Gs2U64gadCZNt3SksQy64CiHOscCfatVYAN8HwjMuWXEmDsODt8Djd0PgNba253K4+ibMTc9nM4pOp0qp4mG7AUEYoilFzNRIRA3arAhag53g1rTparNoCoyEVJutcU0N0MZOZNm7/1A9yOrv6eITH/6dloRn0wwjwic//Du87X/8AcNjtSqrJ546xNiJLN3rMi173JUgCAI+/unP4vvNKWsOw5BPfObmGXPoTpVuS/KqFz2Hvp4uRo+d4Nv3/pxcoXja/cq2wyf+7nP8859/uOE2nkIIIYQQQgghhJhbf3uMiZJLGIYMZsscGi+Tcar0pq15Z6J5fsBI3iFbcumIG2zMxOlJW/S3x87h6YUQa14QTAVn+dUbnI09CjtvhgP/ScPP77znwdU3Qe+VTLeA06jNwZRZlWfh1GqzaBIiUm0mapoaoO3ZdwCgXib6tutfiRVtvFVAoywrytuufyV/+U9fqH/vsScOrPkA7Y67f8BjUz+TZvjOD3/OQ4/tm/W2TQO9/OOf/R7rMu317914w3X89u/92axz0h58bB/f/eH9vOrFz2na+YQQQgghhBBCCAGX9rUBtVEYSctlOGeTK7ukYwbJaISYqaMrhR+G2K7PZKVK3vZQSjGQidOZMOlJW/V9hBCLEwQhOduj6HiUKn69MigR1UlZtcBD5gtOCYJatZmTr7VtXG3BWRjC4M9h181w9IHG1iodtr0Srno3rNvamvOtVUqfqjZLSrWZmFVTA7SRYzOHGz7jioubuf28rrniEqAevDN67MQ5e+zl6NiJLP9w81dnfE/TFB3pNsYn8ova86t33zvnbR9+z6/NCM8AOjvSfPg9v8Zvfujjs+/3rXslQBNCCCGEEEIIIZpMKcX2/jQdCZN9Y0XSsQjZkstE2SNn24ThqfettX7sSVtkEibRqTaQUnkmxOI5ns9QtszRnE3VDwnCENvz60UHMUNHU4qIruhvjzGQia/dVqlheDI4q3qsuuAsqMKT98CuW+DEE42tjVhwyfVw5Tuhrbc151uLlAa6DkYKogmpNhPzamqA5jiVGV+vP4cVYF2dM8Obxc7oWi3+4p++QKlsz/jeDde9jP0HhxYVoB0ZGePhPftnvW1jXzdXbb9w1tuu2n4hG/u6GRweO+22hx7bx5GRY2zoXd/weYQQQgghhBBCCDG//vYYnQmToWwZy7BZn7LkQr4QLXY0Z7NvrEjF8+vBtTP1OzdtOrjuiBs4ns+RnL32guswhEpxquLMZcZ/oNWg6sDe/4AHvwCFo42tjabhirfCZTdArKM151tzVC04M61am0YzcbISR4h5NDVAi5oz2zWOZ/Mk4+fmjT+bK8x7lrXkvvt38cOf7ZzxvfXrMvz3G9/M+z76qUXt+eP/enjO264+Q6Xh1VdcPGuAVtv3Id52/SsWdSYhhBBCCCGEEELMzzJ0tnan2NKVlFZyQrRQEITsGSkwmncYL9Vap4ZhSDpm0JWMYhlavXWq4wUUHY/RvMNYoUJfewzfD5kouVza14Za7Rf2p4OzamX1BWdOAR65DXZ/GeyJxtamemrVZpdcD8YaClNbSWmgR8BM1v4vsnYzA7E4TQ3QurtmVpzt3ruf8zb0NPMh5rR775PAyflr69etzXS+bDv8xT9+/rTvf+i/v4t4zFr0vk88dWjO2y7YNDDv2gs2bZh73wOHF3skIYQQQgghhBBCLJCmKTIJk0xCLh4K0Qp7RgqM5GwGs2Umyl59lqChnz5TKW5CJmHi+QEjeYehbJlJxyOcCpO296fP9fFbLmZF0X0H8kengrNgqY/UXJNj8NCt8NjXwLPPfP9TZbbA1TfBBS8H3WjJ8daW6Wqz2MnZZqs9lBYt09QA7aILNgG112MYwhfv/A6vecm16LP8oWimqu9z69e+XX9cgIu3bm7pYy5X/3jLVxk7np3xvZdc+wxe+OwdZ7XvE0/NHXQ9PTg97fZ1nXPetu/A4KLPJIQQQgghhBBCCCHEUjuasxnNOwxmy+Rtj02dcdrjZw6rDV1jYyZOmxVhMFtmMFtGKUVHwlxV7Rw13yFNoRYypRJLfZzmyh6EXTfDvm/X5p01ou8q2HETnHetBDzNUK82S9WCMwkjRRM0NUDb0LuezRv7ODQ0DMCBwaN87G//jY++/zea+TCn+T9/8288dfho/X1m00DfmpyrtWffQW7/5j0zvpdMxPngb7/zrPc+MnJsztsy7W3zrs10zH370Xn2FUIIIYQQQgghhBBiOXM8n31jRcan5p0tNDw71fT9D42XSVou+8aKdCbMlT+P0LXByaEmj2EXJggDf6lP1DwjD9eCs4P3Nb528wtrwVnv5U0/1tozVW0WjddaNBpxCSNFUzU1QAP41V95OZ/4+5vr1WDfvvenDI8e5w/e++ts7G9uO8fDR0b500//Ow/v2Vd/PKXgra9fezO1fD/g43/3WfxgZvnz/7jpzXR1nl07y6rv41TcOW+PWfO3hoxFo3PeVrYdfD9oeZWiEEIIIYQQQgghhBDNNpQtU/F8hnM2mYTZcHg2rT1uknGqDOds0rEIQ9kyW7tTTT7tOeJVwJkAtwxhsHqCszCEwz+BnZ+DkYcaW6tFYNurYce7IXN+S463piitVmFmJqXaTLRU0wO061/1Qu78zn+y78BgPdR66LF9vOW3P8yzd2znupc9j6svv4iO9PxVS3OZyBfYuftx7rrnJ9y/61HCMKgHZ0rBtvM38vpXvKDJz2r5+9I3vntam8XLLr6AN73mJWe9d6k8f99e05j/ZWQY87+Blco2bQ2Wb+fyRU5kcw2tEWIlyk7kKdsO2Yn8Uh9FCLFCyPuGEKJR8r4hhGiEvGcIcVIQhuwdyjFacCiVXfqTGoXJ0qL3S+oBw2WbwWM+ruOQjlTRVkg1jVIKFXholQKhO0non2xnmC8UsZ0K+UJxCU94FoIq5qF7sR77MpHcwYaWhpEYztbrcC6+gTDRVftmvtCCQ64BSqE0HWUmCMwEYWgROiE4i/+dE8vXYv69sS7T3vRzND1A0zSNT3z4Pfz6Bz5GLl+oh2hBEPDznbv5+c7dAGzoWc+mjX30rl9H97oMiXiMaNTANAyUUlRcl0rFo1S2GTuRZeTYCQ4NDnNk9GTLv+l5Z9OPkWlv45MfeQ+atraqmUaPjfMvX7hzxvciEZ2P/O6voZrwR3a+6jMAXZ+/nDwSmf92u1JpOEC796cPsHvvkw2tEWIlKtsOe/fX/nEWj81f7SmEECDvG0KIxsn7hhCiEfKeIcRJ5SocLSuOVRSGCskfPfs9J1zYHyrWR0MOPBoSb/rV2+YyjAgxU8MKHVSlSMWpEIYzO2TZToWnDh8BIGbN3alqudEDl/Mnf8GFxZ+Q8Bv7IL+jJdiXupYnU8/GK8XhgQPAgdYcdBVTSmEYJnrUwo/EcUKTSjXA87x6NiBWp8X8e+M33/mGpp+jJW/B/T1d/PMnf5/3f/RTHBk5Vm87euqLemjk2IwwbCGe/ktx6r4betfz1x99H33dXWdx8pXpk39/M7ZTmfG9d7/pNWw5b0NT9rei85eeV6vzl2F71fkHaM7X4nEuL7n2GVyweaDhdUKsNNOfsnjNS55LpiO9xKcRQqwE8r4hhGiUvG8IIRoh7xlCnHRkwmb/iTKPj07Sl7boiJ99G7mJssdw3uHiniQXrIuzoSPWhJO2hkaAcotQKRBWq8DsicZ05dkLn3MV6bbl35ZSOXmsJ+4k+sSdaJXGqsX8ZC/OJW+hsuXVbIhEac7V2TVIKZQeQRlT1Wa6RSiJ2ZqyXP690bLPMGza0MvnP/3H/N2/f4Wvf+c+gjA8bX5fo6/52dabRoQ3vfal/OY7ricRX75/UFrlnh//gp/88uEZ39vY182vv+11TXuMM/13PVNA5nneWe0/m/Z0qiUlmUIsR/GYRaYjLa95dXTLrgAAIABJREFUIcSCyfuGEKJR8r4hhGiEvGcIUXPM0TCjATGrSld7krh59pdaI2aViQoYUQszlmBdZnFjcFoq8MEpQKUAER8iZ762F7OipNtSZBY51uecKIzAQ5+HPd+AqtPY2nXbYMdN6Be8lIQWobFeW6JOaRAxa7PNzCToy7wEU7TUcvj3RktfgYl4jN/7nZt42/Wv4ot3fofv//i/mCydnKfVaHfBUwO3jvY2XvLcZ3DTr15H97pMk068skyWyvzVP9962vd/73duImoubmDpbCK6jhU152zleKYZaeXy3H9wYlYUXV9bLTeFEEIIIYQQQgghxMoXhGH9eqXepFll0/uEYW3/ZSUIaqGZkwd/7oqzFefEfnjwFtj3XQjn77R1mv5nwI4bYeNzGr/YLaYo0HQwE1PB2dorkhHL1zmJcM/b0MPvv+cmPvjb72TnI3v55cN72bPvIAcOH2Eif+bhkUpBz/p1bB7oY+vmAa695gquuGRrU+Z7rWQ7dz/OiezM/rvXvex5XHPlJU1/rA2963ny0JFZb5vIzV/KPD7P7Rv6us/qXEIIIYQQQgghhBBCLAVNqXpm4jcp7JreR6na/stCGJ4MzqoeqyI4C0MYeQh2fhYO/7TBxQrOfzFcfSN0b2/J8dYEpUEkCtGpajNNX+oTCXGac1oDaRgRnr3jMp6947L69xynwrHxCYqTJUq2Q7Xqo2salhUlHosSsyzWZdrPOIdrLZqt7+uP7n+QV77jd+dcUyhOznnbje/9Y7RTqsH+4eMfqs9Ru3DLeXMGaGMnsvOec+z43LdvO3/jvGuFEEIIIYQQQgghhFiOElGdmKGjFDheQLwJly9t10cpiBk6iegyCBQqRbBz4LuNz+NZjsIADv4Idt0Mo7sbW6sZcNFr4ap3Qcemlhxv9VOg62Aka8GZYS31gYSY15I3EbWsKBv7e5b6GKtGYbK06LW5wsxqwGr1ZMnyhVs2cfcPZv80xpOHhubdd77bLzz/vAZOKIQQQgghhBBCCCHE8pCyDDSlsAydouORSZx9gjZZqWIZOppSpCyjCadcJHcS7DxUK7XQaQkFYUjBqVKqeNhuQBCGaEoRMzUSUYM2K3Lmaj3fg33fhl23wMTBxg5gJGD7m+CKt0Oya/FPZC2TajOxQi15gCZWhuc/6wr++l9On7cG8MDDe+dd+8DDe+bZ98qzOpcQQgghhBBCCCGEEEuhPWYQ0RUdcYPRvIPnBxindHdqlOcH5G2PnrRFRFe0x5YgQHPL4OTAc5Y8OKtUfUbyDmMFBz8ICcIQpxoQhrUWl1ZEQ1MKXVN0t1n0pi2ikacFM24JHrsTHv4iTI41doB4J1zxNtj+ZoimmvfE1go1NdtMqs3ECiYBmliQDb3dXH7xBeze++Rptx0ZOcbORx7n/2fvzsMsy+s6z79/Zz93iXvjRkZGZkZl1l4UVEFBlTQ8SIuiogKKgtDI0BTN0zP2zPS4dU+3Ps7Y9ozjMk+rj9Py9PTM2IK4ICrSIjKKqIxoI0tRRUlVkVXUkktExnb3e/ZzfvPHuRGZWRmVmTfzRmRE5vf1PDxVlRHn3HODjJP5nE98vt8HXnr3BR/7/MNfZWllfdtzvvyeu7jp8MGpX6sQQgghhBBCCCGEEDvNMBSLTZ8ozVnpxyz3Io61Kld8vuVehFKKVtVhseljGLu4Ay2NIOpAEl7z4AxgZRDxzPqIJMvphSm9MCPJ8vOmSCoFjmXS8C3iLOdMP+LWA1UW6h4EbfjKh+HRj5RjKCfROAqveE85rtFyp/vGbgTKKMMyZ7NtduWhshDXmgRo4rK97U2v3zZAA/j5X/0A/+HnfpwDrebWr623u/zC+3/jhc/3xtdP/RqFEEIIIYQQQgghhNgtR1sVTnVDjjR9TrYDZjyL5hUsQ+sGCe1RwtFWBdc2OXoVQdxEsrhsnMWjPRGcFVrz1OqQ9WFMJ0hZHURoral7Nq2Kg2sbmEAOxGnBKMlYG8SsDxMO1j3s4RLuqY/RePaTqDye7MXnXwwPPAi3vV5GDE5qs23m1MvQzJbgUVwfJEDbx775NQ/whT/54ETH/OC//jkeevSJbT/2n3/933Fk4YXn+H7Xt7yGP/zkX/HwV49f8LFnTy7zzv/uJ3nj61/DoYMHOLO6zp/8xd/S6w+3Pdcr7rmL7/jmV0907UIIIYQQQgghhBBC7CWebXLXQp081wyjlBPtAGCiEK0bJJxoB8xWbOaqDnct1PHsHQ5wsuSc4Czf2deawFOrQ9YGEUu9iH6Y0vQdDtSdbUdj+rZJs2KT5i7Jma9x2yO/x23d/4JiwiDw6Kvg/vfCTa8sgyBx+TbbZm693BUnbTNxnbmmAdpwFHD6zBrr7S69wZAwjEmzDMMwqPgeFc/F9z3m52a5efEQti1537WklOLH//mD/JMf/V8Iowt/gqPXH/I7H/uzS56n4nv863/+IEr+QBJCCCGEEEIIIYQQ+9xi06czStBac6Id8OxGQCvKONzwLroTLc0LlnsR7VHCbMXmWKvCoYbHYtPfuYvNUwh75VjDPRScQTm2cX0Ys9SLGEQpi02fmYvtgdOamfYjLD79EWbXvzTZiykDbv9WuP9BOPjiq7vwG81W22wG3KqMuRTXtV1NpM6sbfD/fe7LfOGRx3js+DOstzuXfaxSBosLB7j9lqO89h/cxze96hU0G7K8cbfdfvNN/PK//TF+5Kd+kShOJj7edR1+6ad/lNtvvmkHrk4IIYQQQgghhBBCiN13z5EZoPwB9JqXsNQN6QYJDd+m5lr4jompFLnWhEnOMM7ohSlKKY62KsxVHQ41vK3zTF2Rj4OzPhTZzrzGVYiznGfWR3SClH54ifBMF7RW/pbFpz9Cvfe1yV7IdODF3w0v/8fQPHr1F34jUSY43nhMY1XaeuKGsCsB2t9+8St86A8+yZcffQJNuenx3IWPl0PrgpPLq5w6s8pnPvclflYZvPK+F/NP3/W93PeSO3fgqsULeeCld/Or/9u/4md+5dd49uTyZR93802H+Z9/+H3cd89dO3h1QgghhBBCCCGEEELsLqUU9y42mK06HF8Z0PAt2qOETpDSDcPznoUqVY5+PNTwaFUd3PEYyB1pnhU5RH2Ie5DnwIQPZXfJci8iyXJWBxEN39k2PFN5wvzSp1l85vfxR6cmewGnBi99O9z3A1CZm9JV3wCUAeY5u82syff7CbGf7WiAtryyzs/8yn/ii195DOCCPyiuxOY5tC74/MNf5fMPf5VvfOV9/Mt/9u6L7u8S03XfS+7kt3/1Z/jdj3+KT/z5Z3nq2Rf+Q+v2m2/iTd/6jbzzLW+QMZxCCCGEEEIIIYQQ4rq12PSZqzqcbAd4dsjBukehNWGao3X5TNS3TQylsEzFYtPnaKsy/Z1nRVG2zaIe5Bl7NTgDKLRmpR/RC1O01szXzw9pzHTEwsk/4cizH8WJ2xOdO3HnsB54N8a9by0DIHEZVBmcOT64tXK3mbTNxA1qx9KMhx59gn/1M/8Hg1GwFXqd+302aQNt03bn+OznH+Erjz3J//4//RD3v/TuKzvxDeI//sJPTO1ctm3x7rd+F+9+63dxanmVJ585QbvTpz8cUa9VmJttcOetR7np8MLUXlMIIYQQQgghhBBCiL3Ms03uXKhz+3yNbpgyiFJGcU6hNYZSVF2TumfT9G0MY8rBhNZng7MsZS8HZ5v6UUZeaHphRt2zt/bG2XGHw8/+IYdO/DFWNprsnN4iXz30vXDXd/Lio/M0nYvsUhMlZYBplUGjtM2EAHYoQHvs+DP88E/9InGSAmdDr83Aa6ZW4aV338Etx45waH6OQ/NzVCs+rmvjOg5aa5I0JY5TRkHImbUNzqxt8OyJJR594in6w+CC8/aHAT/yb36J//Pnf4KX3HXrTrwtcRE3HT7ITYcPXuvLEEIIIYQQQgghhBBiTzAMRavq0KruQhChNSRDCLuQJ1feXrgGRnFKXhQkWU6r4uCNTnPkmd/n4OlPYRTpROcaNO7m9G3v4Ou1B1gZJtxl2IzilOYL7VO74UnbTIiLmXqAFsUJP/Fzv0qcpOcFXDP1Km98/Wt487f9Q+667dhVvcbxp0/w8U/9NZ/8y7+lPxhtvU4UJ/zEz7+f3/0PP4vnSkIuhBBCCCGEEEIIcaMoCr37bR8h9oJ4CFEXsnhfBWebwqQgzjWt0dd54PQfc3D1b1EUE52jc+AbOH3bP6LfeikohZfm6EFClBWEyWTnuiEoA0y7bJq5tfLfhRAXmHqA9jsf+1OWVzdQ6uz9+s3f9lp+7L95F7VqZSqvcddtx/gXP/hf8YPv/j5+8T/+Fp/49N9shWhnVtf58H/+M977jjdP5bWEEEIIIYQQQgghxN4VpTkn2wGnuyFZrq/NvikhroVkVDbOshj0Pg2JtMY78wVe8ehvMtd5eLJDlcH6oddx+ra3E8zcft7HNr/DtS53rAnYapu5lTI4syvSNhPiEqYeoH30T/5yKzxTCt73zu/hB9/91mm/DAC1aoV/82P/NYcOzvFrv/NHW6/7B5/4CwnQhBBCCCGEEEIIIa5zp7shx1cGxGlOe5TQCVKicXi2SalyJ9VsxSZKc051Q+5aqLPY9K/dhQtxNZKgbJyl0f4Nzoocvv5peOiD3LT2xESH5obL6tHvYOmWtxFXDm3/OeN/KgXGjR4SbbbN3HoZnJk7stVJiOvSVL9bnnr2FCvrbZQqb073vfjOHQvPzvWD734rX3zkcR557EkAVjfaPPXsKe645aYdf20hhBBCCCGEEEIIsbuKQvPYcp8zvYiNUcJSN0RrTcO3ma+5eLaBqRS51kRpwSBKOdOLWOnHHGn65LmmM0q458gM6kZ/uC72jzSCqANJuH+DsyyGJz4OX/4Q9E5NdGhq1zhz7HtYvvktZG7zop8bJXkZnlsGvmNczRXvUwoME5xx28yZzmQ4IW40Uw3QnnzmBHC2ffbOt7xhmqe/qB94yxu2AjSA408/JwGaEEIIIYQQQgghxHXoseU+y92QE+2ATpAyV3U41PCwzQsflFccaFUd0rxguRdxsh0wjFL0uKZ272Jjty9fiMlkcdk4i0f7NjizixDv0d+C438IwcZEx8beAZZueRsrR7+Lwrq85miQ5jiWOd6DeAPt91IGWM44NJO2mRBXa6rfQevt7nn//aI7bpnm6S9q87U2f2hoo93btdcWQgghhBBCCCGEELvjdDfkTC/iRDugF6bcMlehWXEueZxtGhxrVZjxLE60A060A5RSzFYdGeco9qYsgagH8RB0funP34uGa/hf+nW++/THsE/FEx3acW/iKwtv4bnWa6lXK7SUw+VEYWletk7n6y6moZjxrvcQabNtVh0HZ3I/E2Japnr3yLLzb+SNenWap7+omdr5NdQs36d/qAghhBBCCCGEEEKIbUVpzvGVARvjfWeXG56da/Pzn90IqHkJx1cGzFUdPNvciUsWYnJ5BmEX4sH+Dc46z8KXfwOe+AR+kU106DP2HXyu+WaerLwcy7SoRJpYx3TDlIM1l9nqxb/n1wYJSikavs3CjHf97kBTBlhuGZy59TJEE0JM1VQDtIrvnfffy6vr3HnrsWm+xAtaWWuf99++5+7K6wohhBBCCCGEEEKI3XGyHRCnOUvdkFbVmTg829SsOLSijKVuSMO3ONkOuHOhPuWrFWJCRQ5hD5J+GaLtR2cehYc+CE//FaAnOvSZ2v383eyb+Sq3MVtxaBqKKCvohxn9KKPp2xSFJkwLDjfcbfcX9sOUXphwqOHjWCaHG942r7SfKTBNsKVtJsRumGqAtnhoHjg7RvGzn39k1wK0v/78w8DZ/Ws3HT64K68rhBBCCCGEEEIIIXZeUWhOd0PaowSt9daD8UJrRnFGmObEaUGhNYZSuLaBb5tUXWvbBsrhhkc3SGiPEjw75Pb5GoZxnTZVxN5WFONRjT3IcyYNnq45reHEf4GHPgCnvzTRoYUyWT30zZy5/R2cNhcZ9UJmRgnDOGO24jBXdch96IVl6zTKCsbrCznSPD8c64cpS72QGd9mtmJz64EqrnWdtLI222bueLeZtM2E2BVTDdDuvfsODKXQaLSGD//Rp3jLd7yOVnNmmi9zgfV2lw//0adQahygobj37jt29DWFEEIIIYQQQgghxO7philZrukEKQ2/3IS0NA7UskKjtSbJi60frnZMA6UUlqFoVR3m6y62aWydzzYNGr5NJ0g5WPfohimtS4yGE2KqtD4bnGUZ+y44KzJ48lPlqMb14xMdmhoupw9/B+t3vp3EL4sQs0CQZKChPQ63o8yk4dm0qg6endMZJbRJUAp822C26pDmBWuDhF6YMOPbHGl4HKi5LNT3eftMjXeb2bUyOLP3+fsRYh+aaoDWnKlx/8vu5ouPPI5S0On2+ZGf+kV+5X/9F8w2diZEa3f7/OhP/xKdbh+lyvvKAy97Mc2Z2o68nhBCCCGEEEIIIcT1qig03TBlEKWM4nyrzVV1TeqeTaGv3QP+QZSSFwVRmmMZiifODEjznEGUMYxy0uJsMwXKZ0S2YVDzTJI8Z2OUcKThMVc7u/aj5lp0w5BCawaRBGhil2hd7jeLepAl7LvgLA3h8Y/Dlz8Eg6WJDk2sGf7+wHfSuf178WfmLvj4VqtMgWvldMOEMMnxbRPXMqj5Jt1RiqkgSHLmo5QgzVFKcajhM1uxOVBzuXNhHz8bVkYZljmbbTPj0scIIXbEVAM0gAe//0188ZHHgfIvKk98/Tne/oM/wf/wT97BG1//jdj2dF4yTTM+8enP8v4P/D794fBs+0zBe97+pqm8hhBCCCGEEEIIIcSNIEpzTrYDTndDslxTaE2Y5lvPWnzbxFCKIAhYiyDOil2/xlGcE6Q5q/2YyM9JsmI8zhEqrsmM7eBYBoZSFFqTZAVhmtMZpXSDMhzLC80ozjna8lFK4TsmWkOY5ozifNffk7gBxUOIupDFcA0D6SsS9eDRj8AjHy7fwwQGRpOTt7yNL9W/Bb9S58jM9m0qhWKx6VNxLFYHEb5jMIozgqQgTFO0hiAp6IYBrYoDCm6Zq9DwbRzL5NYD1f3ZPNtsmzn1MjSz3UsfI4TYcVMP0F51/718xze/mj/9q89t7ULrD0b87L//df79r3+Eb/+Hr+KBl93NfS+5k/m52YnOvbbR4ZHHnuRLX3mCT/313zEYjrb+IgflP9/wulfzqlfcM+V3JYQQQgghhBBCCLH/bdcwWx/GrPQjTKWIspxemBGNw7NNSoFnm9g6pZ0ovniiB47PYtPfvWvXmtOdkEGUkuUFUVZQ9yxmKw7mNrvLXKtszeVVTXuUsD5MxqFg+caOzVUwxw+VtOaatuvEDSAZlQFUGoHe/QD6qgzOwMO/DY99tGyfTWLuDgYvejv/1xN1bmrdQZorjtUv3fScrdjUXJP2KMEyDepeuTIoLQpaVYfVQUSjYlN3LQ7UXA43fA43vP2382yzbebWwa5K20yIPWbqARrAT/7Q+1heWecrjz+1FW5pXQZpH/3kX/DRT/4FAL7ncfjgHAvzc1QrHq7j4Dg2CkWcJMRJwiiIWFnbYHl1gzCKtl5j8+80557/vpfcyU/+0Pt24i0JIYQQQgghhBBC7FvbNsySnBPtgH6UEmcFnVG5V+hIw+doq0LdszCVIteaKC0YRCnL7YSVULE+THh8qU9nlHDPkRmUujDAmrb1YUwvTOlHKbnWHGn4VN1LP9oyDcV83aXimKwNYtaIUeOxlL5TPmxXCoxdeA/iBpQEZVtrPwZn7afhoQ/C8U9CMWFD88j9cP+DcPM30l7tkD3xEP04o1mrnLeL8GJs02BhxuNg3SVIC6I0I0k1BRrbVGhgcbbCixZm9tf41a222Qy4VbCkbSbEXrUjAZrnOvzqz/yP/Ntf/n/49Ge/sLWbDM5vJgdhxNefO83TJ05f9Hzb/QDQ88/3ra99JT/1o/8Uz91HN0shhBBCCCGEEEKIHXa6G3J8ZUCc5rRHCZ0gJUpzVgcRwzCjF6VEacGMZ3Go4WMYsDqIsQy1tS+s4kCr6lC3Cp57RrPUi8AcbbW57l1s7Oh7iNKclX5EnBXEWcGRhn1Z4dm5Nj9/dRAzsFOWeor5mrM1orLq7rPmitjbkhDibvnP/RacLT9SBmfPfGbyY299Hdz/Xjj8sq1fCpKMAkgyTdWZ/HG0UoqqY1J1zn6PVmyTlUGEbxuEaQbsg2fCyjzbNnOqZx9wCyH2rB0J0AA8z+XnfuK/588+83e8/wMfYXl1A9j+vnCphvzFjrn95kX+2we/n2961Suu8oqFEEIIIYQQQgghrh9FoXlsuc+ZXsTGKGGpG6K1puHbWIYiSm2yrCDTFocbNkpBfzzecbt9YQCWadB04GjTox2mnGgHKKWYrTo7Os7xZDvANBSdUULNta74uXPVtaglZZBYdU1OdULqvo2hFHXPnu5FixtTGkPUKZtn+yk40wU8+9kyOFt+eLJjDQte9EZ4xXugdesFHw5TTT5+luva0xlR6I33F0ZZQZjs4a+zMsA0wa5L20yIfWjHArRNb3jdq/jW176ST3/28/zxn3+WLz7yOFl+fuX3Un/peX7A5nsur77/Xr79m8pz78aYACGEEEIIIYQQQoj95LHlPsvdkBPtgE6QMld1ONTw0MDXzgxIMk2UnT8K8WL7ws4149vUqjbPbgTUvITjKwPmqg6ePf0WV1FoTndD4jRHKcXhhkc/ymgVBeYV7AtqVR1GcUY3yBjGKf+g5WOZiqYvAZq4CllcjmqMR/srOMtTePJP4aHfgPbXJzvWrsA9b4WXvwtqCy/4aYXWW893p3WH2DzPnt1fqExwPHCkbSbEfrbjARqAaRq84XWv5g2vezVhFPPlv/8ajx1/hq8/d4rTZ9ZYb3foDwOSJD17YaaJ77n4vsvBuVluOXqEW48e4c7bjnL/S+/GseUvNUIIIYQQQgghhBDbOd0NOdOLONEO6IUpt8xVaFbKEWdL3ZA0z2mPYmqedd4oxIvtC9sc57ipWXFoRRlL3ZCGb3GyHXDnQn3q76UbpmS5phtmHGl4GAYMoox2kDJfm7zNYRqKimuy3AupuRaeZbLY9DEMecAtrkCWnBOcTbgn7FpKQ3jsD+Hh34LBmcmO9Wfhvh+Ae98O3swlP91Qais/mtZXaPM8e2p/oew2E+K6sysB2rl8z+U13/AyXvMNL7vgY3lekOUZpmFgWbt+aUIIIYQQQgghhBD7XpTmHF8ZsDHed3ZueKa1ZmOUMIgyNNCqbP8DytvtC5vZpqF1uOHRDRLaowTPDrl9vjb1IGoQpeRFQZTm3NSqsDaIaVVd1ocxFduceBcalK2VQZRxtFUh15qjrcqlDxLiXHkKYQ/iwf4KzsIOfOV34Ssfgbg32bEzi/CKfwwv/m6wvMs+zLcV5vi2EKcF/hSaqlGSoxR4loHvTGcs5BVTxtndZnYVrqAZK4TYm/ZUSmWaBqa5DxY+CiGEEEIIIYQQQuxRJ9sBcZqz1A1pVZ2t8AxgmOTkhWYY51Qd86IjEJ+/L2xtEFN73pMk2zRo+DadIOVg3aMblvvTpmkU50RZgdYw41nYpkFeaKI0Y20Yb13r5Z8vox+leLaBaxkcnPEIkpyVfsQozim0xhi37uqeTdO3pZ0mzsoziMbBWZFd66u5fP1lePhD8NjHynGTkzjwInjgvXD768t9ZxOqOBYG4FiKUZLRfIHgfhJBmuNY5vh79RpMKttqm9XBqYEtbTMhrkd7KkATQgghhBBCCCGEEFduc19Ye5SgteZw4/yWSJhkFLogzQsa3qUf+G7uCxtEGY6ZUJm5sDlScy26YUihNYNo+gHaefuTlGKu6jCM07JGNoxZHcTU0pxWxb5oIJgXBe0gZRhl1BwTBaS55rn1EXmuKbQe730rn437dvlw3jIVi02fo63Kjux4E/tEkZeNs6Rfhmj7xfqT8NAH4ck/m7wpd9Mr4f4H4eirr2qHV801MRTMuBaDKCXNXWzzyltaaV4wiFLm6y6moZjxdvER92bbzKmV/5O2mRDXNQnQhBBCCCGEEEIIIa4Tm/vCOkFKw7cveEgdpwVpXgZStnXpB+Kb+8KGUU7D1wTJhQ/gfcdEawjTnFE8/VF25+1PGidpxzZHLiqFZ2e0RzGjOKPqmHi2iWMZmEqRa02c5vSjlF6YkReaGd8mSHI2RsnWKMhRkhONw7NNSoFnm8xWbKI051Q35K6FOotNf+rvUexhRTFunPUgzwF9yUOuOa1h6cvw0Afgub+Z8GBVNs3ufxAW7pnK5SilqFmaGd8iGBWsDRKONC9/BOTzrQ0SlFI0fJuFGW8XdqApME2wa+DWygBNCHFDkABNCCGEEEIIIYQQ4jpx7r6w+dqFDbOC89tcl8O3TYKkbLRF6YXhweZ5tC7bYtNWdU1820QpiNKCigMKxc2tKjU3YakbUnUNBlHGMM4ZJQlal42zYByMGYbCswwcS7ExjMmLMlh7cqXPjO9w58EaN7UqzHjWVvAWpWXL5UwvYqUfc6Tpk+eazijhniMzqB1/aC+uKa0h7pfhWZayP4KzAp75DHzpg7Dy6GTHGjbc/eZyx9nszVO/tBkbbNPkYN3hTC+k5prb7lW8lH6Y0gsTDjV8HMu8oGU7VcoAyy1DM6dWjmwUQtxQJEATQgghhBBCCLEnFIWmG6YMolT2EAlxhc7dF+bZF44WMzi/zXU5D4Ycy0BrSPKCeJvJdZutMKXYkSZI3bMxlMKzzQtGRM5VHequyYl2QJDkuJaBZajyPpLkGKpsyMVpGaZlhUYDnSAhzQrmqi4N38IwYG0QY5sGc+PzV5xyhGWaFyz3Ik62A4ZRih6/33sXG1N/r2IP0BqSIYRdyBPYgVB46vIUvvZJ+PIHofPsZMc6Vbj3++G+H4Dq/I5cHoBlwLFZj/UIgiRjqRcCTBSi9cOUpV7IjG8zW7G59UAV15qPLT6vAAAgAElEQVR2qCVtMyHEWRKgCSGEEEIIIYS4pqI052Q74HQ3JJM9REJclefvC3s+1zZwTAOlIM007mU8GTLOaZjpbcKEMMm3vler7vS/N5u+jWUqZis2Z3oRaV5gmwZJXrA+iNkYJeSFpuKYpLlmY5gwjFPSXBMmGaahmK+5zPgWo6SgFyYYSnFoxqPqWsRZwcl2SKvqkheaYZxyrFVBUb5v2zQ4Nm6nnWgHnGgHKKWYrToyzvF6kwzLPWdZXLa59rpkBF/9KDz82zBanezYyhzc9y64923g1nfm+p7nQM0BS6G1Zgk43Q0ZxjnzdeeiO9HSvBz72AsTZnybIw2PAzWXhfoUwy3ZbSaE2Ma+D9D+4m++uPXvhlK88uUvoVqRv7wIIYQQQgghxH5wuhtyfGVAnOa0RwmdIJU9REJche32hZ3LdyyUUtimQZhm1LxLPxoqzmmYbTe2cBhneOOgu+5NPpLtUgyjDM+jNGelH7Pci6i6FkvdkDTPt0Y3pnlBN0gJk4wgzcnyAt+2aFbKAG6pG2MYMIgyZlyLg3WP2apDw7doBynrw5gozbYaRze3qlvvfxRnJHmBZSi+tjKgH2VsjGK+6c75cgeTtGP3tySAqAtptD+Cs6ANX/kwPPoRiAeTHds4Cve/B170pnI84S67c6EGlPeSimOxOojoRwl1z6Zim3iOiQnkQJTkBGnOIEpRSnGo4TNbsTlQc7fOc1WUKscyOvUyNLN3/+shhNjb9n2A9uM/+6uc+3e3eq3Ke972Rt7xPd+O5zovfKAQQgghhBBCiGumKDSPLfc504vYGJU7jLTWNHyb+ZqLZxuyh0iIK7DdvrBz1RwT01DUXJNOkNIqCsxLNC2SrEApcEzjgsZamhf0wpRDDQ/LVDSvYKfR5TjaqnCqG3K44fHlkx0qtkWhoT2K0UDVMTGVQcUxyYuCAqiWy9II05z2KAYUozgFpTg042KZqtx5ZhjM11wqtsnaMIZhDErhWhFFoWmPknL0o9YkeUGaFXztTJ84zYnTgmNzlam0Y2WM7TWQRhB1IAn3R3DWOwVf/hA8/nHI48mOPfgSuP9BuO1brukuL4XiroU6jYrNM+sj6p5JL0zphRmDKL3gB2gcy2S+7tLwbRzL5NYD1atvnm22zdw62FVpmwkhXtC+D9A2bd5c+4MR7//g7/HbH/tT3vuON/O2N74e275u3qYQQgghhBBCXBceW+6z3A050Q7oBClzVYdDDW/bEU6yh0iIy3exfWFQtj7mqg5pntMNUtpBynzt4q2LMM2xDQOlFJ59foCz3ItQStEajzPcqYDHs03uWqjz9NoQXWieWh1sPVifrZSh3alOSJYXpLmmVXG2wqy8KDiZZHSDhDgrmKs6JIXmaNXBOueeUx2ng6uDmKwo7zULDY8wyRhGOWlR7pYrioKNUUKc5awNY0yDq2rHyhjbayCLy8ZZPNofwdna1+ChD8JTn5r8eo++Gh54EBZfCXvoB04W6h5N32a5F7HSj5irlr/3N3c4KgWeZWAohWkoFmY8Dje8K995ttU2mwG3ek3ad0KI/ee6SZbOvf9rDe1un1/+v3+b3/zoJ3nfO7+Ht7zhdZgXmaUrhBBCCCGEEGJ3nO6GnOlFnGgH9MKUW+YqNJ9fk9mG7CES4tJeaF/YuQ7UXTZGCa2qy/owpmKbW+HR8+WFJohzZqs2lqGoOGcfXneDhPYo4WirgmubHG1VdvS9ASh9fgBQ5uiKXpiSFwWD8TjJcwOmNCv3wmW5xlRgKEAr4MIwodyjVrA6iKi6Jr0woebaVFyTGdvBGT/Q92yTIM0xDcUzGwGrg+SK2rEyxnaX5SmEXYiHoPNrfTUXpzWc/gJ86YNw8nOTHasMuOPbysbZ/N07c31T4Fomt8xVOdaq0I8yRnFKmBRb7UvfMai6NjOetbWLcWLKPNs2c6p7KkQUQux910WA9vyR3ufeB1fXO/zC+z/Ib/zeJ/jYf/p3u3thQgghhBBCCCHOE6U5x1cGbIwfFF9ueHauzc9/diOg5iUcXxkwV3WkkSEE2+8LO/a8YMsxjTLsKTRRmpVjC2HbEK09SlAK6p5Fq+pgqLL90g9T2nHKbMVmrupw10J9R78HN+8dFddEKYM7DtYpdDlecRinDMKMpMjJck3TN0jzgiwvRy72woQ0LfBsk4pTjre0DUV7FOM7BtY549vWhwmGKve6hWlGq+JydNa/4IeyZ3ybtNDM11wWZlyygonasTLGdpflGUS9cl9YkV3rq7m4Ioen/6psnK1+dbJjTRde/N3wineXu872CUOV41+nNgL23N1mbk3aZkKIK7bvA7R/+c/efd5/P/3cKb7wyOOcXFrZ+jWtYXl1fbcvTQghhBBCCCHE85xsB8RpzlI3pFV1Jg7PNjUrDq0oY6kb0vAtTrYD7lyoT/lqhdifNveFHWn6nGwHzHjWBd9rc1WHYZyWD02GMauDmFqa06rYWzvRRnHGMM44UHOwzXJc4mA4opvAyW7EkVadY60KhxrejrehNu8dy72IFx2qU3VMlnplS2xtELMxLEN5w1B0gnTrOMtQuJaJgYI050DdRQPDJMN3DPphtjXmchClDMfvWQGOWe4eSwqN/7xs0LEMtIYkL8gLJm7HyhjbXVLk4+CsD3kO6Esecs3kCTzxx/DQh6B3YrJj3Trc+3a4751QmduZ69sPNnebObXyf7LbTAhxlfZ9gPaO7/62bX99db3NFx55jC88/BhfeORx1tudXb4yIYQQQgghhBDnKgrN6W5Ie5SgteZww7uq8x1ueFsj5Dw75Pb52o7tXxJiP9ncF5bnmmGUcqIdAFwQom0105TCszPao5hRnFF1TAqt6UcZNcfCsQx822CpG7LcHhHmiiMNj5vnqhxqeNxzZGZH38929w7bNJjxbdYGMUGS06o6ZEVBxbFwLRMFWKZCKUU/SrFNA9MsR1AaQJzm5QjGKKVVscmKss0WJhlRWjBbsUlyjdaaJMvxn9euM8etL62hGIcyl9uOlTG2u6AoytAs6pXts70cnMUD+OpH4eHfgmBjsmOrB+Hl74J73lqOJ7whKTBNsGtl28y+ur9bCCHEufZ9gPZCDh5o8aZvfS1v+tbXAvDcqTPX+IqEEEIIIYQQ4sbWDVOyXNMJUhq+vW3TYhK2adDwbTpBysG6RzdMt5okQtzoFps+nXHgdKId8OxGQCvKtsInAIXi5laVmluOEKy6Bt0gZbkXMYwzXKscI9gPN/eKwcG6Q8fXHKg5vPjIzK4ENy9077DHoyizvCh3tSU5raqNZZZ7ymzTwDENaq5JZ5SS5gVag2EauJZBlBZUHQizgjApxz9u7lCrOCbxKCErNGl+YfiSj9tfSlG228Yu1Y6VMbY7TOuzwVmWsqeDs9EaPPI78Pe/D8losmNnb4FXPAgv+i4wpzT2cL9RBljOeLdZrRzZKIQQU3bdBmjPd/NNh671JQghhBBCCCHEDW0QpeRFQZTmzNems4+k5lp0w5BCawaRBGhCnGuzGaaUouaVIVk3SGj4NjXXwndMTKXwbYP5usupdsAwzqm7FkdbFVyrDKlvmvWpOBaGUgRBwJqj+YZjjV1rPV3q3qEB1zKpuhbz9QvHICZ5gWWWe6+yXGOb5R64OMvQWhOnGYMoI8xytC7vK5vBi9agtwlhkqxAqfI8rn3+612sHStjbHdQPISwU45C1Hs4OOuegId+oxzXWKSX/vxzLbwUHngQbn1dGSDdcFT5vt1qud/MkealEGJn3TABmhBCCCGEEEKIa2sU50RZ2QDx7Ok8+PMdE60hTHNGcT6VcwpxvVBKce9ig9mqw/GVAQ3foj1uPnXDcCtj0FoTZwUoONbysUyF1mWLbXG2QsO3qXsWdc8mixzOPAGutXsP7y917zCUYjxRkWKb4MQxDZRSWIYiyQt8TCyz3GGWFZpRnFNoiJIczzYxDbXVOlOqbOqdR2u6YUqSFWyMEjzbJE4LXNvAdyxqjrltO1bG2O6QZAhhD7IYdHGtr+aFrTwGD30Avv4XTNyMu/kb4f73wpFXsPWb/UaijLJpt9k2M+WRthBid8jdRgghhBBCCCHErii03npgb07pAeB5e4j2cuNAiGtosekzV3U42Q7w7JCDdW+84yxlfZDQDZOtQCzLNTXXYr7uUvdswiQnzQtcy6DimAzj3X94f6l7h2sb45CsbIa51vmj3DzbwFDgOSbDKKPmWmzmTFqXDTVdlGFaxdn8OpQNM8tQ2Gb5yVlR0A8zumHCWj+m6pp0g4Sqa9KP0q2gzjQUpoIwy89rx8oY2ylLQog6kEZ7NzjTGk5+Dh76IJz6wmTHKhPufAPc/yAcuHNnrm+vU2bZMnPrYFduzPBQCHFNSYAmhBBCCCGEEGJXnNsSyacUdp23h0gerAnxgjzb5M6FOrfP1+iGKU+tDljuRRgG2IZBNB5f6FkGwzhnGAcoVR43W7GJ0pxT3ZB5d/eD6kvdO3zbRCmFbRiEaU7dO38nlFKqbM/lmpHKGMYZFcccf6wMzjbzF2scliV5gWkolFI4lskgymiPYvKiYHUQM4gyCq0pNJzpxVvnssc71xzLYLUfszDjcdNsBZAxtlOTxmVwlgR7NzgrsrJp9tAHYO1rkx1rufCS74WXvxtmjuzI5e1pSoFhlSMa3Vq550wIIa4RCdCEEEIIIYQQQuyKqmuOH3RDlBZc4eqf84RJjlLlA/Sqa176ACEES92Qfpjh2SbtUYJScGjGo+7ZeLaBqRS51kRpwSBKOdOLWOnHHGn6dHTKmVChd7Hxeal7R9W1sAxFzTPpjFLyqsZ83ijDGc9iEKXUXYt+lKH12YYZCtLibBhfFAVxVlB1TQxVBl+jOCdMctqjmFGS0aw4NHybY60KjmmQa02aacI0oxOUQVmcak61Q5r+gBcfrssY26uVxRD1IB6B3pn3WjYzM0ZxSpgUFFpjKIXvGFRdmxnPuvgPa2QRPP5x+PKHoH96shd3G/Cyd8DL/hH4s1f3RvYjZYDtnR3TKD8UI4TYAyRAE0IIIYQQQgixK+qejaEUnm1OrSkxjMsQwBg3TIQQF/fYcp/lbsiJdkAnSJmrOhxqeNuOE6w40Ko6pHnBci/iZDvAJqOfwtdWR8zP7c5D/kvdOwylaFUdkjynG6S0Rwnz9fMbXpZplHvIxiMb2+PdZUqVIxqzrAxktIZBWv57xTZJ84Ii0vSilH6YkRcFB2ourarLgZpDxSkfrVmAa0HNs2gVBWf6MWuDgI1hTHsY89Wl/tb5QcbYTiRPyx1n8WDHgrM4y1nuRaz0I/JCU2i9FXYqVTYzjfF4zoUZj8MN7/xRofEAHv09eOR3IGxP9uK1BXjFu+HF3wtOZbpvbM9TYJpg18ZjGqfTzBRCiGmRAE0IIYQQQgghxK5o+jaWqZit2JzpRaR5cVU7gNK8oBemHGp4WKai6UuAJvaWotB0w3SrwbTZZqm6JnXPpunbGMbutSxOd0PO9CJOtAN6YcotcxWal1EFtU2DY60KM57FE6fbdBLF6iDhdDdksenv+HVfzr1jvu6yMUpoVR3WhwkVx6Tqnv/Yq+7ZRGlBXhRsjBKSPGcQpdzU9EmychTgKM6Is4IZzybONY6h6AQJ3TDFMgxmqw4znk3NtV4wtDcNgxnPounbJHn5Wmd6EZYpY2wnUuTj4KxfjkTcISuDiGfWRyRZTi9M6YUZyXik6SalwLFMGr5FnOWc6UfceqDKgurDw78FX/0opMFkL9y6He5/D9z5HWDeYH9+KaMczeiMgzNDGuRCiL3pugnQfudjf8Yf/dlngHK29W+//2eu8RUJIYQQQgghhDiXYSgWmz5RmrPSj1nuRRxrXflP2y/3ItS4ebLY9Hc1iBDiYqI052Q74HQ3JMvLNkuY5lttFn/cmrTM8nviaKuCZ+/sA+QozTm+MmBjlNAJLj88O1ez4nBT0+PxDDpByvGVAXNVZ8ev/XLuHbZpcKThkRfl13ptUO4le36IdqDm0AkSaq5Vjn3VsD5MCNKMKM0ZxCmtioMyyq9ZPy3Gn2/Tqtr4jkXNtZivXfxrt7mLrVkpQ7uNUQJoqq4lY2wvpSjGoxp7kOfAzjTrCq15anXI+jCmE6SsDiK01tQ9m1bFwbUNTCAH4rRglGSsDWLWhwm3mmvwyMfQpz+N0hOGe4fvg/vfC7e8tgySbhCGaaJMC7x6ud/shmvbCSH2o+smQNvodPn6c+Vs4evtB26EEEIIIYQQ4npxtFXhVDfkSNPnZDsoWxpX8BS5GyS0RwlHWxVc2+ToVQRxQkzT6W7I8ZUBcZrTHodVUXphm8WzTWYrNlGac6obctdCfUfbXCfbAXGas9QNaVWdbb/vtNYMk5wwyYjTggKNgcK1jTI4ckxmfJuKpTnTj1k8kPPc+oj5GW/HW3aXc++Yq7mM4hytNWvErA5iaklOq+pgGuXets4oIcnLhlmaF8zXXZI053Q3YRBlFEDVzomzAkU5JrZZcThYdzCNcgzkpcbF5oUmiHNmqzYN36buWSx1Q47O+rSHiYyxfSFanw3OsoydCs42PbU6ZG0QsdSL6IcpTd/hQN3Zthnt2ybNio238TQLT/4uRzqfR016fbd8EzzwIBx++ZTewT6hDAzbw5qZR9cXoTZ3ra9ICCEu23UToAkhhBBCCCGE2Ps82+SuhTp5rhlGKSfa5cirSUK0bpBwoh0wW7GZqzrctVDf8QaMEJdSFJrHlvuc6UVsjBKWuiFaaxq+zXzNxbMNTKXItSZKCwZRyplexEo/5kjTJ8/LcOeeIzOoKf9kcFFoTndD2qMErTWHG955H0/ygvVBzMYoIS80WmuS/Oz+J8c0UOP9T67KqVjlCNUnlgccXxly96E6wI627C733nG0VYaQSikGdrkPbRClFLoMm0ZJhmuqrSZZN0joRxmGUjQqFlkONc+m4phEaY5hKA7WXRq+Q8O3MI1LN4baowSloO5ZtKoO83WX3nKfKMvphilzVZuVfixjbDdpDckQwi5kZVNvp60MItaHMUu9iEGUstj0mXmhr5/WNNe/yOLTH6HR/spkL2SYcOd3wv0PwtztV3/h+4kywfHArVMYGZ3oKQolf1YLIfYXCdCEEEIIIYQQQuyqxaZPZ/wg/0Q74NmNgFaUcbjhXfRhcpoXLPci2qOE2YrNsVaFQw1vV3YwCXEpjy33We6GnGgHdIKUuarDoRf4PV1xoFV1tn5Pn2wHDKMUPa6p3bvYmOq1dcOULNd0gpSGb593TZthX5rnDKKMYZyTjsOzTUqVIxJrromlc5YCRdiP6cTjXWFZjqHUjrfsLufeoZTi2FyFqmuy1FMUheZkJ2B9mNCPUhTle7GtjKpjYRmKqlO2i4ZRRsUxCJKCvDCwLZPFis1is3LZoeYozhjGGQdqDrZpMl93sU2Dhm/TCzOavo1rmyilZIwtnB+c6WJXXjLOcp5ZH9EJUvrhRcKzIufA8mdYfOYjVAfPTPYitg8v+T54+bugfng6F74fKANMczyisVbuOQOKYZcsz6/xxQkhxOQkQBNCCCGEEEIIsevuOTIDlA+7a175AL8bJDR8m5pr4TvmVlsnTHKGcUYvTFFKcbRV2QonNs8jxLV0uhtyphdxoh3QCy9/v5htGhxrVZjxLE60A060A5RSzI4DkWkZRCl5URClOfM1FyjHNZ7oBHRGKYMooz2K0UDVMWl4Lraltr4H00wTphmdUcr6IKSTKPQoJezG3DxXYcazxw2znW/ZXe69w7UN0ixnbRjTDVKSrKDhWzimiT8OzGzTwEChVLkrLa9pelFKoTM6QYJpGBxp1CcKz9YG8db4yiPnBHs116IbhtwyV2EYZzLGNgkg6kIa7Vpwtmm5F5FkOauDiIbvXBCeGXnEwVN/ypFn/gAvXJns5F4T7nsnvPQd4E03CN/TNttmTh2cquzXEUJcNyRAE0IIIYQQQgix65RS3LvYYLbqcHxlQMO3tvZFdcNw2ybLoYZHq+rgjke5SfNM7AVRmnN8ZcDG+Pfv5YZn59r8/Gc3AmpewvGVAXNVZ2qjSUdxTpSVrTLPLgOdE52AzjBhbRgzjHPqnsVsxb5gRKEFuBbUPIu8CNG6oJ+CHiU4joVtGhyouRfs89qplt3l3jvWBjHDOCXKivK9VcuQpOba+LZJVhRYhoFrG9RdC8Mw0GiiLGdjmBOlOWGScsIxufvQDOZF2l15oWmPEoZxRtU1ma+5tCoOc+OwEsB3TLSGrNAszHhkN+oY2zSCqANJuOvBGUChNSv9iF5Y/l6cr5/9ultJn0PP/RGHn/sj7LQ30XkD9yCrd7yDY9/4TgznBvmzSSkwrDI0c6tguZc+Rggh9hkJ0IQQQgghhBBCXDOLTZ+5qsPJdoBnhxysexRa7+guJSGm6WQ7IE5zlrohrapzRW0iKAOUVpSx1A1p+BYn2wF3LtSnco2F1lvBkqlUGfaNUtaGMaMk52Ddpepe/BHRIMoI0wKNwlTgmGWgFCQFnXETajs71bK72L2jPUyIs5xCF0RpgetaNCs2plKEaUEwvr/E5IySnE6Qbo2onK87rA0StE5RCvphyvGVPnM1F982cSwDQykKrUmygjDNCeIcQ8FczcE21bh8o3luY4QxbsOZSqHH/z8cOLcFeKOMsc3isnEWj65JcLapH2XkhaYXZtS9soXohKscefajLJz8JGYeTXS+Uf1WHl34Xr7efA23zs/QzC2aO3Tte4YywS53m0nbTAhxvZt6gPbEU89O+5SXZaMz2U+GCCGEEEIIIYTYGzzb5M6FOrfP1+iGKYMoZRTnFFpjKLU1Dq3p2/tzx4+4bhWF5nQ3pD3ey3W44V3V+Q43vK3RfJ4dcvt8bSq/5w2ltp5xR1nBUjfc2nd2OeFZVhS0RzFhkpNkBTULZisOq6OUOMtZHyWkeXHR8GcnWnbb3Ts6o5TOKKHimCx1cw7OlLvIOqPk0iMqg5RukDLjW0SpRT+K8O2yORalOUGSX7gbzjCY8W0KrekFKc2KjbZguR9t/RCAYxokecGZXsSMb3PLXJX7jjbG57jOx9hmCUQ9iIegr/0OrFFcjjNNspxjepk7vvKHHFj6S4wJr63Xehmnb3sH3QPfQCdIiQcRhdaM4pTmdvvU9julwDDBmZG2mRDihjL1AO09P/zT1+wHD5TivL/ICCGEEEIIIYTYPwxD0ao6F4yCE2Kv6oYpWa7pBCkN375ogHQ5bNOg4dt0gpSDdY9umE7l+6Hqmvi2iVKw1A1J85z2KKbmWZcMzwD6YUZeFAziFNc2iRUYBjiWQZhkKKVZG5R7zi5mp1p25947kmzAoYbH184MqDkWRQEbYXJZIypbRUE7SFnpR1imouoa9MKUm+cq1Fyb2YpNkhfnBWPDOKMbpvi2QdU16YcZG6PkgqAtzQqSvKATJHxtpc/8jHt9j7HNszI4i/p7IjjbFCYF3sbf821f/zDH+l+a6FiNor3wGk7f9g6Gzbu3ft0bj+eMsoIwuXbtuh2hjLNtM7tafuMLIcQNZEdGOF6rEEsaw0IIIYQQQgghhNgtg6hss0RpznxtOo2MmmvRDUMKrRlE0wnQ6p5djhI0DU53QyxToYFW5TKaMuPrCNIyBKk5Bn0gzTV1194aZdgeJRxqeBiXeDizUy07ONsIfHptxCDK8GyDKC0uq2UHYBoG8zUXE3hybYhplA0w2yz3pB1u+qRZQTF+8NUZpViGQcOz6AQpWkPFNZmxnQtGPS51Q6K04HQn5GDd5fGlPp1Rwj1HZq6vMbZFDmEPkn4Zou0VuoBnP8vi536NOzb+fqJDC2WxtvhtnL71+4lqRy/4+Ob/E1qz9XtjX5O2mRBCbNmRAE2CLCGEEEIIIYQQQlzvRnFOlJWNJM+eTjPDH7dZwjRnFE+nudP0bSxT4domgyjDMBRVx7ygjbWdMCsoNOUuMcvAUFBoiLOCZs0hL8oRiFmhGcXlXqmL2amWHZSNwCDJ+frasLz2CcKzc81WHZpDhzDNidOCpV7EQsOj6pjUZ8oxnSc2AjSaQVyOnC0bbg7mNmGgZZRf+/m6Cyjaw7Khpsdhy72Ljf0/xrYoxqMae5DnwB4JkvIUjv+/8OXfgPbTTNLZy02fM8fexPIt30fiHXjhzxv/UykuGSDvabLbTAghLrAjARpcmxaa3NeFEEIIIYQQQgixWwqtt55/mFN6KLF5nmm2WQyjbC6dbAdAOXKydaB2WccmWY7WBXmhqdoWkJMU4AO+ZeJYikxr9Lg1dakADXamZQdlI3C1H23tapu7gvAMyr1k83WXIMkYRSH9MKEXpFvvb2MY0w4S1oYxwWXskWsHKQpoVmwOzfhUHJMT7YAT7QClFLNVh8Wmvz/H2Gp9NjjLMvZMcJYE8NjH4OHfhOHKZIc6TZZv+T7OHHszuX3p75Moycsxm5aB7+yzEYdKgWGBU5e2mRBCbGPqAZrvuURxDJT34Pe983u4567bpv0yF/jEn///7N17kGTpedf573vec817ZVV1VXdP99zULY1GGl0x2AgbXwDbWjvWxhZejLGBIBaWjWCDDW6xwRKxsMASG8sSi1kHu4Bke2WvbcDC4EtgywJki8XySCONZkYz0lz6Xl1VWXk/9/fdP05WTl+quiq7q7p7pOcTMdFd3XlOnsys6qnIX/2e59P8xm999tjvRwghhBBCCCGEEAKqtslublYeUdi1e56jbrOc6db47a9u0wg9rg1TclNymLeF8tJSmCon0VqRpIbcQiPQuFrRbfhcH2ZkpSHND7f/6ThadgDjpODaIGGaFwSuPtyIyn20I5d25NGfZozSgqvDmHNZg7ysGmm7LbGDwrNJWjBOClYaAZ7WrDQD/NmuvNe3pzTCjJc3RizX/Yd3LONerIV0VIVnRcZDE5zFO/CFn4Uv/Bykw8UOrZ3kyuM/wObpP4TRhw+SpnmJ7+pZW/DuP+fuK6XBD6vgTNpmQrnZPZ8AACAASURBVAixryMP0N7+xFk+/8Ir8499z+ND3/Deo76b23z+Sy8f+30IIYQQQgghhBBC7KoHmsjTKFWNOKwdQXEonrVZIk9TD44uUAk9zZluNNu15dAb5/haH9jQsrzZssuKkmFS4DrV9XXrPr6urnGRxtxxtOygGuFYGEuSG5Zr/qFGVO5HOw6rzYCdWYDWnxRcG6W42iEvS3qTjEbgHhiebY5TGoGmGbqc6kTz8KxT8+kmBVf6Me3I5WJvyrm15l1f732VjiHpQ5E+mBFUexlegc/9NLz4i9V1LWDcehuXn/gI2+sfqoKlBeSlYZTkrDYDtKNohcc27OveKQe0noVmDXDfQk1HIYR4QI78X/Wnzj3O5194Zf6DCy995fWjvgshhBBCCCGEEEKIB64ZejhKEXr6yEYRjtOC0KvaLIcZh7iI9VbEUt2jFXoErsP1UUojK+nW997dBaBQWGuZZgWFsQSuQ+hAbbaXKy2qBtkijbnjatkleYnFUhpL4N77W17N0KMVeWyOUgJXcak3YZwUQJUb7fd6l8bQm+aMk4JGoFltBCzVPZZvuf3Jdkh/mtGbZIRezJOrjYd3xxlANoZ4MAvODtc2PHZbr8CzH4VX/h3YxdqMV5rv5iuP/ADuo7/3rhtYm6MMpRTtyGOtFT6cO9CkbSaEEHftWAK0XdbCi6+8ftR3IYQQQgghhBBCCPHAdSIPVyuWah7XBgl5afD03bee8tIwiHPW2yGuVnSiow3Q6oHmbasNLvZiQldjsfQmGZO0oDZr0/mug6MUxlqywjBMcvpxRm4MHc+n7kGiLcuz8YhZYVAKfO0QeId77MfVstudImgtWHU0zahu5HHRdWhFHs3QY5TkbI1TGoHLNCvwXQetFOXs+UrykklWooCVRkAzdFmqe5zt1m47t6cd2pHHzjTnRDOkHx/dPrgjlU2qUY158nAEZ9bClWfh2Y/BG7+14MGK8olv5YWT388F9zGuDWJOJwWtu/haG8Y5gzhjvR3hu5qT7XDhcxwbaZsJIcSRONYADWBja5v+YESn/RapoQshhBBCCCGEEEIcguMoTncikrxkY5hydZDsGZQc1tVBglKKbt3ndCc68jZSM/TQjsOZbo00L1FKUQ80o6RgnJRMs+ymiXxVUUXRmB3naujWPaYuqFmLJc5LPMdBKUV0yB1ex9WyC32NQuE6iuyQ+9gOkpWWVuix3AhoBJqlms84zXEcxfbk9ufL0w5LNY9m6OJpzalOdFvz7EaNwKUfxxhrj6zFeGSyaTWq8aEJzgy89u/hdz8KG88vdqzjwVPfA+/7EXTnLCdGCaPrY6ZZwZVBDLBQiDaMc64MYlqRx1LN4/GVOoH7oHfYqSo48yMIGuBJ20wIIe7VkQdojz6yTr0WMY3j+Z+98MprfNMHnznquxJCCCGEEEIIIYR4oM50a1zqx5zqVPvFWqFL5y6Woe2O8jvTrRF4mjP3EMTt5+bGXMmTq3X60xxfZ7Qji7WWrDRYy7xVpoCL/Zhm4FIYe1NIVhrLNC1Zqnu4jjpwnxocb8uuPXt8oa8ZZwWlsfuOptxlbbUzLSsNeWkw1uIohacdtKMYpTmhr+nUPM6daLI9TmkEHuvtEF87tz9fSqEdxXLdZ6UZzHee7SfyNdZWQeQkXWwE4bHJYkj71a8PQ3BWZvDlX4HP/STsvL7YsX4d3vWD8J7/Cuor8z9ea4YMpjnWWq4Al/sx47RktenfsUWal4bNUcYgzmhFHqfaISuNgLXmA2yfKQe0WzXNpG0mhBBH6lg2W77jyUd59vmX5j/k8KIEaEIIIYQQQgghhPgaFHqa82tNytIyTnIu9KYAC4Vo/WnGhd6UpVq1J+v8WpPwkG2uRdzamNsaZ5zt1lhvh0zSgjgvSfM3Q6TAc4g8zUoz4Poo4WIvph8X8/P1JhlKQTN06db9Q+1/Os6WXTN0WW+FXNiekpWG3iRjtRnseduiNAyTglGSY2wVpBWlxQIKcLVimBSMk5xmWL0urchFO4pH45xHlmsYY6vnC4vD7PnyXRq+njf0DqJnt7MWjD2asZN3LU+qxlk2fTiCs2wCz/8LeO7jMNlc7NjaCrz3j8PT3w/B3lOxzq01gKpNWfNdro8ShklGM/SoeZrQ12igBJKsZJqXjJIcpRTr7YilmsdKI5if5/6StpkQQtwPxxKgPXXucX73iy/NP37pK68fx93c5MRKl3e87bFjvx8hhBBCCCGEEEKIG53uROxMMqy1XOhNeX17SjcpONkOD2yzXB0k9CYZSzVvHmad7kTHdq37NeaaobfvOMXA0+xMc7r1gCu9EZmBaVYyzmCl4eNpvW9QdaPjbtk1Q4+1Vkjka5xCMU4Lar6+rRk3SnJ6k4yitMRFSZKVFObm8CovDElR4rsOuTH0pzlpXu17Qylqnqbm3/vbauUsNFOKQwWQx6JIq+AsnTwcwdl0G577WXj+5yEdLXZs51F434/AOz4M+s4htkJxfq1Ju+bx2taEZqgZxDmDuApWbx3P6bvV53k78vBdzeMr9fvfPJu3zZpVcKaPdk+iEEKImx1LgPad3/qNNOpvfrPXaR3//rOPfM938JHv+Y5jvx8hhBBCCCGEEEKIWz19qgVUbZZGmHGlH9OfZrQjj0bgEvkarRSltcRZyTgtGMRVm+VMt8Zy3We9Hc7Pc1zupjHna4dTnYjSWCJf81qmuNxPWF+q0wyrMXZ3Cgrh/rTsOpFH5GueXK3zwtURoeewOUoBqAcu1lq2xhnjtCDOCkZpgbXVc1LzHVytUKpqG+0UBt91SHJDM6hGLA7ijDg3QDX28S4mdd4mzkqUgsjT1IP7vEOrSCEZzIKzh2B85OAifO6n4MVfqsY2LmLtaXj/j8Hj3wLOYs/jWjOkE3lcHSRsDBOW6xZjLUnx5njO0HVwZuM511ohJ9vhfdx5Jm0zIYR4UI4lQDv/xFnOP3H2OE4thBBCCCGEEEII8dBRSvGu022W6j4vb4xoRy69ScbONKcfx7e1WUJPs94O6dZ9glmodZzNsxvdTWNuue7Tn6YoLIWFtDAooBW6LDf2b5/dz5bdjSMqL+7EGGPRgeb6KKWRldXOtqxgmOQkuZmFVu58T5oxllFakOQlrah6y6wdwqlOSJIbtic5aV4ySquGUrd+7wnaOC0IPY2j1L4NwCNXZLPgbPxwBGebL8GzH4Ov/PriDbiz3wjv/1E4/cF7CpUCV/PYcp2z3RrDpGCS5sTZm+NMI9+hHni0Qvf+NQWVUzXM/Ia0zYQQ4gE5lgBNCCGEEEIIIYQQ4uvR6U7Ect3nYm9K6MWcaIYYa4nzct5miWaBiaurwOdMt3YsO8/uZJHG3DQruT5K2RonjNOSSEM78phkJRujZBb+PBwtu90Rle95pMPnLvSp+5rI01zaiRnGOVlpsNayVPMJfY2xliwryUozH9HYCl2UUqSF4YkTdZZq1XVf2YnpTTJcrbi0M+VUJzqweXcneWkYxDnr7RBXKzrR8QYkJs8YDbaZjnaYxDnGmgcXDlkLl34Hnv0oXPz/FjtWOfC2P1QFZ6tvP9LLclT1Ohz3a7G/WdssqFXBmVeTtpkQQjxAEqAJIYQQQgghhBBCHKHQ05xba/LkaoN+nDNKciZpOW+z1ANNM6zepHecB/Pm+GEac4UxDOOCcZqjlUM90Kw1A7avWxqB5kQnYpIWvHhtSOhpmqGL6ziz8z+Ylt2NIyrPrzW4tDMFLKHnMM0Uw6Qk9DSTrGSSlfNr1UpRDzU1T5OX1Qi/052QVuhxahaKeo5ie1KNFuxNci72pjyx2tj3Wqy1jLOSOCtIc4PB4qAIPIfId+mNU5RSdOs+pzvRsX0upGnK9evX2extkaYZpTEPbjyhKeHV36waZ9dfWOxYHcA7vxfe+yeg/cjxXN+DIm0zIYR4KEmAJoQQQgghhBBCCHEMHKcKR45i1N9x2a8xd2UQc6WfEPkOjqraZsMkx8UQaWiGLqOkCoZqvqbuu2BhuVE93gfZsrtxRCXAl6+NKEpLYQyrzZBW6FIYOw+QXEehlAIsxoB2oBv5rDYClurVzjao9sQ9ulzjS1cHtCO/Gn1Z92/bH5eVhq1RyvYkozQWa+2s+Vbdn68dplnJ1jjl/FoDZ9bQO3Km5PrmdS5eu8Y0TuhPMwZxQVaUt40U9V1NO3JJi5Jrw4THV+qsNcOju5YihZf+bbXjbHBhsWODFrz7B+GZH4Ja9+iu6YGTtpkQQjzsJEATQgghhBBCCCGE+Dp2Y2OuN8n43MUdrKmaSVvjAtdRPLFSY7UZUuYpn92+xPkTdTw/ZBhnbAxT4rykU/MxxqKA82sNWpH/wFp2u2MiLXC5n7A1TsHCUs3Fc5xZYFax1mKwFCW4WtGthzRDl6V6tbPtRme7Na4OEkpTjYJ8Y3uCsRZPO8R5ycYw5fowobSGrDBkZfV8wJv3lxYlk7RkqeYR51UwuT3Jjq6dZ0pMPOD1y9e43h+xPcnYGMYkhcHXDq6jcF2FqxxcrUApjLFsjlK2xlkVohrLYJpzbq2B4h5ev3QEz/8LeO7jMN1e7Nj6CXjvD8PT3wd+/e6v4WGz2zYLmlVwpuXtWSGEeFjJv9BCCCGEEEIIIYQQx8wY+9COc9zlOIprwwRjLOM0Z2ea0wxdunUfXzsYaymNRc/2uLVm7brTS1Wo1JuNN4w8zTgteWzlwTXvdkdUKlW15ZqRS+hrXK3ne9DevC142mGpXo2h9LSej228lacdzixFvNGb0g41oyTnP76yRc3XFMYwikumeck0K3BmYyxDV9OpeTRDl0Gck2TQCDSOgp1pTmngxStDdiYZT59q3RTuLcQYSIeQ9Pnq1T7XhzEXelOuDBIAmoEHlmofXzZ73I6DUtVr3wo9CmO5NoiZZsX8OTq/1lz8Wiab8NzPwPO/ANlksWOXHof3/0k4/11fQ6MMb2mbfS0FgkII8TVMAjQhhBBCCCGEEEKIY5LkJRd7Uy73Y4rZbq04L+fj/B7kqMNbvbo15tk3dnjx6pBRWrBS9zG2aibtjh5M0pSNRHFtmBJFEZ528LTD2W6NVuhyoTflQm+KUoql2W6vB6kRuJw7UWdrnBK4DjXf3XOkoprtAFuu+6w0A3zt3PGcCstOXOBqhacdXrw6JM7K+WjIas+ZJs2rP5tmBYWxtEKPR7oRzdCjFbpoR3GxN2Wc5PPA6l2n24s9SGshGVThWZGzMYrZHCV8+fqIyzsJ7VBjLGyNUwpjbhvf6DoONd+hKA2udmiGHqMk5wpVENmueYcf57jzBnzuJ6txjSZf7HGsPwPv/1F4/JursOlrgbTNhBDiLU3+1RZCCCGEEEIIIYQ4Bpf7MS9vjEjzkt4kY2eak+S3758KPc1SzSPJSy71Y86vNe978PTq5phf+sIVtkYZV4cJkeuwNcluu1ZT5EwK2BylpHbEqXbIciMAmO8Ce317SiPMeHljxHLdXzgQPMq23iQtKS0s1XzOnWhggDirdrcZLA5qFna5NHx9YPvLWMvWJGVrXLXzxml1jc3Qxc7aXaGrcV2navLlJYUpcJSiW/fwXUVWGh7phKzMQql2lN1d8GjtrHE2gCIHLGlR8urmmJc2hlzcjgk9TT8ugCqsbQY+rqtwUNXYysKSFCXDpGCYFHSiagyn1jCMc2q+y2tbEzqRR+De4XXc+BI8+zH46iepBmcu4NHfDx/4U3DyvV8jO8B222b1WdvsGPbbCSGEuC/eUgHaK69d4LULV+gPxzTqEafWVnn3O96GvsNPBQkhhBBCCCGEEELcT8ZYXrg65NogYXuScaUfY62lHXmsNgJCz0ErRWktSW4YJTnXBgkbw5RTnYiytPc+zm/Ba332jR22RikvXxvjew7NyCPyNL7r4CiFsZasMPTHJXGpuDxIMY5LaSyTtORMN0IpRafm000KrvRj2pHLxd6Uc4ccAbhIW+9kO6QVemSluWPIZqydh4Cuowg8TTO4+7fDLvViBtOcQZyRFYZHuiEnW5qrw4SsjDnRCglcZ95EU6rafjbJSrKixFhohx7TzMzPuXDwaC1kY4j7UGbcmHJeHSRc6E251IvJy+o+6oGmFXro20JHha+hFmhKYxkkOTvTjLTQdGs+mTFcHyU0Q83VQcJjy7eMHbQWLnymCs4uf3axJ1JpOP9H4H1/ElbOLXbsw0o54Pqz0EzaZkII8bXgLfEv+a/+5mf4iZ/6F1y9vnXb39VrEd/3nX+QP/VD30uj9mDHAgghhBBCCCGEEEK8cHXI1X61f2pnmrNc91lvh3h7/ABwzYdu3ScvDVcHyb2P87uLa728M+XFq0OuDmMCz+Ed6038PdpGgatxKbnuWWq+w9Y4mwVc1bWeXa6aNifbIf1pRm+SEXoxT642DmyMHbat585Csd+1Fkc5rLdDar7edyRmUZp5qam0CzajbrE9TulNMzZHKUlueHTZJ5qFXMZYnlip0whdssKQlxZrLUopPK3wXYeytGyNM3rTDFc71AN9U3vvUMFjOoakD0UG1tz0V8Zavrwx4mo/ZhTn1IJqf13NP7gBqB1Ft+YTuiU70+oa25HPOCkYxDkbw4Sz3RpOVUOEr/xGFZxtfXmxJ9EN4J3/Jbz3T0Dr1GLHPpQUOLpqmUnbTAghvubclwDtd7/4EptbO/OP33HuMR575OSBx1lr+V9+/GP8q1/9FPt9jzOexPz0v/wVfuPTv8M/+p//Co+cPHFUly2EEEIIIYQQQgixkMv9mGuzFtAgznlsuTZvGN3Jg9gjtnutX94YM0oKIs+lFbp7hmc3chQs132MctkcpWySombtr+VGgKcd2pHHzjTnRDOkH+d063s/B4u09a4OEl7fmjCIq3DNcx2+ujmmHmhWGwGgbhuJOYhzzCxcS3LDIV6KPeWl4cogYZTkDOKcTs2jHXlM05LSWixVEKodh8jb5yRetVPs+ihl5OVcGShakTcPVu8YPGaTalRjntwWnO3aGqdc6cdsTzIsipVGcKjw7EbV7X16k4zALcnLKtBcrgcMx2M6r/8KfO6nYXh5ofMStOGZPwbPfASipcWOfRhJ20wIIb4u3Jd/3f/G3/8/2d4ZAKBQ/OxP/J1DHffRn/s3/Mtf+VR13B1+UMlauLKxxZ//a3+Pj//436LZqO9/YyGEEEIIIYQQQohjkOQlL2+M2J41qA4bnt3oqPaILXKtm6OE5YbH9iQn8g7/VlF9Ngpxr0CoEbj04xhjLaNk/wDtMG09Yy0bvZhRUuC71Z/nxpKlJUs1RStwqQcupzvRbSMx25FHb5IxTHLa0f7XcZCNYcIwzrjYmxLnBaHncqWf4GnFJCtp+BrtHLxipB64NLIqlKoHms1RNbYTuC14HMQ5S15ZNc7yeN/gbNfrWxOy3DCI87sKz3bVfE1SaPpxRit0GQ97nBr+Es1PfgLS/mIna6zB+36kap15b/XJUTe2zZrgv9UfjxBCiIMce4D2ymsX2OoN5h9/w/veeaj22RuXrvF//T+/eFNwZi006hHrq8v0+kN6/WE1S1pVf3d9u8f/9k8+zt/8S3/2OB6KEEIIIYQQQgghxL4u9qakecmVfky37i8cnu26lz1id3OtNc/FYLE2x3MX27m2XyAUzcYqxnnJJC33PPawbb1LvZjtScrmOGWSlrQij0eX6yR5yeY4ZZgUBJ5LnBuW6/5NIzG3xym9SYZ2FF+5PuJ0J9pzlOZ+8tKwMUz4/MU+/ThjGBeUxqJVSW9iiXxNb5KRhR6u1rRCF/eA83frPpO0qAJBnbHeDqvRiEAjcEnylMgpSPtXIDQHBmdQhYyXBzHDJJ/fx71ohx7udJPff+3XeGbwmwQ2WewE3Sfh/T8K5/4w6P0qeW8RN7bNgmYVogkhhPi6cOwB2hde+ArwZoPs2z/0ew513E/9wr+lKMt5OBb4Hn/1L/wo3/Wt34SefSPy2ede5G//w3/K1etb89v96qc+w1/4sR9kpds5lscjhBBCCCGEEEIIcStjLJf7Mb1JhrWWk+3wns53N3vE7vZauw2PzVEGgL7TCKB97BUI7Z7H2ircudVh23rzvWPjlGlacqIZzJtvNzbgQq8KHJuhi6+dm0Zi9uOcNC9JCsNL10a8+5B75bbHKVcGCcM4px/nXB+mxLnBdapdbGAYJgVxVhC4DjuTbN62a4b7h0baUdQCzTgpaUeWSVrQDD1cR7EaKcrxgGKww9j4EDQOda3DpKAoLdOsrB7/Idpw+2knl3jm+r/myd5/QLN3+Lmvk++FD/wYPPqhO4+Teujtts3qszGN0jYTQoivR8ceoL3wymsA82Wu3/z73n/gMXGS8quf+sw8FFMK/tZf/nP8wW/6wE23++B7nuIn/t5f54f/27/BeDoFwBjDr33qP/HD3/+dR/9ghBBCCCGEEEIIsS9jLP04Z5TkTNISYy3ObDdWM/ToRN6RhUAPm36cU5SWnWlO+4a9VndrkT1i93qtjlLzrKO0duE3i/YKhPTsdVaKebvqRodp6924d2xyS3i2qx64NPKS3iSlHjhs3TASEao237tOtfjtr27juw6vbo5Zb4eznWl7M9ZyqRfTm1aB2MXelHGSkxeWQDvVdYQaXzv0JlU4N81K0sLQDFyMrfatrTR81D4hUuRpplkVYObGEGmDnw/JpwOS0YDMq2Hs4ZtbkzTHYilKg681Bgss9rV2YvJlntn4BI8Of2eh4wB4/FuqxtnJ9yx+7MNEOeAGVXDpN6RtJoQQX+eOPUC7cPna/Pfrq8t0O60Dj/nMZ79Alhfz8Yzvf/dTt4Vn83OeWObH/th/wf/xz35u/s3eF158hR9GAjQhhBBCCCGEEOJ+SPKSi70pl/sxRWkx1hLn5fyHYiNP4yiFqxWnOxFnurUj3+l1XA4bCo6SnNIYkry8YziziMPuEVvUrddaGIOvHZSiConu4t2iGwOhOC/Rs1Au8jT14ObX+rBtvc1RSl5W4yEbsz1ne+nWvHkDztMZJ9vhTcHVajPkidUGr26OCVyH5y8PeN+Zzr4jNm8dGem5DpGrGaicTs2nGXmsNALSoiTKDfXApRN5JEXVSMtKg5217labe38u+K6Drx1qnqWWDfAmOUWRE+cF1tp9g8f9xJlBoWbBpSUvqtf0QNbyyOhzPLPxi5ycvHjo+wOqcOn8d1XBWfeJxY59qCjQGjxpmwkhhLjZsQdoVza25sHW+SfOHuqYzzz7ReDN9tn3fee33PH23/OHvpkf/+c/j8ViLXzl9Uv3dM1CCCGEEEIIIYQ4nMv9mJc3RqR5FXTsTHOSWXi2SykIPc1SzSPJSy71Y86vNTndeXjfqF40FJykBUlhsBZC797aZ7sOs0fsbkzS8qZrLa2DUgpPO8R5QSNc/O0i33WwFrLSkOYGYy3h7Dm6dZzhYdp6xlp6k4xRUmDtnXd6aceh7mvGadWAG2clzVvCtnesN9kYJriOojSW17cmdBsFJ9vhTfd/68jI5brHtWHKKC1xZ63ARqhphi4mNriOmk9QakcegeswiHMgRylF6Dm3PX7XUdQijZ/F1OM+aQmFrkLEJKvWmYSuQ+Qf/vPIWIvvVq+j7yqSwlC/Q46rbMETO7/NM9c/QTe5cOj7AcCL4J3fD+/949BcX+zYh4m0zYQQQhzg2AO0yTSe/37pEO0zgBdfef3N8Y0ovvED777j7TutBuefOMtLX30DgMFofPcXLIQQQgghhBBCiAMZY3nh6pBrg4TtScaVfoy1lnbksdoICD0HrRSltSS5YZTkXBskbAyrEXtladmZZDx9qrXvmLsH5W5CwauDZP53d7NHbC8H7RG7W8ba+WPRShF5DtpRNALNzjSnawx6wR1azg3XmpWGSVqw3g5xtaIT3RwgHaatN0kLCmMZJyW1QM9HQu4n9DST3QZcVtwWoHna4W2rdS7sxHRqPt26xyDO6U+zKhQLXFyteGN7ws40Z2uU0ghcerPXvhW5TLNqVOXuNfuuRqmq9ZWWJSF63qwcxDm+LuhNqrDV1dVzHLmKBlNM3GdnNCSuezS9Nxt407zEd/Ws5Xj4EY6OUtR8Pf+8jLOSMoJbs0ltUt6+/Unedf2XaOabhz4/gA07qPf8ELz7IxAebo/cw2e3bdaogjPv3nYVCiGE+Np2pAHaJ3/rs7f9WZKk899v7wz2vM1NrOXVNy7PP2w16/zOcwdXyMPgzZ9EmkxjfvO3P8t+31t+2+//4IHnE0IIIYQQQgghxP5euDrkaj/mQm/KzjRnue6zfkubZ1fNrxpEeWm4OkjmO6V2x9y96/TD8Wb8vYSCANOsYJjknLMNjmKIYzl7fhYd53eQW3eeKaVYrvvkZUl/mtOb5guPoTQ3XOv2JCPyNN26z+lOdNveu1sbcMZWe9PivJy31/pxFVxOsoL18OBrubUBt5dm6NGOCk51IhwFpzrRPCDtxzHb44ydScbWJCX0NFo7tANNO6rCNk87tEOf3d1ikevgqOoxTNISYwyO4xB6mrQwjNKCwNVM0pJTHY+GinGzIVmaMJimlMbgOQ6+V50vL6vPqdVmgHYUrQWagJHvEHmaRuiiUcSqZBBn8+ZeUIx459av8s7NXyEsR4c+L8DQW6V3/o/x2Id+qGqfvRVJ20wIIcRdONIA7a/9nX/EXt/P7QZZn/7Pn+fT//nzB57nxuBrMBrz1//uP1roOowx/LW/s/cxCsV/+jf/fKHzCSGEEEIIIYQQ4k2X+zHXBgkXelMGcc5jy7V990ndyNMOZ7s1WqHLhd6UC70pSimWZkHLg3YvoeBrWxOSvGCalXx1c8wzpzv3fD3xbJzfXnvE7kU90ERe1VZKckPNh5VmwPYko1sP2Bqn1Dy9786xvWSFme1QM5QWnlxtEHiaM93abbfdbcAVpeH6MGGclhTGYq2d7Q+DnUnGMMnZmeY4CgoDrdDF3Wev101tPfb+ierdkZg1X/Not0490IRezIlmSGEMn7/YpzAGdp+6mAAAIABJREFUg+Xx5fqbrTHPoRm6bAzTm0dczsZTlsYwSUtGWUk7rK6vEbhkRYnvOTRUQicfkmcx06IaxZkUBtdxZuMaq9d2c5ShlKIdeay1woVC03rg4cyC0K1RSify2JnmrLDB79n5Zd7e+w08kx58ohtcds/wW60PM330W/nu9zzyFmxrSdtMCCHEvTnSAK3VrKO4+X/ug9F4HqoFvk/g3/kb6jTLSNIMmM0UDwI87+DKepKmpFn+5rU0GgtevRBCCCGEEEIIIQ6S5CUvb4zYnjV3Dhue3Wj39q9vT2mEGS9vjFiu+/Pxdw/C3YSC1lqSwhB6Dg1f8/r2mCQrsUAn8jizVDv0eEprq91dcVZULSwsG4MEC0yykrp/dG/hNMMqbAk9zSjJ6dZ9fO1UozWNJckLNsdV2HLYEC3OS8rSsDXJePtag+W6z/m15p6vqaMUO9OMy/2Y3BiywjBOSnJj5j9UPYgzxmn1fES+RpHNr/XWnWJwS1uPvZ/zG0M2VyvOrTV5crVBP8652JtwtR8yzUo6kcfZ5RqR79Lwq+t//spwzxGXrchllOQ0A49hkhNoh8ivWmtLXkGQb2LLnF6u57vxSlPtOmtFbhXQ+ZphnDOIM9bbEb6rOdleLOxphdW5unWfYZyzXlzm23q/yFOjz6BZbH/epdo7+VT9u3hOPcXpbo2nOnVW7rRQ7WEzb5s1wa9L20wIIcRdO9IA7dd/9sdv+7M/8H1/liyvgq0/+uFv4y/+mR+64zn+15/4aX7ul359/vH//j/997z36fMH3veNx/mex7/72cVaa0IIIYQQQgghhDjYxd6UNC+50o/p1v2Fw7NdnZpPNym40o9pRy4Xe1POrTWP+GoPZ9FQMCsNW6OU7UlGOWtO5caglWKclSS9KVjYHmestUJWmgH+Ps2pvc6VlYaitFwZxKw2At7YmtCOXM4s1TjTrd1z0NiJPFytWKp5XBsk5KXB0w7LdZ9xmlcJ0zjl+iilkZd0a94dd6JlRbUDTjuKk7UqOFtvh3u2Co2xXO5P2RqlTLOCN7ZLQldTCzQtz8d3HRylCFwHR6Wkeck4KUjykmbgYmzVmltp+DeFk7sNOF87BN7e17rXSExnFjqNkpxTnZDeNOPMUm0++nDXfiMuXcehWw8wNiUvS4y1LHmGjuozTUdsDid06z6hVvMAbRBnoKpwsh15jJOCK4OYVuSxVPN4fKVO4C72GjtKsdYKCTaf472XfoYzw2cXOt6ieL31DXy6/WFedR4jLw1N1+FkJ+Lt660jHSF6PKRtJoQQ4ugdaYC2l2ajxvbOAIAXXn7twNs/98LLKFV9r6aUwzve9tih7mc4msx/36jfPh5ACCGEEEIIIYQQ96YKP2J6kwxr7cItmVudbIf0pxm9SUboxTy52rhtX9b9sEgouLsbLS9LRknBOC3JZ2MHja3ez9gaZ1gL2lFYLNuTjFOdiOVbQpk7nWsQ56RFiVYKz3W4NkjICsOlfsz5teY9jbx0HMXpTkSSl2wMU64OEs7ORi3u/opShF5Bb5IySQvqvib0NOVsRGNaGIokJ8lLrgwSstxwfr3JuRMNTi/VePpUa8/7fuHqkFFSNdwmWUkrdDnTraFved3rgSbJXeK8pO5pCgvDpJiNeKyCsNXmm62oJC/xtINSimiftt6dRmLeupftVncacdkMXVCGtRqQDIj7Q66ZAt9RWKAwlsJUe9mmWck0K1mqeSgUWWHoTTJakcepdshKI2CtueDXlTXw+n/k7Gc/ymMbX1jo0FJpXmp9M5/pfDdXWJuNlKwe/yPdGme7tXv+Oj9WyqnCMn93t9n+Qa8QQgixqGMP0NZPrLDVqwK0L774FTa3d1hdXtrztpeubvDlr16Yj3x8+5NnCYPD/STb1k4fqH6KaKmz9zdpQgghhBBCCCGEuHv9OKcoLTvTnHbk7bkbbBGedmjPdjWdaIb04/y25s9xO2woaK3lws6UnUnOKKmCJQvUfU07DPBchbUBgeegelVYc7E3xQLL9YDSWMZpXgVUljueKzclpTGcWYqIfM1aM+DaIGFjmFZjFkvLziTj6VOtQ4+IvNWZbo1L/ZhTnYiLvSmt0KVT81EoHu3WaQRVuFcPnHm4N8ky0jRjkCk2hilBYCmNRTtwfr3BStPnQ+dXeGJl77Uau2Myt8cZSW443YlICwNYuGXsou9WYZhWisJa2pFP4DoM4hzIUapqdM13kM1CKe2o+djFW43TgtDTOLPdZTfa3csGb456vOl69hlxuVTzqbmWk17GoN9jK43BGtK8ZGosaWEIXIesqMZlbk8yPMchLQxKFWitWG9HLNU8VhoB59YWWElS5vDyr8Dnfgp6r7LIV2OqQj7b/Db+U/OPMPGWcB2Hll+1/wZJzpluxDvWmjyx2li4DXfslKrGMnqNakyj9xYaLymEEOIt5dgDtKfPP8HzL30VpaA0Jf/4Y7/A3/xLf3bP2/7fH/8EsNs+gz/4jR841H1Ya3nxldfnwdsTZ08fybULIYQQQgghhBDiTaMkpzSGJC/nI+zuVSNw6ccxxtr5jqv76bCh4IWdKTvjjM1xyjgtaYbuLLC5+fan2hFxVo36046q9oKNU5K8YJ7QwL7nmqQFg2lBK/JYbgScWYpYbgTkpeHqIOFib8o4yectrHedbt/V4w49zfm1JmVpGSc5F3pT4M39dMt1n2bosjVK8XRGO6rGSw4misGmZa0V4LoeW+OMk62IcyeafOjc/uHZjWMyB3HO29caTLKCi734ppGI8+tzNVpB6DtMkhIT2PnoykGc4+uC3qRqk+3EOYqqCbZc9/cMFfPSMIhz1tshrlZ0opsDNEep+ftK5Q2v041uHHHpxTlFWeCkE8J8SpblBI6dndcSuB7jtCDOSiZZyTSL0U41mtINFb7r8NhKnXbk4buax1fqh2+eZRP40r+C5z4O443DHTMzdds8v/Jhvtj9DlKnTk1B23Gqr7+0oLSWc6sNznRrd9eGO07SNhNCCHGfHXuA9s2/9338v//63wHV94m//Mnfot1q8N/86A/ge9U3K0VZ8k9/5hP88id/+6bxjX/4W37foe7j1QuXmUzj+Tc65x4/cyyPRQghhBBCCCGE+Hp20Ji7uxH5GmshzksmaXkk51zEYULB7UnGziSfjx080Qzm4/tu1Qw9OjWfJC8JXE1clLRCh2FSVPeXFoAiyYubzlUay+YoZZwW1APNaiOgW/NZnl2Tpx3Odmu0QpcLvSkXelOUUizV/bse53i6E7Eza95d6E15fXtKNyk42Q7xtDNvXZ1sh4yzkjgrCLXhilf94HNpLefXm7x9rRrb+MTq/u2pW8dkrrdDvnxttOdIRAClFI3QozCGSVoySgvakUfoadLCMEoLAlezMUzISstKI8DTmpXm3q/h1UGCUtW+s9Od6LZRofVAE3kapaoda/tN8XxsuUbdc1gPUtLxDtd6I3qlIfI0gevguQ7LDZ9xXDBKSxxHoRXUfM2JVkg9cFluBJxuh7jaYa0VcrIdHq7lFe/Acz8DX/x5SIcH3/4GA3+NL6x+Ly+1v5nc8TDG4mBRKKytmoRLNY+11l224Y6N7DYTQgjx4Bx7gPZ73vtOHnvkJG9cvjoPx37mF3+NT/zaf+AdTz6KchQvv3qB0bjaYbbbPvvWb/oAp9dXD3Ufn/z079x07De8953H9niEEEIIIYQQQoivVweNubsbu+epdojt3fw5TgeFgllpuNKP52MM7xSe7VpvBfSnOTW/ClXSwjBKCq70Y6DajRZ5mvV2hDGG66OEaVriKFhp+DRDj27N50z39mBstyH2+vaURpjx8saI5bo/b2ctandXWRVYVWMb+9OMduTRCFwiX6NVFQJppbDGkpmqIfa2kx2WZ2HYfjvPYO8xmd4+IxFvfG7bkcsoyWkGLsOkIHAdQk/TCFySvKQfZ5RTy2PdGs3Q5VQnwtdVm2qSFsR5SZobBnHGtWHK2W6NrDR7Bo7N0MNRitDTezYhlQLfUfhmSjsYspmMuWZzTjR8JmnBNDPEeX5jybBqxQUuK82qSdgIPE4vRTyyFFEPPFqhi3OYr6PhZfjcT8MLn4AyPfj2N+g3nuRzK9/LF4IPMM4tybDEUgXVrqNwHIWvNWttn0e7dWqBu1gb7rgoB9ygCs38RjWyUQghhLjPjj1AA/gf/uKf5r/+q38Xa808RJtMY559/iXgzQkGu39Xr0X8xT/zQ4c+/7/59U/Pj11eavPUuceP42EIIYQQQgghhBBf1/Ybc3drYGGsxVGKwHOIZs2i/YKC3fMoxeHChCN2UCi4NUrJy5LeJKURugeGZwDacWgEVZtpGOfUfBdfKzaSnHFaNdHqgTfbgwWt0GOtFdKpuXhac6odzptne+nUfLqzQK4duVzsTTm31ryrx6+U4l2n2yzVfV7eGNGOXHqTjJ1pTj+Obw6EFJSFoelazp+osdIKOL/WPLABt9+YzBtHIjJOuT5KaeQl3dk4S+04dOs+xlZB5jDOAfC1ojDVyM/VZkAz8FiqV4HUlVlQV5hq5GR/WjUH676uPkczw39+vcfpTsSZbm0ePHYiD1crlmoe1wYJeWnwtIMCPNfBL6e4cZ8iT8mMoR1qal6d3iTD1Q7NsPo8yo25IQy2tCOPbj3gQ+dWON2JFtsntvUy/O5H4Su/DnaxdmZ68oN89ewPcK3xbi7sxEwHyWxfXfXcARTGErkOoacwttoRd26t8QDDs9luM78GfhP8u2tWCiGEEEflvgRo73nnOf7Gf/en+dv/8J9hjOHW70d3P7YWfM/lb/3lP8f6ieVDnfvff+ZZrl7fRqnqPN/xB77hiK9eCCGEEEIIIYQQcPuYO08bNkfpTYFFVpr5hBhfOyilcJ1qdN5qM7htx1iclSjFLGi7/y2TO+2+stayPckYJQUW6Na820+wh2FcsD3J6ERVgysrDZOsBBTlLLyw1oC11AKXwFVMsoL1dsi5E41997Dd6GQ7pD/N6E0yQi/mydXGbWMJF3G6E7Fc97nYmxJ6MSeaIcZa4rycv56RpxlPpmxfgEe7NZ55fPlQzbc7jck8261Vv1GK0CvoTVImaUHd14SexncdQtch8zRpbrgyiFFUYWfgalqhRxho6r7LS9dG5GXJKCkYxDk705w4Kwk9B89RbE0yaoE7v5ZL/XgeADqO4nQnIslLNoYp1wYJT6zWCUyCTgaYLCErbw6xvNkIxhPNgGluSPKCLLcYLL1xxlLN5/x6k/MnmvvuhruNtXD5d+HZj8GF3z7cMbuHKgfz+Ldy6YmPcNl7jJ1pzvWdGGvtm58f1lKUlsKa6ldTfc0qquD3Yi8mzgzn1hoo7lOgrRzQHgTNqm2m78vblUIIIcSB7tv/kT787R/izKl1/sE/+ThfevnVPW/z1LnH+Ct//kd4+u1PHuqcxhj+8U/+AvDm+MY/+t3ffmTXLIQQQgghhBBCiDfdOObu0k61g2s3sBgn5bx9s0sp8ByHRqjJypLtSXZbu2qcFoSexlGKZni4gOoo3Wn31TgrKY1lnJbUfY12Dgi2rGVzkrI5zEhzQ9/mNEKPE82AlbpP3Xdxdqqgbrke0Ag1oCgMrIQeWVEFRGe7tQPDC087tCOPnWnOiWZIP7597OCiQk9zbq3Jk6sN+nHOKMmZpOW8UVgPNHms2fyy5YmV2qHHRt5pTKZC8Wi3TiOoxkfWA2c+LnOSZVhbBZlxbkBV11iWBsdR5IVBO4pxUvD61oRBnHN9lJIVVVgZuA6PnKjRilxakctKI2CcFFwbJGwM02qEZGnZmWQ8farFmW6NS/2Yx1bqDAZDzHCIozLy8s7tL6UUdV9T96vnYxjnDOOcR7pNOjWf00uHaFJZA69+Cp79KGx86VDP665SeVxc/3auP/mDXDIrBJnDdBIzjHM6kc9K079jKJuXhs1RxrVBzDQrsLMv4vN32Wo8HFUFZ8Fu26x2jPclhBBC3J37+iMdzzz1Nv75P/gfeePSNZ59/iW2en3K0rC81OZ9T5/nbY+fWeh8VzY2+aYPPsM3ffAZoBrf+Ogj68dx6UIIIYQQQgghxNe9TuThOBBnBa9vT+lEHoO42vtUCzQtz8d3HRylMNaSFYY4L9mZ5PSnVcBTGsskLTnTjSiMZRDnrLdDXK3oRPc/QLvT7qs4KzDWkJeGdrj/SMVdm5OUcVy1qNKipF0LeXS5RiOonqeap4l8DUqx2gxYbvg0ApfeNGd7kpEW5XzPxaPd+oH31whc+nGMsXbPvV13y5k1Bvc631Yvv22y0EEOsztvue7TDF22RimezmhHNzcaTytIC8POJMNgscayNc7YHFcNyDcDUM1SPaAduTTD2UjMWbuuup+AvDRcHSRc7E0ZJ/k8MHrX6TZPrYZcvLyNY7Z5/cqUk+2I1gKfl8M458ogphV5LNU8Hl+p33lsY5nBl38Znv1J6L9x6PsBKHSNN059N1868WG2TIPJTok10/lo0KdPtmjXDv6cqPbRhTQCzZVBzBWqULBd845+nKNyqoaZ36z2m+n7/zUvhBBCHNYD6UQ/+sj6kQRdj5xcW2hXmhBCCCGEEEIIIe6e4yjS3MyDr36c80gnYqnmo/cYHxi4mmboUdYtvUnG1jibjQTcXYZevVHfrfvzMXr32367rwDS3JCXVfjjuXe+tt0W3k6cMclKVho+ncij7ldvveRl9bw5sxZbYSx5adGOw2ojoOZpNscpjFNQikaQsVTz7rhbLvAcrIU4L5mki+3Iup/uNCbzRr52ONWJONkOGWclcVZUjxuLQ/W4Xe0QpwVXhwlJXjXQSmNxtcOjyz6dyEcphXYUy3WflWaAf0v7ytMOZ7s1WqHLhd6Uq4OYmjZc3xix7uYMnYSspslyj8v9mHFasnrIFtcgzmhFHqfaISuNYP8AKhvD8/8Snvs4TDYXej6zoMuVx76fjTPfTenVWQFqeclzF/tsjarG3KPdGpPM0F6g2LUbFF7ux9R8l9e2JnQib7G9bXuatc38qArNvDoLp7BCCCHEAyBDhYUQQgghhBBCCHEol/sxFuhP83koEXl6z/DsRtqpGlc1X7M5StkkZZpVowHfeapN4GnOdB/MCLdbd19dHSTzvVyGg5tTAIUx9CYpcVbSn+bUfU0n8mmGHmp2nLEWyyw3sMxHE+6qB9VbNNdnDaz+NKNd81CofXfLGWPpxzlZUYVrD6s7jcnci1KKZuDSDPZ522oW2L62NaHmabLScm6tTjv0q3DRd2n4ev7c72e5HlB3odfbJO7lvDZWtB9pc26tMb+Omu9yfZQwTDKaoUfN04S+RgMlkGQl07xklOQopVhvRyzVPFYawfw8N5luw3M/A1/8+SpEW0Bcf4TLj/8Am6e+HatvfhJHcU4rdNmZZBRGEReGQZwReQ5LCzQTW5HHOC25Pkpohpqrg4THlg9uQ+5J2mZCCCHe4iRAE0IIIYQQQgghxIGSvOTljRGjpCBwNWe7NaZZUbWmeDMAupPd21zoTdkm5UQzpBW6nF9rHnqf1nHY3X11qhNxsTelFbp0aj4ONzen9nuEw7igNIbtcUJhLO1IM8kKaoFma5ziaYesMHBDIKdm7bsb1QMXNU55eWPEUt1nGOdox9l3t5zvKoZxwVeuj1ltHjxi8kG505jMu3VpJyb0HApjeepkk3estw59rKPAcyAoRzTMgLgYcXEr48nV+jwwOr/WpF3zeG1rQjPUDOKcQVwwSvLbXgvf1aw2A9qRh+9qHl+p394861+Ez/0UvPRL1djGBYzab+fyEx+ht/aNoG7/OrG2ClInaYHvOqw2fPpxwcQtuD5OaYTuHdtzt1pt+gyTjEGcszGsAmXn0I0xaZsJIYT42iEBmhBCCCGEEEIIIQ50sTclzUuu9GMeXa5hseyMMxinXB+lNPKSbs1DO/u/UV8awzQvSQuDo6BT87DA6U50/x7IHkJPc36tSVlaxknOhd4UgMBzZm0vyAvLnhmhtfSnGZf7CZuTlFbgkRUG13EYxgUKcLVimpVM0pxpluNrjesoPK1uOE2106ssDUluuNqPCT3NY8t1WtHeu+W2xinDpGC1FXClH/P85QFPn2od2Ly63+40JvNuZEXJlUGCo6ps5vGVwzWkquBM4ZdjnOmQssgwxrDc8OjH6W2B0VozpBN5XB0kbAwTlusWYy1J8WYbMJy9LtpRrLVCTrbDm0ceXn8Rnv0YfPU3wJqFHue1zvt59ewfZbL8HqLA3TfEmuYGYyzTzBB5mkbokZVVqBb5mt4kY611+F1mnnZohh6DuGC5bhkmxcH7Cedts0b1n3s0+/iEEEKIB0kCNCGEEEIIIYQQQtyRMZbL/ZjeJMNay8l2iLsb/ihF6BX0JimTtKDu///s3WmUZWtd5/nvs589niHOiRMRGZmRmXfgDnDhMshFQbAAKRUVB0BRtFGoKtsuq3u1vXp1afvCWr26ylVaq1a3XXYvu0qXS6raCRVFcQBUKFARlBnuPOTNMTKGM+/x2ft5+sU+ETnEkBF58475fN5l7nnHOWdF7N/5//+S0JP4roMUgmoW+GSqIi4qBHDbQpNhUiAdQcOTaG2elflnlzvejRjMru90P+HUZkLoOWhTBwqpKmmFOx+jrE5yntyMGaQKhzrgSlWFEIJUXZpLZowhrzRZocmFIVMVvnspRNqYFkwyxSQvUVrjOoJeM6AdeURXVedtzZbT2qANbE7r+XIXhikA9x7vPE136frs1ybzejy+EWOMwQjBytWB1S4E4ElBoBNkOqJUOUpfCrP2C4wCtw4xb+k1GGclca5Ii0vz6CLfoRl4zIWXBVzGwNnP1sHZmc8c6to0gq9Gr+Vrx97OsHk7nnAQgxTpCDqRR6+5cxZbpkq0MZRa0w7q4KoT+aRFSpyXeNJhqR0coooMGrNqQW0Mca72DtCEBD+EoG2rzSzLsqwXHBugWZZlWZZlWZZlWZa1r2GqKCvDIFF0Im/7Af6tvSatoOD8MKUZOEyykmleERfFzpaD0mG+4dEOXTwp6TU9Ak9SzuZ43Yi2fk/Vy1bqNoBCCFphwblBwrlhSqk141TTDOpWeNoYclVxYZSzOk6ZFiVlpWl4Lo3AYz7y8Ny6cs0YKCtDXlaMUkU6C87GmWKSlUSuZJKXTPOScabIlKbXqCuIHFFXW10doEFdzZeVmhPzEYErUaXmdD9BCMF803/Wq/qutlebzMMaJgUXxxnzDY9BqvadnVcHZw6+TpHZEK1yiqradd1rBUaOEHQjb/9KLF3VlWaf/8+w/sChrqsUPl9sv4k/897CyD1Cu/JgnCMEuI5Dw3dQlWaYKo60givmmhXKUOq6Pajr1gGWdCD0JUmhaYeGtKgO1GZ1S+hLjIGs1KTFVZVzwgEp69lmttrMsizLegGzAZplWZZlWZZlWZZlWfuaZKoObFTFUuvKWVsLTZ926LIxyfFkQScyGGMoqktt7uo2iHWbu17DIwpcNiYZp/tJvQy4c7lFO6wDimerGk0Iwb3HO8w3fR6+OKET1VVFT2xOWZ8oHl6b0gnrAGWcKopKU1YGgSBwJSfmIzq7hEKehMiv56LlqqLUhmleMs1KtIa8rEiLkkxpOpGHdAR5XFBqg6rMjv0B9BOFANqhy9G5iIYvObWZ0AoLHr44YaHpP6tz5a62V5vMw4Row6TgdD/Zvq6eELR3qQqEuuLMNzlePqIqUtQewdn2+e0XGF1LmcODH65nnI3OHGrTwm1x/+Jb+Wz7WxmYFmlacqzp0wpcNAZV1kHpOC23K+O0NqRKc6wTIIRAXzZbr343za7JdRgqNbuuwwVoW68cY0Abg51tZlmWZd2MbmiA9m/+r1/jn//IO1nsdW/kbm+Yj33yMxRK8bZ//E3P9qlYlmVZlmVZlmVZ1vNGnFfbc59Cb+fsKl86rHQjjnVCpkUdBuVKozE4CALPwXXqNoj9WFFNCzJV0o8LPBmjKk01a4nnyrrd38le41kLgI53IxaaPmf6CdIRGOqWeKvDjE7oYqhbMo4zhePUIaKBXVs8bslUhSMEvaZPoQ2F0mxMc0KvxBEQFxWhV7e/rGbtBY0Bw84ALZ6Fb4utAE9KFtsBvnToZSXnhymdyOVMP+Gu5fbTcn+MgWGiiE1MnFfb7Qybgdw3BN2tTWYvKznWCfediaYqzYVRRj8umG94zEUemarIlEZeFeK4jiAQJW4xxBQJRVke6Jp2BkYHkE/gK78LX/5tSDYPts3WpuEiDyx/D1+aezOtVoeu1lRJQaY0jUDOWqQKfOnQDKCKYJQWDBK1/V4EWOmGOIjtLEszC7sAz3UwBpTWFOqA1zSzFTd6rsQLQmj0wG/aajPLsizrpnJDA7Q/+ugn+eh//Tt+6O1v5b95x7cz1z7YENen22c+/1X+3//yQe5/5HF+7Iff/myfjmVZlmVZlmVZlmU9r2hzqcLl6sDickII2oFL+6pKl8244NywrgLaavOYzgI0YyAvNamqA6T5Rh2OnB2m3L3cftZaEYae5K7lNncstVjpRnzpzJDAdRjGBUobAs8hqlx6iz5ZqenHBdpcCmIul6mKcapo+BJf+oBhkpdsTgsCT+A6Dp50aM3um57dayFAcOX9jvOS9WlOK5C0Q5eVboQ/C5+OdUKGSUE/Lgi9lDuWWje0mi9TFY9vJDw+FSydn9BqVqSq2q40jDx5zRD06jaZ54cpw6SgE3m0ApfIl9uz89KiYpqXjFKFEIKTvQYLTZ+0qKiM5tG1mGr2wnQdgS9KXDVG5FPUAYOzLVuBkRBce1bYdB2+9Jvw1d8HFR/qOGXnNp645fv5UuO1jAtY6UTMRR7nhumuVWRbpAO9pk/oVQzigj7F7J47+J7Ac+qWoWVp8OWV+zFmK1g7GEcIDA6NuXn87jJebwEaz41nfJZlWZb1TLrhLRzzouDXP/DH/M6HPsrbv+PN/NDb38ryYu9GH+aatNZ8/G8/x/s/8GGfyahSAAAgAElEQVQeevzJ7V/mLMuyLMuyLMuyLMs6HEdcqnCpDlqdQ12ldXqQMIjreV/9OMcATV8SuQFaw/FOyJG5kIVWwCRTrI4yLo5zVroRVWUYxAUvW5lDPEt/1DuO4GUrHYyBpVbA554c8ORmQlyULM8FhJ6knNZhRlUZLs+LtK6DskxVhJ7DXOjRnrWADD1FmldsJjm+dJhvBMhZ2FVWejb7SuDJ+v8qreknimlW0gokS62A+abHwmWzsDzp0Ik8BoniSDu8obPlzg1THr44YWOQMC7g0fUYOVQ7Zt1dKwTdrU1mP64rq4Zpuuv+jnZCek2fYNYGsqw0D61O6sCoMkTS4KsRFBPKssQc4jW6JSuq+niuQ+TvUQ03OAVf+M/w4J+CVoc7wNFXol71I3zOuZfNuGQ0SjnercMzYM8qsqs1fAn49OOC2C1Zm+Ysz4Xbs9KysqIRyMv2MwsF99jf5aSUSNdH+y36E0FsIDUBjWCfuW+WZVmW9QJ2QwO0RhiQZPWA0yTL+a0//Ai//aGP8U1f/0re/u1v4hvvewVyn5L8G+H8xXX++GOf4o8+8kk2BkOA7V++jIFm47k1RNeyLMuyLMuyLMuynuuagSTyJEJQt5g7YCZzepAwmBasT3OmeUU7dJlveEjHYZIpfNehEbh0Gh69pk+v6W+36zvTT5hmajsMufd452m8wprWhmGqmGRqR2vCY52QUmtCTxL5ks24vqaiMmSqrl9KVImUgrLSFJUmV3UQNhe6RL5LK3BZavnbtUC9ls8kV6RFhSPqqjLfdUiKen+lNhSVYX2SERcVAlhsBfV9bHrc0mvsuIZW4DJMU7QxTLKnHqBpbbj/wpjVUcZmXPDoWsKkFISuw9H5BqHnbFeMZUofOAS9vE1m6KUcaYdoYw5U0daPC1xHsNRycfMBvlCUpbqu4GxLoip8V85+3lcFRhe/Cp97Pzz+cThEJRcAt34T3Pc+WPk6zm3GFP2YtUlGJ/K3wzNgzyqy3TR8SaYkw1QR+ZK8qHAcQcN3GGcllTZIR6DK+vXnOXWV2m4cx0FKCV6D0muROyFpUXJ2NOZoJ0RKQTeyAZplWZZ1c7qhAdrv/cov8H/+ym/ysU9+9tK3ZrTmU5/9Ap/67Bdot5q86XWv5k3f+Gpe/fKX0LpBYdZDjz3J333+q/zlX/89Dz12CrgUmm2dx2Kvw0/+s3fz1jd/4w05pmVZlmVZlmVZlmXdLNqhhyMEoScPHMpsxgWDWLE+zYmLiiPtgOZlrR1TVc0CA0F0WdmWJx1u6TWYC11O9xNO9xOEEMw3/aetnWOmKs70E84NU8rK7BnkpKrEcQTaGG5dqMOcaVYyzUtSVc99y0uNdARSCJqhpOFJpOPQa/rb1WcCWGoHJEVJ6DmoyhD6LqmqWyKOM0XgOZCAJwW+W1d1tUMXT0pWZuHTbiJfYkx9f+O82nWdw7j/wpgLw5TT/YRBopgLXY6EhhPzEXNXnUPD51Ah6OVtMvcKLnebqdYNJXMi5qjZ4EJ/Qmehse8MtWtRVR38LbXrKsC50K0fLJ3+NHz+1+Hc5w63QyHh7m+HV/8oLNwJ1G1QL44zRml9P5baV9670HMRIt9RRbaXTuSTFilxXtaVh6FHWWnGWckoU/QadWtRdxbKhe6V+3OlRLgB2m9RyAbKOJTagNacG2aI2by+493ohrYBtSzLsqznkxsaoC32uvzcT/8L3vkd38x/+LXf4YFHTm0HWMbAeBLz4b/4FB/+i08hhMPdt5/kpS9+EXfedoIX3XKco0cWWOrN43m7n9ZwNOHiRp8z5y/y6KmzPPLEab70tYeZxMn2MbYIUf878H3e/b3fxvt+4LtoROGNvFzLsizLsizLsizLuil0Iw9XCuYbHqujDFXpfQOLotKcH6bb886uDs8qbUjyivmmh+uIK5ZtH3NW5nZqM6EVFjx8ccJC098xU+up2mpNmKtqu5VgNgvPtmy1EtRak+QVqtIstUMavkcnqs9pY5qzERcErsN8w0cIgRTQCj06kYt0dt6vyJcsNgNSlRK5knbkUlYGA8w3fXqRx5G5sN6XI1ho+iy2g+2ZZ7vZmlFnTB3aPNV7szrKON1PGKWK2xYaOFpx+hp5ymFDUMcR2xWI+zIG8glONmTJiUmcOmxbnxSsdK//mc/6pEAIQSfyWG65OI98BD7/fth4+HA7ckN46dvhVe+BuWNXLNqqDBulJe3Q2/H+aXjOrlVke5EOhL4kKTTt0BB6Elc6dCOfQVLgOyVZUTEXuUhHEPlyVm3mYvwGldtEibqqUlewVVm3NUPvZK9B4ElO7lLlaFmWZVk3ixs+Aw3gvlfcw/t/8X/jr/7mH/iV3/gDHnvyHMAVYZoxmgcfe5KHHn9yx/ZRGBIEPoHnUVUVeVGQZgVltXMA7NW/0G79n+d5vP2tb+Kf/OB3szD/9Ld5sCzLsizLsizLsqwXKsepW+hlquLiOOfCKNu1feCWjUmOqir6cU4rdHcEZP24nhnWDl16TR9nj/lm3YZPLys5P0zpRC5n+gl3LbdvyDVd3Zrw/DDFGEMn8lhqBbu2Jnx0LWGQFBRlPaNqbnb+S+2Ahy5OCDzJaNZWr9vwCF257+w2Rwh8z8GXDnORS+RKUjTHuz7NwOVFS01awaz9o7//vrZszagTgj3v60FkquLhi5O6kjCpw7Nuw2c8Pfjsr6cSgl7eTjNTGqliZDEiQNHwJcstjwsjyZF2yOoopRXIK1oiHtQ4VYzSgpWW4OTZP+HWv/0gTM4fbidhB17xbnj5D0DU3XWVOFdUWlOUFb1deqAKUbdKvLqKbN/Dug5DVc+hq4yu22DqlLyUnB2mBK5DK3BZbEcEYXNntRn6iv0Nk4LT/YT5Rj1b7+7l9g0PrC3Lsizr+eRpCdC2vOUNr+Etb3gNf/sPX+Y3/+DP+ewX7wcuBV1wZQC2JUkzkjS75v6FuDqUg153ju9721t419v+Md3Ojfml+vlkoz/k9LlV1jcH9IcT8qKgqiqiMCCKQpYXe9x28hjHjizesAHMG/0hDzxyis3BkMFoQrMRsTjf4daTx7jj1hM35BiWZVmWZVmWZVnWs+tkr8HZYcpKN+JMP2EudLcDkssZY9iMCyZZiQF6jStDjTivWx4utnw8KVlqB/se91gn3K6KCb2UO5ZaN6Sl3NWtCReaPkc74a6VdVutCUttyC5UbExT+tOcQDog4NZek9CTnOkn2/PKtOaaf3d70sGTdUCRFBWVMax0IpbaISd7jT3bNO4nLarttpPNa7QB3M+ZfkKuKs4PU3pNf9ef9UEcNgS9vJ2mADydUSUDyjyl0hWh6+DMKvI8R2wHZ+dHKcChQrRxqtjYXOO1w7/gxff/CV4xOtzFtY/W1WYvfTt4+7cXTQtNXpm6W5K3ewVhr+kzTNV2FVnoVjT2GYbmuQ7GgNKaQhmOdT2SoiTJS1zpEAUByp+juXiM1G/uqDbbstVysx8XzDfq2XpHO+HT1jLVsizLsp4vntYAbcvrX/MKXv+aV3BudZ0/+Yu/5s8/8WnOXljbXn49Oc5WYAbg+x5veM0reNu3fBOvf80rcOXN8+2YOEn53Q//JV/46kPc//ATDMeTA2232Ovyxtd+Hd//XW/hrttvOfRxjTH80Uc/yYc++km++uBjew7qPbmyzLe+8bX86Pd/J80bNPPOsizLsizLsizLeuaFnuTu5TZVZZhmitP9epzC1cHKtKiotGGaVzR9eUXrwjgvWZ/k27OtVvYIrC7nSYdO5DFIFEfaIcP0YDPY9rNba8KDBES+dFhsB4yzkmlRsT7NQQhaQcFC02eaq/phxTRnbZLTUhW9hrdr+8at/WljUJVhmChuW2yy1AqYb3rXFZ4BTPOScDazbWvm2mFpbTg3TOnHBcYYjnWe2kiMg4agW+00tdZkaUI+6ZPGE7LiUtWbEOC7kk7k0ok8NuNiO2Q6N0yZ5hVLbX/f15WqNNON89x65oN8y+Zf4uprf4n7Cr074L73wZ3fCvJg91gbs/0ca6+nVp50rqgiGyQF4O8Zojlc1q5zForNN0M2c8Gx1hG012CsBV+8kDMX6Vk1o9yurEyLimleMkoVQojt0PZoJ+RlK3OHuCGWZVmW9cL0jARoW44fXeLH3/MOfvw97+DU2Qv87d9/ic995UEeeOQJNvoH/5aP77ncdfst3PuSO3jdq+/lNa+8h8B/ar88P1+tbw74f379dw+93UZ/yAf/7OP8wZ9/gu/5tjfyU//iR/C9g/3S98Tp8/zrX/xVvvLgY9dc98z5i/zab/8RH/7Yp/jp/+G9vPG1X3foc7Usy7Isy7Isy7KeG453IwazUOV0P+HUZkIvKzl2WRCWFiXaaFSl6YR1dVmlDf24YJqXNAPJUiug1/BZaF2qPtPGEOclqarIlUYbgyMEgVfHBPV+DZPsqQVoV7cmvKUXIR3B2iTbcdy6isvdboUYzNotRr4k8iTTvCL06uqqduheamspBKFX0o9z4ryk6UtCT+K7l9pCFqUmyRUXhhlKa3wchIC80kSewyQvD9y2cYuqNKNUcbQT4sq6JeD1GKaKsjIMEkUn2jmv67CuFYJutdPcmOSkWcZ4sIbOJngOzEcuwZyPBCogV5q4qIPYjWnBkVZAWtStCI92QtYmOeOsoB16NDxJ6MvtbbOiQo5O8aIzv88dg79Gmp2jQva18nXw6vfBrW849LfBHSG2N6n2WW++UVeRYaA/Cx2zUtIJvR0z0bZCM891CHyPzSqkX/rMHWniuQ5xUXJ0Ltye7TdM011n+x3thPSaPsEsJLeVZ5ZlWZZVe0YDtMvdduIYt504xg+/49uBOtA5e2GN8xfX2RyMyLKcrFC4UhKFAe1mg6NHFlhZXuLk8eWbqsrs6WSM4UMf+a9cuLjBL/2b/wVnj2/FbXn89Dn++U//Wwajg1W6bVnbHPBT//o/8L//y/+Ob3vT657KKVuWZVmWZVmWZVnPoq3KFCEErbCeHTZMCjqRRytwGSWKpKgoSk1eViSTkiSvcAQstnzaoUev4XOyVz+kV5VmfZLTjwtKbTDGUFQaY2bVRtKhqDSro4x26HGkHXLrwvWf/1ZrwtObMdrA+WG253GFELiO2J5zFnl1oOU5ddjVCl36cU4zcNiY5Kx0I27tNWkF9X1pBg6TrGSaV8RFsR1eVNqQqhJVGQyGhuegtaFQdRB0bpAhRI50BAtNn8V2gH+AEOvCKEOI+nyPd6PrbnU5yep5XZmqWGrt32LzoFqByzBNdw1BH1wdM5wkTPrrTEZ9QilY6AS7BneRV8+XU1XA+qRgdZwxF9VhWa40dyw1GaWKUVoyydT2PT8SP8Qr1v6QW0f/cPiTv/1NdXB27BXXefUQ+Q6hOwtJlSbaZ7bYSndW8ScgcCuGaUFaVESeJHAdPNdBIqi0IAgiUrfL40ULH5/FVkBvVkV2x1KTs4OU0EvryjZjSFW1/RqPZpWKrqxnHJ7sNezMM8uyLMu6zLMWoF1tsddlsdflVS+7+9k+lZvSZ7/4NT7wx3/Bu7/32/ZcZ3Mw4id+5hcOHZ5tqbTmX/37/0S30+YbXvWy6z1Vy7Isy7Isy7Is61kkhODe4x3mmz4PX5zQidwrKlzWJhn9qWKQFDgCIs9lvunRDl08KVnphNuVZ5vTnPOjDFVVddCUVSitd1TJOMAkL7k4zvjimQFLc8F1VclstSZ8fH3KmUHCsU7EZpzveVzPcWiFkqKq2IyLurLLEbRCySBWrHRD4rxkkpV4suBYJ0SIOvRqhy4bkxxPFnSiSwHdJC0ZpgWRJzGmotQGRziEvsMkUzy+NsWZBXS+dDjv13PSTsxHHOtGe1albbVIPNlrEHiSk1vVcNchziuysr4f4R7zug4r8iXGQKoq4vxSDdbqMGY62GCwvsrmJOFoOzzQHDNPOqx0Q1qB3J5/dqQd0Ag8Aley0DRorWle/Ay3nfpd5odfO9wJOy68+Dvh634UercfbttdNAMPRwh8VxIXJd3G3tcoqAOthu+yNsmIfIc4L0kKjdKawDjgN9iofAaVZC7zuGsu2P7ZX15FdtdymzuWWgxTxSRTxHm1XWW51Uq1G3k3ZK6gZVmWZb3QPGcCNOvGOLmyzEvuvI1bTxyl3WoCdZvHz325bpW5n9/7k7/aN0D7xV/9LfqD3VttRmHAW9/8Om4/ucLmcMxHP/F3rK5v7livqip+/v9+P7/9yz934JaRlmVZlmVZlmVZ1nPP8W7EQtPnTD+5osLl0TWJL1MEcGI+IvTcK6q4vNncr7P9lH5SMMnUbNYWNALJnOfjuw6OEOhZq8NxpphmJeeGKe3Q44HzYwZxwctW5g7V4rCfFDy+FvPI2lb1WbrvcVNVMYgVw6SumKq0odKaViAZJnWVU9OvWzl2IsO0qGgH9aMWXzqsdCOOdUKmRUWcK05vJhhh8KXDNC9RpWa5HbLU9jHANCvZjAsiz0EgWFd10NQKXIZJwZObCUc7AQvN4IqqtGFScLqfMN+oZ6fdvdx+SpVEV8zrup7B9bvY2o8xYDCgNXk85PyTZ9gcTlkbxhzvRgcKzy63tf65YUrDdwk8ySuPNdEPfxT/y/8Fb/j44U7Ua8DL3gmv+mFoLR9u2/3OM3SRjqATuaxPclS1e4Xd5eYbHq1A0o8LGqGPIwNKt8nY+EwLGCQxi62AxVbAHUdanJxv7FpF5szef091dqBlWZZl3WxsgPYCcOLYEd75Hd/MN7/hPk4c2/uXu0995ov87L/7ZeJ09+G4T569wNpGnyOLvR3Lvvi1h/nzj3961+168x3+4y/8DLedOLb9fz/2Q9/LT/7sv+cLX3t4x/pnzl/kNz745/yTH/zua12aZVmWZVmWZVmW9RwWenK7wqUfF5wbpmxOc/pxDo6hrAydOZdes27duDVL7Gw/ZTPOWZ/mxHlFO3SZb/g7ZjwBBG4dBiy1Ne2gbpn45GaMmSU89x7vHPh8v3B6wPo0Y32SEUjJ0lyw73HboUfVrOe3bUwLUlXRa/iMspJe02djWtDwHVSlMcaQFuV2gLZFCEE7cBlMCzzpYAxUBtqhh+9KludCHAfirMR1BALYmBa4jsBzHfJSM0kVG65DJ/SY5gq1oNmMC460A/JS048L5hset/QaHO2ET2mGldaGSVayOc3ZmOac2nRmwVQ9E05fXqZ3CJUxSEcQeYKwmsJ4yOraiGkSszpK6ET+ocOzLXORxzSv6A+HvPjiX+N9/A9wk4uH20k0D6/8Ibj3XRDOXdd57McRguW5kLys2JgWrE+KS60a99rGcWh4HtFcj1I2GJYek1TRKCqGWUqvEfDio23uOTbHq2+Zt1VklmVZlnWD2QDtee7EyjIf/NV/d6Bv3P2j176K//HH3s2//aVf33Od9f5w1wDt9//0r/bc5if/6Q9eEZ5BXZH2r/7n/5bv//H/laraOR73g3/6cd73A991qG8KWpZlWZZlWZZlWc89mao40084N0wpK4Pvbs0Jk4xSRTNwGaXldhWadAT9pGB9mpPkFUfaAc1g/8cTmaoIPcmRuZDFdkB/mnO6nyCEYH427+tazg1TzvZTVkcZmdLcutBgvnHt+V7SESy1Axq+ZH2SA8X2/KpmUF9jWdXtGfPZDLOrbU7zK665FUjiog4Os7IkdCWhJ1kdZziOYC50KUqDQNCNPLQxTLOKOC/JK80wVcxHPo+tTZmLPF5xssNiM+BoJ9yeUXdYl/8cz8+C0EFcANAO3e2ZcHmeM1b17LqDEgLQhiU/Y14lRIWLVgGro5RRqjDGsNS+/uootxjxmosf4uiTf0RYHXLsxNxx+LofgXu+G9z9A62n6lgnZHWccaQdsjpKaQVy19BQSol0fbTfopBNlHEotcGXsNAKkElBEEvuPNLmyFzAvcc7NjyzLMuyrKeBDdCe51x5uJYMb3nD1+8boO0mTlI+8bef23VZMwr5ljd+w67LThw7wn0vfwmf/eLOPuOr65t87ssP8ppX3nOoc7Esy7Isy7Isy7KeO84NUx6+OCFX1fYctLQoWR1lxIViLa/IlSbwJK1QkhSKi+MCVwoypQ8UnlVaExcV8w0P6QiOd0JavuTUZkIrLHj44oSFpr9vy8JMVTx8ccIgLWbtFj3aweGqnbbOc22SE3mSotTMRx5VZXiyn7AxyVls7QyBVKU5P8qYZIpJqvDcuuVjK5AYAFOf3zSvWOlGuI7YDuXSsiIrKipdB3lJURJiGKoKVWoWWwGdyCUrKu65a+66K8+u/jmeH6acHqSMMkVclHQif3smnEvFWAkeXU9A+tvz7HYjAE8KfJ2SxRdx04QyDGn4HcZZSaUNo7SkHXrXbGe4myC9yLEnPsjy2T9DVvnhNl58Mdz3PrjjLfW8s2dA4EpuX2yitSEpyu3ZbXORh+M4SCkxfpPKbZKLkFJrdAVwqervRrfrtCzLsixrbzZAu8mEwf7f6FpZXtzxf//wpQfI8mLX9V9+z537zjJ7zSvv2TVAA/jkZz5vAzTLsizLsizLsnaltWGYKiaZIs4rtDE4QtAM6rZ63cizFRfPIq0N918YszrK2JwFLsYYOpHHUqvJXOixPs0400+RUuC5gkGsOJMrgFkg5tP0r/3gv58oBHUV1ELTRwhBt+HTy0rOD1M6kcuZfsJdy+0993Gmn5Crio1JQTuU5KWhMubQD0WagUurqEOmE/MRGEGv5TNIChJVcWojwXUcWoFL5EukEJwdpvSnOU/2EwzQlQ6Ls9ApUxXGaJKrwsRW4DLOStxM0fRdjKnbYY4yharqdSNPUs1mlS3PHb5ySmtDPyn4wukBZ/spg7RgY1KHm4stvz4fXzLKFMtzAZU29Uy4qWJYCMZZyZlBSpxXnOxFV3SYqYMzB1+nyGxInqVc7I9YagfIWYXdhVFKpTVFWbfFPIzG5BQrj3+ApQsfR5iDV8IBcOLr4dXvhZOvm5XGPbOW2yGjpK66Ow+sx4pKBsx3e1R+a7vaDK68LlVpLoyyG9qu07Isy7Ks/dkA7Sbz0GNP7rnsJXfeynxnZ6uHBx87tec2d95+ct/j3Xnb3ssfeuz0vttalmVZlmVZlnXzubodoDb1Q3tj6mfdkSdxhMCVguPdiJO9hq2+eBbcf2HMhWHK6X7CIFEsNH2OdsLtKqJW6BIXFctzsDHNafouvYbP/RcU/bhAG0Ov4bM+LVhq713BFOcl06xksRXgScniZese64QMk4J+XBB6KXcstXYNVbU2nBum9OM6HDoShpwdpqjScI3it131mn59XnnJQjNgzpWshi7HuxFN3yUrNcM0xRgwxnC6nzDNS1RluH2xQbfhIRAks7aUG9NyRyWeKx16TZ/5hkemNEWlUZVmLvJYG2eEnsORdsjtSw3ODjLGWXmgSjy48j32+FrMRpxxYZgxzSvaoeRIGFKUdUtKIcBBEBcVS62AdujRkIa11XounHHk9iy6WxYaCMCVgkBnuPmYqkhRVcXqMEMIQSfy6plvQpAWmryqA8DAO0D1mTG0B1/l+OMfoLf+2UP+1ERdafbq98Lyyw657Y1313Ib6bp4rXn6yufJseGxixXNILkifK2MIS0qpnnJKFUIITjZa2y/3663XadlWZZlWQdjA7SbSJYX/NKv/c6ey//Zu7931//fL3Rb3mVe2hXLl/Ze/sgTNkCzLMuyLMuyLOuS3doBZrPwbIsQEHpyFixUnB2m3L3ctlUYz6Bzw3qO2Ol+wjBRLLYDfClYHWVoDA6CwHPoRC5lpcmUZH2a0w5c2qHHNC/Jioq4KHGlQ+g5tMOdnU3ivGR9mtMKJO3QZaUb4V/W5s+TDp3IY5AojrRDhqmi19xZyTSctUMcJIrFVkBRajzpkKqSVnj4xyLSETQCyTSr6EQGqeHOpRbzDZ/5pk/kye3gd5KVFJVmfZKz1HZYaocsNH1KrTHTnDP9lFbo7tnGUghB5EsiLoVijgOqNHiuQ+BKek3/wJV4l7/HHl+f8shazPqkngnXiTzy0nB2mOJJh8hzmGT1zLVsnNPwJM3ARTqClguLLZ9JXrFOjiMEvabHcsPg5mNMkVDM5qGPU8UoLTjaifBdybFOXS2nZ9VzAPtGfkYzv/Z3HH/8A8wNHzjUzwrHg5d8Vz3jbP7Ww237dBAOSA8RtLljvkU0VcSrE271Ln3mbYWv25vMPvOOdkJ6TZ/Ak/Yzz7Isy7KeITZAewEzxpDlBatrm3zuKw/wW3/4UU6fW9113X/67u/hza+/b9dlZy+s7XmMXnf/bzvtt3wyTRiOp3TnWvvuw7Isy7Isy7KsF7b92wEGhJ6zXY2RKc0kU6yOMi6Oc1a6EVVlGMQFL1uZu6KNnHXjbc0SWx2nPLYe0/AlG5McY+qKpa1KQV86CCEYJAopBKHrcGGUoXTdlm6+6ZMpjS9L+jE0fIl06nCs0pp+ophmJa1AstQKmG/W856u1gpchmmKNoZJtnuANskUldZkquJEN+L8KKMVSAaJoqf19nEPI/IkSVFQVppxWvGSY21WuhHfdMci47zcbj16bli3jszLitsWW5ychR5fPT9mkpUYoNc43Cy2rWObWUh3kEq8q99jpzdjzgwStIFASm5daNAOPCpjUKUhVSXjrCQrNUZDUVU8uj7hzqU2W3er4UvCwCXOSwKhyIfn0SWoy1oqjlPF+VHKXOQx3/C4fbFJ4NZxmSPEdgfFapfrFFqxeP7jHH/8d2nEh/sCbikbTO78XuZf/15oLh1q2xtP1MFZ0AC/DX5je8lKp67MPNNPCL2UI+3QVt1almVZ1nOIDdBeYH75/b/Hr/3OHx94/dtvWeG/f9+7eNPrXr3nOnGc7rksCvfvsx6Fe7fiAJjGiQ3QLMuyLMuyLOsmd612gJdr+HULva15QGf6CdNMbbeRu/d455k+/ZvKmX7ChWHKZ0/1CaVDXsJmXKBm4dkWIeoKsVYgyZQmLzXSEYyzikmm8GUdnmJk72gAACAASURBVAxThes4rE9ymoFLpiriokIAi62Adugy36znPe0m8iXGQKoq4ny3GAbivKqDIFOvv9D0UVXFMFH0E8VSa/+/W3fjuw7GwNokJ/TqKrDj3QjXdei5/hVBXlJUdfXbbH7bJC+ptGGaVzQvCw4Pe+yi0uRKH6gS7+r3mDFwrBNxfpiy2A6Yb9T3wAUCt27B2ZsFmecGKcyqxR5Zn7AYuWjqqqiFpks2HpFsjpiEDmtVwPJciKo065OCUVowF3msdEIWWwHL7UvPECLfIXQdhIBcaaJZKOSUCctn/oyVUx8kyDYOdW8yr8tXlt5Gec87ueXYEeabu79unhGzajOCNvgtkLs/ggs9yV3Lbe5Yatm5j5ZlWZb1HGMDtJvYG77+lfxPP/Zubju5su96cbJ3gOZ7+7+EfG//b9Ltt+/9DEcTNvrD69rWsp5P+oMRSZrRH4ye7VOxLOt5wn5uWJZ1WM/258bqOOfhtZgzg5RJVnKiGzLnG9I05Vp/LXR9cCo4258wTVImcQQq4+jc4QMR69pKrfnoV1Y5tZEymOQEsg4/Gr6k6Uk8KXCEQBuDqgyZUqwm9ewrXwriTEFVIQVkhUJrmOQVaa4IXYeFlocvHZq+pBW4uKJiPnCZ9+sOJrvJS02aZYyngr5v2Aj1jnX6wynjaUKaZcSJJBCgCkXDhf44walKGsHhKnpUpZnEGVMH7lpqkmcZDRHs+Dv16mOXhcPGNCdOc6ZJRq/pk2bZoY9dFAVJChPXMPYNVIr+OGPYEJxe1ej5S+39rn6PrXQCLowLhokiKxQLkbPnObRcODHn8kS/bivoS4dRkhH6Hnq6RhoX5EXB5rQgyyWjOGM8TYiLen7aYsun40HgVCwGmv5ovL3vMi9JkoyqVGyMKhp5xsnzf8It5/8Ur4wPdU/i8BinTr6dL0TfSGpcblWSMs/oj8pD7ecpEwLhSITfRHsNjBNhUgPp9MC7aApobueMBtDoXNHPn44TtqxnxrP9u4ZlWc8/1/O5sdjr3vDzsAHaTexv/v5LfPpzX+Zb3/g6/uVPvIdOe/dKsCwv9tyHlPv/keG6+y9Ps+v7DfCv/uYf+PIDj17Xtpb1fJKkGQ888gQAjWj/ik/LsiywnxuWZR3es/m5UWp4MhZMFIwKwXxgGJ07/H7SCh7IBQ/5hs94cGvT4B6+K99Nx5j63uUVFFpgAAH4jiGQEEm4vCPmqang1FSwmgm0hq5viFzYPdqqaSAtIa8ECihKyDV0vHrfVQnDuK56KqYGV9T/33INHQ8Gbn1Oe1Ea1jPBxhnDqQDuj8yOdS6mgo0cNjLB5hmD50Bc1q+5SSk4q+vj+Yd4zSQlrOeCjg/+dI1g03DxwZ3r7XbsYSEYKxgXgrFfX/NhlBrGqt52zTOc8a+8Dw8EsDy7D7u9x9aAzVwwUgIpDMkBiry0hsy4BJFL20nIxxd4bCLRs9udVfXPuiFhLjC0JYQuTAXM+4aBB49dtU9j4Ewi8PJNXpp9im8o/x6PwwVeF+QJPhO9iYe9e6k2HDaLCzQlDM9D/wnDM9XR1fN93CCkchvk+OTKUCh1RVWmZd3M7N8olmUd1vV8bvz4e95xw8/DBmg3Oa0NH/nEp/nKg4/yH3/+Zzh6ZGHHOmHgE6e7fxutrPb/5VaV+y+/VovHvbzlDa/hzttPXte2lvV8svUti+98y+vpzdt2RJZlXZv93LAs67Cezc+NxzcSlvoJD68l3BO6HO9e/0O1c8OMcVZy95EGt/YavGjxWWzd9hyXl5pzw4zVcU6pDdoYcqXRGBwEgefUM5ccwdG5gOPdkEGi4PEBk3NjkmHGLfMRS+2d88b2kuQVpwcpRaUpKs1S08NxHDbigmmu6YaSucilE3mEnoMv63NwhGC+4bHQ9HZt6TlIFOdHGfccbXHnYoMTl1VebTk7SHl0I+GB1SkrnZD52cyxs8OUYaLYiBVpUdEMXLqRi9ynTV6lDcO0ZGOa41eGlx5tce9KmzfdtfNv6b2OfXaQcnGaszYuONYJ8eThUp5pXtKPFSfmQ47NhSy2fPJS8+h6zG0LEbf3GrzkaP0F2d3eYxvTggujjLPDjF7ToxXs/2jIlYKmJyiTCXk8oMwqzgF3n1zE931KbUiKivGsgvRIK2Cx5bPU8lieC3b9uQHI/qPoL/x/dDc/hWBn5eB+Nrqv5NTJ76PffTkNIXgVcHGS081LbluION4Jd30t3FBb1WZeA+23MDLE5mWWtTv7N4plWYf1XPncsAHaC0yjEV16QRlDmuUHqvI6v7rOT/3cL/Fr/8fP4l5VVdZsRHsGaErt3mN+S6H2D9Cajev7hbbbaT8tJZmW9VzUiEJ68x37mrcs68Ds54ZlWYf1bHxuaG346nqBEh5RGHDnsbk9H7QfRBRFPHBhjBIeiXHpdTt2XtAuzg1THh5MyJVgWjkMEkWmqssqZQxCaEJPMt/w6BeC4XrBOFPElUOuHRbaEcvzTYJrdBy5XBQC0uWRtSmlhtVJxfGeTyOAuMgpTL3vrHLIKhBCz2aoOUxLyKealW7AwlWzvQZ5TG9O0m23uOXo/I7ZXwBO0GAjd+glBqTDXKsJwD2tBk9uJgg3ZRArNqY5m2lJ5Lm0fEkzdIk8iQGKUs/ms2kEDt1mhCcdTizN8eaXHWdhjzlqux27Pat88zMIAv9Q9xFgojJakaQZRSx1m7RDj6QoicKKuVaTXrfNYm9uz/fYqBC4vsb3NXPNcM/jS0cQuYIWKbIYkoiMc2VJ4EtavsOLjszh+j6FMqRlyeoo4+h8kzuOtLit1yRVJZNCo1U9yyvyHZq+y9zml3C+8H44/elDXbfBYfPYP+Lc7e8i7twFwFYfnXGqKIzilqUO8y2fF5/oHvq+Hphw6nlmfhuCVj3nzLKsa7J/o1iWdVjPhc8NG6C9wLz3XW/jve962xX/N01SHnrsST72yc/wxx/9FIVSu277wCNP8LFPfobv+ObXX/H/zWYEm4Ndt7nWDLPkGstb1xmgWZZlWZZlWZb1/DZMFWVlGCSKTrR7ddFheNKhE3kMEsWRdsgwVbuGKTcrrQ33XxizOsrYjAvOD1OMMXQij6VWQOg5SCGojCFTmkmmWB1lXBznuA6kquKxtZiG76A0ONfRG2++4aGNYZorEHCmrwk9F8cRtEOXxZbPcjukMgZVGlJVMkgUw0TRawZUut72ll4DgUBVmlGqONoJcaWgG+0eZHQjD1fWlWyrowxVaQywMcmZZCVlBUWlCVyHtCgZJAWbsUEgEAIiT9L0JaHvMt/waPiSC6Ocu5Zb3LHUYr6x9+tst2MHswo7IUCVhmsUgF2h0oYkr5hveriOoDnbOC2qS+c6m+e213tMG7MdmO72c3Rm+2mJFLcYU+QZeVV/eTbyJHFa1u0+BSw06+CwUBVxXlFWmlPrMVlRoY0hKzXGgKDi+OZnmHviAzijhw9+wYB2PNaOfxvnbv9+8ubOGe7jVHF+lDIXecw3PG5fPFy4e2BCgh9C0AavyTPWH9KyLMuyrGeNDdBuAq1GxH0vfwn3vfwlfM+3vpGf+JmfJ9mjouyjn/i7HQHaiWNHeOL0+V3Xv3wA8K7Lh3svb7cadDvta5y9ZVmWZVmWZVkvRJNMUem6qmdpj+qdw2oFLsM0RRvDJLMB2uXuvzDmwjDldD9hkCgWmj5HO+GuwWXDh17TR1Wa88OUL54Z1sFNURJ69T3V1zHcaTNWNDzJRW0oKo0UgpWOzzBVRJ4kcCWudHCpZ6K1Qpee1vSTujosUyVbyc+tvSYXRhlCCHpNn+PdaM+KQ8cRHO9GZKri4jjnwdUJAKqqmGQl07yi0pq81OSVmQU+dT4SuA6B6yClw1zo0m34FGXFyfmIFy019z3ubse+MMqYb/oIIfCkQ6pKWuHBH8304wIhoB269Jr+dgA2zUtCT+IIQTusg8S93mOOENvZz+U/R0dA6ElaIsNXmxR5SlJe2XUmcB1G2qCBXF1qu9hPFRfHGaX2iTxJoiqKskJUijsHn+Tlax+im1848HUClG6T1Vu+iwu3vQMVzO9YrirN+qRglBbMRR4rnZDFVsBy+wbOVxICnMuqzVz7mWJZlmVZNxMboN1kXnr37bznnd/Of/qNP9x1+YOPPbnj/158x6186jNf3HX9i+v9fY+33/K7br9l320ty7Isy7Isy3rhivNquzol9J5a9dmWyJcYU1dLxfn+7eZvJueGKaujjNP9hFGquG2hQXefqqktnnTotQIWWwEPrk5wBKjKkJeaotSHqvKZZIppXqLNrJ3fLOwZ5yVCgOuIXWeBScdhqRXQ8CTr0xymOQiB1jGjVHGy1yDwJCd7+8+8O9lrcKafYDCzSjpZt64Emr6kE0Z48wIHSJQmzhVxXpGokrzUtEMPVzoIDNIRnOw1D3TcrWOfHaasdCPO9BPaQT1nrRVIBomipzXSufZ7IM5LpnnJYsvHk5Kldh2K7VWJt9d77PIKuKKs23VGnqQpCvxyQJknxHuMY/Dcej/GQKENxhjOjzIuDFMypdmcFnRCj1vaivtGH+NFZz9EUOz/3OBqmd/jK0tv48GFbyFsdmiUktCpkEAFZEVFoiommUIIwdFOxHzDY7EVcNdy61q7PxjhgDerNvNbttrMsizLsm5SNkC7Cb307hftuWw0nu74v5fccdue6z926sy+x3rkib2Xv/gOG6BZlmVZlmVZ1s3q8jZy8gY9nN7ajzHXVyH1fKW1YZgqJlkd+myFVM1A4rsOD10YsxkXDJKDh2db0qKsZ1cFknw2ByxVmmleblc6XUtZafpxQVqUFJVhue0zykpcx6E/zZmLPIQQ+PsEcg1fMhe4nB9n9OOCvNTcsdSi0poj7QD/Gi1AQ0+CAF0ZirLi4jjjeDdipRvuCK86rqQzC6GqWQXcNCtZH2dcNIajnYiFps/dy+16v9cQepK7l9tUlWGaKc4MEgLXoR26DBNFP1HXrMKM85L1SU4zkLTDutpqq3pwr0q8vd5jkSfr+z0L0RZ8TVANKbOY5BpzzB0uvceMrsOzcaJYm+SkRcmJIOet8ce59dE/wy3ja96byxXtWzhz2/fx1dYbMNIjKA15UQdll7+dhQDfrQPETuThu5LbF5tPvfJMCHBkXW3mt8C7MZWxlmVZlmU9f9kA7SY0jZM9lzUaO3/hfM0r7yEMfLK82LHsKw8+Rl4UBP7uf4D9/Zfu3/NYb3ztqw9wtpZlWZZlWZZlvRBd3kauukFh19Z+hLi+GV3PN5mqONNPODdMKSuDNoZUVXULwtkcq9VRxto0YxjX1VqHCc+gbtOnKkPgStqB5PwwJ/QcNiY5R9ohcp/2hVvGWUlZGSazNoMN3ydRCa4jyEsoqjokuWV+54zsSmtGack0UxSVYZgUjNOShZbPJFMkRcWFYcb6JOd4N6rbJZZ6R5g4yRWjRJGpisB1WOmElNrQj+tWn3tdh3Qceg2ftCi5MMroRl7d0nHWmvGgjncjBnGBMYbT/YT1ac44LelEPoOkoOHJ7XlmV16/oR8XTPOSZiBZagX0Gj4Ls8BtmBT042LXSry93mPNwKUVSG7rSsppHzGtSEvFQd6FmkvvsbioUCjWpzl+fI53Vn/JKzc+hTS7z13fy/nwDr529B2Mj72BuUZAoDVJXpEU9ay1buTTDCSOUwd+oevgCIF0BMtzIcc64VObeSacOizbCs4OUA1oWZZlWdbNwQZoz2NnL6zRiEJ63bkDb2OM4UMf/eSey48s9nb8X7MR8aZvvI+PfOLTO5YlacbHPvlZvutbvmnHsifPrvLFrz2063GOLi1w3ytecuDztizLsizLsizrhaUZyFklDGRKc8hcZ1dpUW0HR83gKTxQfx44N0x5+OKEXFX0Z9Vl2Sw8u8SwOsopdUVRGToNj824YOEQs+E0l6qYFlsh/aQEDJmq2JzmHJnbv+rHzObRpWV9bq3ABQyRJylKTeQ5LLYCMHBmkNKYvS581yHO/3/27jzIsvSs7/z3fc9+97xZWZmV1VXdrVa3Wt2tXQiQwEILCKkRAgkJgxEwnmGA8IwjwGA7HBNhm5nwbNgeBxHDmMEx9uBBM8SYRYCEsCQEAxJYSNBSq1td6rW23Cpv3vVs7znvO3+cm7eyurKyMquylq5+P/90V+XNc89y7617zu88z1NU1WaqZJgVjNMCPQsKC9ZHGYutjKzQNAKHZzfGjLOSxVbIXM2bhYml1jy/GTNMCjbH1QyyRuAS59W+m2TFJc8rhUAbQ15oElUSZyVSwD3zNeJc4zgSM90H+6lA2/bwcnXuLoSgEXp8fXXIxjAjL0pO92KWWiGN0N31uY80fJqhR7fmc6JbBXf9OOd0L2au5u1aEbfbe8yVgkCU3BOM2Zj0eH48okydfc8LVMV07pmo5q7dFb/Ae1d+k9dkX0LuK4K76HTzDfxJ8318Sd1DpFzClRGLTYXrVMGf78jqeEiIVclSy2ehEUwrIj1aoXsdQbkAxwGvUc028w5xbpplWZZlWXeM2z5AG09iSq0JA/+KVU4vV3/1+FP897/0b3n3t7+Fd/+Nt/DNb3h4z33U6w/5F7/y63zxr69cFfatb3xk17//gUffuWuABvBL/8dv8MiD93HPXcdmfxcnKb/wL/93tN79C/QH3/cOxMvgjlDLsizLsizLsnbXDD2kEISewyhV+76Av5fxtMJJCrHv9oIvNVobnlgZsjpI2ZzknO8nGGNoRx4LjYDQkzhCUBrD5jhnY5Rxrp/hSsk4rSrWxpniZLeG4OrnZJKLVUwIWGj4nOsn1H2XrVhRD9xdK6e2pUqjTTW3KvQcHClQpUGVBseRHJ2GWYvtkCQvGKclkyxjkBSkqiQvShJVIoWgEbg0Q5es0NR8l1cs1JlvhvQnOU+tDik1BK7kuY0JvidZaPiAoDfJ6cc5W3FOtx7QDF0SpZFCcKIbMUqr543z/LJWgZ6UzNU9mqGL51wMp/JCc6YXc/9ic9/HTgjBI8fbzNV9Tq2NaEddHj834NxWwsY446m1EaHv0PAkGoEx4LuCwHNQpaHmVeuSl5q1YUZvkjNX8zjZrbHUDi+riNv5HsuKkppT4uUDyCdEJqcoS9qhx1asCL2Smn/1MDArNK6AV6hv8IHz/467kytfX9iNRvLs3Fv5T53387SpriHUZVXXNt/wmat7zDcCMqWZ5EU15ywXHG2GGFOFp8udaF+v3V0JCW5QhWZ+o2rZaFmWZVmWdQW3VYD251/+Kn/xV1/jrx8/xZmVNcbjasAvwI/+wKP8nR//8GW/UxQFw/HFloRRGBCFL58+1aoo+OQffZ5P/tHnCQOfB15xkgdecTcL8x0a9ajqNb814NSzp/nyV79Oll+5lYIjJe9719t2/dnrH36A93zHt+4aovW2Bvzo3/3HfPc7vpV7TizT2xrwB5/7Amsbuw8KPrG8yA9//3uubYMty7Isy7Isy7ojdCIP1xHM1TxWBymq1LOZTtdClZpBolhqh7iOoBPdmQHaEytDVvoJp3sxW7Fivu6ztGMe1k5jr2C+ETBKChxHcGGckaqC7ZTo7m79qs8XeHI2K0sVhnrgUvMcgmml08YoA7hiiJaXGqMNhTbU/GodJ5kiUQVHmwHLnZBXLbXQ2rA5zvCdkvODmEQVDOOCvCypBQ7NwKMeOMzVAyLPYZAoPCnojTNA0Ao9Tvdi1vKSuZrHchgR+Q53z9V4fGVIqqqZa8YYzvQSunWfyHMwWtCt+bSjqlouL/WsBWa13QJXVvPFFprVtYYnV4b0Jjmhl3DfQmM2c2y/jneqGWpnejGh6zBXH9Mb52yMcs71Y9bHOZEn8VyJLqrnD1yH1WHKC72YRJW0Qo8Hj7VYaoUstcNZddtOncgj9CR3t11GgwswNChdAuA5kqONAK0NaaHZmuSAv2eIpsuSe/uf59sGv8eSegEO0KmxlAHPHn0XX+68j9PlHHFeUg8cWqEHCFYHCarQxHnJsiuJPIdOzUOVARujnNVBUrV0nL52HzhAcAnbs83qVWjm77/1pmVZlmVZL2+3RYD2h3/85/zqx36HF86uAPDi9vd7FSqlWc73/+c/T5pVX9pf99AD/Mr/9I9u1Kre1tIs5ytPPs1Xnnz6mn7/oz/wPu67+64r/vxnfuKH+OJjT9DbGlz2syTN+K1Pfu6qz+E4Dv/wv/oxW01oWZZlWZZlWS9zcjpDKlUla8OMlUHKyR3zmw5qZZAiRBV0HO9EBw41XgrO9RNWBymnezGDRHHP/N4zzar5ZRohBUvtkKI0bIwzGGcgBI3g6u0cI99FCIHnSBJV0Io8Qt8lcCSeKzDA+iijkZe7zhJTpaaYdiaRAgaJohcrAs+hHfkcbYbM1302RhlKG873Y85uxQzSAlVqAldiNMR5idZmVmWWFZpzAkLPwQCTrGS5E+E7kl6ckxYlSa5ZH1fVdwbBciekWw/oTXIujPPZTLFW6NFt+CSqJFN6Njct8OS0HeilrQLbUVW1dbQZ0k+urXoy9BzuX2xy30KD157o8IVnLvCFZzdZaoX04oxRWjDJNY6AQVwAaTX/y3OYr3s0ApfNScarj7V45Hh71+eQWnF3GOMMNrgwHnA+d1nuXGxVOFf3SVQVGPaoZqmlqjouO/NYR+fc3/scD619nDm1dqDtVF6D1ZPfy9ePPsrpxKc3yUlU9VrZGdaFvkOca5qhIcnLWSDrOZLlTkgjcDg/SDhPVcnXrnksNq/SdlFIcP0qNAuattrMsizLsqwDu6UBWppm/LNf+rd86o+rqqbt4GxnYHa1WdKNeo33vfNt/IdPfBaAx544xfm1DZYXF27EKt+xvve7/gY/+dEP7vmY+bk2/+s/+/v89D/8H9gajA78HFIK/unf+wne8vqHr3U1LcuyLMuyLMu6g5zo1jjbT1juRJzpxbRCd89A6Er6cXXx/0S3RuA5nLiOIO52laqSU2sjNqfzzq4WngFoc3F+mRRiNhdufZQRegXn+wnN0MXfo/Kv4VdtFxuBw1asaIbVZYS5hoekai848tQVZ4llRUmsCiZ5gdYGKcGTgm7Dp1PzONLw+frqiN4k50xvwsogZZwVJKrElYJMaTKlkbKqxPIzhe9IisIwygoagUs79DjaDGahiyPFbBtHqSL0JKrUtMMARwoWmgE132FjlLFBNp1J5nL0aoHM9j4JXPpJgp7Od7ve9qPn+wmB6/DgUpOvr4xoap+FZkjoOpddH0mLklTpav5YN2JrkvP4uQEPL7cujkkoFSQDyEYc9XLOGc1CI2B1kNAIHFo7qjOPtauqOiFg4hb0E0WSJ4S+Q0skvH7waV67+UlqxeU30u4lCxc4f88HWTvxXjIRcPbChElWEOeXh2cAoSvpKzXbxhdXNG6v87l+Qs13ee7ChE7kEbgvDsVEFZwF29Vmd95ngWVZlmVZN88tC9CKsuRnf+F/4UtfeXLWHkGI6gvhbkHaXr7/vd/Bf/jEZ2eP/8yffpGPfuh9N2bF7zDduTY/+SPfzwff+459Pf6+u+/iX/+P/4hf+Je/yuNPPbPv51mY7/AP/s6P8fZveeO1rqplWZZlWZZlWXeY0HN4YLFJWRrGqeJ0r2rPf5AQrR/nnO7FzNU85us+Dyw2Cb07r9LkTC8mUyXn+1X7wf3sIykuzi/T0xPteuDSUCW9SUY9kFwYZSx3rtzSTgjBfN1HlSX9WLE5UbNlL7cjar7D+UEVzu02S2yYKCbT6rFaIDFG4AjJXZ2IZuhxbivh+V7M2jBlECvivKo8awYuzcBDSDFrrZgXmjTXJGjiTFFXLmnuMlfzZuHgi7cx8iVxVl1n8FxxyWOgChNHnuL8QNCKvH21EY18B2MgUSWTrLzq4/ey3ZLzhc0JK4OMuZrPyW5EWhhUWYIR+J6g7rmEvkPkuwSOYHWYsTrIyJTGGIMU8NBiHdIqOEMXAASuw71H6mhtiPOC84MEuBhICVFV5kWeZH2cEfkOjDd4zfrv84bhZwlMeqDtiRsnOfeKj3Dh2DswstrHvWFKUWr6SU4tcHZtE+m5EmNAaU2udr+TuhV5jLOS9VFKM3RYGaTcMz9tQyokOF5VaeY3wLktGi5ZlmVZlvUSd8u+UfziL/8af/nYk5cEZ+1mg/e962288ZFXcaTb5j/72f92XyHaA684ybGj86xubALwn/76iZdFgPaOt74J13X48y99la88+TRnV9b39Xu+5/HG1z7IO9/2Zt7z9m+hFu3vLrtt955c5t/88/+G3/2P/x+/86k/5vGnnp31IX+x40sLvOft38KPfvhR6jXbZ9yyLMuyLMuyrEsd71RVNMYYTvdint+M6aYFx64w12ubKjUrg5TeJGeu5nGyW2OpHXJ8jzDodqa1oZ8oRqlikpWzNoL1wKHuu5zZiulN99Ox9v7O4XbOL8sLPavW6dY8JlnBKC3wnJxj7fBi9dIujjQDNic53XrAmV6MnM4HCzzJfCOgFXlsjDJ8J6cdmUtmiTUCh2Gi2BACgURKuPdIndIYtIGn10dsTXIKrSmNJvQcAtehXfMuaZsYeg7aGFJVsjXJKTWM0gJXCsppa8qFxsX9sr2N46yk1AZXCJwXbWM9cGnkJb1J1c5x4yph4rbt5RhzMZi8Fuf6CWd6MY+d6XN+kDBfD9DGsDHOL5nDlikoywLXkYSuxHMkJ7s1WqHLyiBhaxTTZsJ6scrR2uXh1GIzZBArjDGcnz7vOCtZaPqz99hc3WehXOXoN/4fTmx8DscUB9qW4dzDnLv3I2wdfUsVZk0ZU72uJ1m1vHa4+2xCyY59ypX36ULTZ5jmDBLF+ijj5HwTGW5Xm119pp9lWZZlWdZB3JIA7RvPnea3/uBzs+AMqhaCf+8n/xZRGFzTMt/65tddbOP4tVNorZHy2gdQvxQ06jXe+4638t53vBWA0XjC82dXWFnbZGswJEkziqIkDH1qYUin3eTeE8ucOL6I61zfHZlSNvw1IAAAIABJREFUSj7wnrfzgfe8nY3NLZ58+nk2twb0ByPqtZD5uQ5333WMV95z5ZlqlmVZlmVZlmVZAA8vtwCmrfRyzvcT+nFOO6pmPUW+gyMEpanmI42zgkGiEEJwoltjvu6z1A5ny3kpSVXJmV7MuX5CURq0MSSqnAUokecwyUteuDBhkCqWmsG+qqSg+l0hBJ6UJKqkOQ0vHCmp+w7jrKQdGcZ5STO48uUB35EsdyJKbXAkjKet+KJppZ83/flSO2Qybb+4PUtsruaxOkzJC01eao61IxwpcJCc6ydsxaqaV2ckdd8jK0qkFJeEZ9ukEESew2BaWSeEwBjB2igFERG6xazF5PY2bowyXEeSa0NpzGUXQbp1fxYm+k7OUjvc9bl3KqcXMoTgqo+9klSVfOGZC3zt/JDVfkotcOjHio1xdskoCyHAk5JG6JCXJZuTnOV2yNFmyFLTZ06MWdtYZTOT6NijfaKzS1tDuH+xMV2eoOa7rI9ShmlOM/RYTp7m/nO/ycLGFxB7hFe72Tjyzay+8gcZze0+qiFWelr9pok857IZedu2QzMhLoZpu/EcyVwjROFCNM8wWKLTsG0aLcuyLMu6MW5JgPZvPvbxS9o0fvh73s3P/dSPXNcyX3Xfydn/Z3nO2ZV1Th5fuq5lvtQ0G3Ve8+Arec2Dr7ypz7swP8fC/NxNfU7LsizLsizLsu4cQggeOd5mru5zam1EO3LpTWd99ZPkskAh9ByW2iHduk8wbQP5Uqw8O9dPOLU2IlPlbHvTaXi2TYgqbEmmlVKCqsXlfOPqN5/WAxdXChqhw9ZEUdbNLMAIPYdJXlW0JXmxZ4AGMF/36ccZgSvxHJ8L44zeJCf0nFmgJ4WgGXqzoA4gK0rO9VO2Gx22QpdxXuIIwdowJXAlWaGJPEleaOLc7BoAbVPTkNGVAhBEnmSQFNT9Aikg8iXu9Gba0HMwgCsgKUtUYXjxZjpSUPOdWWvKb6yNCH1nOt9NEvkuDd+5pEIvyctZuLmzdeR+aW34o6+v8+zGmNO9GFXoaj0Ch5bnz+bHaWPIC02iSrYmin6sWGqFDOKMWjFkKcxxS4UvNKuDjLovL21ruINA8MBik3bN47kLE5qBJDj/F9zz9P/L4uhrB1p/Ixwe917H48c/QvvkI3Rqu1eVAaSqQBtDoTXN4MptR1WhZ2Gh710eoAkhqhuBvYiaG/D8CNqiwSA3dA609pZlWZZlWft30wO0oij4wpe+Oqs+W15c4Gd+4oeve7n333vikj+/cHb1ZRegWZZlWZZlWdattlcbumbo0Ym8qtrEsnZxvBMxX/c504sJvYSjzXDXiiwpBK4jON6JONGtveRmnmlteGJlyOogZXNSVdwZY2hHHguNgNCTs4q7VGmeXh+xMQ2s2pHHma2ESVZyohvt2XpRCkG37pNP55f1JjkLzSp486czp/JSkym9r/V2HUkz9Jire4SeyzAtGKwMr1opKAWcmKvRj6uQcKEV8OT5IYEjyEpN6DsIIMmr9dj+jDDGUGoodFXNZqjaNiptkFIQupLCGBxHsjmd6TZMCrp1f7aNrpQUpgqQElXQCC9eBim0ZpgUbE6qloBGV3PWmqE3a58ohMCR1Ry4I80A35GMs4Jw+jpsXqEl4V6+dn7Ak6tDnr8QM0wU98zXONIId63OCtzqs1O2IMsVjhpSbE24IA1Z6LLcCS9pa7g2TDnZrV2xMm6x7tI9++eYL/2f+P2nD7bibggPf5Bzdz3KJ75wlm7jBG5e7Bmg5cpQaIMx4LpXfq2mhcaVVbvRcEeAKqXEcT3wGyi3jsIl14pRNmacF9c9g86yLMuyLGsvNz1A++rXnyFJs9nssw+//904+2w/sZf5ueqeo+3viBu9retepmVZlmVZlmVZ+7OfNnQv9dDDujlCz+H+xSb3LTTu2DD2iZUhK/2E072YrVjNWlDu1pqx5sNiO0SVhklWshXnlMbM5lCfnN+7fd3CbH6Zz4VxTs13qAfupXO89tG2rx/nbE0Urz85hyMFrdBFG7OvSsH7Fxs8e2HCcifkifND1gcZcV4SehJKQ9N3GGUXZ26ZaQC3PUetWkcoS02cF0hAaUPNd8iUpu4I8sIwyQscKenWPJjOPPOcKtCL/KoVZldrHCkZpQW9SUapNVlRMEoVpTGMs5JWVM62wXMkjcBBTdsnHm0GDBLFUjvEdQSd6GAB2rl+wtMbE1YHKVux4lgrZLF15epJzxGErqBuYhwzpJ/FbAxTQt9BG5/Ik8zVfZqhxyApmK8bhmlx+XqpBJ78OPzVv8cbnT/QOhO24bV/E17zEYg6RP0BUpylFbiMUoUqr9xWVGNmr4srtWYsNaR5SStycaQg8h1c10V4AdprksqIwlSz7sDMwsHrnUFnWZZlWZZ1NTc9QFtZuwAwO5H+pte9+lCW26hf+oUzTtJDWa5lWZZlWZZlWXvbbxu60HOYq3mkquRsP3nJtt2zbg4pq+qp7WqiO8W5fsLqIOV0L2YwrT7q1PbeRkkVPrcjj07NZRAXbJAhpoHiXu0cPUey3A4pdRVqb4wyAFynCiGuNnMKqvDsdC9mruYxX/d59XLrwJWCDy+3eexMn+cvTHhmY4wQgrw0BK5ESjmrpFOlYZRWYVqhNaU2aG0otUGVGk0VpkEVvGhjGCYFNa+a6dYIICmqeVulMQghaPrVuiTTzygEjNOqLeYoU5TTiraG73Kk6bPYDCmNQRWGRBVVQBgruvWA1UGKFPDQcovjnehAIW6qSk6tjVjpJ4xTRT1w6NZ3P3auFETeNDjLhmR5RlZqfEcwV/fpTXImbsH6OKMRutQ8h1Gq0MYwydTFAC0dwFd/Ax77vyHt73tdAWgegzd8FF79veBd/KwWQtBwDa3IJZ5oNkY5y51w10VIxOxG5yqovXx/DZLqmLRqPoudBkGjS+HWUSJAaY0pgR0h72HMoLMsy7Isy9qPmx6gbQ1Gl/x58cj8oSz3xW0rlCqu8EjLsizLsizLsg7DQdvQjVLF6iBlbZix3IkoS8PWJOfh5daebegs606xHaBsToPm/YRnAIEnp+0EwZMOC02H9VHGyFOcHwhakXfFCiCA+UbAJCsxxrBBxvooQ4oqfPIdSeDt/ruq1KwMUnqTnLmax8lujaV2OAu+D1op+MzGmPm6zzPr1b4ojeFoswpeHFHNS8uLEikl2mgwAimBaQebWuCCqYK1QkNelFWsYiCXgkGsWGwE5EVJ5Dnk07laRxoBiSqJfJdnLowIpCQrNanSRL5D4Aj6iSDyHALXwXUkLhC40AhdulrTixVnt2KyouQVCw1WBynf8aqjBzn8nOnFZKrk7FZC6DkIYfBe1NbwYnCWIPMhKsvIykvbFNZ8h1Q59BNF5Dv0JjmtyMOYqhVikmsYrcJf/zo88ZtV9dlBzL8S3vhj8MrvBGf3CruWB57jcLTpszpIaAQOrV2q8XxP4E1bMxaFwX9R4XGcl2gkdx1pEjbnqB05wkS6FNpwMSq91PXOoLMsy7Isy9qvmx6gaX3pFyB5CO0bAUbj+JI/txqXD821LMuyLMuyLOvwHLQNXbfuzy7In+nFjFM1a0P3yPH2zV59y7rptgOU8/2Ebt3fV3gGEPkuQgg8R5KogoVmSCOvqqnqgcPGqAql93KiW/1cCMHIUzx3YYIqDRvjjPlGQJwXu84vE0Jwolubvb8fXm5dstyDVAoudyJOrY2JAhfP1VwYZwxSRaE146wgVSWqNOiymFamVUE907DEdeQ0MHOI8wLPlRTakGQFshCU2tBLFK3pfk1ViedIXEdydyvghc0EDKwMUzxHcqQREHoOSV4FVK4jdv38cqSk5lVz2gSQqSqg25zk+66i1dpwrp/Qm+Roo2lHPuujbNZK05VVq8YGCU4+Is/Sy4KzndqRT5InTLICz5G0p+FVbXSahW/8Fpz5NOgDzgdbfiO86cfh5Fsvzse4AlfCybmQCynEecH5QRXSvThECz0XITJcKUmLkto08BJCUCJRTohfb5LVmrRqAQoH9N5tGa93Bp1lWZZlWdZ+3fQArdNuXvLn/mBEo3b9bVvOrqwDF1tDtluN616mZVmWZVmWZVm7u5Y2dFC1kzvZrdEKXU73Yk73YoSoWpLZdo7WnWxngGKM4Vh795Z3u2n4Do4UNAKHrVjR1Zpu3WeSFYzSAt/JWWqHe7azE0Jwcr5GPXA43TM0AhffnYZOk6xqbTh77MX5Zd26T+A5h9Jy1Rg43oloRx6JKmkWmkbgMkoLxmm1LXmpEYBxAAGeK/FkFaZVbSEl40whpUBrCF1JUciq1aOBNK/CuLmaxyQvmat5OFKw2Ar5xvoYbxrCGQNZofEdSV5qXCkQQuC/KECr9k/OOCvoNnxqnkOiNAjBqbUR83V/X/Mc+4miKA1bsaIVehcbEorq+NZFjLuP4GybIyH0HeJc0wwN/sZXefdzv8Hdwy8d9LDAK74D3vjjsPSaA/3akYYPrsAYw3mqfxfGWclC058FkTVPIqWg5kuGaQEIgsBnUAZsqgDteTRcl8B16OwjhFWlvq4ZdJZlWZZlWQdx0wO0uRcFaKeePc1dxw7W9mA3f/W1py7587Gjh9Ma0rJuZ1qbO3awumVZlmVZt69rbUO30/bjn9+MaYT5gS5EW9ZL0c4ApX2VlosvJoRgvu6jypJ+rOjFioVGQC1wGKcl7cgwyYp9VePMNwIGiaJb95mreyw0Qpba4Z7zy050a4fy3pSimofVCFzakYcqNIEnSZQg8iWJklXrxVLjSknoVa3/qjaT1ToZYxACHClQhUFrgSMFUgoyVaLKkmGiuOBWk92aoct83WdznNOJPM5tJcw3AnwpGGUFSV6Q5CU1v5ohFrqC3gQKbao5aKUmcB2ONHyaoUe35mMwnO8ntCOXM72Y+xebV932UaootSZVJZ2aR6o0nchlTqa01BZ5ltBLFarUFFqjDUgBrpR4jiRwBJk2qKKk0AYDpLni5OjLfNfqp1iOn7rqOlx6MFx41aPwxo/C3L3XdDwB7l+sbl4WQlDzXdZHKcM0pxl61DyH0Heo+y5KQ2o81so6eVonLgyR79IMqn26XSF5NSuDFCGqqseDzqCzLMuyLMs6qJseoD30wCsu6QTw+S8+xjvf9ubrWqYxhj/47OcRorqLLAoCHnzltX8BtKzbXapKzvRizvUTitJcdWD3YZ3wWpZlWZZlwbW3oXuxTs2nmxYHvhBtWS9FOwOUhUZw4N8/0gzYnOR06wEXxhk1zyHyHOK8qmhLVLmvAK0f5wzTgtfc1eFI0+ehpRZ5qW/KDXn1oFpn3xVgqtltUoAOq7aIC3UfpQ15qckKTeDK6aywi+uwXSVWalCimFVruVKgHUleaPJSszbKuPdIA8+pwq+n1saMs4JWVG3XIFF4ruRsL2aYKtJCE6uyqpIygIDAldMZaVUl2rF2yGIrrKqgVob0Jjmhl3DfQuOq+2mSlaSFRiI41ooYj7bw2GTSSxhTBaDGVNc3ih0tDIWATGnyssR3HAJXIkzBa+O/4NtGn2CpOHewg+DV4OEPwut/GBqLB/vdXQgEDyw2adc8nrswoRk6DBLFICkYpwrP9cAL2cJlQ7ps9HMWmobFVoDnOCy3Q+b3+X7oxzm9Sc6Jbo3AczjRrV33+luWZVmWZe3lpgdo3U6L++89yTeeO40x8Kk//nN+6kc/xJFu55qX+fuf+TPOrKwjpoOFX/fwAziHNFvNsm435/oJp9ZGZKqaebAVK9JpeLZtu+XKXM0jVSVn+8mhtFyxLMuyLMu6njZ0uznWDmcXRfd7IdqyXoq2AxRjIPQOfr7qO5LlTkSpDakq2BhntEMPY6gCJ6Wvuox+nHO6FzNX85iv+zy41OLYTTxHaIYeUghaocf6KMOTgs1JjpRMq7wCsqIKsSZ5QV5oHCmrwG2HYFqlFjgO40zhSElpIAoclDYMkqpCrxE4LHcistJQasM4K6n7ziz0f2ZjTF5o6oEDRuC5chaeOQK0MeRKIwKo+ZL1UYYrBfONgHbksRUrjjZD+tOKvr0YYwgcwbyfs2gmTOItxuMxq8OUVuiRa0OuykvCM1VWx3o7P/TMmLerz/Pd6jPMm97Bdn7Uhdf9EDzyAxC2rv74A1pshnQij5VByvooY6ntYPwaE2qk+OhxihxkuI4kUSU13+W+hca+KzFf/Np9YLFpbxK1LMuyLOuGu+kBGsB3/o1v5tSzpxECcqX4J//8V/hXv/Bz1xR6PfPCWX7xl39tVn0mBHzfd7/9Bqy1Zd1aWhueWBmyOkjZnOSc7ycYY2hHHguNgNCTs6HfqdKMUsXqIGVtWA0UL0vD1iTn4eXWJXdwWpZlWZZlHcT1tKHbjefIA1+ItqyXIm3M7KY35xq/j8/XfcaZqk5+xxkXJhmTvORoGaB33lH3IqrUrAxSepOcuZrHyW6NpXZ402+w60QeriM41g453UtwJSSqRADBdFZW5LvkpcEYQwzEeYHSctZlA6pWkJHnorXCTM+BtCoJHJdSGxwBzcAl9Bzm6z7roxRtNKrUNEOfjVHGhXHGJCtwXUngVDcfNkIX1xE4omoLCdVxS3LNyiCjW6+CuMk0iOsnCm0Mo/Tqn1uhSaln6zDeZOIExKkiK0qywrA6TAk9h8B1qvM6CZO8mG6LxM37fGfxOd6j/4Qm8cF2eus4vOGj8Or3g3t9NzxcTeC63HO0zcnjTYYmZKRglFaVjXfP1znXjxklBb1JRj8pWBmkHGuHe/47cru8di3LsizLenm6JQHaD77/3Xzstz/F1mCIMfDFx57g5/+7f8U/+dn/klazvu/l/NkXH+Mf/+K/Jk6zWfXZPSeWecdbr68lpGXdjp5YGbLSTzjdi9mKFfN1n6UrnGzUfOjW/dnJxplezDhVmOlJ9SPH2zd79S3LsizLukNcbxu63TQCl36S7PtCtGW9FG3P/wIo9wi7rubkdts6IZBC0puMON9PcB1BI3CJfGd2Y12Sl4yzgkGiEEJwolubnUc8vHz4VUhXI2XVYj5VJa3QZXOSg4FxXrAUXAx32qE73URBLksSVTIqNK4r8aRASonjCAptcAClNaU2qFIyV/cJXIda4DLfqFpaZkqjyirA7Mc5vXHOZpwDVSi51IpY2qOattSG3iTnwjifts43JIWDMVUAOMnKK290Noa0T5T3EUVCUZac3UowBib5xarBul8dO4BRpigKTUNt8H3pf+TtxZ8RoA60r8et+xg+9LdYfuOj1byzG0lIcLyqss1vIqWkA7y4z9CrjzX52vkhqwNvdlNoP85pR95t/9q1LMuyLOvl6ZYEaGEY8F//7Y/wT//Fr84qx/7si4/xoZ/4B3zk/e/iXd/+Fu6569iuvzuOEz7/xa/wO5/6Y/7yK0/Mqs6MAceR/P2f/uhN3hrLuvHO9RNWBymnezGDRHHPfG1fs0Y8R3KyW6MVupzuxZzuxQghmJsOXLYsy7Isyzqo621Dt5vI3+eFaOtlT2tDP1GMUnVTZnYdpu35X0JAqjTXODoQgeDubp1GkDPJCxYaAd26jwHO9pNdW7svtUO6dZ/Ac25Ia/eDHJcT3Rpn+wkPHmvyh0+sIaUgL6oAbOeKtyMP3xGMsuq8JitLVGFISo0xJcWOtpVSCNr1qiJWIsBUM9EGcUE7LIlVwSgpWB8mlKaaKe1JyUIz4Egj4Ehj74PhSMFCM6DmO2yMMjbI6Gp/Nod61+q/fAzJAIoMjKY2raBThWGY5hiq7erWffKiWkcpBcbAfHKad8Sf5JvUX+Jw9dacO13ovI6/nH8/o4U3cXyuhjMpWGwe/qUfKSXCcSGoQ9AErw5XqawUQvDI8TZzdZ9TayPakTsbS9BPbs1r17Isy7Isay+3JEADePRd38bTz5/l//rNP5gFYIPRmF/92O/wqx/7HTy3WrXtgOz3P/OnfOKzn2ez18dgLvkZVP/9qY9+iDe99tW3apMs64ZIVcmptRGb0xOL/YZnO20//vnNmEaYc2ptxHzdtz3jLcuyLMs6sMNoQ/di28u54oVo62UvVSVnejHn+glFaaq2etPwQghm7f1cp6pwOtGt7fu77s0K5bbnf4WecyiVlvN1n8VWVTXVCj3uma9RD9xD2y/7ca3H5YHFJmVpONaOeGplBAJGWYHryEvWL/JdAlcyyUscJdBuNUssLTSlhlogkaIK4Wuew9FWSOhLzmwmbE5yNIZJXnJh2u5ymBa0Qm/W2nG5E9EMvX1vbz2orlOsjzIcoRhnBYXWs9aSQBWcpUNQKZiL4VcrdNHGkBUlW3GOJ6tWlmlREqeCUapYGD7Ou5NP8priawc6DhrBue63svWqv8m48ypIFMN+Qi1WPHdhQifyCNzDOu4C4fp4rQVMcxmaRw68hOOdiPm6z5leTOglHG2Gh/qetizLsizLOiy3LEAD+Lt/+wfR2vCx3/7ULAjbPl/OVTF7nDFwoTe47Pd3zj37L37oA/zYhx+9GattWTfVmV5MpkrO9xO6df/A4dm2Ts2nmxac7ye0I5czvZj7F5uHvLaWZVmWZd3pDqsN3U7byxGCSy9EWxZVN4ZTayMyVc6qVdLphfZt29UqczWPVJWc7SdXrVa5kaHcbrbnf83VPFYHKarU1zVDUJWaOCu4/2iDY+2I19zVZpIVN60y73qPy9Yk54HFBmvDlHGqUIVmK86pBS5N30HKat9IKWmGkkbgkqmSfqrQWuO7AikF3ZrPg0vNaYWYy/lBQpxpltoB8/WA5U7EXN3DUM2EVlqz1Iq4Z76Gew37vx64NPKS9VFWhXtpQTN0IJ9AOrgsONsmhUAKCFyHOCtpRC4136HmCV45/kve3P84J/JnDrQuCoe/8N/K15c+wKsfemQ267oVeYyzkvVRSjN0WBmk3DO//3EZuxISXB+CJkZqttRzaHHtl5RCz+H+xSb3LTReslWllmVZlmXd+W5pgCaE4Gd+4od43UP38z//8q+xuTW4WsX/JYyBbqfFz//0R3nXt33TjVtRy7pFtDac6yf0JjnGGI7t0Zd/P461w6rn/yQn9BLuW2jYkxHLsizLsg7ksNrQ7ZTk5SywqAe2wsCqaG14YmXI6iCdzUsyxtCOPBYaAaEnZ/OSUqUZpYrVQcraMGO5E1GWVWDy8HJrFixsu1Gh3F52zv9aG2asDNKL88yuwcogRQhBt+5z11w0bUV4OHMJ93JYx+WhY01WBgkPHWsyyQoypSlKQ2+cMXQkNU8SuA5SCrQ2ZIUmzgtKbfAch8CTLLZC7u7W6DZ8TnZrCASeIyhKwz1H6hxrhyy2Qo6mAWc2YxqhR1mW3HukjnMd50Hdus/qIKZd85BlSjPfgJHeNTib7TdT9dLJipJa4OKZkrvXPs2be79HJzt3oOePCfms++38gfsOvNZRHum2McDOLVpo+gzTnEGiWBtWr7VrukFBOOBHVZtGvwrhdNxH7bjp+XpIWb2G7exLy7Isy7JuR7c0QNv2zre9mW9/y+v5+B/+Cb/5yT/i6efPcLWbWU8sL/J93/12Pvw97yYM7Bct687UTxRFadiKFe3Iu647VKHqsd+OPLZixdFmSD+5/tYxlmVZlmW9vBx2GzqAcVYQTqt9DtJOzbqzPbEyZKWfcLoXsxUr5us+S+1w1+/ENb8KNVSpWRmknOnFjFOFmZ5YPnK8DdzYUG4/tud/LXcizvRiWqF7TR0mtm+KO9GtEXgOJ64jiDuowzwub7q7S2+cszbMSPKSVJVM8oI4L9mKFdrkF1vGSoHvShqhR913OD4X0Z1WmM3v+ByK85K5us9SK+QNJ+fo1n0ujDL+otbDH6Sk2sBlcdP+CQGRLzleF7TFFnICOlusqrP2MEwLBIKGyPnO7A95c/+TNIutAz33QLT4TPBuPi3fhgibBK6k7leXdZK8nLWYhOrcrxl6DJKC+bphmBZ0ov1+vgpwHPBbEDSuum2WZVmWZVl3qtsiQAPwPJcPPfpOPvToOxmMxvz146c4u7LOcDRmOI4JQ59Oq8nCfIc3PvIgS0fnb/UqW9YNN0oVpdakqmThkO4mbQQu/SRBG3NoF70sy7Isy3r5uBFt6AaJYqkd4jriABd4rTvZuX7C6iDldC9mkOx/DrDnSE52a7RCl9O9mNO9GCEEc3Wf453ohoRyB7Fz/tc4VZzuxQAHCtH6cc7pXsxczWO+7vPAYvOmzYY67OPSjjwW2yGvvavNqbUxzdBlmBQMU0WuNAZDoTWOlEgh8B1JK/KYq3kstkKONAP8HcfuSp8nk7xgrubhSYFxJb1YHfj8SlAdv4bMSUY9onxAWiiidodEFcDe+yHpr3HXU7/Om174PYJycqDn3nAW+aPae/iC981kxiPy5OxmBqajLdLi0gANoDa90UEbwyRTV/983dGmEb8J8vpu4LQsy7Isy3qpu20CtJ3azQZv/9Y33urVsKxbbpKVpIXGGAi9wzl5iXwHYyBRJZOsPJRlWpZlWZb18nEj29Ad70S2vbRFqkpOrY3YnLZW3G9Is9P245/fjGmE+axd440I5Q5qe/6XMYbTvZjnN2O6acGxKwR527aDvN4kZ67mcbJbY6kdXnNLyYO6Ecfl6Y0xRxsBqSrpTRSt0OVVi81ZBVqiCorS4DqCmufQrnnUA4+G7+xaAXilz5NJVtIMXRwpWGiGDFNFzXMuC5x2sx2c1aUiKAeM+0PWtiY0ApeJrmZ1JfmVWzcyOAt/9WssPvlxZJkfaH+d9e7lc4338Zj3erKyqn5r+y6h51DzHRqBw/qomuuWq8vb+ITTc7+00JesozZVRdokUyTKIIREhnWCeofIa9D27dwxy7Isy7IsuE0DNMuyKtqYiy1LrqVf/S62l2NMtXzLsizLsqyDuhPa0Fm3rzO9mEyVnO8ndOv+Nb22oAprumnB+X5CzZd84ZlNXEceaig3X/evqfrr4eUWUM0Fb4RVK8l+nNOOPBqBS+Q7s1aSSV6NwCLsAAAgAElEQVQyzgoGiUIIwYlubVY5t72cm+FGHJd25GKAwHNmnyftqKouW2yFGGMY5yVJXs1IywqNKnKSXBL57iVB2l6fJ9oYHCnp1qs2ndpoNsYZwBVDtO3grCYVYTmgjCdsTlJ64xzHEVQTzWB9mOE6ksiX1AOPVuhWlWEbX4cv/zt4+tNgNAe5HfIJ9yE+U/tuTrkPIqTAMYIokESuREpJJ/KoBy5FWa2DMaC5/Nxu+5VpDBRGsz5Kef7ChHODBJC4nofxGpigiZN7+JMcKbZwnepGiRPd2k2rbrQsy7Isy7od2QDNsm5jUgi2c7PykMKu7eUIwbUNkbYsy7Is62Xvpd6Gzrp9aW0410/oTSu0jrXD61resXZIP855en1MaQwScajhz5lezP2LzQMvRwjBI8fbzNV9Tq2NaEcuvWllVz9JLpkJLkT1nltqh3TrPsH0/XezKs/gxh2X3iQn9BxeebRxyeeJ0gZVaDYnOaU2GGPIy6ozhxDgOxIhBI4UzNd9PFey0k+u+HmyfV7VDF0iX+JJAeOM9VFGQ5V0ax7OtF3hzuAsKAfoeMI4zdmcVOsLUPMdMiAvNOcHCeO8qH5mDEvjx3nt6m/TvvClg+1jBI9H38QnvO+i33gFrpS0AVcKhBBIAbXApRlUlXTV7+w4t9tlplsJFKVhc5yx0k+mN1A6JMZhoCMGhUdaFuRlDymgFXkcbQYsNKuqwLP95Ka/1izLsizLsm4nNkCzrNtYPXCIPAchIFWaazzPv0SSl9Xga8+hHtiLVJZlWZZlXZuXahs66/bWTxRFadiKFe3Iu675elC1X2yFLl9fHRP5ksBzePWhhj8J9y00rrnd3fFOxHzd50wvJvQSjjZDtDEkqpyFRZHnIIW4pVVBN+K4tCOPrVhxtBlS912W2lXF2VfOD/j80xeIPInrSBKlUdPwbJsQ1TIiT7LSj0mU5p6F+hU/T3aeVx1pBIy9AoQg9Ap6k4xJVtDwHTo1n7lAUy8HqMmIzSQjVZqtWBHnBcG0rX6cl+RxTj8paAQOdV8yd+5P+PbxJzieP3egfVFKn427vovHF7+Hr8cd+lsJdd8hnK6vKwWeKwkchxff/6gKXe0LKfG9y1+D68OUtVHCIC3wPYfciVhLfQaFS1FqHKFwHUHgylnV4+ogpR/ntCKf5U5EWRq2JjkPL7d2bZtpWZZlWZZ1J7MBmmXdxrYHQ4fT4c/d+vUnaOOsIJyehDfDqwyRtizLsizL2sOL29Cd24o5P0gIXIknJZ4rcEX1XxBobRimt7YNnXV7G6WKUmtSVbLQCA5lmVII0qKk0JrWDQh/+sn1fU8PPYf7F5vct9CgnyhGqWKSlWhjkKKasdUMPTrRjZ1LpbW54vP34xxVlod6XBqBSz+pqqJGqeLVS02e2RhjNPiu5IXNBI2hE3m0I5964OBKQaENk6xkkOSc3VJIIbhrLsJoiFXJQ8curwjceV41Tgvunq/TCKrWmY1AUmiDLHP89ALD/pi1PJ8GdoZEaQyGwHPI8hJHgiMFpTbU3ZJvyz/PuwZ/yEK5dqDtL9wGq3d/Dyt3fx8qmMPkJZGa0Ao9PEfs6zWVFhpXyqpK0b0YqmpjWB1krI1ytPTpmzqxikgySeBKTnYDPEeijSEv9Gw+dpyXdKdtSeO84PTmhHGqMNP08pHj7QNto2VZlmVZ1kudDdAs6zbWiTxcRzBX81gdpKhSX9cJvyo1g0Sx1A5xHUEnsgGaZVmWZVnXbrsNXc13WBumaAyZKrkwyojzixU0rhRIWVU5nJircd/ROo3Qs63BrMtMspK0qKqNQu/6gq5tBtClIS40njycZb44/DmMG92krEKTw1jWQaSq5Ewv5lw/oSjNrhVw57YS1kYpw6TgnvnDmVUY+Q7GMAtvnlwdUfMcpKhaI949X6sq0PKStChJVDn7XSGgEXgsNENUWQWuUkDNc3hiZXRZ0LPbedV83adb94gnE9JxjyIZkxaKPBDU/QAhYJgUYAomeYkxehbikY958+jTvKf4LG0zPNB2J/48Xz3yKPmDH0AGjdnf1zyJlIKaLxmmBaU2s1aNuyk1pHlJK6paOkb+xQBtMy5J8ThfuKwXDnkB7Uiy3I4um/kWuFVAW9YNvUnOhXFOPXBYaAT4jmSQVG01hRDM1X37mW1ZlmVZ1svKLQnQfvF/+/c3/Dl+7qd+5IY/h2XdaFJWbVpSVbI2zFgZpJzsXvsJ68ogRYjqxPx4J7qhd7BalmVZlvXycK6f8EIvphW5rI8ESa4ptKkqRUqDMVBqg+9Kar5DaTSDtODh4217Ida6jDZm1qrPOaR2cUVZvSYNTKshr9+Lw5+XqnP9hFNrIzJVzmawpdPwbJsQMEiqvx8lBc+sj7l7vs78dVaibR9fY2B1mKK1mc1TfOt986iyCnSKPWagudPQ0XMEK4P0ikHPzvOq9WHG1iTn7rakjLfQ6QiV52RliZAQTKtmVWkIXEGhBQ3hIIQgUlu8afOTfHP8OWqkB9refnCcZ+76IM/OfzvjQtJMXJZ37EIhqhsci1IzTAsGqaK7Rw//QZKDgHrg0o6qGW6u6zIsPLakx2NbKac2R7QiB8+RLO0Snl1yPKRgoRlQ8x02RhkbZBxthrQjl61Y0QhzTq2NmL/JAa9lWZZlWdatdEsCtN/43U9f1rv7sGx/obYBmnWnONGtcbafsNyJONOLaYXuNQ09357TcKJbI/AcTlxHEGdZlmVZlqW14YmVIauDlM1J1QrNGHhwqYEjq9Zg28GFKg2q1OSFRiDwpOTZ9QlxVtq5OtYlpBCzc8VyZ4pzHbbDMyHAFYdTgbYz/NGHtJ430+7vX0M78lhoBISexBGC0hhSpcnUiLVhNbuwU/OQMmGSlZzoRtf8/t0+vqXWnNmKCV2HrVhxz3xtdr6z1A6ZZAWJKsmUnrWVDDw5nensIqfP7zmS5zfjS4KenbPiTnRrrI1S7us6nF85y1PrKegSbUDpi+GcJyVxrtkYZ2AgLwx3iQu8afN3ed34T3EpDrSdZ/z7+GL3e/la+Hru7dRRRdW2c5DkNAKH1o6uIN26Tz9RdCKfrTgndEtq/uXz7uK8arc4V/MIfY9j3RYybBPLkKdWE56/MObU2ohWzUOXsNgO9gzPdtp+3PooY+QpHClohS7n+wntyOVML2bONjKxLMuyLOtl4pa2cDzs8wx73m3diULP4YHFJmVpGKdqdlfmQUK0fpxzuhczV/OYr/s8sNi86YPHLcuyLMu6szyxMmSln3C6F7MVq9k8s73aTatSszJIOdOL7Vwda1f1wCHyHISAVGmu4b6xy+SFRoqqwuawKtC2wx8hmAU4LyUHef/WfLjnSB0pBHFeVXCVxszevyevsaVjkpcIAaO0wJGC8/2Ebt2/5Dxne27zfmY3d2o+3bS4JOi5f/HiPLTQZBwxW5xeP8+gP6IXKwJH4Djysoq7VGkKrVmIn+b96ad4TfZlJAe7gHGm9Qa+cvT7eELcR6I0nchlbZyzPK2Eq/kO5wcJwCxE8xzJ0WaI1glZ4bAV54B/SYgW5yX9WDHXCFnotJjvzqMabQotOLMVszZMeW4zJvAcAlfieIIjzYNVC9YDl0ZeVSXWAwfXcTGmqggMvYT2EZugWZb1/7N3bzGWZfd9379rrX09lzpVp7r6yp4rORxqKJqMZMS2aMe62JYsyhIlmUaMQIDzlARO8hIkDw4CBHAcBH5JHDh5yhVJYMmSIFGWackSzciJFEqMHFHkcDgi59I93VXdVXXqXPdt3fKwT53u6nt1V09P96wPMJjp6epTu/bZp9C1f+f/+wdBEHw4PJU70O7084n3Jx/IBcEHxYX1nINFg/dtrck7+wXDynDuAW9SjRYNG52Y54Ydzg6yUJcUBEEQBMEjuTIu2VnWpU3KoxMj9xIryXPDDmtZxKVREfbqBLfpZzFSCLJYndhuMeM8eaIwzp/Yuy4Pw592CurpemPaw7x+8yQiUpJTvRRrHUVt2aVGCEE3VQ9V5zivDamSbT1gqvDec26QPeyXBcC5QbZq3sjjkpe3ekhT4soxb23vMZoUVLqhMg5rHQsrWMslm72EWEocHt1Y8vHX+PPzX+dV8+1jfX6H5K2NH+Drp3+Sg/x5AAbOU+oKt7xfUTaGbhqRKEmkJFfGJfPastVPiJVkoxNTNAY8jJZfS2UU/TSiaBxOSIabp+j01vF5F9XJqC3UxvDGzoyrkxIpBMNeQmMdp3op6iF2/w27CYvaMKsMiVKsZW2V4+l+1u6GC4IgCIIg+BB4IgHaD/6573uomodGaybTOW9dusqiaN+pdfgwn37tFYbrayd5mEHwgfLa+fb6FkLQy9qalXHRMMhjemlEnqhVzUrZWOa1YVJqhBBcHHZW7yo9fJwgCIIgCIKHUWnLm9dm7C/3JT1oeHazw4+/V91a8OG0nsdESrDRidmZVGjr7vmGsfs5rA7tZxFFY3H2ZN51Oa8NWaxWE1JPi4d9/fYShZKCXqo4KBzDbsz+QjOLNVcngrU8PtbzpK1jUmr6WYypDbVxDI75GHcSK8l6HlNpR+oq5nuXWVOG7+xM2J1VXJ1UeAdb/ZSza+0k2LhsQ6pOBK8Vf8D37f8ap+t3jvV5jUj49uYP842tzzFPTx/5PSUFeawomjbMqozjVE9iHZwfZHSSiOuzimnV0M9iOrFio5ugraPnIoyDSWGZNoIoXyPuDhBxQkTEMFXszWrmtWFnUjGrNOly32Q3URSNJY8f7raPkoJOqphXlkHeVmdW2uC8Z16HAC0IgiAIgg+HJxKg/Vd/599/pD/vveePXv8T/rdf+hK/89V/hRBw+eo1/oN/+2/wyVdfPqGjDIIPFiEEn7wwYKOb8Oa1GYM8Wi36HpflbbUjWaw4O8gYdhPSZQ1keGd3EARBEASP6vKooNb2jnVrx3G/urXgw0lKwYVlxd21ac32pOK5R9jduz2pyBNFlkg2uynTSp9IKDcpNWcHGZESrOdPT4D2sK9fIQSb3QRt2/rA2np6abSq+Nud1Zw/xs8a25MKIQRZLIlkxGg52fQoBG2AdqHrGY2uw1wxi1NKJdmb11xdBkwX1nPW8piDQnN9VtGLDC9c/20+s//rbJjrx/qclerx+qkf4/WtH6WO7v5GxTSSlFojBSRSMq0sL53qstVPUaqhnykmpWZSGmaVXu5jEygZkXUzokGXuUuZa081Mww7Eo9gdn2x+tlvLY9QMufKpGSrl6KkoGiqR6otbYO/tgnF07b+lNpShPc6BEEQBEHwIfGUVjgKPv3aK3z6tVf4p1/+v/m7//X/yGg84W//p3+f/+7v/Sd8zysvPulDDILH5sJ6zmY34fKoIIvLtiPfe0ptV4uv8+W7YSPV3oC4OOyEd3QHQRAEQfDInPNcGZeMltXSJ1m3lh3Wrcmnb59UcLIuDju8Ny45v55zeVSwlkUPFdQeXlsXhx20cwyyiO9cX5xIKCeEYLisHn1artlHff2e6qfsLxqG3ZS9ec1mN2FRs6z4azg7yB5oH9zNz0ulLf28nWbL4ocLNQ+Ds8SVRPUU3ywo5lPmWZdpqZhUmoNCMy1vhGcAp+KK75l+kfPv/iqpnhzrc87iTb55+if49vCHMer+5zGO2j1r2jnyWNEYi/OeTqJ4brjO9qTi2rRis+sBgUFA3MPEXYxMuT6tGBWal/OYzV6Ccf62n/2uTkrSyIKAfhZxsNAAqEeoLU2Wx91Yh7EOaEM058L+jCAIgiAIPhyeygDtZn/1h36AutH8l//t/0xRVvzH/8U/4Of/+79HtxMmbYJnVxYrPnamz8tbPcalZlZpFnX7Q5hc7iHoZzHrefzU/EAfBEEQBMEH37jUGOs5KPSJ1a0NlpMgp/sZ4/Jkdl4FT7ds2Z5grWdeaS6NCoBjhWjjouHSqGCjE7PZTXjpdJd394sTDeXSWHHxEYK499ujvn4TJTm/nmOdp9KGUdEgBKuKv0Vt7ltneevzIiWrfVrHDXpuDc5sU9JYizcWaIOe67MKIdp/D/KEtTwmKXc5/84vc+byl1C2PNbnvKrO83uDz3Hp1GdZO8Y9B4lYHVOkBLX2VMZRNo40Uryw2eW5zR4zDYXImfsO2gug/dnu+18YspZGTGtz15/9To9S3tpbMK0MkZCrdRfW+4e+8XMYiHrf7hKENrQLP2MGQRAEQfBh8dQHaACf/9G/yK/95u/wjW+/xe7+Af/Tz/8af/tvfeFJH1YQPHZStu98DTeagiAIgiB4P8wqjXWOSlu2eumJPGYvjRiXJc57ZlUI0ILWhfWcg+Wk1KVRwTv7BcPKcG6Q3TP40daxPakYLRo2OjHPDTucHWS8dKpHGqkTDeVeOdN/qloeTuL1u9lNmNe6TVTmNbuzBu00Z9ZSSm3vGqDd7XmRQjCrZkAb9DyIuwVnh278l2e00ERK4L3nebHDc1//Jbaufhnpj7fD67vRR/ndwef4A/8J8iyh20A/v7GT/X4cN8KnSEhqHN7T/l+hIMmQSZ9B0mVwjwcdRnf/2W9nUq2OJ44EiWpDNG086UPe+XH+xnE3xq0m3jpxmEALgiAIguDD4ZkI0AD+2l/+C3zj22/hPfzKP/sK/+7P/SzqEd8RGwRBEARBEATBDYvaUpn2xu/D1q3dKk/Uaq/Oorb3/wPBh8Zr59udUkIIelnD1XHJuGgY5DG9NCJPFEoIrPeUjWVeGyalRgjBxWGHzW7C2UG2epyTDuWetv3CJ/X6XdVfCoEUku/sznh7b4H1HiXEsZ6XS6OCPFYIAZV23CvPvDk4U/UE11RHgrNDVWMRApxrp73i3W/yV3Z+hQsHXz321/pm/hm+0vur/LF7gUEek2hHoy2dWFEb98DnUS/Dp1jK9piiiCzLUL1NGJyB6NHfONBN1epcIgRCCGIlKbWhlz3crZ/D0CxREuM8nTRCCkEvfXqC4yAIgiAIgkfxzARon/7kx1f/PVsUfOON7/CnXnvlCR5REARBEARBEDxbnG/37sCj7dW5mbqpIsw94ARK8OEghOCTFwZsdBPevDZjkEeMFg0HhWZcltx8uQjRVj+eHWQMuwnpsgby1pDrpEO5p8lJvX4FgueHXXppg/OerTKhl0bUxvHe+HjPSz+LkUKQxequE6h3Cs70HYKzQ4W2JEqyvvtVPnb5lxlOvnGsr88JxXfWP8tXuj/GVXmuPYaiwTpPrCS1sXjv0fbBA7TaONIoIs8S8t6A0sS4/hZRt3ci4RkcPZfOepRsg66DQjN0DiWPH5qW2hJLifMeYz0XNmIiJVjLn5lbSUEQBEEQBPf0zPyt59TGALhRofDdS1dCgBYEQRAEQRAEJ0gKcWSvzkmwN1WEyRMK5YJny4X1nM1uwuVRQRaXnO5nOO8ptcV7VrVyUggiJbiwnnNx2LljveLjCOWeFif9+t3sJkRSMC40a1nEmbWMCxv5sZ6X9bwNZDY6MTuTCm3dahrwuMEZgNaaratf5jN7X2SweOdYX49VGdcu/hhXnv8835h1KIoGM29Qog0c28CsPXbjPMa5B3pcKRVRktHpD2g6A0YiYe4N2kHvPjvjjuPWc7mex2hrGReaUaGPXdtpnaeoLRvdmElpONVr6yMvrOdIEaaFgyAIgiD4cHhmAjR7y19eJ9P5EzqSIAiCIAiCIHg23VwRdr+6tQdVLuvW8ljRDbVgwV1kseJjZ/q8vNVjXGpmlWZRW5z3SCHopop+FrOex0h5/yD2JEO5p8XjeP0a69jsJbx2fo1zg5z1Tnys50XK9txW2nJtWrM9qXh+2CGOJIl98OBM2orTl3+DM2/9It36+rG+Bh0P2H7hJ9l57icwSTtZuG4qjHVMK8O8MiSxpKztkeff3SODVFISxxEi6XC9Ttg3ElRCLCJ25zVnBxmREqznJxeg3XoutfPESjHspuzNazqxonuMZWijRbN6Y4PFc2GjQxorLg47zGezEzvuIAiCIAiCD7JnJkB77+q1I79O4pP7i2gQBEEQBEEQBA9Wt3Zc89qQLYOK/glOYwTPHuf8iYRnh046lPuge5yv30hKLg47D/WYF4cd3huXfGQjZ29W4+o5uSkeKDiLmiln3/0i5979VWI9PdbnrfIzXH3xZ7n+kb+MU9mR3xt2E8alZj1PmFcGiQABi9qsPuZOl0QcRcRJio27VCJnv/RcHhcMuzEg0c4jhLgxyXXC19XhuTy/nnN5VDDIY6zzVNqwO68BHihEW9SGeW3oJJKDouG1c2tsdhNeOdMnixXh7cpBEARBEHxYPDMB2j//l78PsHq34Mag/4SPKAiCIAiCIAieLfeqW3sY2jompX4s0xjBs6PSlsujgivjEmP9iUyKnXQY9zT4oL5+s1jx6tk+77qKvDxg5+oM241Zu8fjJeV1zr/9S5x570soWx/r8y36L3LlpS+wd/bfAHnn6yRWsp1KdCXDbsL2pCSWgnnjkEAkBdFyp5gQgjSOkGmXJuoydimNdYwLze68ppso+llEL42YlJqLwxuTXCctW9aMWuuZV5pJqYkUbX3jvOb6rKanLcNOfNedaIvacG1aoW07YvfyVpeXtnqcHWRPbX1pEARBEATBw3omArTX33ybX/wnv40QrDrrX3n5+Sd7UEEQBEEQBEHwjLlT3dpzj3ATeHtSPdZpjODpd2Vc8ua1GbW2q11l1TI8O3S4q2yjE1Npy3vj8q67yh5HGPe0+MC+fus555iwYIyNDWUkuDIumdeWrX5yJOTLZ+9w4e1/zKmr/wLpj7eHazL8FFde+gLjU99/Y3n6PWx0YorGgIfGOnZnNY22IKCxnjyJyLMMn3SpVY/SKqraYmy7c2xeGXqpYquXEimYVZqNTnxkkutxuLCec7Bo8N5zaVRwUDTU1jHspmSxZbSoWdSGbqLIYkUSSZQQq6/xoGgQwKCT8NJWj09dGHB2kPHa+bXHcrxBEARBEAQfZE91gKa14Yu/+Tv8w//lH9Nos/o78OnNIR994SNP9uCCIAiCIAiC4Bl0a0XYWhax/hDLlMZFw2jRPNZpjODp5Zzn9e0pO5OK/UXD1XGJ955BHrPVS8ni9qa/9Z5KO2aVZmdScW1ac349x1rPwaLhtfNriOUPiicdxj2NPlCv32YO5QRMDd7x8laOcxYhBJ0k4vqsYlo2xEpwZv4Gr+38ChcmXzvWp/AIdjb/db62+ddYe+Ezx564O7++rHYUYJ1nXhmyJMKImIlYo1YDrJEUpaUx7fW0aCwCONVL6SSK2joQko1OwnPDzvsyyXUYdgkh6GUxV8clk1LTGMt6J6YxjqKxjEuNNp7GOiptkQI2ugmn+ykXhx0+errHx8+uPTPXfxAEQRAEwXE9kQDtf//lf/bQf7bRmtm84O3LV/mj199kUZSrdwse/vvn/vqPn+DRBkEQBEEQBEFw6NaKsEujAuBYN+HHRcOlUfG+TGMET97D1CW+vj1le1wuJ2g0m92Es4PsSADivKepDca55eNF7C8avnFlwul+graWSak5v57xjfemXJ9XTEvDuGiII8nZfvbQYdz76U7nTwDGecCvqvgepILyOK9f7z3zxlI2hlo7HB6JoLaWvXnDmX72cK/fW4KzQwLBK2f6DDoxf3JtRllL0iu/y6evf5GL9ZvHOmfICF79ca68+Nd5y2yyt7ugnjU3ArEHJGin9rppTGmBpE8pMq5Xij+5YmjcHlksyeOITiJJI0U3aae6GmMRAgZ5zPn1fHUNvx+TXEIIPnlhwEY34c1rMwZ5xGjRsDtraxyLxuI8KCHwCvIk5sJ6xkY3IY0Uzw1zPvWR9ROfwPwwVqcGQRAEQfB0eyIB2n/zP/yjB2lMuK/Ddwre/Fif+eTH+ekf+8FHf/AgCIIgCIIgCO7o1oqwd/YLhpXh3C0Bx620dWxPKkaLho1O/L5NYwRPxsPWJV4Zl+xMKi6NCial5oXNzpGARy+r5kaLBuM83rcTNDfeWOn52rsHfO3dAy6sdxjkEY117M8bisay0YnpJBGz2pBEkl4WkSyv204Cw26yulYvjwrmlcYvf/j85IXBEz1/s0qzO6sZFxq1DBqs96znCaf6CWtZfN8Kyvu9fhvr2JvV7C8a7E3n11jPpGyotKOXRXQShbaOze4Dhud3Cc5u4wynr/wW3/udX2BQXjreSYu78Mmfhj/1N6F3mi1jee/ymNP9jJ1JSS9V99ytdispJU4oSpkykh10rpgsGuIIhj3JojFo45nXhtoI8thhnWdjGZZt9VOG3YR0GVy+39/rLiyDu8ujgiwuOd3P+IT3lI1lVmtq48ADAmIpeX6zwytn+5zpZycaZH2Yq1ODIAiCIHi6PdEKx5urMo5LiKPBmffwfd/7Kn//P/sPUY+wCDkIgiAIgiAIgvs7WhHWVuyNi4ZBHtNLI/JEraZ6ysYyrw2TUiOE4OKw875OYwTvv4etS3x+2OHdUcH+8s/cGp7tz2uuTiq0tcwqw7yyaOdWj1s2hlltMNazaAy7sxrtHP20DZYGecyisTS2opcqtLXsL5rVhNChWEmeG3ZYyyIujQoujQqEEGws9309ifO3O6vZn9dY5yi0pdZtCJXGijxSREqw2UvY6mf3raC82+sXYFYbpIBFbZjXlrKx1Kat+BMC1rKI1CrccgLu997av3c41CygmoCu7hmcuXrB3u//POvf/gXOVLvHOl9VvM61Fz+P/sRP8/LFcwjamwVppHjxVBfnPEVjuDopAe4boimlUFHCgc1548Dx9qikajxp7Dk7yEAIRvM2wI0URBI6ccR6J6afRbxwqrfcffbkA6EsVnzsTJ+Xt3pPZPorVKcGQRAEQfA0e2p3oN38l62L507zNz//o/zMj//QkzugIAiCIAiCIPgQuVtF2EGhGZflHW+Onh1kT3QaI3j8HnV32eX9gspY5pVh2E1W4ZnznvdGJaOiYVZpRosG76GTKtbihFgJDhYabSWxFCxqQ1Ebapn03fUAACAASURBVOPoZxFlbXhxq8eF9QxtodSmvVYLzbCbtvutas1zw84qfIEb1Ybv7Bf0soY3r83Y7CZksXosdXR3On/OeUpj8N7TS2PGZU0aKfppBF7QOIeg/T3vYXtcsjMpsQ5O9RPe2V3wkWHOv/bcBhudBCnFba/ftSzim1cnXDmomFaaaaUBSKO2lnC9E9NPczqpwnvope2thDd25nesuXTOM51NKKcjysUCYw1SCPJE0k1j1rIIefiO2PIAvv6P8P/fz3Naz451vsr8HK+f+yn+uPdZut0u5+sYd23OK2f6q48508+YFO0U4VXaQGdeW7b6yZGJWSEESilE0sFEXd48sLyxs2B7UqGdY5BFN1VWttexdo6DhWZvXq+uySyO8N6TJ4o/8+Lwkd/ge1LXmZSCYTdh+KATg4/ocewxDIIgCIIgeL89kQDt1Zef52E7HJM4otftsD7o88qLF/neT3yU7331oyd8hEEQBEEQBEEQPIg7VYSFeq4n50nvGHqQ3WWHbqtL3F+wv2hQUmCc5xPnbkwnvjcq2V/U7M5rFrWln0VsdJJVjeHurKbUlqIxNNaz2UtZS2PeHS0Ylw15HDEp2krC02spvSxmo5NwULbhR6XN6l2azw+7R45zvZMwrAxXxyWDPOI71+ekkXwsdXSvb0+5clDw7WtzdmcVnSRCW8eiMcxKg7aeYTdm2E1Wu8+s8+zOK66MSzzQT9t6Rec937pa00sVu/OKy/slL53uHjmmw9fvl9+4jhKCJBKkkeS5jQ5reUykBImSCCGIlgHMVj8lVvK2mku8xznPINbs713HVAWNMVTmRr1mFkmkECgpuCAPOPf2L6Le+CKYmuN8R5ivfZQrL32B/bOfBaE4W2quTkqu0gZhg07Mmf6NfWcfO9OD5e91kojrs4pp1dDPYtayhG6eIrI+pegw0YLXL0/YPqiYVoZIts/jS6e6vHiqeyTMSVH00piLw86RitqysRS14Vs7s4eu/Xzaaw8f6XvBE6xODYIgCIIguNkTCdD+13/wnz+JTxsEQRAEQRAEwWPwpCvCgg/Gzfb77S67m8O6RCkF7+wXzBvDmX7KtNRs9lL25zWjomF3XlPUltP9lG5640fZWaWZ14Zppam1o58pjPWMigYPOAfaOLanNWva0VhLJ4mRAvpZzGYvYbRoYF6DEPTS5ra9XucGGeOi4a3dBW9em/PR013GhT7ROrq3duf84bsHfGt7yqwynOolTErN/rydujPOMcgTisaipGEtj4ikpGjaOsdIwu684aBoyGNFP40RAi4flOzOa7b6NZUxtx3T/qIhUZJ+FlE0MS+e6pJGavX6TWNJHiu66U1TYzc9b4M8YndWc3Vvn/2dOYPYoI1hUhoac/u5Od1c5tPXf5ULe/8Sca9daHcw3vw0V176G0w2P3PkTbmHlYxXxiWdJOLtvQXreUwatde4QPDKmT6DTszbewvW8ohCexYu4ToZi0VGPXVoW7R1s4XGLSftzg0yXjnTZ7OX3vPYTrL282mvPXzU7wVPqjo1CIIgCILgVk9thWMQBEEQBEEQBB8s73dFWND6INxsr7TlzWuzu+4uexCJEmz2Yq5tV9huwtVJRZ4ork6qVSh7a3hmnVtO/Bgq7Ugjwby2NNpSmXZ3l/UeD0wrjXOeRa3Z6Dg6qcQ6h5JtQDSvLVncTpr1s4jkpkmZSAoKbbg8KlnLY+aVIYvlkTo6Qbs/bFJoRkXD5dECKSQf2cgZLxpePt3jey8M7lhH99benF/7+lX2ZjXb05I8jrg2rdhbNNTaUjSWbhqxaAzWO6xzTCuNAJyHojEcFAZtHbVxSASxNHxko8N6J+JgrtHW8cbOjEVteW6zi7Wea5OKcdmwv2gYl4aPn+0/8PMmaAOPcx2HG+/x1s4I5yzGO870czY6McNOQhpLlPf0x9/g4tu/wOnR/3us68Ij2D/7Wa689AUWg1fu+nFrecy8tlyfVfQzxfak4oXNo9OEZ9Y6rPd7XK8irpaKzCn6pt0p5317Pb2zX+A9jBaOj59t3xhwp6mpu7lX7ef9PAu1hyfxveBRzmEQBEEQBMFJCgFaEARBEARBEATBB9ydqhkFcHVSMq/amrydSfVQN9vPZP6+n/9+Lo8Kam25Oi6P7C47jlo7kkiRRop5bdC2vRHvvGe0aOil0ZHwDGBSGqxzzGqDcR4MNMYyKTVaW4SAREq6SXvjXUpBFimMcyxq39ZBpjHOg7aO0aKmm0r2Zu05OnTpoEBrx+68ojaWl7d6fOLc2qrKcHfW7sAyzq9q5/I4YlJqvnFlwrv7C97ZW/DeQckPvXp6FQQcBiZ/+O4Be7OGN3fmJLFkLYuojWM9jxk5z1Y/ohNH1NayqNt/AIz1FI3FOYeUbTWic579RU1lFI11bHRSjPPMK83Lp3s4z6oi78q4oDaORW0f+HkTAmIpSFyFqidc3Z0wmRbMyppppfnIRs6wE7fnzzuG136PC2/9Av3JG8e6HpyMuX7hL/HeCz/DQXyWyliacYXDIxEkcftc5olaTcZt9ROmVcOk1FybVu1ko5AgJCQ5pD3SuMtFIbhwh9fUewcFp/sptXZ8+uI6z98SwD2oW2s/L48KPnbTXra7eRZqD0/iewE8/DkMgiAIgiA4SSFAC4IgCIIgCIIg+IC6VzXjlXHJotLsLxqKxnJxo8Or5/p0ktt/zLvXzfaxNA91bIeh3qRo+L239rk2rRjN2/rDWaVvq/y77+Ph8cvaPAFMS828tvTSCO+5bbLR+zYUKrRlURvSSLFoDNo4lBSkicI1DvAIIUljgbEeL0BJwWY3Yd5YppWmsZZ+GjEuG9armFg1nBtkCCHaSZqFZloZauPY6LRTlrGS7M9rrk4qtLXMKsO8smjncM6jrUdbR9kYLh8UXDko2VvU7M5qfugTp7m40VntPPvW9pTtaUUaS1492ydWksujAu0cUgjW86QN/1A459hbNFyf1pTa4JxHSUGkJHZ5jTTWtaFpaZiWmlhJ2lhF8NJWl1fP9rk8Ktmb1ygpsNavdhnerbrxRnBWosoJRle8O1rw3kHB3rzd+yWFaIPI6ZxPTb/CR975RTqL9451XZmow85zn+PSxZ/kmukxWWisa6fCtLuxTy2WErF8Lgd5vHpO+lnMpDScXpPMjGQwGELShejo9XPrxKxzfnU+slgeCVAfxmHt52jRkMUlL2/17llh+yzUHjrnuTIuGS0avPecG2T3/0P3cNxzGARBEARBcNJCgBYEQRAEQRAEQfABdK9qxlll2JvXTMoG63x7s194vru74Pwgu+u+pjvdbN9IYdI8+HHdGupNSs3lUcHVcUWiBNemFddngmgZUGz10weqwJOIVSCSRILRQiOEaKfPsgh1y43zylish0lh8MtfG+PoJBHaOiptb3ywACkEcSTQxpFFCutgkMWkSjKtNNAGiddnNYO8DdfSSHJ1XDKrDIW2rGUxeaIwznNpv2BUtPvJ2sCAZV0hGO+REmIELlY01nNlUjKtNDvTmuuzinODdlLru7tzZrUhjyT9PCaJFKU2WA9V40hjeSQ08EBRt/vF5rVBAlJKIueJZHsOpWjrCO1yR5pSDmc9lW5Dro1OzFoe8UfvjVnUhm6qWMsjHKwCqkRJhBCkkeTsWsr53JDUc+q6ZHtaMpo3XJmUFI1hWhp6SURsCz557Tf4weq3WLMHD35RATO1zhtnPkf98Z9iYlOuz2qMrVnUhqJxmGV4tnpKBURS0knaKcBxqTm7lrPRzdhtFLZ7mll6ikHnwabIxqXGWM9BoRnk8bFqG+8kVm3F50GhOd3PGJf6rvW2z0rt4ZM8h0EQBEEQBI9DCNCCIAiCIAiCIAg+QO63B0lJwXd35zQmpmws3Y6i1o7Lo7Yyzbq2mvDiMMcDi9pQakut3ZHpos1uwvVZDVawVwtq4+57bDeHevvzmu1JxZWDkt15zf6iWU1x5UnMsBPTWMv+ouH8IGOjm9z1WPJYEUdiGdqAEpJSa7JIUhnLVv/2QLAxbagyrzVKCIzzdJKIJJIY50C0U2pCsgyZQCIpjMF7j3aOBLkKGCbLSa3RollNjs1Kj7aW0aKmk0Q0xiEE7M5qYiXYnddtDWQWEUnBZBkgVMZRNbatlaQNBdNIMS50u5utsbzdWRBJiZKw2U3YXzTky2NpjMN7j/WejjoagFyb1oxLzbxuAz/rQXqPXH4tSkrschdaFksiJQFPYTx1ZdielLhLjl4aYaxjf15jfcIb12b00nj1eWIlWM9iullDc3CNt3cbFO3XZpaTjKN5w7hsGIo5P1L9Cz5bfoUO5bGu93Fyjt9M/wrfGvwA54ZrsO9QsmJRG8alBg9ZouilMXEkkQgcHm0clXFMS0Nt4dSgy77vg+hy4B3dOmK9svc/gKVZpbGuDV637hJAH1cvjRiXJc57ZtXdw59npfbwSZ7DIAiCIAiCxyEEaEEQBEEQBEEQBB8g99uDdHVcAp55rdlaS9nqpVjX7gnbmzeU2mJsu68rjdRqL1dj3W3TRQeF5tq4wTi4Mq64cPrOx3RzqLczLXlje8a0MmRxG1YJPJGQZJEEL5iWmr1ZRSdRnBvk7M5q8DDsxni447E01jGvDFIIrHNtEIXFOEii2ydZtPXMSo1zYPGksVx9nBQCicB6iJaTbZFQsBzksg6suzHOlMWK2jqK2iCA0bzmzFrKpDTMqnbCrZsotHXU2uIRjEtLUVu2egmldhwUug3daoP37WN2Ekmk2s+/nkdcn7fVdpfHBZ1FRKwk650Y4QXe+dXxa+uXzxvLAKxVNJr9eTuVpa0nkoAUeASetjJSiXb3nRRtTWEatcFaJA2jecPevKbSlk6icLAKTmMpOTdISSNFGglSu8BVe0x2F+waDUKsnjO/3Eu3oa/xef2b/Lnmd4k5XhXobPAKf3zmp/ij+DNsTxsEsD2pVlNvlXbtZFyWcPsgU7v/bDOO8XHOfpPw3UohtKCbNExKw8VhF3fzyNp9LGpLZdzyuXu0yalDeaLwHkp9Y2/drZ6l2sMndQ6DIAiCIAgelxCgBUEQBEEQBEEQfEDcbw+S9579RbMKdYaddmJIScFWP6WTKC6NFmxPKvqpIosV3ovV7qhDhzuk8kQxLhrGc8HrO3O+/6P+jjfbD0O9r1+d8M7ugjyR9FLVBkelZl45Sm2IGkEk3WqP1LzSfG1csZZH9NOI7amgu9xpduuxdFPFpGxDKOs91jmUlHjnqI2l0hZt2zBQCMG00Mxqg3aWSKrV9Nbh+fCAxyMOAzQJN99+97eEK/1EUdSG2lqmtWFWGua14dq0RgDXZhVatyHbWh6jjeP0WkbRWGaVZlppKu1We8NurZyMpGQta4NBQTutUzasdovV1vOR5c447/3qHIlV6OfYmdTMak3R2GXdZRsKGutojMR5Cw6c8FgL6TKEk0LQSSOmlUYbx6RsJ+HyJKKfRyRK0ssieoniVNyg9AytK7S3DLsxl0YN46LGelACPiav8DOLL/E95R9wuF3tQe0MPsMbF36a/bXvZVJp6kq3lZPeMy3M8tpRnFnL6CS31w9GShHHCT7pUqsupVXY2JJaw+6sbustreegaI63g++mc66O8efuRa2eT+4a5j1LtYdP6hwGQRAEQRA8LicaoP2b/97fOcmHe2hCCP6Pf/h3n/RhBEEQBEEQBEEQPLAH2YM0byzWeea1pZu0dX2HvPcUjQUEk6JmUrQh1sVhh808IYkkUgic9zTGUWrLtNTMG8vUCC4flPw/b+3zZ1/eRNx08/vKuGR7XPLVt0fsTCryRFE2Fo+jmyiGeUIsNVLCeh4jEFTGsDdvqxC9g6vjiiySXNjIySLJRje57VjGhWZRaxDtjrdZZVjPI4rGsjOpiaRYTWUJAZOyYV61Uyn99NawSiynscTq14h2yuuQuOUGv5SSRElmlWZWal7fmaKEYLSoySLFvLZI2Q6xTStNJ4mIFg31chdZpR2DPL7nzqlEtaFirCRJpNoqSevYndckkWJaajZ7KUKIVXB2mBnszxv25zXVsv4yFsuqSlhO4TlcmxoipMA5T6khjpa1kNqCb8NFox1uOZkYS8Vapjib1nTrCba21PZG1FhpQ6wkUsDF4pv8pP3nvKpfv/uFfAcOwR+lf5qvbnyOxdpHyaVCLNpJuEmh2V80OOfRzpMowWYvPRKeCSFIogiVZJi4x4yMyni09hzGot20vb3x7v4CIWC0aIiOsf5L3nTO7QkFNYePI5Y7+O7kWao9fFLnMAiCIAiC4HE50QDtu+9eWdY5nOSjHl/4O1UQBEEQBEEQBE+bB9mDVDYG5x3aOgbZ0Zvte/OGWaWpTbt7S+DZ6GSkkaKfxUc+9vD/2a6n0Zr3DOzOGt7en7OWx3zywgC4Eer98dUJ2+MSJQVF0+782ujEKCmZlA1mGeoBpLFk3gB4Fk277yxWAmMd82XFWyTFKvy7+Vh25xXv7hcUjeVg0eCcI1KC3VlFpOSRnzWnVUNl2ipD7RyzSpPH7Q40vZzy6iSKxvrVjJRb7STjtgkxaKsl542hZ2JsoXHeMyk1U2HawAlW1YhZJLkyLmhM+5hb/fSe4Rm0dYzGW3BtmBlHCqVgXrb1h7uzmvVOTKwEkWzDCL2slrw2q6hM+9wLQCmBWgYWVoDzy4k9wFmHcZ5YShpjmVdQGYd17d65QR7j8ZzqRKyriqGZUk8ck0SycdN1Z6xnUtR8dPr7/K3pr/OcffeeX9+ttIj5V90/z5fiH+E79QA1E8TFlLUsJora899ox6I2OO8pG8upfkqs2t9TShJHMSLt0sguUx9TNw7r77yvr5tGREowqwzWtfvRHlQ3bacYhYBKOx5yDdkR5XJSsJ1KvPO18SzVHj6pcxgEQRAEQfC4PJYKxycZYD3p8C4IgiAIgiAIguC4HnQPUq3dssYQ4ujGD16zSjOvDdNKU2vHmX7GrDbUtg2WNjrxbRNX0IZIp/sJb0mY1oZ39grO9HM2ugkX1nMujwq2xyVv7y7QziGk4nQ/XU37QLufTAiB8DAuG8wCitpQ6nZaLovaSanaeq5Ny9Xk03PDDlIIKu1obBsMSdrdXeOiwXrH/qKml8TkcVsBGSm5etPm4SSe955SO2Lp8d5Q6vb381ThHOSxWFYcOrRr6yWFEMS3TO9NK9MGOdYzKTTdRNFJFZGUxKqtnqy0W1U/jsvl12g9nVRRW7sMQO7+A7EU7bSYkQ4EdFKFNo4okpSNpdSGSWnIE7m6LnYm1TIM0lTaImiDuEiK1WdSEpxtHz+Ssq3Sw2Oco7ES7y2VsRjv2ewkPL+egJ4j62tUc8014fjIRgd3U4CjXMPF61/mZ/f/CZvm2v0u4SMK0eGr3R/mt5Mf5L06wzcC79vnOYkU1jlyGWOsZ14bisbQGAeinZyb1p5BP6WUXRY+pZwLnDPEkSeP5F1vOhzWfmaxoqgts8pgjGsrOSvNorY434aI3bQNbtfzGCkF/SxGirY+8qSmtua1IYsVUojbQuxDH7TaQ+c841Lf83zdzZM6h0EQBEEQBI/LiQdoIcAKgiAIgiAIgiA4ngfdg+S4/Wa7dY7RoqFsjtYIauepGks3aYOf/A77pKCtRYslDDvtjqz9RcOb12YM85h39hd8e2dG0VhiJdnqHQ3PALJIUWtLaSzzymCdpzaWxjhiJXGy/Tmxse3U0P6iRsr2xngsJWncVhka65lUmrKxaLvcFSYExnsKYzktxZHz0k0kWaRoIosDSm1At6FSnirWkxgk4AWLxrBoDNY6ennc7h1TN8KKw/BsXhush0QJTq8lGAv7VrOWx6SxIlOKWWPop1G7w0xbamNJE0m1nPQZZHcPDZxnNQ0ngFRJjG33pi1cG+KNFjUDH7O/aNpQtNQ0ywDwsL7SLasfpZDceqm0gYwnjSQCgXeOwniUkpxfi3i+a1hnxvVizvVZW60pEHg8UkBsF3xi7zd5bfef0jHju34tdzKW63w5+0v8n/FnWfgUXTkQ7TSgFILGOea1pjES6z2RksTLfyrryZMIn/XZF332xx2ElNSmXu6wa4NPKdqgZi2PiOTRL35UaCIpONVLcLRTnV/65jZ5HLUTbtquzmG+DGUiJbiwnvOR9ZxICTY6MTuTCm3dI+0j07bdNXd2kBEpcdfg6YNSe1hpy+VRwZVxibH+nuerIwzmDkOA63n8RM5hEARBEATB43KiAdp/9O/8Wyf5cEEQBEEQBEEQBM+Uu013jIuGSdmGYFu97l3/vOTozfYImJRtXd1sOalxWCOYKEml2wmtxjpy7hygHU6odJKIbpZwdVwyyCO+uT1le1wxLhsa4zjVvz08896zN2/acMx7ZssqPokgiyOyRCFoQyOlDWVjlwFKu/Mpku1EWaokjXUUTTs15LwnjxUeiKXgYN7gnefMWkaiJJGSON9OXh2OpGnrAUcaqbbaUMLpfsakNHjvqRpHbR2ZdaTZjYm8Nni07fSc9XQTxXonpjFQNIY4EnSSdj+al0CzDMFEW7PYTWOc8yy0XYZjmkhCe0raEFBJiGU7iSeASEiM9MsayXZXnXWeWWW4PCrQNmt/XWsKbWl0m1Z42gTOe7B4kA5nD0M1lqGGaz+n9ySRopspFI51WZC7ArfwTCWwvPYE7S66uBrxF4uv8Knxb5G48jiXNbvROb7c+VF+R/5paitotMc6g6cNCqVsA99YtQFnEinS5YIyIQRZlmKznAOTcmWi8GNDlszJ4og0ksuPaycm23PllhNOKf2svSYXtWFeGU71Ugpt2J/XdGLFpGyQ8vC1cOOYhYAsVmx0YipteW9ckkjBsJtwbVqzPal4btg51nm42fakQoj28S6s58g7VIbCB6P28Mq45M1rM2ptGS13MN7rfMVe8+5CsDOtOTW88TFStmFkpe37eg6DIAiCIAgelxMN0L7wEz9ykg8XBEEQBEEQBM+0B6nKCjcMnw33m+7Ym9XsTCt2JhVrWUwvi0juMLmRxm2QIwRo40mUZ161IQse+jcFXNFywsrYdlrpbtrgqZ3IurCRsTdvGC0aJoXm+qxiWmqSSDLs3D79cbh3zVhHqS2JEjSmvY47iTzStJdFikpbrAUrHPvzhjRW9FNFqgRKSZSwgGez2+7BaneoWZJIUhvL3ryml0aAoDIW69oqRyUESMgiifUs96sJrPOsZRGNsSgJgyzGOt+er1ITCZjUhqLSFMsA0nlPYzxx5FfTgJGSrOUR46LdqWW9w3mPdZ5OEuFwTAtDWVviStPL4jZ8WCZISrRBUdm0u9REJIiWx9eeG8mk8MvQzODGZTtttay0vLkV8rDC0jiPczf9ngew4NspoSySnOkpuqLElWNmRYWWgvVOQpQopJBIYNPs8Hn/Zf7C3u8T8+A7wwC+I1/it7s/yqX+9zOuDIvaoq2lNu2BJUqglMAjloEiaOeJtMVmMacGfZxOuTLxXJo0zCuNkpo8UfTSnEiKVf2otZ7atju9FrWln8Y4X1MZQyeO2J3XdJM2KIuEpGwc7+wv2OgkfPR0j61eShZLlBBY76l0G8LtTCquTWvOr+f0s4jrs4pzg4z3Dkp6qSJWsp001G71PTqN5TKciu444TUu2tfQxWGHNFZcvEeI9CRrD53zvL49ZWdSsb9ouDou8b697u91vsqqZqbhzesLiCe8dn5tFUhfHHZ4b1xyflkBu5ZFd9zneD/HOYdBEARBEASPy2PZgRYEQRAEQRAEwd0dpyrrwnrOxWFnNVUUPH0eZLpjd14xryyLRrM7r1g0lvPrOZu33EzPk6jd36UkpTYoBdZD1TjSWB4JXA/v63vuvQep0hap2qq3fp6gl1WSeJiUmlI7zq0ly1Dqhpv3rjXWL2/8axqrcd5hnSK66bI1tp2+Mq6dvMojSdomS5TaYZxnWhs6aXvDfS2LqYxhb9ZQ6bYeURuPSGGjm9AYy1gaPO30mVh+zamSy8/vV9WTzsP6MojpJgqEoGosB5VhUWsmlSFZflwWK9Y6MS9sdjlYNMtptDYJE6uvxbPMvrCu3e3lPFTaEDlBrR1JdON8HT4XjXFksWJRG7pptAya2omhJBLY6sb3g0TJNhPz7W4zbfwqkGuf07bSE3fjeTbLr/N0V7IVVahmxMGiQC/DxihTaOsQGs5Vb/Fz9jf4s3wdyd2vjzv5dvYpfokf4a34Y1gH3dqgraexlqJup5/SSC7PyY3wVgpJlkSk3T6LuMe1ecbOpGJetwFmLAVxJBFeMK40ZxNFbRz9LCZWkKFwzjFrLNNKU2nDpGjD0wuDfHkePI1pf//iRs4Lp7o8v3n7VGcngWE3QVvH9qTi8qhgoxPTzSKmizYU/r++s8dmN6WTKBp7o0KzDbHbCcRhN2Grn66qCsdFw6XlY212E14507/n9+8nWXv4+vaU7XHJpVHBQaHZ7CacHWR3/PyH56sxlm9catgpBX94ecKohrd3F3zq4mD1xo9XzvSxtg33L42K9us8Roh23HMYBEEQBEHwuIQALQiCIAiCIAjeR8etyjqsFnvlTJ8L6/mTO/Dg2I4z3RFJwbt6wfXacnlUcmatnaya15rnhp1VdNNLFEoKeqnioNAoKfHeY72no47eYD68pg73T92JdW1tYirayZpeomjSiHFZYp2jbOxqyupmxt6+d62tILREsg3FamMxvp2Ys64NyJxvw7xIthM33SRiXrcVito60kiy0UnIErnc2eYZdGLWfUyhLR5PaSy5tmz1U5xvg5qDoqGbRlTLSaHKOCJpqLUlixV5oljLYjpJRBJJZpUmW/7beE+WKE51YoyHM2spgzzmxc0OFzdy9hc1l0clRW2PTPV556lMO5XknMdYh3Ye6QQyEvTSCCEF3tOGPrWlsY5ISiIl0M4yX2jSSOIj1YYz3tONFbV1TEqDtm0FJ7RhmfXgbBsS3Rx5CQH9LOJ0LjkVV0RmzqJoqHU72coy+NHG8bL9Oj8jp/72xQAAIABJREFUvsxr7s3jXc9I/rj7Z/jdtR/nanSB7UmFWe5mizXM63byzHpPIkVbsbkMm7I0opOm2KjL9SZht5HMJgbLHG0ctXYoKeklqt1BF7WTZPvzup0eFBBHajV9l0hBLWB3XpMoyZm1DON8+/x4mDeWQR5zqp/ecZLzZrGSPDfssJZFXBoVTErN7rxGCYGxnm9tT4mj9tikvFEnGUtJL1M01rK/aDjdT6lN+7rY6MQ8N+xwdpDd9/v2k6o9vDIu2ZlUq6/5hc3OPUOuxjr2ZjX7i4baOoSA98YVcw3X+hXzxrDVS1dv/Bh2E7z3XBoVvLNfMKwM5+4Szh06DDOPew6DIAiCIAgelxCgBUEQBEEQBMH74GGrsg6rxaz1HCyaI1VZwQfbcaY7Tq+laLsMEpRgb15TabNKwZ4fthM0Qgg2uwnaWsaFZn9R45c7saJbHtcsqxkjJe5603pUaIQQpIpVVV6etGFOUVsqY5ePffSam1YGY/2RvWvTsg2DIiWJpcB7T20dhbFoDziHde00FQi0cejIURtLqdsJsCRSdFLFYFk7FymJ9+2xdYxi3lhiJah0O+nUSSKUMDRphLGeNFJ451nUjuuNoZtEdBJFJ4nIE8V6J0JbTxZLppVGSkE3icnjNrDLIskLm+3E0oWNDto6ppVh2E24Oq5wzuHxLBpLURvKxlALgacN8g5DzPZ8ibZaUkDjBErAZjfFe48DjPHLnXBt8OAcpJH6/9l7s1hJssQ87ztLbLncvEttXT3dPeMZDknPkJRFSjQ1FDftoiRSkknrQfaDYcAw9OIHw4IMG36wBdkwYMOCbdoQLEOCbdDiIkqWbIk0h6skUiKHQ5PD4TQ5PdNdXVVdy82b92bGdlY/nLhZdatvdVd1V1Uvig+o7q6uvJGRESdOVJ4//v8fohsZoiQDWkm0FDgRcQ8IZ1KkCMALFezKFtFvWK17CBGpQMs0rwg83+p+jR+MP8MnuM7jGM56Mn4x/4P8k/kfw1SX8SHSdUncA8FOlbPuTBLTBpdhoVP04aTMKIsKo6csfcFRF1hueopMgUjuuc6mY6qkRCnBNNO01lHlCh8jLkSOWouWfrtPQqROtQuzJFoFIiet5fJOyVFj2SmzrYuvyB7NzbVTZSghePn2hjKT3F33TAvNhVlBZz0BmGhBrlU6pzZwe91zY9VR5Yov39kwLzXf9JFdLswKrixKPnV155He+1nHHnbW8/KtNYfDQxxvJ56d3rOsTx2FhycdjRVMQ+T1o5aT1vLGSccnLs64OE/HKx/mgpcOpszK9POrxrCoMmZFuh5P73mn18Fxm+ajF/Yn2/nyUY/hyMjIyMjIyMjTYBTQRkZGRkZGRkZGRp4B7yQq6/5osU1nt06UTz+/eNa7P/KYPK67o8qScFJkikwLpnnqdGLTgxDMCrONc7wwLzisDfvTgi/fWW/dZQ/qqsntJBBCnHHhxBjpXBLgbq97ShlpB21i3TuyYTtKDQIQ4H088/PrztIO4tps6F1Lr0jdW6WW9D65ihrriDa5kyLJmWR9wHpBCJFJrpKjK0aKTLJTZJwWe92LoRRcXpTMjef2Sc/eNEcrgRBwWHu8j7TGkam0ID/JFb0XFFrSu4DzSZi+edxv3UN7k4xSK26vexaVxkeYlhm9jwghWPeOWa64uijpnUeKyKtHLUKk+ErrI70NyMExGkJyAiZXnMJFj0ZjXKC1jkzLFA9ZZkQi15YNnQsQYdVYZoUiAkomQS7XCimSQ6qxjmjSUTl9zU6puVDBggbfbzhue0JITsLT051j+CP8c76Pn+GKPnz0AQzUYso/kt/B3/WfoY8LJq0isx2TXOFDpMwUizLHBs+6g84FXAjsVzl784qsmNDIKdeNZrPxGJdiERHpgQIpRRqjSuBD+swxwiSXgCbEgPGRWaGZFZoiU9sIxdNxrUTq8KuNQ2nB60cNlxcVMUYymWIWq0eM/nt92WIGR93tdcfHLky4sqgQiK1wtOk9697d5+4UGO+pN479Sc6iyuic5+uv7jyWa6rM1DONPby2bOit58aqZX+aP/R9Yoy8dtRwVFvWnWNZ90TSmJxmkRf3Kzov2PSOvSqnNf7Mgx8H0xwp4dI8Z1Hpret61bbnuq6vLEr2pznFcDxG59nIyMjIyMjIe80ooI2MjIyMjIyMjIw8ZR5XTDnlwWix15YNQgj2hmiukfcnj+vuAJgWGi0Fs1JxVFsOpgUXZ0USuDLHjVXLvNTJpaVkciUO0Yp31j0+xDML0j5EOuuZlXoQeFKM4nHr2HSW2niOW4OWEqlSxN+dTU/jN7gQOGkdi1KjZOp5qq1jl3z4fEPfl0nxiGqIiBPbf4DWijxTdMbRWlBSkikgRiyCXEvmlWZeZsltlCXBrdCpoysfytO2QoVI7ruP7E3wIUVAnkbf7U5y3lh1HHcG4yOLUmNc5O6m58Ks4Opuyd40P9NfFWLk2rKl7h3WB1atpdSK3gZiGbl90nFn3aOkQEnBcmO2vYRHdc+6T9GKPiQxx4aAiwKBwIdA3TuE0PjgsC6Qack0U/dFU8KsUCzrtN1179BK4kJAeMH+JMfHJIqEGNFCgvBkUjCvMi6VgTk1ptuwas22406I5ErbEQ3fJ/8pf4qfZ5fNY43fdXaBf7H3J/kF/Rnu9hLZGpRLgleuJJNc43zAR8nFecG6tyxri9aKnWLCZGfBRk45sZJN5wjRbrftYjqP1qeoR+sC01zjQtjGP7Y2kCuBCxI1CCuzMo2VGOPQAZjGUKmTmPe5147onSdGwU6huXncsTfN0FIwLd5+2eNw07NsDHc2PZkSLKosuQERfPLyjMONIVOGRZWE3gf70BqTYhyJcGlePtbxPuX53Yqj2jz12MMQItdXLcvhvZ5bPHx/XztqONqk47LpPfNSszfJMMZwVybX5XxS0NmGSBJVv+byjFsn/fbBjxf3JxzMCualpsxaLs3LsfdzZGRkZGRk5APDKKCNjIyMjIyMjIyMPEXeiZjyIKev/+phw6w0vHxrzcE0HxcY36c8qrsjxEjdO9rT3q7h341x3DxueH53wqzULOueaZEi5a4Oi+IH05xNb7k0L6h7y62TnqPGcGGaI6Vk07u0MK0V8zJj0zuWtcH4wOHGsD6NL8wYohYFrx91zHoQJLeWlMAQ6XjSOq7sRNTgGoohReslt1BCyeQIgrRIr7Uk04oqi8ToUELRe08+uIL2Jjk7ZU5pUkxjXxvE4E6D1BFW957aOMpMMsklxic3kvWRq7tlEgqkoMgkx3XGqjUYF9mfaeal4uK8ZDHJuDAtCDG5s1rjWLXJrbbpPUeNYVZotBC0znHSStadIzv9rDF1nW16R5UpaqXIpae2ESUEUggkyUHlQhj2H3yTnHCLSRJjylxuoyk76wHJtNBseouSglXTU2jFbpUxLTWb3iNEEjB9iFyZ5+xmjiqc0LcNR12/TWI8Pe77ccW/oX6ePyX/GRXmscbtsnyB37j0fXx57zNEoXkuBNq7DT5EjoPBuuRo7EyK57u6WyV3UTHhyGq8yVmFghvrQGt6lJJoIRAyNfiFEDHWw+AaO3UdlZnCBQk4GhMgWspcEWNECQkxbqMUz8OGtD/L2rA/zbmz6bedcPvT/KH9f9uf94Ebxx3rzlL3nss7JY1JbrNFFTE+cnW34rlFycb4FNtpU2ykJI29Ktc4F3h12bDu3Dueo0/jCoUQTy32cNVanI8cNZZFlT1UnDusDUd16oOrjefSvDhXjFRSMCkUm244Xi6c++DH5UXJd3zNRVat3R7r02tyWqR5arfKHtrZNjIyMjIyMjLyXjAKaCMjIyMjIyMjIyNPkUcVU96O3UnOfpecSItKc23Z8DWX5094b0feLY/i7rA+cGfds6wNLtxztKS+LUsk8vpRR9N79mY53ock6CjDc4ty24H34v6EpvccNZbGJtcTJBNYZz27k5xIZNNbNp1j3TtWTRJVdqucealZTDJmGl5eHyZnSQxcO2oxLglkPkQa4xBCcHfdsVPlQwyboe6TCBViJBt6uoRIjq3kIpP4cJ8tToIKkjyXzEvNTpmTa0nnkkgUItTGYrynyjUxRja9w4fIpveU2mN9R2c9zgcu7RQoKbg0L7k4L1I86hA198Zxw611T4jpnEwGh8th07NuHZve8ephTWM8k0xxeV5wMC+4NC9SxKSLXD9uWNWGxniUFCwmOfNJ+kwRsNEQQsSFFE2ph4X/GMCS4iu1koQQ2SmzrfOss56T1qJkiuNsrYch+lHJe+KIdZ4QInuVYlo6qrBhtd5w1Pb4CAqBVsnB8wK3+PN8lu8WnyMT97rCHoWbk6/jNy5/P9d2fi8IgQspRrDuHSEkoUvJ5GDsXSAES5ErghCIbM6KijtYbnc9tUkiYzac+34QEwGMj4QYyFSK+AwRpExuSXWfaNLa5ESTAqSILGvDziTnYJqO6YOYQdizPhBiZNUaXtqfkinFxfn5otv93Fn3WO9Z1klInRY6idsmXcOtccwLjRCCeaGZP8zRVqQI1HczRwsh+PTzC/amOS/fWj+V2MN1Z/EhCfYXHyJKGh+4sWq3sZUPE89OqTJFc3q8rE9i2EMe/Ngffo2MjIyMjIyMfBB43whoN2/d5Z/+yv/Hb/z27/LKazdYb2rWdYOz7vE3JgQ/+6P/05PfyZGRkQ8dIcTxKciRkZGRkafG40RlPQrPLUpWjWFZG8qs5eMXZ8/sPvUs75kf5Pvz27k7Djc9N467e51KnceGsF0YNy6JRZ313DzxuBBwAfy6Z1HlrDuHkGLrgqlyhVapd+y0/2rVpljAxngak6IGG5vEmEWVcTAryJVkf5pi1dZNiwmwah1S6UHYENxZd2RSsBmcLoebnoNpkTrAekdnPXUvMC4ghNgKd0oKjIuEOPwibkUnKSCXgjJT5INtSg0iivGexgiKDFywuBBpek+mBXVv0RK0kWgJrQm8elhTZopL8xKB4KX9KYXuWDUn2BDxIXDSWjobuDO47owPQ3RcZF5oLu+UnHSOSzsVV+67Po1z5EqRKUnEA2IQOmGSa+res1NoOpdiCE/HqBICmXHmvBeDCymEuD1uZZb+3PpApgS9TZ1dO6WmyhS99cQYeK7q0WZD37WsjN0KlDKmY/Z18VV+UH6WbxO/+dhj9VflN/DP9/804fI3bfen7n2KhAyB1gV6l869dYHOBfJMoLMCV+zwVTsHn3NtWWNDEnQmuSJTgoggxhTBGSL4EAgxUGQZpMRQWuuppCJwegwBknAbhtTHXEV6r2h6y+tH6SGE+eDiO+XUzWZdYNM5ruxUzMuMq28TfQjJBbqsDesu9ZqdCju5Tq5I4wO9DW+5jft5UnP080N/2LVl88RjD+ve07k055ye9we5uxUVe2alftsYzIcdr/HBj5GRkZGRkZEPOu+5gPbV12/yQ3/rR/m5X/o1Ykx/0br/qap3wtskNIyMjIzQWc+1ZcP1VYvzcczhHxkZGRl5KjxqVNajkinJoso4aiyX5iWr1j71J/mf5T3zw3B/fpi7I8TI68uWZZOEnCSqwqRQ7GTJiSVFcnPdPO44qnuWjeXaUUuVKU46MWzfMC/zMz1MmRRMc83tdZdiHGfF9r1DTPs0FbCociZ5EiF3Ko2WknVnuXnc0zhB3TtOekPnkoMkU4pl3bPpHL3ztDJ1PUGK1rM+qSZKJNEsUxIfU4RbOgZJRHEuDkKRRCnBrBoW5IWAGGlNoLHpszTWI4UgLzUyRKpcsVNmTHJJlWl6n0TBdWepcs3N45adSvPi/oTlxnBn3TMpdBo/AXyEIpN0ztPZQDs8oLk/zZkVGdYHFlXG/cYmFwLLuqc1HuMjzy2So+ektdvxWGaCRVXRmMBxl9x4xkeUjGiZIv2qXNK7JAJ2tqXMFFqKJJLlGuMDvjU4n8SjMhdkWlIoONAGsznieN2ybA2ZFARAE0FEfr/8bX5A/TSfFq881vh0UfLZ+M38Q/WHWVUv8LHJlF0fKLVk2ZphXwO1sYRB9CyVYlIWBJlz6Aqu+ZywEYh1D6KnMUlstCFQaYWSkkmu8AFcDBibROBJoZjmCusivQtIkttMClBKMs01Ugh6lxx0vQtEksPsuHMomVxrnQ1cnOXbL/7OBzadp3eBQkt2p5r9Sc7BQ9xV91P3bnDceSbFvT4/NWw7Rgg8+gLFk5yjU5/YnI9fnD3RBwpCvNeXqM5ZPIkxcngqKgL7k+xNr3kQef/xemBB57188GNkZGRkZGRk5N3yngpoP/Xzv8xf/e/+Jm3fP1AO/c63+W7Ft5GRkQ8/11ctL99a01u/jUTphsWQU04jUfYmGZ31vL5qHykSZWRkZGRk5H4eJSrrcZkVmlXbEmJk3T1dAe1Z3jM/LPfnh7k7Xl+2HNZ96hPqPfNSszfJz0TXnfLS/oRprtkpLXc3PbfWHY3x1L1jWfdc3qlwIRACOB9prePuxhCjoMoEkzwJAVpBiILOSZ6fV+xOciotQSQ31Z11z6Z3adsOdGsJQnJhVrBTaso8ucReMQ0xpu6nSBJIokiq5kRLlEpiWmdTX5iPEaJI3UxErI8pV5I0fqtMMxniDI97i/OBzjp8BI1gViZxzxKYFYpMC3aqDCUlJYpSp964zRBJuVz33DzuKLVi3VnurHta63nxYMreJOfFg5JXbjdMcstRnbavpCSX0LvIunMcbgzeRzItUy+dcZx0ljLXZ0Tam8ctkJxjl3dKdioBIpIrwaZz1NYPbruADzq56GJkp0rdbRdmOUomkeXOpudObfAh/fxeodiTDbpZc3fTsunMvbjIEFF4vlN9nh8QP8PHxM3HGpdtzPkH4dv4cf+d1Pk+01wjbGDVGKpcY4OhGWI+excQAnKtKIscIytuthk36jh0zHVD1GGGdcnRF0KgP02OFKkPTkrwNgnhs1IzyZKo5pXHmBRZOik0hVacXgaVUPjBkalkEqSklMQAdzaGae6wPsO4wE6laa3n9rqnd55cnwpKOS/sP9qc0NokSNkQ2MnuzaV+mHiEAMnjLVA86TlaSvFEYw+lENs1F3/OAsrG+G1s6jRX58ZmPki4/3g9sKDzXjz4MTIyMjIyMjLypHjPBLRf/rUv8J/+1/8zISTX2fDw4Rkh7ZTzRLEHRbZROBsZGXk7Qoj81s0T3jjuOKxTKXeMKcro4qygzOS2lLuzgXVneeO449ZJz9XdCu8jR7XhU1d3tt0jIyMjIyMjb8WjRGU9LlWuiDEt/Nb943UdPSrP8p75Ybs/n+fuONz0LBvDnU1P8wh9QkIILs4LSi2ojWVeaDa946hOcYQg2CkylBLkWjApChZVxrq1g1PFpe172PSOq7slF2dn40PvDpGGJ51l3VviEAlYFgqlBK1NfVfGRya5RAqNIEVMCpFcQYHIUQsXZql/Kc9Sd1fXe6wP+MFFWOg09gutWJQZ8yKJYa3xdCYM8ZKknjIJnQlIGci0TKJIkQSvGJOTbWMcAsgkHNWWz/fHVLmkyDREcDFycVbw0QsTruwkIeXCPKe1no9dnLE3LObfPG453PS4kMScL90KXF2UHDWG1nmMjZRabTu6Uuyk4qQzCNIxmpcZe5Oc3t7rQRMCQhA4H1EKnIfeBja949KsoNCSo9pwVPeUUnBxqpnTkJtDjk7S/kDqAAtASc8fE/+cH9Q/x2Vx9FjjcRVn/F3/B/mH/AFaMQUNlU6xnyFETjpHWDVkUtJYh/OBMs/RRUEdJ3y10ay6gHEOrSQ7ZU5nU8+Z8wEhIiBoXRz6wtI58sGjpYQh1jHXavgOHzFdIIYkVmZScL+GLEVyMvbOo2TqyltUGYVWtMZzuDEcd45pblm0mp0qZ3+abd1su5Ocj16YPvJc0Nt07mNMMYSnmFMRUUmKx5y7n8Uc/W6YFooqS+ejs4EHazlb4wgxHZdF+WgPfrzd8XqWD36MjIyMjIyMjDxJ3hMBrW5a/pP/6ocIIWyFsyLP+d4/9O18w9d/nF/4pV/jp//JrwBJKPtv/rP/gK43nGxqXnn1Op//wsu8/Mpr2z8H+P4//p18x7f+a+/FxxkZGfmA8Fs3T7i5alPBfGM5mOZceUg3wiRP0T7WB24ed1xbNmw6SxxWxD79/OJZ7/7IyMjIyAeQt4vKeieciRZ7Sk+Rnd4zXz2suXncM8kVO1X66pAizyRVppgWmkmu39U988N2f37Q3WF94MZxt41fezvx7H46H5hkmpV0aJHi/S7NCw6mOc8tKrQS5EoiRBJuehuwwfPqYcMrdzZomdxo3p9dBF93NglyjWHVWnrr6QJMhicaN50DBL31WB+3cXxllpxm1gWs80gEjXHc2aTYwiSlnH520Ergg6C1nkIrpoWiLBRVnlxG695iXOpMqjJJIMU9NsYxr5JjqcwUhU5Rk531hAh1b7E+kiuFFIE3jk1yvkjBRw8mSCG4OC/JlOLCLOdLtzbbOLpMim1EqJTpmC5PDERoTXIyxZjiA3Mtaayn94F5kVHl6TOcdGBD4Li19EP/mVYCJSFHgUjXqYsRZ9N16mNAK8/1445L89Q9d3kqOeo3GHPMcdPjvEcJgZbp+p5S86flL/D96hdZiOaxxuHNuM+Phe/ip+Lvp41ZGis6RaDmOol7MYJSgnWbYi2lUmTFnCMm3DqWnPQOH3qqQlPkqZut0opVJ5hkKYLSukChAr2NqTMNKFSKzzyYS2Z5ihec5oraJGE1iaop8tHFs4sSkdRpFiIsqoxpobmyU+JCiuLUSrDuXTqmRHarDK0FnQ1cmhdoJajyt7++YoxsjOdu3XN33XPcGapaUg1iX2s82XBtPcr27udZzNHvhnmZIUUShM8Ts5KomMZHph/tvtVaTyaH43VOrO77XVQcGRkZGRkZGXkY74mA9uP/989wvN5sxbPLF/b5H//aX+aFq5cBeOXV62de/+2///e8aRtf/J2v8EN/+8f4pc/9JkLA3/vHP8fB3oJ/7y/+uWfyGUZGRj5YXF+1vHHc8dqy4bi1fPRgwu6Dj1ueQ6YkL+5P2Ck1ry0bXls2CCHYm+bvq7iokZGRkZH3J28XlfVOOBMt9hQcV9dXLdeWDb9+bcWN45aDaUGIkdvrfttFdr9osz/NuTgv3tE988N4f37Q3bFqLNanWMoUe/doX8HWnWPTeTYmiRtXdkqqXCGEYKfSFFpyeaekyO6JmQK4tmyJQGM8Xz2s6Wygynsigv1pRoyRWycdt9cdd9Y9Sgq8Ty1PzkPnPM6n2EXjPZNMERDkStD0jp0q58JM8dqyYdUYAISBaZHcRgJSH5oUNMZTaMGs0CgpqI1nP0Ra4+gG58+md9gQIIIUoLUgVwrisB0Fd2tDCJHee3obqPvkhlr3FgE0NsUO7lUZ149a9oe41Ku7Fb2P+JBiGo3zHDXJYbPuHTHCrMjQu3C4sQgBvfGUuQJOf85SZZoYLcYHtEzHYt05JMkZ2RqPsZ6q0MzydG4iqX/O+0BtHLXxCJIAfFBG2s0d3HrF8dGGpvdJ3FOCQkuekyu+N3yWPxp/iVKYxxp/X45X+ZH4Pfys/yaiUNtrVgsJpI69GFI8YusCrQnMqxxRzDiOFa+3gqPaYLwjV5JMSUKISJUEUTeIX9NCUQSJD3EY95FNn2IvhUhiorERXUn2Jxm18YSQOg3LTKUIUiewLhCU3LrQjAsYF8i0YFYoLs5KlBS4ECGmuSdXqYtvViiOO8uVnZzeBfanOZ0NFOrh86LxgbvrnsMhOvPuumfVGjat51AaKpOO2WFtuLJTAJFZ/ng9i097jn637FZJUN2bZLxx3G37CU8JPN6DHz6knr+9aYaW4tw57v0uKo6MjIyMjIyMPIz3RED7iX/8c1vxTArBf/kf/6WtePaofP3XfIy//p//h/xvP/7/8Nf/l/8TgL/5w3+fSVXyb/35P/k0dntkZOQDSmc9L99aczj0qTzq4tz9nL7+q4cNs9Lw8q01B9P8TCfGyMjIyMjIg7xdVNY7oTUeIRhEkyd7H+qs5599+S5fuHHCG6uOSaFYNZY7m3udxZAWhjMpmZUK4z2HteHqouRgVjzyPfPDen8+dXcUSnLzuOWoMdxdG447Q5kpjltDrtW2i+w8XAgs6z5FHNpAMcRY7k5yfAwUOjmznt+r3rRA/+LBhM45dicZB10SFure8dqypu5zGuO5s+5YtRYpBHIQqrSAg1lOnmka4zhpHTOV3D29DViX/GW987TWcXFW0FtPa1NMqQ+WTKe2qNSfJdmt9PYzLqocQWTdOkx2z73VGoeIgiJX5FpSakWIKSbyqDWcdAItBL0P23jGXEkWkzxFHMYkuvTRc9I5bIhc3CnorGfTW6ogCTFwWJtB1DNJVBxERyUFiyrDhZa6swQpqU1ACsG80PiYHHE2pAhJrWTq8QpJGOudRyvBfJIxyzVVniIHU9xk6taaO431gUuVYCGOWd85ZrVuWbaG4NNnFcC/Im/yF8TP8pnwq2gCj1O99fnwCf5O/B5+JXxtii8UoCVbZ2Cuk/DU2oANgSAUi+kEm025RUXdSLwPuBjQWrIzyZIDKwoiAeuT+/Q0TlWIjBf2Sk661F0XYyDPFJE01ykJZa6wPrDuHJ3z9N5DTG6k3kIIYEXA+CR6GR9oeg+CIToziXYb4+mMTyLa8Fn61nLUWJyPdEPvnPOBMlO8cdLz4v7kTcfoNCLWep8E6t6zagwnrWPT2+SMyySdTWKn8Rmr1rIcnLGPytOco58EUgqe363orOfWSeoPvP94Sc4++PF2i0bLOjlA52VyI58nGr7fRcWRkZGRkZGRkYfxzAW0w6Njrt24lb4kCPi2b/lGPvW1H3/H2/uLf+5P0HY9f+N//wlihB/6Wz/GH/iWb+TjL33kCe71yMjIB5lry4beem6sWvan+WMvzp2yO8nZ7xw3Vi2LSnNt2fA1l+dPeG9HRkZGRj5MvF1U1jth0zvKLEWxzcvsCexlIoR6o135AAAgAElEQVTIz/z2bV65s+G1ZYN1ASUFk0Kxk+XkWiJFcrAYF2it56i2rJr0uXyI1L3nhf3qke6ZH9b7c6klt9cddzc9N1YdQsCtdZfEH9+ghEAMDq29Sc7+PCeEdExTbFoSmWrrOG4dVSZxPlIWklwJyixn03kWVaTu3bljoMo0l3YK1p3DhRQjeTDNmRaa49YCyRGS6xSnOMsEK1OzWyqOTUjxhkIwr/T2nG96x3JjsCGJXNuetcF2JkVyV2VKAMkxZAY324VZgfGpCy3EiJYCKURybrlIkQkEaRvTIjmATjqHsYHaJNFlVmoKJSGm10gBLkSaIRZwmmuUShF8rQnEGDjaGG755CJrjcdIgQ+pX+9BkfW5nYJXnSeSIgat99Qm9TllStLZkJxYUlAbh3WRHsfO0IGWD6LmokxfsYUQFBpmKqcSPaY5obAdt08aDmtDOzjg8kzwKf8KPyA+y7fK30oZho9IiIJfDJ/mh/338KX44vZ9MwFay3S8BIAgU6lrbGeSM6kqjkPFDZdx58gRo6EsFJfnJZveUeWS6ZnYwiRqdjaJlFIkAdyFSJUpdieauvPsTdLPHG16jAcRk9C+MclNab0n05IQQStJtB4FdMZhhCSSOvMyJZBSsFtlHDVm6JBUTPIU4ZhcsILeBWyI3Fh17E4zXIxMC82Xbp0wLzV7w5wSY+S1o4ajOvUDLuueCEzz9JkzJVHDmNRSsOkdmRQc1ZYLsyJFxfaWF/cniEdQNZ/WHP0keWF/wuurlqu7FdeWDTul3s7BRSYHlzFYF3kr02xjPBuTehAzpbg4P78z7f0uKo6MjIyMjIyMPIxnLqB94eVXALZREt/zmW9519v8d/7NP8NP/fwv89VrN/HB87/+8P/Ff/GX//13vd2RkZEPPiFErq9alrUhxshzi/Jdbe+5RcmqMSxrQ5m1fPziDCnHpyhHRkZGRs7n7aKyHhfrk3PnyqJEq7TA/KT4wo1jvvjGCV+923AyxCleGOLTHqTQinmZ4aeRZW24uzG01m+7yF48mLzlPfPDen++vmp5+daabnBlvXZUU/ce5wO5khx36dyrwaH1xkmHvxHZneTsTTJCTIv9h7Whd36Is5ODOJUxKzMyJWiG49Zaf+4CfYgRJSTzMuPKTs61o44ykzTGIYXAhkiZKZ5bVMxLjbWWE8G29yiNU7F1ikhxT+Bqbfo8B7OCj8wr7m566t4jBqFNK828SDGGSgreOOnZ9ElsU0LQ+eSuW3d225sUQnLdOS85rC2CJNa0NrnOci3orKfpHblW9IPzzPqAsYFJoakySe8CV3YK9qcFjQ3c2fT4GLl90mNcGK7F8x2KUkr2pzl31/02UrDIUnyhD5EYAqs+EIlDj1eg0OlzFpliXugzXVmCSIFhYjd0zYbbJw25Eiw3FuMcNni+XX2RH4if5VPqq481zkxU/GT4Fv6O/y6uxUsIku4mh3OU3j85jcpM4iMUWUZRTahjxVe6jOPe0rsksEZA+8hJ5xBwbofV6YMAbe8Ig4BmfSRTkkmm0jgPkVmhMdYnd6HzSCvYLTOsC7Q2IlxgE5OIG0LEx7S31qcYSyGSsDUpFD5yxil4P5Nc0xpDlJHLO8n5eioWxxj51VeXfMtL++xO8iSebQx3Nj2b3g/iWoaSyVVYG8ek0BzVBi0FB9OceaHRSnLUWKwPnFpwX9qfvuW5eZpz9JOkzBSfvDzH+8ims7y2TB17u5OcKtdJiFWS1jpm5fnLRiakeNW9WcW8zLj6kO5K+GCIiiMjIyMjIyMj5/HMBbSj1cmZ33/dJ156258x1pJnD/9LllKSP/vHv5v/9m/8H8QIP/tLn6M3hiJ/Ahk5IyMjH2hWbYp2OWosiyp7V4uWkDpXFlXGUWO5NC9ZtU/GTTAyMjIy8uHk7aKyHpebxx1CpN6x53erJyYSXV+1/O6dmjeOO44ay3M7JZd33r5LTEnBxXnBJFfcWffcoUcIwbRQHMyKh94z36/35xAiq9ay7ix17wkxObGmRRIMd6vs3GMeQuS3bp7wxnHHYW346t2ar9zdIITA+TBE3g0dQCFSe8+y9tt9P+kcN1eCxSRDCcmmT+ISgJKBnVKzahwX50l4izF1OfU2nPs57u/ek1KyN8lobeoPO1VbLu+U7Ny3uB+B1nlam1xdxangNri2jAv4IYJfKYmWqYfqYFoQY0+VpQhGF1InWBiiFuelpjUu9aXFSO8jm85hXBKjMpXG0anjRUvoXCTEdP0oAcalmMNCKyaZYneapR4s6znBMik0s1zRuUCmFJmS7JQZt9c9dW856Sx177i4U7xlvGeuJJlOQlFtHLmUZHkSWXyA2Bg669BCEDM9dLtJZoWiynUSHQHtGzK3pq4bbjRdEkN9pAkR73u+I/wKP6h/lo/KW481PutY8A/Ct/Gj7ju4y+LMuRuMZgCIIbqxzBSTMkcVM45cybVGcNwZeteRK0mpJVHBSWcJQbDpLLuT8yP4IImnWqfOPR+SyDm8I/NCc9I5poVikymUSnGehZKse4cPkUwK5qUexFYIWgIe8ISY/l+VJffZJFfnOgUBQgg01lMbx4W8YHeS8ckrMxZlxq+8ekSMafz8xvUTdicZxiXRtjaeS/PiTEeXEIJJrlluDI1JQu9OmTEvMy7OC+recWfTw6YHIZgV5i3jHJ/WHP00eH634mgQ419bNnz1sGG/c1zZKVAyddAdNZb9EFDy3hztQxL5N1bwXKa4OCvYn+QczM53n31QRMWRkZGRkZGRkfN45gLayaY+8/uL+3tveo3WZ3fLmLcW0AB+3+/5V7f/ba3lN7/0Ct/8DV/3LvZ0ZGTkw8C6s/gQ6Kzn4kO+1D0us0KzaltCjE8sjmtkZGRk5MPLW0VlPQ6nDqsX9icUmeKFdyHE3c9pF9nNVcums0wLxf708e6ZpwvSt9c968xy41iwU2UPvWe+3+7PnfVcWzZcX7U4n2LkkqOObewYQO88O2XGosrQSm7FtdeP0rG7tmz4nds1QsDVRcW6WyOkINgUX1jlitZ6hExxenXv2fSeTAVkoTDOMykE01zR2YAPESmgd4F5CUdNiiIkJqdYiOfn/d0fwWbcaS9UckCumtRVdnrOfAhsek/tILaO3iexTCLwPiAEtNaluDwf2asycp2cKZnKcD4yyTWTPB2jvYmisZ7OBDprOekc69YihKDpHUolnSfPJD4EpoVmWmgkEID1EPXnQkRLiZSCKoMoJIWWKVK0SsIVQhACXJznKCkwmxT3F0lRflPjeP2owfnU+1Wpt46O00qiRHpNlWnmpaLKM2wIOB/onMQ4ARJmWnJhlieR1EUmEyhpiO0Jm6bldt0SSVGdSgpmvuMz/hf4M/wcF/XqkccmwDLO+Yn4HfwD/wc4DuW5KY9qqEhQAiZFzrwq0eWctZhwtwkc1ZbGeKS85yYrtcS4CFiMD2RRPnRMGRewLjDJFUWmyKVg3TsKrci1QAiNGfrOMimZFTKJlvOC1no2Xeo48xGIkRAikUiVS6RIAqkJSQr0IaKEGHrkwrbrzvnUl9a7dG1Mcs18ELtO4xW/+cVdfuXVFWWmiES+fGdDa5Ij7rlBwEkOwntRtOvW4ULgwqzA+jTuLs7S/HH/3FZmKSp2Xmryc0T/pzVHP00+dXUHSELirEwdcavGYFwS550P3F737E/z7fFqeo+xgWkWuTjLOZgWvLD/8AcuPkii4sjIyMjIyMjIgzxzAc37s09JluWbvzBPJ2cjXJarE2bTt/7L56WDJMSdPiz36us3RwFtZGSEuk8RSqk74d093X5KladujtZ66t6//Q+MjIyMjPxLzVtFZT0qq8bw2rJhb5JxMM355OX5WzppHofTLrLXj1rKTCFEJNOPv8A5LTQz41nWhmmRHGm7k+zce+b76f58GrvY27TvR42lG8QzSAvI697R23CmG+ryomR/mtMYz/WjlsNNz6q1HExzjA8Yn7q2tBQsmyRQmC4iSI6MEFJHniD1CHU2IkTAeYcPAR8CO1XGJNdEUrzicWswmaK1gauChzqFqkylCDYpaa1nUWapK2wQHqaFTsKYcemzGYcJEE2K5UuL58l9Z33Ex9RnJoXEhsBUalwM9EPsniS5wxaVJtcK3VmmORw3hl4FNjJFQE7KQSjTDBGRkjIfYhJjHKIc/SDWBapMUGSSSa4ptCLGmLrQtAZS/1ZnPVIm9xKk74OnPVWTPB2HxnokAhs8b/UV+NQB54FMCHofmUvItca4wKwIQ29b6lxbTHKuzDNyt6Y+vs1h29IYh/EBLQVaCUp/zB9vP8sfi7/AnIZHqNDacoOL/Fj8bv6x/2a6kMbBeZ5DQeq0m5Q5s9mUmM2pZcmqD6xbgwuRzrjkogOKPMUiSgEmeMTQP+YHp91WOR4wLtAaR6YluU5xlblW3N30tM6jlWaaK2JMgupJ21NkSWieFXrog0vz1azQGB/pXbrGOutBCEotyWISdHOtWPeO1oZt9+Lp+VEyidaZlKxay4V5EmVOz/netOBrr8y5dtSkazaTNL0jUyKJP6t7c4MQqaPtwjznwjxn1ditMF0bvxXPpoVmZj3LumdaSO6ue67unhWMnuYc/TQRQvDp5xfsTXNevrVmUWmWteHOuuf6cYtxkbubhlVjqfJ03PemGTpKmkO4uih58eDhazUfRFFxZGRkZGRkZOR+nrmANqnOimNdbyiLs4sH0+rsX0Zv3Vny4vNX3nK7D353XG+ad76TIyMjHxrC8IQ2pIWFJ8Hpdt7qye+RkZGRkZH7eVhU1nNv0RkDSWi5edyxrA17k+SyuLIoeX737eMVH4X7u8hCDCyqnNvr/h3fM/enOXXvWHeOXKV9hjffM98P9+cHYxdvrFpiTKLXxVlBmUmOG8v1VYsSgsY4rq+SGDEvMq4dtVSZpBvEnuPWMskUry5rcql48WDC/iTjlbs1jUn9cI11WJc6p6pMooeYu0kOtfHUnWNDpNAKrQTTQjPJNYtS07nASWuH2DxBb1PM4nlMC42WglmpOKotmboX+5ipJDUcNxYXkjC27jwuQikEUktADCIc+OhwLuIC5Bq8jxgfCESEi2iZ3EFCJAfX/jT1ud3d9NRGAAKJGBx4kroP7E40UqRes0wpdJ7cRr3zhJghYupLEsP5VEIMfYKS49aSq9TdlQ2xcnFwJyUBTJCpNBZ8gEkmubMOKVqwD8zLgJTnH7c4lHBVSiAl9C6yNp5FmYTDGJMAOis0H93LeGnSshDHXF9vODxuOO4s3kfyTHEx3OVPdD/Nd4dfosA+xkiG34kf4Uf5w/yy+EaikHiSoBljEivj8Asg04pZmaPyKY2sWLoM20XyzG+FycYMcaE6dbslkXH4Fe/996kI6QJoxdaJaV0g06nrrMzUtuutzBSd8Uzz1HsnhnM6yRU+QGeTs+viLCNEwarpqXtHHLr0OusRJEGsswGGqjElBVrKbVxpmSsmuUJLgRDJvSkFaCXYn+Rvug6eW5Qc1QY7XJuzQvP8XoUUyQV3qg8ml6ZAy+SO6qznuLXc2fTcXvfMjGd/mtyN+5NsO7dlyvDcokQI8dTn6GfF87sVB9Oca8uGMmu5NC+5tFPyyp0Nd9YdrQlcmObMyvRQQC48x2XczvHn8UEVFUdGRkZGRkZG7ueZC2gHe4szv6+blt2d2Zn/9/yVi8A9UeyLv/OVMxGN53Hj1t0zvx9DAUZGRuBsB4h/QmLX6XbEWzz5PTIyMjIy8iAPi8o6dWlUuUIJgY+pQ2rTO46H6LsX9iccTHOuLMrtdp4E93eR7ZTZdlHex/iOvigoKZgUik3nWVSRde+Gz3z2nvl+uD//1s0Tbq5aXls2HDV2e3wzlWLsXl+2LBtDaz1HjUGK1GfXuxQhV+pTwS6w6dLCejM43y7OFY3xTHPF7iSJiod1T64k1nsykfbXG7fdn1RNdlZkrLLU7QZsF55vrJJT8KixWwHpQeQQl2a8Z9VY7mw64nB8qkxRDy4qFyPWBXIlKGVybBmfhNtIRCBRQ19VrgS5Sv/d+4AS0HpPoSSIuBWuYoypN2rd0/Se1jm0TE7DEGFRKZQUxDhEJsokelkft0KcVKl/ScvkMFMy9Z0d5JoyS+6kSaYw/jRmLol6ahBY8sHtZH0Y3kNQZZoQw1YQO49TEW5eZdvjctLZ9BkjzIqMiTRUvmZhjrBRYirNUWMwPglcH+M6f9b+NN8eP48S53fUPYzPxU/yI/EP8et8Ai0lAYF3Yes6E4Kt8DwpMqqyxOkpS1+waiK1sSiRXFcuRHyIBGIStHxIo2uIJK17R4BtF136w4gPgdY6pBc4lzrzJrki10k8W5T3ZoZcycGtGTEhps4w45haz6xQNCbgApy0jru15bhNXWin1+j+NGdnEN58iNTGpd40rdj0HucDRaZAJOFyf5pRZJpKS+5seqRMAtipoHdKpiSZltR9ctd94lLFC/vTbQ/gabdhkaU+t+TGS2P32rJFCME6syxrQ907JoWiyhSZFKwaS5kprh0lwf1pz9HPkjJTfM3lOR+/ONt2QU5zxe2Tklvrjs4GykzysQtT+q7jKw+ZZj8souLIyMjIyMjICLwHAtpLDzjJXr9xayuYnfKJj71w5vf/7HO/yb/9A9/7ltv9J//i14F7aRM78+kT2NuRkZEPOtPhC68Q0NnAO6iceROt8ds+lGkxPkU5MjIyMvJoPCwq66ixrNqW+3UkIdJi5pUhJrAYYiCf9ALk/V1ku5NsWHAG6yLFO/ymUGWKxiS33ao2594z3+v78/VVyxvHHa8tG45by0cPJmciNV9fthzWPXc2PXXvmZeavUlyogBbgeikM0gJLkSuLkpurFoCqStt3VliTB1mmZZkSmG9Z5KprbMmQBIuBFSkrjE/RCZOtMY9oL9kg2PGD26o2jj2HtL1dnFecFgb9qc5X7x5QucCmTx1ZkUa79FCMMk1kkAt7vVoSZkEjShT5KMPScjIdepWMy4QpCCGFHU3KxQhRprec9xYVq1l0ztWjcUHj/EQeocSApErNr0dusrAhbAVB40NuJBcQ9ZLtExxoq11aJXRGMes0HTWJ9EsJCGvsw4bItNCIQVUOglkIUakBD0IjcXgmCqUPNcJY3xAieR+2t3J2XSOSHqPg8ISuxPu1MfU1qGrjExk3Fw5nHN8vP8i3x//X34vv5029ojPWPko+MX4Tfw438Pvihe2ImrvImL4nR+sYZkUTKoCnU2oZcU1k3Fy7GitSTGOEpRKTjIbIpmEXKbPuRWsQ4oDLQbrYGc93qf3kSJS9ylascoVRS4plEJKwbzQbxKq9OD0cz51lfmQBuzHLiSxqswiL+5PBidbYK0l695zZadgp8zJlWBWZkBk1Vga67fvMysjm94lx+XgSrMedicKHwK18exNstQvl7/5XGqZrkMEZEptu9LeCiEELx5MmBaKG8fJGbfuHJvO0xhD06fIUx+SW/LyTvXU5+j3Ajk48vanOS/uT/jCjbNO3S+9sUZHR+OSk7Cw/pk++DEyMjIyMjIy8ix55gLaix+5QqY1zqenLb9y7Qbf+ns/feY1B3sLPvLcJa6/cZsY4XO/8UW+8KUv86mv/fi527y7XPHDf+8nzzyR97EXn3+qn2NkZOSDwbzMtkXp686y/5BFpsdh06dYISnE234RHxkZGRkZeZDzorJOo9JOHwarhvuMVsn19ML+5KlEX93fRbY7KWhMS6YkrXXMynf2VeFUHDI+YNrA7iR/0z3zvbw/d9bz8q01h4N4+aB4drjpWTaGO5vkoLo0L7ZdSKdMixSp+MZJhx9iEAudurpmhR6cd2kRWQmIMW7Fhd1Jcjd1LuLCPTeMljKJGgp6F/AxdeYdTHPEoH5sekc1xNUJkdwwV3fjuY67TEmuLsqt46e3AbRA+EGgMZ7ZrCDXMjmNSCKFCINYMfSlGR+QQpJJSaFOYydTn1QIyW1WZZKj2m6P7+2Tnta6we2TnHXGJdHG+kBjAzEEhIQY0ufKpMQGjw9JMAoRjIvJ9UbqZWulZ1YkF5od3GdKpS6sKksRg/My26pFUgjUEPk3ydVWAD3p0r7ef02FEOltYFoqlIDndgraUiKMxTRLbt495qjuCTFSDOJvbywvnfwL/t3+J/kkrz7KMN1iouYfhd/Hj/jv4pa4iBryFEO8p73ZkJxXVabZm1f4bMbSZdxt07m3oU9jgSR+KiEIAZCnYmhyDUoJrZGsO5PiH6M6MyaLTKZYzpAO3bRUTPMMOQj501ydG3t5OuwiSaxcNhZBGuM7ITlrJ4XGh8CddU/dZ5S5ZrfK2ZvmCJL4vKwN687SWse0SPumpGBRZRQ6xXaeXk/lEJsqgHmpz1wfZ/YNgQuR+0ydj8zBrGCnyriz7smVYVFFYoyse8vNVc+Fec5L+1NeOpi+aY4OIW7dW3Xvt9f3tEhjc7fKkPLJJVg87fd72IMfr989YWUEr9xtqDZheO2zefBjZGRkZGRkZORZ8swFtDzL+NQnP8bnf+t3EAI+/4WX+Qvf90ff9Lo/+p3/On/zh//+VhT7j/7qf89f+yt/iW/8+k+ced1XXrvBX/lr/wOrk832L/DTScWnHyK2jYyM/MtF6ssQ7E0y3jjusD68ZdfM23HacXJlUaJV6uMYGRkZGRl5XM6LynoWi60Pcn8X2U6huCVTdN5RY9kPAfWQiMC34lTMcT7SWsfHLkzfdM98L+/P15YNvfXcWLXsT/Mz4pn1gRvH3fZ8nCeenaIllFpw49gwzRWrxrJTJcFASrHt6jqNp3MhiUshGAIxCR0kwUQKMCRX2angFCJkMtDbQJmnKMPOehZVhg1hKxDUvXuoYHgwK4b9kMwKxbIxLEq9jTZ8sCvuVHDxIdAMriI1aExaCfRwjrQS6CA4MZZMK1obmBWRw9pgXURIUFJSZEm/kMDGOJyPdM7TO4+WAnyKcSREpEhWvDBED/Y24HwgVxIlJTG6QYCL2+jAKlep58p5pplCSclOde98ZUpux2M2uM4yKTjuLMetpfeB+SAOrXsHAvYnGVd3Ci7oDhVOuHGy5u5JS28dQkDwEW86vjV8jj/S/yTPxdtvOTYfZBNL/r7/DD/mv50jkisnl0kIlILByZUEoFmRUVUVLptyMxSs68BJ67Zi1/a8Df/IleD/Z+/Ngi3LCjO9bw17OsM9d8ibY1VWUcUkqgCJQQgxGDEJIYFaasuWWuG2ou122A8d0W7bD45w2C9+sqPtB0fb4Wh3RzsckqV2tzEthJAYBZQgNEADAkQBRZFZOd+895x7hj2twQ9rn5M3qzKrMrNyqtL6IggiKs89e1rn7LP2v/7/Tw6473Awb8O5Dm48iXVu5YrEgFZBCFVC4Lvtew8bvWTleLwey+EjCAKtcZ5DgwwhBELCsNBMypbDw5xDw4xBptkrW86OS2rjyHSImpyULfOmpawdExWiUJfC3VLkXH6ezo5DpOeRtZxEKQ4Ns2vv3IHFtbdCoiTH14PDbF4bytYyLTVV6zgyLDi51eNND22svqOr1vL9C1POjEuM9Xd8UUTVWk7vLu7a9p698CMXlgs/9jyy1aPf793VhR+RSCQSiUQid5O7LqABvPUnX8e//c738R7+4pvfDWXMz/ph/iu/8B5+52Ofom5C7Muly3v8/f/qv+fVj5zk0YcfJNGKH58+xzf/+od471ZCmxDwq7/wc6gXMQGPRCIvH6QME7iqtVzYrzk3qTi52bvl9zs3qRBdZ8OJ9eKOPtSMRCKRu72SPXL3ORiVdU+2f6CLzAFb/ZS2683aXbRsD67zcPp5WIoykzJ0BV3rnnmv7s/Oec6MS3bnIWLy2Ci/6t8vTWtaa9mdNwwyfV3xDEIMXp5qrCsxTmC8Z0td6SurjWNaG6QQzGpDbUKn08RYlh4jf+AJvxAC0YX2CQRWWqSES7OK7WHenU9JkWo2EkltguBWtvZ5HXdKCka9lF6qQgeUdVSNo0glizoIfLIT7mrjcEJQNWHb0oNEImTou7oKH0TBxAehtHUJ/UxTJDCvoawNAkGqBYva4hw4HM4Fgca6IMTJ1bFDpiVKeKo2OK+sg8o7pAhOuF4iGeYJaScSee+Z1S3rRejvyxO1imuEsM/WBTeTdZ4ja1noTROCVFmmdUvdWiRhTL5iI2FbL9gyEyaXaxadcJIlkkODDFdPedP+5/mQ+RybZv+65/xa7LLGv7b/Dh83P8OCvOu8CyPhoOtMScGwyFBZjxk9nqoUs1mLdTVaiisdf51bLQyeIMKqTjB0LgiVUsggdhK668I1C25A54NgmCcaLQTzxuBai3WeqrGUxq665K6H6dyMxjn2K8fhYcYw1yunn3WeYaY5N6nIdPhMtCYIds/sLci1ItGSRWMoW0fVGkQJeRquW3kg0rE2jt15g1KC7UHYzvH14rnjcjU+O4fci6xYXDpah3nSuUstD2wWnFjvrb63z4xLnrwwpW7tKpa36sSsJUt31kYvoWotz4zLW3Zn3e3tLTm48OOps4LvZ55XHOqxNhzE3yaRSCQSidxB4nOBe8s9EdDe966f5p/+zscBmM7m/OlffJN3vPWNV73myKFN/qPf+GX+yb/4fxDiSmHy9354iiefOrV63WrVWzdGjh/Z5rf+vV+6K8cRiUReGjy42eOZccnx9YLTuwvWcn3VavMbZbxo2J03PLjZI0sUD76IB32RSCTyfNztleWRv7k8u4vs0Ko3K2NnVtNL1POKSNeiMY66tXjveeXhwXXvmbfj/uy958yk4kc7Mzb7GecnFUfXCn58eX7NyeS4bDE2RMYlSrC3aLqYwTCpOL27CEKC8y8oai6FLiUltQldZwef1Q9Sxe6ipmkcs8YEccDTdX95tJIkSqJkEDccntZ4rPUo5alNiOQ7P6kpW8uRYc5a9xB/rdCcHVc0NjjUrsd4ER6uv+nkOt+/OGNcGuZVy9ZQ0RhHYy27syDM1C6MgTRRDEg3qg8AACAASURBVAqNtbBoDMZ1x+aXck8QTuatRQowDvoyONyGecJ+1VK1jto41ooE54KTrTa2c1aF41r1Z3lQeLzztDbst5YCIQUSQWuDE806mNSGQW1IVMK8MRir2OilrOUJjXWUjWVem9WYzZPgcFoKMEpKtouUXBt25zVFKmiNx9uGoZihZxUTb1koiRChO20t1xySMx7f+SSvnfwxuVvc1Bg9K47wcfk+PufezNQLnASxVMy6AWN9cO2NegU26XHZ5OyVsF8ZWmu6frIwdhIlSJSk8aEbTHRXpZcovA+9X86HaERBOGaHJ+/EMOvDH3k8iZR455FJiFO1nftvUrUkkxotBP3s+eJQgzC8X8ED6znbgwytwvg4sVFwaVozyjUX9ks2ehnOwawO46ZIFM4HEXWzlzCrbYj1BOrGUQtHsTym1uJF+Nv1QpNIyXovxDdeD48nUeLF6mdX8eyeRec83zl3dT+Y955RkbA9yMgTiRIC6z1V65hWLecnFRf2a46vF1jr2Zs3PHZ87Xmdfkvu9vauh5SC9V7CRgavPtzn0Obolt8rEolEIpHI9YnPBe4P7omA9sjJE7zn7W9mZ3cPgO98/0fPEdAA/sNf+0XOnr/Exz71hZWItmQ5UFa56x62N9f5x//dP2TQjw+1I5HIFfIuf9/a0CVyajc8+LiZh3TjRcOp3QUbvYStfsqrjwzjTSkSidwR7tXK8sjfTK7VRXZ8vQgulNZwaRY6lm5GRNudN8wbw9agx7FRft175ou5PzfWsTOtObW74PykCm6qxrBeJPx4d87F6bUnkzuzitO7c568MGWzl1G1jqaLrKtby+V5WCyTdL1La7lexRY+G8HSDQTGOoSU2ANa1qw1eOfZK1usDcKA7uIIAWzXfyb8la4upaH0Au/9yl2mladnQkfVME84NEhDtxNhDvTsGMYlB3+7PLjRo7Vhe391Zp/Dg4zGehaNCfF0TYsU0M8leZJ0x+Tpp4rdRcuiNSxaR1+E2MilGJaocMwbRYittM4zrVoWTYjZy7Xk0ryhbB2N8YRDDxO4sHJW4pzDEVxoiRI0xgVnloUi1SRa4lpLaz2L2nB+v6TpRLXtQcbx9YJBrkmVYGfWcHFaM2hsJ4CG/rdRHqL3ytowyDSjQrPR08ym+9SLCdItUDh0IlnvFQgBiZSsNed4w6Xf51WXv4Dy7QuOy4P8QDzEJ5MP8oR7HOsFrXekmq73rpvPAmmiWOtl+HTIji/YmTn2Fi0S8AdEWe9BdGJwl3rJ8mwqJVbxjM6zitFcTp+lFCRa0NjwF9Y5skQzzBISLRBeUDcNRaqw1mO9Z1I2GOs5OgpClu4iJp0P470ylkuzhiKRrBcJJzZ6aC3CeOgl5DrELH777ATnYHdeM6stx9ZzrPWUbRA8p3VLZT21dUgpkVJQJJqyNeyXLUIYtBSkWrLRS1BS0MsVm/3nd8caB6lSIMI5vx08u2fxO+f2OTcuObW7YG8R+gqPjvJrxtH2Utjsp7TWcW5ScXp3waxqVy7Ux0+8sAh1t7cXiUQikUjk3hGfC9w/3BMBDeB/+G/+wQ297r/+B7/FY695hH/yf/4r9sZXx2QcdJ+9/10/zT/6T/4OhzbXb/euRiKRlwEn1gv2urimU7sLnr68YLMyHLvOpHPJctK5O2/Y6CWc3OxxdJTHm1EkErnt3K6V5Ufy27nePvJy51pdZFv9lFndhh/bszoIEq1ls5c8byeadY5Ls4Zzk4rDw4yjazmPHh487z3zVu7Pl+cNp3bnXNqvuDirAYFHIYUh0w2X5801J5NrecJfnZnwzLhkvzI4DzvzK3OKedMyLQ2z2rDRT9mbNytR8VoRiYkSaClQUtCENDxMp6CVjaVqHGVraY3tFv4JhlmCkMGlp6XEerp+NIf1BDHJgZTh9VqFCD7roWwdi8bgfLISzVZxfh3GOc6PK364M+fitKJIJIeHOXmqyLWiSCS9VDEqEjb6CRf2ayZly3jmmc9hXlnwhiLVFKmkaiHVgtYKFo2hMTbsjwuusXCeJcYLJgvDTFpaG+IhZQvzxtK0thMpPcFTBkoFd1emFa0TWBveyziQQuJxGAtlY0IPF+E7supcb5lWK3fRMNf8xNEhO/OG2gRh7dyk5Ox4gXHB2ZanmkPDlGlt6NcNI9Vi633SasFaCipPybVk1EVBbs6e4rVn/1+OX/pTBDcnvnxDvo6Piffzw/Q1WOeDs9BZpAxuQ9M6lBQkSjPo5ZRqwHmTsT8xLEy9Go8e8C6MTynC+LLG4RXUJghZIXoSCq1oncO5ENEoRPg3RNdj14quMy+8sxQSCWSJpEgUi9aSparrSuOK6887duY1wyy5apwFx6qlSCTH1gs2+ylaSYz1q9/LCLg0q9mdN6tg0oOdgtMquADzRLBoLOf3LdY5ysbT2uB6RAga61cif5pIcq041M+oWsvadaJLW+tojWNUaBDh83a7exbnteH8pOLU7oJJ2fLwVu+GxP9ESU5u9ljLNad2F5zaXSCEYKOLn70eZ8blXd1eJBKJRCKRe8P94jiPXOGeCWg3w0c/+G4+/L538Jff/Gv+7be/x87umLJqWF8b8MjJE7z9za/n2JFD93o3I5HIfc5jx0NRuxCCQR5uQuNFw6gIcUhFqlY3obKxzGrDpGwRQvDgZm+1ynP5PpFIJHI7uV0ry8fS3IO9j7xUuV4X2aqPTAjyJDzonteGfqrCg2x9ZeLWGEfVWuaNZb9sGfUSHj7U4zXH1nj9DbgcbvT+bJznhzuzMJmcNcxqwyBTHBpkHB0VPHKo14lSV08mz08qEOAc7Mxrdmc1s8qw1UuDc0mH3qhLU4lzsGgsdevYcTXDTON8F285SK+ahKZaIYQg04p5bVDQRQ264KppQ3+WlMFRpoRASFaxjY3xWGPxncdIEnroECARSClQAlIVsv6KRHBxv8Zah5ShpyyIUrAzq/ju2X2e3l2w6P57ohR1G0QTJQQXZzU/3llQW8e4bBnkmlGRUrcOrSSZDKJg2TrmbY3sHHZVG9xmWgqUkigBVSek+c49VzYWJWHUy+inKghntmFRGxoTes+UuuLY01KiZXA0hRjB8O+ZCFLLonEc/OoTUiKlx/ngFpxWhq1BSqoljXH8xY/HLBqD99AYS6Yl40XL3ryhlykskCnPmqpp9y4wl45eItgogsPw8DBno9CMLn+dE0/9S9Yvf/2mPkcWyV8mb+GT6Qf5oTtObSy5EJ0wGq6vkgIpYFTkyCRjRo/TTcpk3lKZ4PTEd2PAXx0Hukx8dARnngcUkGiJlsHNZ63FEbrDlj1w1nqs8IBFydBH59yV6FAtJa31tMaxlmukEF0UqeDyvF5FKAoRohYTKUmU6GI5Pf0sfDYHnSh28Pdyay1/+fQei9p2TtD8KifrMA8i7X5pULLFeZjVivGiJVGCItUoEboGy9aglaCXqPDZeYHo0nOTCikFD2318MCkNLe1Z3F7kPGDSzMud6vBb1TMOsjy9U9fXjDIG568MGWrn17TrVu1licvTO/a9iKRSCQSidw7ouP8/uMlIaABaKV42089xtt+6rF7vSuRSOQlihCCx0+M2OinPHlhyqjQKxv0uCyvaYM+OsrZ7KdkXcxUXKkZiUTuBLdzZflGBpPmLux05GXD9brIHtrsM8iCoNXPJNPKMKst86Z5zj0zUZJMhx6sI6OCR7aHvPe1h29o1eON3p8vzSpmlQlCCYKHNntsDzNObvbYGlwd53ZwMvm1U3uc3Quxf2VrSZXk0CBjc5CS6SsPjxMVxLB+ptnoJZStY78yK/cUwPbwynYKHQSgIpXYmScFWudZNBbnPPuVQXXHL6VEdxGHiQpinvUO2R2/86HTwDqPlBIHJCoIX0G0UFyYNjy81UMpyaw2VK3l3KTm3Ljk7KSiMY5Fa2mDzQglBf1UM60MF/YrjA1Ot2Vk44VJydFR0cUngvVgLEgF0ovVeV8rEurWUpsQryikZFQEYTHVIXJvlGuGRcIw02FyP6vZm3sWtcU4j+qcetZ5lAz9YqH7zWO7TrjGeFIlyRLJME8oG9t1p7lO7AHjQpQlhNW5O9OayaJBLXvufIgntN4zry2jfsKRvuZ4YUjMmKqpmS4ajFJkOmWjl7I90By99BVOfP1fMtj//o19aDoaEr6of5ZPyJ9jmh4NEZU+7N8yNtB5j5aKQZGh04IZBWcqzXjRULUhJtELUEE5xVu/8rwdFNH8gf+X3fWVkk5EtLQOnHcroY7uui6jMoUIglk/C3GIWgr2qxbhPXmmSbViLdc0NkR0Hh5ktM5zaJCRaRHiTp1n3lgWjaGXataLhAc2ejy01XvO7+VPfvMstQ1i8snN3jVjYLWUbPbT0IHWWE5dnqOlYFobMiUpMkkiFWVrqI1DCDqB+PmjS5edxRu94FDrZ+1t7UH2hMjXs+OSzX56S+8JQdTarAxnxyWjQnN6d8Grjgyf87rTu4u7ur1IJBKJRCL3hug4vz95yQhokUgkcrs4sV6w1U85vbsgT0oOD/NYxBmJRO4Zt3tlORZ2akFtbk/nS+Tlz/N1kW31U4a5Zmdak6iGURG6uZa9YUJAqiSLJvSHndzs84YH13njg+s3fd98vvvz7ryhNkGYEkJwdC3nZCegPV8s235lyHRwrYxnodMs04raOFrjOfhMXwix6lcWQjAqErKuCw2CIz3vxJ3uRQzzJIgQQoSIPRsEqtqEzi7V/fdECaQIAlLZhuOwztN2IouWEofvXEKhVyxPgtBkrEdYhxCCRW3w3jPIEw4PM56+PKcxjlltmFUtzod9XCsSNnopmZZ4H4S4/arl4rRhd9aQJUH4ujxv2eon9FPJUMMDmxlSpTTW0hgXou+cJ9V+VT7tgV6qsd4zyML/j4qEw2sZh4c51jnOjBe0q+MLjiiP78RC0ELQWLtyWtlO/GkF0Aa3W4i0DOJa3ToSrYL46H1wQCoRRBnvGZctrfFoJYKQmye8djvj4b5F2jk4w7hpsMax1c/QSiBtzbFnvsAbLv0+w+rcTY3VGT2+mP8cXy7ey0XTp2oNTW3Ik+DOCj1hIUpxWGTobMCMPpfr4NbDB2dinihqYamNx3b2M8eV7rLl+T6IFKAE5IkgSxR162g6V5r1gPNI4RFChq4014lNHlIpKHKNsx7fdZkhIO/OaZFqMuepWxs+V8JxaJhSJIoi0Vye1YzLlmOjnK1ByrFRwcNb/ef8XnbOszMPDkSAUXHtqMUDHz4GmebBzR47s4ZUN9StQwnZiX2a2jQsGkNtPAJ/VaTkkmd3Fv9E52797tn929aD/MrDA354ccZuFz17bJTf8Htdi2OjfCXQ5UnJo9sDpLxybM55zozLu7a9SCQSiUQi94boOL9/ue0C2s7uOPaQRSKR+548UbzqyJBHtweMy5Zp1TKvbbdKV9DPFMM8Yb1I4qQyEoncUW73yvJzu1OMhzPjihOHb/PORl62PF8XWaokx9cLjo1yZo2lbAx163B4nPVMqhYpBa8/MeLhrR7H1otbXul4rfvz3jw87O2lmqp1PH68z7H14poP0A/SWMfZccm0MlgPjxzqszsP5dtl65jVIcZwybLTLIhWoS9pOdmclC2pMuzOwyIb3Yl2a4XmmT0Y5UkQ5ZzHdC4wJQWtdUgpyZQCEbrRMA4vRIg17HqxvA9dWamSOOdJun6wIpEr0c16z6w2ZFpSNZZJ2VIbx3jRMq8NRaIY9RIyJUGEXqnGOPJUkSjJoNDMa8VEsXLH5VqyXxkECuPBOEEvFaRa49JwHipjmSw8Zec6ss5RW0c/0+SJRIogWK0VCUII9qvg8mtbCwRxTKkuhtE5jPMYE1xX3vuVu884D4Qer6a7tg6PtT7EWXLldeG4myBaesi0ZL2nwENfGY6mM4ZtTT0XPHyoR9tKhplmb9EwGe/yxp3P8rPzTzOwk5san1O9yR8l7+Nj9U+TqD6517TWhP3zntb4ENkooMhSyIZcNhmzSrJoLYLgGsu0oq90t3grRFMKoDUh0HPpMjs4wpUI5xEf/j7VEt1FMRoHjbXhNaH8DCHAh5OMc1BaC40nSeQqqnGznwDBtdcY243zILzV1uF86A8b5prWOXqZ4th6wVqhOTzIef0Da6wV6XN+L4/LFi3DQo5MhzF8IwzzhKoNjs992tUYH2aaTEvmjUGJ0B2YJVeE8xfqLL6dPcj9VGOsZ2/RMiqSF9WrBmHF+KhI2Fu0HB7mjMvQu7hkXLZ3dXuRSCQSiUTuDdFxfv9y2wW0j/zWP+Ltb349H/3Au3nn234SraLCGYlE7l+kDF0GceIYiUTuBXdiZfnZy/ssWji/X+Ocj4sAIjfMjXSRpVKgMo0SoSt0WhuUlLz6SP+2doUevD83xnWuiZZXHOpzYuPGeox2pjWttezOawa5ZnuQgQ8rMvNEcmlWsz3MUF1fVKpDzJ0SoWNpKQHmSXCsTevgZtuvzOp3Q3CXSbaHGZfndRCcGkvbiWPWObSUJFrS2hBBVxmPlI5MqVWsYWtDdCOETrE8USgJWaK66EVPIQWTMgiAvVTjgLIOEZMn1gs2O2dVEE6CA6qxjmnZsmNqjPVMqgZH6FbzQOM8yjpmtWdu4dKspm+uuHuWUYvbaxmHhxkXZw3eSRAwrw2NsawXKXVrEYT+sd15TdM6GusBgfWh3wwB1kukdDTWIoW4IiAKgCA2Cli5o3wnRoGncQItPc6FjjvnPMbCqNDkmWJDtWwmFbKtuHC5ZD8RbPYyvHNIJWC2w0/tfpK3zD5P7qubGo+z/km+d/xX+MP6DZzZt9RthXCeeW2QAkwnnGWJZq3IcOkal2rFuBRMyoZUh/OYyCB6Lb+Wi0QhALNowiKucGrxHlK97CgLnjTnPakUQVzrIjGLRGOcI089rnIYlnGN3Y53Dr/WOiweLaFqLCe3+gwyRW2CsJUqSWksVWOpWktjLLM6XNNL05phnvDao4MbjjWfVi2Zkhjn6WdBKFw5N1+A7UH32RKCVIXvmLq1gGdaWtZ7nYsPuDyrb6iz+Hb2IJ/aXWBd6H3cflZ07K0yyDTjssR5z7S6WtCaVu1d3V4kEolEIpG7T3Sc39/cdgHNWscTf/4Nnvjzb7C+NuRDP/ezfOQD7+KVDz9wuzcViUQikUgk8pLmTqwsX8s133cC43xcWR65Ke7HrtBbnUx677k8b5hWBg9sdl1Im4OM89Ma8FRtiJ08PAzvmWsVovFSybyyuOyKAD3IdHCuGYuuWjZ6wW21u2jppYo8SVjvJZzaLZnVFfPa0kuCeyrPg6AhhWcVguhDlKGzHuuCcCS7HrIiVWgVxBEpgmMJAOGDEOI8s8qGGEIpePhQn43ecx+sJwpoPKWgExJbGuNCN5cIMYnGOmoDrQHtCe41grBTpKpz5AW30jBPeGCzx1+fm7JoDc6zEoRa5zg3qWmMY2/RMK1aUi3xwmOdxDhHqhReepzlSmdZF+soAEuIJ3SuE/CER9A5qDxIHM4FAUkAvUxzcj1jM23p+V1sVXNxasCH/V80loumwu5d4EP1H/HW+qskmJsaf/vrr+N7J/42f5W+HuOgKhcs2hrTiZ6JhNJ4ikwzKnJaPeBik7E/s0wWJgiQXa9bIg8IWwdwhGvhvUSKMB5EF2lofYj1XHaZWRtceVpKUq2QnVgKoJRAOFbnpzOigQoOMNV1oK0VCalWrPcyRoXG++BI1FVLP9V47ylbg/PB4bc9yHjFVp/jnbP0RmLN57VFqnBd14uEeW2xfX/guj8PQrA9zMgTye48RJkuWsu0MszrlkQLzk7CyuxlDOYLfQ/dzu+2eW2pTIiwzZMXd89eUqQK76FsLfPaXvVvd3t7kUgkEolE7j7RcX5/c8c60LyHvcmU3/34H/G7H/8jXvPow/zyB9/Nz7/nZxj0b2zVaCQSiUQikcjLmTuxsryfaYwlriyP3DL3U1forU4mZ40NQlNt6adq5TJTUnBokHJ2XNJPE/bmQTToZ7pzpyQY55jXlmltVt1NqntQXzWWfhcl6bxnVhkODTLWe5peqilbR20s89qwX4Vo6J4Pwo8UEuNMF9kYHl5LCZmUgMd5QZEoMhUca6kO++zx1MZSNcFdZJ2jtR4hJetZck3xzHvPfmWoujjJsnUI77uoakmmr5wP60L/VW1D7KXSnkVrMM6x3ktJlWCYaVKtyBPJ4WHO6b05AEWm2B5mbPZTamPZnYXoSikFa4Vmv4Rahi6r1no8fiUkWQ/WOZwN6oV3YAkKUO0d7kAZmHMgdXBdDXPN8aHmaN6yoffYn1dM2nCsAFpJqtbykHmKj5jP8Gb7DeRzmsSenx8N3sS3j/wtTvVeQyoli8oyLhuMdaRKBrFVCo6u95FJxp7tcbaW7O211DYIiV0dWRDHHCCX0tYVrPeUtcE4yDQoLxA6iBtFomitI0lDx6ASPnSW+SCirSTIA4cmpUAgQt8cdI40gVCSYaZIlGKtSLuePL36XGz2UzZ6IT6xsY6yUcwqg1KSY6OCNz20zutPrN/wymXng/g5zBP6aRAzd+cN28Mbv88N84ReqpiUQdxr2hAbergT9F59dHjT30O347vNeX9FtHyBGNkbZfk+3nd9dQe429uLRCKRSCRy94mO8/ubOyagLX/bLX+P/fUPnuZ7P3ya//n/+L95z9vfzEc+8C7e9lOP3anNRyKRSCQSidz33ImV5cv3qVsXV5ZHbpn7pSv0VieTZWNw3tFaxyi/+u8GWRC7Mh3iAi/NaiCIz6NCM61ahplmvwp9Y8uH52knzHjvGZcNtXEMMhUEnfUQ87ZoDLOqZTxvKTEh+rEySGGwXuCdRXQRe1KCd57KWxIl6Scq9LApQaYktXFdB1kQzJQEgccRHoB7IM80qyf/B9ivDGVjWLSWprXgIU81CIf3wYHmPWghsARhzfml8G5IlMBqhfMNa7nueuRCX1ljHHvzGilDX1s/lSFq0YNxIVoxnM+EunV4LzpXlUSJLmISEN6jZXDitTZ8D7Y2uPN8F2cIIVIzTWC9l3EoswxEhW4XOAdTFcTIzlRH1VpeVX2Lf1d8jsf9929qrFkkX8t/hi/2P8SF5AF0JUmbEuPDKt5+ptjoJSAERZ5gVcE8G1H5lDOTBdO6OdDLJ2itxTqovMN6T+4UiZQhztKz6rYzzpMoQaZVFwkqGFeGWdc5B9DLFIs6uA4F4fzUxuIA2/WnAZ24Fs656US0PJEIIVnvpRSpCn/nFPuluepBihCCIlUUBKH0/H7Fei9le5jx4Gb/pj7nsrvOa13H4GY/ZWfW0EsV/ezGH0EoKdnsBxF3v27ZHmZsDzNe/8A6rzo8vKXvoRf73bY8NggC6O1g+T7BqXr1Nu/29iKRSCQSidx9ouP8/ua2C2jvettP8pW/+BbGhgtz8PeY99A0LZ/+4lf59Be/ypFDW/zS+9/JL33gnRw/sn27dyUSiUQikUjkvuZOrCxfPgxz3UPxSOTFcK+7Qm91Mlm3QXTyHhJ99Wcr7USxVAehygMXpzWD1rLZS9jspzgf3Fj7ZQuEh+5ahR6q3UVDUkmOr+dsDzI2+glb3fk5spbzyu0BZ8YljREkSiKlwBpH20XzaRHcVg6PFpJEC7SSoaOqE1ZmdYgaVFKQKkErJVKCsZZeoihbh171tXnSA8dYNsGNtWgtxrggzAhH2VpSLRBCUzaWpZnPOc+0dUgPxgISxosWKQ1KCC50bhwhwDiPd55F6xEYrPOc3ispEk3a9by11tMah5ZQtg4pgzCWqiBCejqhrdu2c8GpJSCIizi8EF0XnGCrn7GVtuR2wmw+Z7dp0UKwNUipTehKs8bwVvs1fsV/lkc4w80Yziqf8sfiZ/iUfj+V3makEnCOi9MarQS9VHFivcehQY7WmiZZ4wf7ijP7LfuTGkQbetCsR4puzCmBcQLTiVnz2mBs6MOTIghyQggguP9UJ16t5ZrdeRtSPh3ozqknAK3C+YHgakt0cA8a68P/uysOt6UHbdnr18sUg0yv+sgWrUVVbYg2vca9p2wstXGsFwn9TLFe3Fh/2ZJ+pigSRaIlg0yjK0PZWi5Nr4jVN8q8NuzMGgZpwiCDNz+8yVse3uChrf5zXuu66OIbEcVu9btteWxCQNU6erfhq7Fs7Mr91s+udtDd7e1FIpFIJBK5+0TH+f3NbRfQ/vF/+w/Zm+zzyc/+KX/wuSf4wY9OA+F3+bNdaecvXeaf/e7H+ee/+2/4qde/lo9+8F289x1vIUujpTASiUQikcjLnzuxsnz541gi4sryyEueW51MOq7/d8vPxWY/DX1HWpMnht15zbw29FO1erhsXehSS5RAEhxxgyzh0HrG9jBno59wcjPE07fWcXG/5nsXpngPmRZgl9GFQSyRnftKSkGhQn9YcB1JhnlCouWqxEqJ4Apa1MERJgQYIUmUpGpDb5r3ntZZ0tB4hXOOaW1oTIhu7KU6nEMTxIVUS5SUGBUiKK0PIl3dWoyHSd2y0ctCD1xt8UrinaPp4h2tC0difRCuGus5vbvg5EYPgWaY6dCjJmCQKXamobvOORDK0TqBc8FNt3KjeYfqrosHjA/OpY1Cciy35HaP8WzBpUVN021fJRItBIU0vLX5Mr9gP8Nhf/mmxtaUPp8U7+YT4l3YdA3nIfee3XkTXuA9+6VjkKWkaYrobVImA2amZWGm7C1Cp9zS0ecAPPTSIFbVJghGpjtX1oWRmSiJCU8ykAK0lAxzjfXQWDrhMFzPxnkSGTotvafrxlMIQjee95BIQdkKrAvn0nkRutOATHWuskQhRHC5Oe+pWkc/hdI4imtEHl6Y1uguhvORWyidH+ZJdxyhR2+zl+K95xJ1EKsby2Y/fd5ONOvCtZjVJog83pOnmu1BxjC/WtCrWsvp3QVnxiXG+jsaOXvw2G5XHNKsNuTdPj772O729iKRSCQSidx9ouP8/uaORDhujNb4zV/9EL/5qx/ir3/wP+tbngAAIABJREFUNL//6S/xR3/yVfanISv/2a40j+dr3/ouX/vWd/kf/7f/iw+++2380vvfxeOvffRO7F4kEolEIpHIfcGdWFletQ6ALJFxZXnkJc+tTiYlV//dwUnPSmQWguOjgl6mQydaJplWhlkdYhrLzsXmnGNcW7wPAk8/U+Sp5MhazqjQ7M7CQ/5Tuwue3plTtQalBPuVWwlvSoXYxhDBR+c+gtZYlJIoD9O6JTGCQapJlCLTklRJWmMRQjEuW9IkxPcpGVxIoUfsyrHNG4vrogGXPWqLxuC4csxShGg8YyxieU6FQPpQ07WMjmytY1EbtJIUqWarn3axg657jUfLLi62sWSJojSO1oT/joD1XkplLMY5qtaTaItE0DhQ3bUIPWHh/AwyxVoq2NQ12i6ws4bzdUNrHG0nnkngcFLzy+YLvKf+HGt+elNj6rLc4o+z9/M5foa9NkRgFkquxkgiBI1zCKnYWh/Q5CN+1AyZzDMGuSfTEo8gU6Hby3mPEoJECjwiHIsUrPcytJTszBqclljrkELQWAcWlBJoOieZ9yGusKe73i9Ba4JIuqhN6KYTQTwLPXBJEDKdp3UOhwE8s9qFcUZwNSYq3AMSHc5vogTWSWpjujhO+xwBbb9s2Zs3nNzskSea1x1bu6nzC7BeJGgl2OglnJ9UvPbosBtmgmnSsjtvmNeGXncPTLVEiuDwbExwSy5qixRwaJDSSxV7i5bXHBmglbjKEXdmXPLkhSl1G3rW9hZtF7V6ZX+ECC7S0PNmeWZc8uojQ06sFy/62Frrbrib8Vq01jEpW46O8ucc273YXiQSiUQikbtPdJzf39yxDrQlr33lw7z2lQ/zn//93+BPvvp1PvHpL/GVr/0VzrlrutJm85KPfeoLfOxTX+ChB47x0Q++mw+/9x1srt/8D/dIJBKJRCKR+5k7sbJ8Xhu0Iq4sv8vcTHRY5AovdN6KRN7SZDJLgvgkBLTGczAxrjFhHpIqSZZItvopw1yzM61JVMOo6Lq+bOgv21s0CGBcNiHaUIRoxgv7FRf2ATz7leHyrEYIWDQO73xwY2lJZUIvmPECDbQuRBjazlWEtSy8JVFi5S4bFQnOK8aLhqaLBlQyCCimE7G6BEB8J45576laS21D59lSGPGeVaThlbmXx1iHlAIlBTqYxpDdPjjvSaREJIJ+qsgTRZZobBdDqKTtXHaSVAnmjcF5KFKJsUEE8YR/h+Cwa3yIBdQybENJgURQpJLNfsJ64kjsnHY+ZX9S40XYcetCPKIQcExO+BX5J3zYfIXcNDc11n7McT7b+xDfyN/KwohusYFlWcqW6NDHphNNnveoxIAdo7m8Z+ilJQvjec3RIWVruwhFiZYS7yHVgtYGQapUwR2mZYgK7aWK1jnqrniuSDS+i3Yc5JqtXko/U1TGs1YkjIRgs59wZq9cRWDWdRAojffkQoXIy6DEokTYj7pzt4lOPG6tx3kHhM/C0oWmVdhn43zonDvAvDb86PKcXqo4Osp400Mb9G4ibnGJlMHpVbWWC/s15/drTm716GeKs5Pw+Z5WhlllWTTNc8SuREo2+gnDXK9EwCNriq1Bxon1AimDk/E75/Y5P6m4PG84Oy7x3jMqErYHGXkSojFt57ibVi3nJxUX9muOrxdY69mbNzx2fG0laN/KsZ2bVCsX6q1wblIhRIiTXB7bvdxeJBKJRCKRu090nN/f3HEBbbUhrXnfO9/K+975VnZ2x3zys0/wic9+madPnwOe60oDePr0Of6Xf/57/K//4l/xs295Ax/5wLt450//JOpFrLiKRCKRSCQSuV+4EyvL9ytDT3q0jCvL7wZ3Mzrs5cSNnreyNezNW7QUNzWZLFKN6ISusjUM8ivTnrK1QRzqHD0QxLTj6wXHRjmzxlI2hrp1uFEQcBadw+zYmuf4esHxjYJ+qhECLu7XTMu2c68ZDg8y8jRE5Z0Zl6RKMm0NrXWIROIIvVXGHewp9DRGoJQjMZKmDc40KUJE36Jx9HONdZ3ryDqUERjnwIdjaK3D+SAY6s7RA0uhpduKD/GWpnN+eedJlSRVCutNJ8CEWMdeP6HT4igSjRSADO6lYaaRQOt853QKotu0NHhAKVb9cUpKrAvuK+891nrAoZXi8DDjaGYZyBnlbMal2YKqcat9t12E50lxgd9Qn+e98msk4uZK0L/hHuFf+/fynfT1DERCH4XHXfUarSXr/Ryre1wyGeMqXKdEQmMs4JlUbfjfIhwXAo6sZZSNZVa3KxGmbi3WOqpO5Gy9wxi3ijNsTYjOTHU4/kxJjo4KJmXL8fUCrSRn9kq2hzlPXZrSWE+WKPppuAbGOWbV1fuvROgIzLRk0VgSLfAEwTLT4Zr20jBO5IGxsBRfrXPsLlp2pjXee16xPeDwMOctD23c1Lk+yIObPZ4ZlxxfLzi9u2At12wNMtaKhEvTmvRZYvXys592/XC66yhLlODMuOLBzR5ZoniwE4++c26fc+OSU7sL9hYtW/2Uo6P8mvfQXhoiW1vrODepOL27YFa1+O7z9/iJ0Ys+tvVbWCo+XjTszpvnHNu93l4kEolEIpG7S3Sc39/cNQHtIIc21/m7v/aL/N1f+0W+/b0f8m/++Et85kt/xnS+AJ4rphlr+dKffZ0v/dnXWR+t8YvvfQe/9IF38sjJE/di9yORSCQSiURuC3dqZXkvgaNrWVxZfoe529FhLxdu5ryNCs2lWcV+adhbBIHhRiaTgzRE3Q2yEP226Vwn5HgWtWWjn6CloP8sd40QgmEWurwO0nb9X2tFwqined2x8MB9Z1YzXjRMa0MiYaOXcnKzh/OenVnDKDecGZdYFyIRjbsifMiu48x38X10PWkeqI0H2wJBfMq0pGoMMtO4TkCDLppFLvvDghjhvCeT8sB2gtMLuk45B3iPcY5ML11q/sA+wXqRkmoZHFWtxToXOrqMI9HBPZZoSdH1c+WJIpGCyjj2Fg2pFOzXBimCy1BKyJSkFQKtYFQojqSGodjDzEou1S21dRgTjn/ZffcT4kf8hv4871DffuGB9Sy+6h/n9+x7+bZ7mCSBJNSOBQdi95pMK3pFTtZbYz/ps7twnN2rQMBakZCmkjxVzGuDdY5ndhcUiWZaG7Z6Kc4HQTO1illtaawjQaJliPuULONEu+hOYK3QpFrgXIjfPDTK8ASH4byxpCqcg+AmVuSEaMN+qlbj9WBsp5JhHDXGYZ2j6OIOnYNeEsSo1npmtSHtPjvWe6xzlLXlkq+YN5a6DcLk8fWCh7Z6vP91R16U2J8nilcfGWKtZ1a1nNoNc/31Xsrx9YKjo5x5bShbG8Tqzn2ada7TfqbZL8PfbfQStvoprz4yJE8UZ8Yl5ycVp3YXTMqWh7d6NyQoJUpycrPHWq45tbvg1O4CIQQbnRvrdhzbjTJeNNc8tvthe5FIJBKJRO4u0XF+f3NPBLSDPPaaR3nsNY/yX/ynv8nnn/gLPvHZJ/jzr38b5/01Ix73xvv89sf+kN/+2B/yulc9wkd//t184N1vY9D7m/sQIhKJRCKRyEuX272y/Ohaxr6AE+v5HdjbCHDPosNe6tzKebu4X7M3D+6e8bzma6f2+OlXbCJ4/vMmhGCrn9Jay3jRsrto2R5k7M4bhIBhrtnspzdcqH1uUiGl4MHNgke3B7zqyJCqtVya1UxKQ9mEvqrNfrYSOarWMUkUiZbMarNy2iVKgACBREnAC6wP0YbOg7MW68ALj+gcQss+NoQIDicXxDhdh/PVGo91Yf4UBKsrApqSIdJPSoGxDgcYF8Qc3Qlgns6d5ll1pwFIKfHOUjrHUrcsEkXZGJwDobq4QGNpEGz2NN4n7MxqWuOCEIinn2p6fc0o9QxEha/HzPcrzrUGJYN7LTjygpj3Nvldfl1/njfIp25ihIFB8UXxFn7PvodnxFEsHiFBibDzxjmUhbV+Rr+XsWNyLroUu5B4Ea5j3YmcddcjlynF3BkWjaE1nq1BOFdaCuZt6JYI55LVeW+dwx5ImHR4ekqylmsODVOKRKOl4OK04fK8obYOCcxqy3ovIVGSw2sZRaa4NK0pG8sw16wVaSd+BbFUiBDBmUhJogTjRcveolld90Qrtocpgzyhahy1MdRtEEUlnVzbibiJEqwVKT95cp3Hj494YOPFu5NOrBfszRu896Ej8PKCzcpwrHOKDfPkmpFCrXU8s1eyO2/Y6CWc3OxxdJSvHiw9eWHK5U58v1Hx7CDL1z99ecEgb3jywpStfnpTgtILHdv1WLrgrnVs99P2IpFIJBKJ3F2i4/z+5Z4LaEvSJOHn3/N2fv49b+fizi6f+MyX+YPPPsHpsxeAa0c8fuf7T/Gd7z/F//S//zbvfcdb+MgH3s1b3vgT92DvI5FIJBKJRG6N272yfCODQ5lfdQ9Fbj/3MjrspcytnrfTuwu+dWaCB87ulXw7m/D48fUX3N6hYcblecNmP2NnVoP3zGrLoUFKohTbw+yG9vt6k9DTuwvKxvDDSzOkFGRSXRUxmSUSROgQGy8ACd7SdZqBlA5ngxQYRLDgAHIepAThQeBRSqI6YawxlsaFqEbnPa1xlBjKxnT+tdB95YFUB/cR3tO64Lpabts6t3JFtdahpMASRKHigIggBSxrshrjOvHMMikNWgmkCWLlonEMckXjugg+lt1qnmGR8PBIs6UbXDVld7ZgXgchxwuB7frSFJb3iq/z7+vP84g8f0PXZklJxhf0O/mEeA/n7IgKA87T1YQBkEpJL03p9YfUSZ9zM8kz+xXWVmRaUiSaxtogVHqolUPVFo+ndZ79hWVYCParIB7OGktjQkyilBKtPH0ERaYZpApEF7dpHLParHottoc5a3lCL1VkiaI2wYG17Mt7oItxVFIwWTT0EsWFac2isUC76vfTKnQDhsQWR9m6VdxkL5VkOrgse4nGWeilGiVh7IPQ18s0wzzBdTGcr9zu8+jhISc3ezx2/Pb1jy/fSwjBIA/C+XjRMCoSBpmmSNVKOA9xmIZJGUTzBzd7q++J5fuc3l1Qt5az45LNfnpLD5Yg3GM3K8PZccmo0JzeXfCqI8N7emz32/YikUgkEoncPaLj/P7lvhHQDnL40CZ/79c/yt/79Y/yjW8/ye9/+kt85st/zqKsgOeKaXXT8qkvfIVPfeErHD18iI+8/138x3/nl+/R3kcikUgkEoncHLdzZXkhDTsvvnM4ch3udXTYS5UXc94e2R4gBHzjmQmNdfzgwpx+mvCKQ/3n/dtlr5l1nr15zVM7c46t5QzzhOMv8Nlacr1JqHOh3+zMXol1HiXDpFd18SjWOfbmDakSWOdJVIiPtDa4xDxgrF91UB2Mr/QAbukg6uL/fOjSck0Qm4wLf9BYR6oVrXPUrcUFwxfee9JEkUqJ1hJng8hSG4tAYHyIDKxtENZSKbBd/9RBV57zYL1DCUFjHQJBu4yQ7A5EiCCuheOGfqYYZJpBrliTDUMxh7Ji6ix00YzB+yTwzpNR82H1Z/xt+SccEXsveE2uuj4M+ATv5k+S99CkA1rj8PaKECmANFFsDgrIhoxtxjMLTd069sqKuuspA2hdS2McprtGtRXQGBDBQVZZi6qDM22YJ9Q2iGOplvRTxbyGrCdJVIgetd11sM6T6hAFmSYSfIizXMsTRkXK05dn9NZCn95SmHz08CCIcMBXnrpMYxwToEgVjQlOsmdHniohGBSaPJHMGstmL+XwWkaiJNPKMK8ttbEsGkOeKqSA7WHG0bWCBzYK8lTdkXhZIQSPnxix0U958sKUUaFX0a3jsrxmdOvRUc5mPyVLrt6n5edut7tfHhu9OKf1sVG+EsjzpOTR7cFNRRzdzmO7H7cXiUQikUjk7hId5/cn96WAdpA3PvZq3vjYq/kv/7P/gM99+c/5/c98ma9967urkuFnRzyeu7DDP/2dj0UBLRKJRCKRyEuK27Wy/Eju+M49PpaXK/dLdNhLjdtx3l5xaMCitnzvwhQEfPOZMc57Tm72nncyuZZramOxzrNeJBjnqY1l7QWKtF9oEjouW4z1XJjWFFpSdu6sJZPSYKzl/H6FcVAkmkVj0SrE5QkAEbqtPASRxgXxbPn4XivopQo8zBuDEkEwCy8XKBnmQK21oedMCFprMS5EFSaduKMbgVIhttET3sN5jyBEJw4yDd6TyOBAO4hzLnSuOUdtPdaFmMNEghSSfhH6vqQU9DLFepGwlkpGssKWE+qyZG6DYws8jQ3Rg43xDPyUv6We4JflE4zE/CZGA1xgi/+Pn+OP/VtpRUbqJT1/9dww1YrRoEeb9LnsCyYLz97CIDFYFwRFjw+OPQ9ah6a4ZQ+cFoJMKyprcS4IYWV39r0P4mYv1aRaMu+EtkyH7q5+dmV8lY3BOM/2IKNIFfPGwqwGITg0zFjLU15xqMessTx8SHF6d4G1DiHCVP3hrT5aCZ48P8V52Bpk+C7ycjkn1jIIra2xOAmPHx8wKhI2+ynTyjAqUrz3nJtUFKnigY2CBzd6PLDRQ6vQufHgZu+Ofg+dWC/Y6qec3l2QJyWHhznOe8qu/1CIEA8qhbjuPi0/d3uLllGR3JAI/nwkSjIqEvYWLYeHOeOyvcpFejeP7X7eXiQSiUQikbtHdJzff9z3AtqSPEv58PvewYff9w7OXdjhE5/5En/w2Sc4e2HnmkJaJBKJRCKRyEuJ27WyfGd3fO8O4mXO/RQd9lLidp231x1fY9YYzk8q1nsJp3dDFOALTSZ7qebRIwOcCz1geM93z+0/79+NFy21dawXCVIIFq1FAD++PGeYJ0zKBuscs8qQKMWidaveMO9D7MrFWUPdWhrjqFpHoiSCIHxYF6Qy0b3+4BRGAEqCkpLG+q7DTGBdiHTUUqA6R5vzsF+Z8N868Ut4Vi41YRxGCLQXXQeax9j/n713D5YkO8g7f+ecfNbjvvo9Mz0z0khCQgghJCRA0kgaGMEKSV5AmNiw14tZv9YmwDZhDF7MOiAwNhCYXbO7XofDG0QsIdjF7GKJh/VGL0AIEBKSRiMGafp9+/atW/dWVT7PY/84WdXd0/fe7tvT3dMzOr+I6Z6urMrKOpl5ojK/+r7PYhwYY+ilEZGUSOGoK6iNhUYjJURCUWtL1Rp05zqrAaUkkZKkkcJaaKwlVoLDueRkryZ1BRebGae3pyjhowhrrb0jTMCKvsR3iQ/x7fEnyEXDQXjC3cu7okf5pHoFjVPUrcZaizK+301JQRorer0elexzzmbsTAy1bn1UprXYrvMrUqLrfPOiQiSh9cmPKAGtdWjniISPtSwaH7WIEEihSeKEJJI02tJqSy9RSOkjO6+k6bZLCMFKL8Fax8VJTRZrrPO9eEpKTq6mWHttZM88ivSBQwM2JhXLWYRSohP+fA9arATaWnZKx0p3jp1czTk0SLHOMas16zsVmzPJfatDDg1Tvun5hzg8SP0xfoeK5bNY8cJjQx46MmBctkyqllltsM4hhaCfKoZZvOc2TaoWY/0xeWRwYxGs12OQRozLEusck+rmBDR4+p/tbn+/QCAQCAQCd4bgOL/7eNYIaFdy4thh/vZf+06+5sUv4Of/3f/F6XPrV8U6fiVjreXc+iXOXthgfWOTaVFSVTVxHDHs9zh6eI2vfuHzWFm+dTdpLo3GfP6LX2Zza8zW9oR+L+fw6jIPnDzBQw/cd8veJxAIBAKBrwTCL8vvTu6W6DBr3bPqZumtHDchBF9//yqf+NIm1sGwF3FsKWVc6hu6mFzKYnaqlro1e16EGufFLmcdvVRRtoY8UTgHf7ExXZx758YlZWtojV0IJvPow0obprVhWmla63wsoPWCTat9L5a1/r2gi2zsRC+/8fMuM4u1AiMF1voYwblIF0nvXjPWYYFGO6RwSCkQ0q/fWbc4PqwTRFJ0kYJgmcdIWkptGCQSDdTaYJFIoDWa7ar1DjRjMRaSSCDxvWjWOZJIsJY6Ujsjrwo2CksiBbV2RNJHG+5UGoD7zBm+R36QN6o/RQl7oH3/p/YF/Kp+E5+JXsxQJgySGGkMrRFUBmpjGKqYYb/Ppulxrom4tF3T6IqocyklkQRL5wD04xFHqoundBhrkVKg8MKk1pZGagyi2+8GpQRla3GxH8tZ7R1RcSRJIsUwjZDysivKWkutLf3URybmke/FG7SG0awmUill42Mkjy/5uX63yJ55FGnVRuzUmiODlOXcX8ob6xjNGqa1oZ9GHBmkrPUSDnUCkxQ+RrRoDC88OuCBQ31ecs/SDd9YuR1zjpSCtX5yYLFqVhsqbXEOsvjW9HzOz++yNcxq87TXd7Of7dnyfoFAIBAIBO4M4b7A3cOzTkA7fW6dd7/3I/z2Bz7Oxc3R4vH5gfOVhjGWzzz2F3z8k5/m05//Io998cvMuq64/Xjogfv4K9/2Bt7+5tfT7x1clXbO8Z/f82F+8z0f5s8fewK3h/Xv5D3HePTh1/A33vGWm3qfQCAQCAS+Egm/LL/7eKajw6rWcHpUcHZcoo171lw83Y5xu2+1x7TWrPYSlvKEY0v5DY/HfBx3uwgdlw2b04Y8hqIxlK0li2Bz6h+Hy8Jc2WiKxrAxqZFDL1TY7vtw2Rh2qpaqNVSNX7exrusQ6yIahUM473bqasu8Gw3/hwWcdhjhz3klBbGUxMo70Rpj8ae+X8FcszFdN9rim7nzTjRjHJXw7wcgu8+irXfdNa2hNVC1lta0tNZRt4bWuO41vsctiyOW8ojDvYSVRJPrCdNixta0ZKoEgzSmlYLWeJED5/hq9wRvc+/h1dHnD7SvrRN81L2Md+o38Zi7H4BIQyUNq/0EhyRTiiyJEFHORPW5UKfslJpZXVNqL0xZB5GSGOs72iLlxdgsUfTiiNpYYmfR1jvUvFPQC5hFa4mlwHrdy+8LJXAOZrWPbVzKYnqxIosVeXL15fWk8YJML/Zz9vyCda0XM6s1W7MGbR1pJOmnivvXet1xdm1kj5Q+klQby9lx6XvVIknV+mPh8CBhmMWs9RJOrvnrrqfTh3E3zjl20aHnO99uBfP1OHf5HA4EAoFAIBC4Gwj3Be4OnhUCWlFWvPfDf8i73/dRPv35LwJc8wvTKxHi1vwa7dnA3/vRn+FTn338wK974skz/MK//xV+5f/9HX78h76fb/z6l93wa7906hw/9Yv/gc889sR1n3v63Dr/8Vf/M+9+70f4pz/w3/Hwa15x4G0NBAKBQOArlfDL8ruHZzI67Oy45PH1yVXOqaq7kT1nLuys9mKq1nBmXN4V8R23b9xaji9nvPDYgGEac3Zccmladw4ShxKCw8OEe1d7rPWSxQXlbheh00rzxYtTnPWiwLiwDNOIlZ4XJLJYLiIeq9YyqVrOjBpGRUNrLOOypdKWQ21MGim2ipbWWGa1QQhHZRyNMYt+MSkB18llnXpmuXx90+lOXmxz/o9MSZzwc4LA0bQObUFKSS/xghXOYYUXiebrmF8VmW7F83jIyz8+9NtguhjJudOt0dY74LptSpRkmMcc7UXcP7AkZkQ5K9luWprWEiuFkl6wwQis1rzCfJp3lO/nRe5Ll4vdboAWxQfcN/Br+o2cckdw+M/h8OPUGsulSc2hYU6cD9jQGRcLxXTWokSLlJf73qyFSDoiCdpc/uxZJImV9J1yDrTzQmESycV+EEJQtxaVKsrWoqQXHJXwUZgWwyCNiaQgTyKWs6svrecC6lIWo6RkKb+8XHXuvIuTmpU8oWwtwyzeN7LHWsdOram060TpikgKVnsJq72EPFYcG6Ys9+LOkXbzfRh365wjhVhc+5tbJHbN1zMXSAOBQCAQCATuNsJ9gWeWu1pA++SffZ53vffDfPDjf0zd+F99Xr6gufy8+WMnTxzlrY++nu/4ltfe4S195qjrg/UGPJX1jRH/8Cd+gX/5o3+fR173Ddd9/l+eOsvf+6c/w9b25EDvc3Fzix/5qf+Fn/wnf5c3v+Ebb3ZzA4FAIBAIBJ4Rnhod5pxj2hjKRlO3FotDIkhjSZ5EDBKFuM7N2OtFh1nr+Nz5HS5sV2zOvBvFOcdyHnNkkO4q7FzYrljfqX3km3FszRpees/SdbfldnE7I9d2qpYvnJ+QJWrhkHF4h8q00Zgdx8ak2dUhc+VF6J+f3aafKDanPubu+FLKMI87EUwzqa/et/ev9YiV4M/P7rC+XaNNixSC8zsVwzRiq2gYFw2Ntljn4xtd5zab940Zi7+gcQ4nHBIvDs330lO1AeMcSkgiISit7T6DF4QiAUYILAJhLapbZu1lZ5vsOqNtl90YKYFEIIVDu66NrXPgRPjjWwlJFsEgi1nLJWuqJGpHzLYMU+xiQ03XJ5YoRS4NLy8+zneY93GS9QPt14KM94jX8Zs8zIYb0ngLGxIBwmGcdwsN8ozeYIlpPGBH+/He7mIikY5MRUTKYpwfzVgplJA0Ti9cfkoKmtbi8K49bS2RtwYSKYGz/liSUlC1BiWEF+EcJFJ2dkGB6fbFUqauukCtWu9CzGJJnijW+imRvPr4j5VkWmvuXclpjWEljxfL9ovsGc0a1rd94sis0ZSNne8N1ic165P6pvsw7vY5p58q8lghhHdL3mSd4lWUjVk46vrpM+/aDQQCgUAgEAjcXdx1AtrZCxu8+30f4bff/zEubGwCu7vN5o/lWcojr30Vb3v09Xz9y158h7f2uYGxlh//2X/HOx88yQP3Hd/zeZtb2/wPP/avDyyeXfk+P/Hz/56V5SGv/rqX3uzmBgKBQCAQCNxx5tFh2lou7tRMao2xvq+o6eLqhPBOHdFF7h3qJxwepiR7xBZeLzrsc+d3OD8uOTUq2CrahYNktxjEXgJr/WQR2XZ6VDCt2kXM9tfcu3wLR+PGuV2Ra5Oq5fH1KYcHCYM0OrBDZt7r9MWLEz53doez44LtSrOcRVzYsWzO/I/U9tq3eSw5NEg4UaWc2ipJleT0qGRrWrM5axl1AtrNGxYdAAAgAElEQVTlSEaHQmCdxXbCjsMLXQLZdZm5hYAm5RU/HMQ7n6yzvses6+8CSOeRecb4bi8piIXAOGi7jjU5XwkQK7HoAHM4hJRE1tFah8FHV8aRI4skq4OUw4llNaqw9YyNcUGjfcRhP5EoJWmNl+gGouaNzcf5dv1+1tz4QPtz5Ib8pnuY/yJfS+nmEYYQRQ5rBdr6+MiVPEWkA7ZdzqmJpNI1sdJIIZA44kh0wqrGAYny+ypSgtpYrHUIAUoqWuv/ba7oiZNCIJxFW7FwJWWRoNKW1jiE8BGakZRoa3HOd83V2nJ+u2aYRWSxouicZ1ksWc5iBplimF172V00utuHkqX02tid/SJ7tLFsly07VUsa+WPgVsQr3u1zzjCLkUKQxWpf1+5BmNaarBuvYRZf/wWBQCAQCAQCga8o7goBrapq3vfRP+Jd7/0In/rsF4C9Ixrnj7/sxQ/x9jc/zKMPv4Ze/vRK3J9rHD28xmte8VJOHDvMsN/jwsYmH/mDP+XUub1/Bdpqzb/9j7/Gz//ED+35nF/8D+9ktLW967I8S/m2N34jzzt5D5vjHd7zoT9YCKBXYozhX/3SL/Or//tPk8ThAiUQCAQCgcCzAykE47Lh7FZJayyNtkxrc7nrqUMI7ywZpIrWGDZnDfd0bpKnsl902NlxyYXtilOjgu2y5cFDPVZuwG4RK8n9az2WsohTo4JTowIhBKv95BmJc7zVkWvWOb48mnFp2jDMIqaV5vAguWGHTNkYPn16TBZLytby+fM7XJo0nN4qiBRMSkWlDY12xEqQxxGqEzau3LeDNOLcdkkcSay1nJvWGOu4BGhjqRtL2wk2c7RxXvgStusqE6h5NmFnjZo/XwnhxTfhP7MX2KARFim92yyJJImU1MaipMA6RyKl3yZ3WYxz+LhHcAi8W2y+b9w8K9L59fcTxVo/4p7MsaJ2KIuCqTGLY1QK/6O4SkMC9MwOb7G/x5vbDzOgPNC+POsO85/cm3g/r8KIFIl3BkZSIBBoK7DAaprQqiEjm7ExsRRNixTQS/y+EYCQ0Bg/VkqKbkwFaaSotUUbL2a2xhE77/WbO/P8OMz76LzgK4V3qbXa4pw/hlvjcNYhEj8OrfEOMPAutqrRaOfIk4jD/ZQ8UQwytWt06az2HXrDNEJJydGlva9n94vsmQvBt6IP49kw56zkMZESrPZiLmxXtMY+rV7FthMijy9nREpc5QIMBAKBQCAQCATgGRbQ/uQzj/Gu936ED37sk5R1Dewf0Xh4bZn/6pHX8vZHH97XKfWViJKSN732Vfy17/x2vubFD12z/Ae//3v55f/nt/jffvnX91zHR//oz9iZzFga9q9Z9qnPPs7vfvD3d33d2uoy/8e//jEevO/E4rG/9d/8FX7on/88f7pLP9vpc+v8ym/8Ln/ze992Ix8tEAgEAoFA4BnFWsfZccHGTk3RGJ68VJAlin6iWM5S4kgsRJtWO8pWs1W0jIuWtX6KsY5p3XL/Wq+7be/ZKzqsag2Pr0/Y7LqHbvRG9pXMn//lzYJB1vD4+oRD/eSGXCi3klsduXZmVLK+XbFdNjjneOhon5ecWLohh8znzu1Qa8NKz/dWzRrD+rjiydEMC8RSUjYlDt+RlScRjbas9mLfT9U5yOb7du5q26la6tbQmLkw5h1nc+Si7szRWkA4ZOdKk1bMkxyveL4AcVlYdcYLYEp6IS1WwsdBCoFSggQv4jkpiCPpnW2ic7cJL0bFylFrvz4lBNpdjjhUAlZyHzu6FmlivY2dNGwCzjnSbv9lkXfKtcayotf5bv0hHuETpLQH2oeP2ZP8mnkTn4xejpQRbt4FB4vzo5cosjRnJvucK2M2JpZpF10/H6+yNbTGdeIhC1dc3RpaDXmqaLWl1sZHZtI5zeSieg7X7S8vwgkkEiEc2jra1nsCXfd+eSSRUtCLFcaCdV5IL1tDax2NkQzSiFgKtLUcGuQs7eJomtWajUlNHiuUlJxYzm76vLzZPoynCm9Va/jM2W1mtWZz1vDiY8O7cs6R0jvqqtawvlNzfrvi/rXeTa/v/HaFEH4M713Jb1hsDAQCgUAgEAh85XDHBbQLFzd59/s+ym+9/6OcW98A9nebRUrxuld/HW979PW89hu+FilvTXfCc4lveuXL+OG/+9f3FRWllPzN730bFy5u8hu/88Fdn2OM4U8+8xhv/OZXXrPsP/32B/Zc9w99//deJZ6Bd6T9xD/+27zj7/woxlzb6fEbv/1Bvu+vvvUZ6+MIBAKBQCAQuFE+d36HSam5NK2Z1ZqlPObkao56yvfSCEgjGGQRa9YyKlouTWuqVuOspWg0h/qp70xzjgs7FQ5/Q72fXv5afnpUULeGc+OStX5y4BvZc1Z6CWuV5ty4ZDmPOD0qeOGx4dMYiYNzKyPXNqc1o6Lh/HaFsXBsKeP5R4bXdaD42EOHFLAxqTk7LlnOYqSAShuSSBJJyaRqEdK7vyptKdqGNJaUjaWfapbzGNUJKJuzhnNbBeOqpWoMtTZESqEktNqCcyiBF8JgIcKorofMdG4zK9xCXJsjhZeRbLfNV0bYW7xTSnTOPmt9B5kXybwzygHa+udlyjvZjAGEd5/FkSTGi06recLh1BKbGW0xZjYzWGuRErIootPyAFBK8EJ5lu8w7+F17lMocTBH4Sfti3infoRP8wIcgtgJYuFdeVIIGuPddcNehkmGnNUp57c0W+XlzucrO91iIeglCtFlVPrIRkksBaU01K3p4h9915sQXgjsxQrTufpALNappBcXLQ5pHLXzgmikJKLrQ5MCEqUQkSONJNPaizr9RJElCmv9nuwlilob4LKAZqxjNGuY1pp+qsgiSWMc967kd6x7q2oNp0cFZ8flojewbA3nxxUbU+/U7CcRZ8YlZWv2jaDdjTsx55xc63FmXHLPSs7pUcFSFt3UHDkuGkazhpNrPdJYcfJpCHGBQCAQCAQCgecud0RAq+qGD3zsj3j3+z7Kn3z6sUU0xpzd3GYPPXAvb3v09bzlkdeysnxnL/SfTfzoD3wfX/2i593w8//G93zHngIawMXNrWsemxUlH/r4H+/6/H6e8a0Pv3rXZfedOMorX/ZiPvGpz16z7MLGJn/86cd41ctfcoNbHggEAoFAIHDnmceajWY1ZWu4dzWn9jaifV+npOTIICVRglOjgvPbFcMs5tCgIY0k2jjOjUuODFO+vFmwcmab+1Zz7lvJOTsuGc28w+rE8tOLKj+xnC1uFGdxyUNHBnfUZXGrItdaYzm3XTEuGsald/Mt5TGD5PrCw6mtgq1ps+icAsgTyWjWMq00lbZoo8ljhYUuts87rcpGo6RkUkl2ypZDw5TRrGZSaUrtu64csJwltNZ3UwlxWejxYo9XoeZ9W0AXzQiuc0bNXWNKdrGOeKENLl8fOS6LaKp77rw/T0iBtZZa+/ew1sca6s5qZZ1DdluUKclKL2ZFNQzYQbcVo52CqmlwMvIinIOq1QgpSKXgpTzOW/V7ebl77HqH/lUYJ/iwfTm/Zt7EE9yHEIKoGxhnwQiHsKAiyeqwTxP1OW8yNkaGSV2hrVuMI/LymABo5z9rjGQpj+ilMRLHxrSm8ZmVRNK/0AtWikntzyshBEo43yenBLGSSKC1lrb1jr9YSfJEdj12/pyXwkdlDlJFqx2WaNG1lkcRcde3Ni4av0+RJJGgbA1FbZACDg8Shpnv5Tu6FN+x7q2z45LH1yfUrWHUuVur1mCt49SoYFJrZrXmxHLOaFZfN4J2L273nJPFihcdG2KMY1q1nBoVAAcS0cZFw6lRwWov5lA/4UXHhnfcnRsIBAKBQCAQeHZwWwW0P/vs47zrfR/lfR/5BGVVAftHNA77PR59w2t426Ov56Uvev7t3LTnDAcRzwDuPX6E5WGf7cls1+Wz4trugk/+2eep6maXZ8PLXvKCfbvMXvXyl+wqoAF8+A//JAhogUAgEAgE7lqujFIcl5oXHRtSNJrTIy9wHRle2210JZPKR/0pIbg49aLLxUnFoX7CtNbMOufSpGox1vLExcTfaHaOojUs5/HT6vcBLwIs5zFbRcvRYca4fHousINyqyLXNib+hv6pUUEeK44tpRzqJ9dNM9icNWzNWjamNbPGcP9aj6IxrO+U7FTeVSgR5ImibA3OQRxJ+lHMsIvim9U+alM7x4VxhTaWWasxxhErhZSOJJI4bam06wQaf40jEQvRTALzXAbXpRZaN+/h8oKYxLucumRBrOWyN80BwiKQGOs71Yzz3VwSR2MswnkHlXEOZQXGGgS+f24pjTjWVxxOWjK3zc60YApESiycZkqCkD4SEmv5RvsZ/mrzAb5KnD7Q/mqIeK97Ne9s38AFDs8r3vxnVfjP4CxSSIZ97zjbsDnrO5pJWWNxV4yNd9cBNK3Fda48IfDip3XkiaJp/egmUpFEBpx3teVJxLGllNZYjI183KL2HXVR5whsnB9o7SxCChTeYZbHisY6itqSRoJIysV68i4ycpBG9BOFkIKqMQgNl6aNjwid1CylEZEUZImiF/vL76U8QuAjRm9395a1js+d3+HCduWdk+MS59yiN1Bb77Q7My4ZJhF5LG8ognYv7sScc+9Kzlb3I4NTo4IvbxasVZoTy9m+c+Y8znU0a1jtxdy/1uP4cvaM9EMGAoFAIBAIBJ4d3HIB7eKlEb/1/o/x7vd9lDPn14H9IxqF8CLL2x99mEde96p9xZjA7WfQv/aGxmNPfHnP57/geSf3Xd8LHtx7+ReeOHXD2xUIBAKBQCBwp3lqlOKJ5YzHLkxY6ydcmjb0EnVV9OIc5xyXpj6qrWw0k1pjgVobhnlK2WiKxjBMfAeSBR5fn3bxcpJae9HmlQ+s3rRj60oGacS4LLHOPe0YxZvh6UauWeej79a7DroXH18iVorD1xEwG2M5Ny6ZVJppbTg6TOmnEVmseGJjsnCSDVJFawRJJMli5R1jHZFUSARFo5FA7Sy1MZSNQQpBnkgSpdDGkkiBEtDSxSxyuWvLWhZKmH3Kds5dapH0Xit3xcXTvFNt0ZPm6JZ7ccg40NpincU6gcN2wh0IJUiUZJhFLMWGZVkimxnbs4aR8eudu25iJdASlJJk0vIm9Qneqt/PvWLjhvcTwJSc90cP8zvyDWzoPlNjkO7aa8A4EqzlfQo54LzJ2No2zJq6Ew8dtvvMSgpiKYmUd9sZ5d1jsouvdA7SSBIryfGVHGMsO5WmaP3+EcJHO1aNwQlHbSyt8WOUKsncLijmoqXzXYapkvRTH/NpsQsXnO+cE8wajbESJQWrvYRh7h1pvVhRJpp67F1e/UQhnPPzRAN5LMmimCcuzqi0Zq0fc3iQ3lZX6OfO73B+XHJqVLBVtBzqJxy/Qmi6OKkW77/WueOeGkE7v6B/YO3aruzduBNzzkvvWQJ8nOkg88LguGhYzmMGaUSeqEU3ZdkYprVmu2wRQnByrbcYh/l6AoFAIBAIBAKB3bjlAtrbv++Hbyii8cTRQ7z1W1/H2x59mONHD93qzQjswWi8s6f7DOAFD953zWNfeOLJPZ9/7PDavu937Mjey7/4pSCgBQKBQCAQuDux1l0TpRgryT3LGcb63qCNSQ1wjYh2adowqVp2qpaqteSxYjWPubBTs7HjY+mGWUxjHTE+bk8KwbTWnB4VC6fOE5emGAf3LGccGuwvFu1Hniicg7I1zOpru2lvFdY6xmXLpGqZ1cbHBgpBP1UcHaZobZlW8YEj12bdje9z45LVXsxKL+aelZxESZxzTBtD2WjfLYePKkxjH7nYaMNoVjPIosV+UoLuhrpBG98f1ksiEp/3h+v6sbSzCweYdY6toiVWPo4vUXIhxLTG0RiHkpcFLzqHmekufp4qms1Z9IsJMBaUdBh7ZVyju9qF1m2LENBo70DTxnaC3eVnDbKIlb5iLdKkZouyLBnXLeA7x5xwaOOPM5DgYChKvkN8lLeYD7HKzoGiGkcs87vxt/Dx7GEqkWGtI0YTaYPfMv9+vSxiuZ9j4yHrTcL6pGWnqhdimRQCKX1iosD30c3dZ7rrLIuV9FGJrSFSgkhJlvKYfqxIezEOmNYRVWvoRYqqNbTGYrs4yEY7lPTCipsLlF0vneyceFIKjLVIJbEO34MmvQMtjSVNd5wfHqZoYzjS77FTac5ulWyVPr5RG8dOpSm7mMRISSa15uy4wlrHfav5whG22k9uiwtqHkF7alSwXbY8eKh3zXlXt5dFxfk5MI+g7cWKjWkN0xqEYJA2NxTneCfmHCEEX3PvMqv9hMfXJyzn0SKaclyW19yPyGLF8eWMtX5C2sVABudZIBAIBAKBQOB63HIBbX5Bt5toliYxb/zmV/K2R1/Pq7/upbf6rQM3wG9/4GN7LltZGvKyl7zgmsfPnL+452vWVvb/xd5+yyfTgvHOlJWlwb7rCAQCgUAgELjTjMsWbbxocmWU4qFByqw2OOfYoObipGbQGNb6CUoKJlXLtNYL8Ww5j8kiyVbZMKlbitqQRJJ+4himMfeu5MSRWDglvnRJdn1EhjOjkkhKjHXMasPJtfy6kYW7obrXzPuybjVVazg9Kjg7LtHG91LN4xCFgLxzdZ3bLomUoJeoA0WuPbExY327QknBPcs5q/2YYRZxblyyOWsw1scmNp0IIIR3VJ0ZlcxqjXaO41d0yU0bQ2PsoussjSRJJLHOUbdmsZ5539jc9VW2mqLxQk4WSSIpKFuNEhJjLbX1jrC5g+zKkZ7vtaeO/jzGsbXOd4/ZeWxjJ7zZy31qALH02yqFpGo10l1eqZSCYRZxKIM1VZPYgqqoGZUt2jriLivS4nDWu9S0tSy3Y75LfpQ3y4/St9WB9v15cYz35d/G7/FKoiQnVoIcwPmYxEgpjPV/rw5SVL7CtuuxXVkuTRvfGSev7oqbC24K3y02HydtLQKBsw4rBVkcMUgVSkmGaYQDDvVTRtOGWAl2CkOeRhjr++wa7fvpjHVEShFJuXAJWufQXQSnknTLfDykMZY48mJtL5bQueKKxqCNpWwtZ7ZKxkXLdtVSNF40M9ZfF2eRd5nOP8us1kRSsF1qlnuGraLl8+d22Jo1vPSepZs6x3fjygjarWJ38Yzus8+nBfmU956LzhcnNVmsOTcuGWYRyXVcsbd7zrmSe7uOttOjgiwuOTrM9pyDIuUjZU+u9ULnWSAQCAQCgUDghritHWjz78oveeGDvP3Rh/m2N30Tg174ldczxaXRmP/zV9+15/Lveeu3EKlrLyRms2t70ebk2f7F9nm2/6+lp7MiCGiBQCAQCATuOua9ZFVrOPIU99fJNf99VgjBJG4ZzRpmtSaNJeOipTWWWWNYSiOcc5zdLplWmqr1rqxBFnFsOeO+lZzGWKpq3pslyCLFoUGCNjUOt3BrzUWZ+w8dvD9s7oIS4tob5E+Xs+OSx9cn1K1ZuD+q7sb1nLn7YyWPmDWGsrUMsojtsr2hyLXRrCFLJIX2kXzjouGJi7POhWXRxvdZXfmejTZsFQ2z2pBGki9cmLCce/faxUmNFL7fLFZevWm06ZxC0HadUHZeVIYXubRxtJ3TrGwNkZQ4oLEaOreYFAIhfQzjPMYRvBA3j1ac/3uOF4dACu+Qmsc1Lrqjuz8iCUnsYyatnW+TJY0VS3nEoaSl76aYpmA6a8HZRdeaxItTcRcTqa3luNvgHXyQR/kjYmcO5Dj7vLuf/088ymeTlyOJsNaxdOXrhUBKwSBVREmPWvW5ZHJmU0cSe8deGkmssyR4UU9wddSlw6Gt69xcFmP9GAgpSJVAKUmeRixlEZNak8WSnUqTRopYCnQniGrrKBpD3HW7RVKiO5vfPDnRuLlo6UerbH1Eo5A+LnKgZOciU7TGoqSgH0tGsxYpBEVjKBpNpS04xyCNiHIfszlMY5JI0mjHtNYkkeDwIGGtFxNJwanNGdOqXZzjX3Pv8o3viH14agTtXo5PH3Xp/383saufRgxa7+Tsp5JLk5p7ruPcup1zzm5kseKFx4Y8dGSwpwt2mMWs5PFtjcsMBAKBQCAQCDz3uC0CmnOwujzk29/0zbz9za/noQeujQUM3FnqpuGf/cz/ys509/jGe48f4b99x1t2XTYr9hbQknj/Q+h6nXb7rXs/xtsTLo3GN/XaQODZxGhrm6KsGG1tP9ObEggEniWEeePWcHZjxqVxQVFWtH3JjmuvWr6SgjNQ15bDuWRaGy5sz9guNdPKR8s5Y6i19V1V1hELiJQgFo6dWc0prbF0kX2dgFZry6zR1K1mu7AcG6ac25rSti1VXeNMw2rvYJ3BW0VLWVW0dURTSi6N9goUvHGsczx+ccbFiRfNLuzUOOd8v1kakcUSKQTWOarWMqtrvrQzQwhBHks2S0svUQxiyebOjHP62m2KpMA6mJU125Wm0ZZzWxPqS5a6dVStj4abi3OrPd9ZtVMZxrOK7aJluzLECoqmZTSV9GLJdqUZFy3GOlIFk7JFa0trLa32N/6V7CIFpUBAJ5pA3bpFTKOV3itlgEiAMQ4nfL8XXcQiAA4U4OYiBf7f1j3FpeZ8xxbOr2cefCdhIW5pY5GRpDGWpVTRG0QsqZrUbFPPKraaFuHo4kC6NxACIVm82Qt4ku8UH+C16tNIcTB30Cd5Cf+3fhOfss8njiRRbVGyQQqBko5eohD4cVvqZVSy30U1asrGRzUuEaEtOLyAKZSj1n6TtXGYTnz0m29ptR+zue6RKn9c9SNBKqEXCbaKlu2ZQ2tDoqBoNK7r37JuHstpAUGk/Kga58U0IQTOuE5E81GkUnbHlxD0EkmrjY/vbFqss2SxxFof8zia1mjnfFebhEEakyhBax1Na5g4RyQleSw5OvBiY1Fr6liiE5BGcr6umRYlk1kObcXxpZuPbAV/fn7+9JgLOxWzouFEX3Buc5uqtdSd81IIQRpJikbTNpqmadiZefHvqeTSMaobNsaWtmnpK7OvU+52zDkHoS+gv/idpwMstm4Z1Xd0M57ThO8agUDgoIR5IxAIHJSbmTcOr63c8u245QLaa7/h5bz9za/n9a95xa5upsCdp2lbfvSnf4k//ezjuy5P04R/+aP/YE+3WFU3e65bXWcfR9H+y8vq5q5iPvCxT/Lpz//FTb02EHg2UZQVn//ilwDo5fs7PgOBQADCvHGruFAKLlWwWQtGpx3RHollxsFMw6wVjBpBZaCykEuYlVAa0M47jGIJjQFdwab0vVfWXbu+1vrXTB0U0ymZhK0NOJc4vqDgaOZQBzBRbDXQOsHOWceZnqN3C64ALpSCnRa2GkGloRc5hjFs77NdxsGkhUILYgWJ9OGEy7HD4sdoHrnWGJho3+o1ax2lkWw1XVeY8/9FQBxBImBLwhOLGDqYaj/2jfEC1M7M/y2BFrDdfpkZTQEUyt9mV4CUoJ+67RZa1zmk8IKOtWZh2prLq7EA0/r9arsIyPmhc+Wu3k22srBQzebLF6/t1mWFQzjJidyQU2KaGdNpw442i+cKuMqNhwOJ4xXyi3yv/RCvkH9xILeZcZLfs1/Lr9s38hfuHn/MCovW1m/TfAwaqGPJaj9nJgZcrHK2Ck3VTmm7cwBgs20Rgq77z29K27n1jLu8PouPtLzyM1kHZaV9ZUALroR6B0oLIwd9BQjHdi0o2m5987HDO9iMngtlULR+jF039HNRszXdsQgUBrT0/44kZJEXT2sLs25fSwENXkgty3KxD9vuvM8VEEEtoB95t90XR4InpWMQQaYclRF8IXH8YQwP9Peec26EQsPZQnCh8kLeF/5CLD6bcZfPMyX8fplqQWvhQuRY2mN+mGo4h2Alcqw/6cXnvbgdc07g7iJ81wgEAgclzBuBQOCg3My88Xf++nfe8u245V9l/82/+Ee3epWBp0FZ1fzwT/4if/Spz+26XEnJT/7w3+GrX/S8PdeRpQmzcvc+BG2eenvhalq9//LrRTzuxSOvfRUveN7Jm3ptIPBsYv4ri7c88s2srd6aSJ9AIPDcJswbt4bHL8740qWCv9wseP7hHvl1+nImVcsXLs44O64RwHIeMa01RWPZqVp8gp5gXLYoIRauqVgJInW5i0kby8a0ZdZoitoQpxHL/ZheKunHEfetZBwZpjfsUNHG8vjFGUeHCceXMr7xeStPO1Ltwk7N4xdnnN4qWak0961kLOU37orbKVvOjCuGWcS9KxknllL6iaJoLdpaTm9VzGrv3tsuW3YqzahoUNs1SoAQkn6iUFLQGkutDWXriBYxdNB3jtT6XrSlLMI6KBrTOeIMRWOQxjsCHQ4nJSt5RCR3Vy1qbai1oamMF28cxEpinPOdXJ2IkieSuIvrM40Be9k55f1PHV2x2Tzmcb7M4QU8iRc4IuGjQodZxFoeMZAVsZlQFiXbVbNww0n88TkXpIQQOAdKWB6Wf8Y75Ad5oThzkN1M5WLe417Db/JGNuQhUAKlfXakEII09nGQzjkEgrWlHulgmbHpsz5r0cayupTSSyTWwcVJQ9Ea6tZ6gVBcDk2k6wuT3iyEoRM8BSjlO8mUFMQSjPUuxixWHBpELOcxVWuZ1oZDg5i6tdhZw2yrQjmHxUcpxkoQK8FKHnfdZqCd9X9b6wU86xYxope75wQiFkRCcnSYsJJH+E/seHJUEiuJto5+qjpnmo+DtNZHfQ7SiGEWcWIpZZhFRN0BUTSGS9OGtX7CUhbRiyVFa3nR0R4PrPV4/uGDx7XOObNV8olT22w/OeZ45s/NWaNpzbXSbSQhrX3fW6UtJw73WM6vvU0wrX1M632r/pw9PNh9Drodc07g7iN81wgEAgclzBuBQOCg3C3zRvgt2HOYyXTGD/1Pv8Bn9nBqCSH48X/43/PI675h3/X0e/meAlrbml0fn9O0+wto/ZvsxFtZHt4WS2YgcDfSyzPWVpfDMR8IBG6YMG88fWYuZmoUFwpLnGQs9XfvD5pTuYqVgT8L4C0AACAASURBVGOngUP9hGEa8eSowIgWVxuyWDEpW4yDYRZzZJgyzHYXnaSKmFQt665i1lr6xrGkIioj0ELROMWg37uhm9KnRgX9Xs79R30/0NFDw5saj8XnbA0bGw2tiGlpefG9S3t2K+3F0gAG/YYvbxYYmdDIhFfef4gsVvz52W1qF3NqVFC3Lfceynl+LPn9JzZJY99Jd89yTnaFoDme1dS2ZVL5751LWUTcRfNN65Yk9l1TSWTZKhpiBVI65LynrOtp0k6Qqt0FNOXAaIcQvqRLdt1YDkHj5iIWOCFJ44jWaFQX/6itQ3Zi2Fw0s1d0nNEJcl1NmX9cQCQky72YY33BoajG1duUZcN2VS9EKCn89s9dRbZ7bU7Dm9UneYf8IPeIzQPtn4nLeRev4zfN65mqIVmsGEhJY33MpUJ0Djkv/mZpgkuGnDcZs7Fg1pSs5AmHl1JWewn3rubU2jDIKk6NCi62Fa2xXnSkc4e5haaI68ZDAnmsiJQgTRSZklSt9RGMAiIlcSgqK+hlKZVpkDJCu5aqdURKYp0jEmLh9LTW7+dESawEtCCSDjTU2otITvrjQdLFOSqwzkc59rOY5X6KQHBhpyRSkl4WIxycWMkxzkd8OueotSWKDMeGGceXs2vOkzwDKyKKRnMoiVkepLiipRUxhYtYW1m+qb4uax2/f6pgo7BoJ5m0PkJy0MvIY0USXY5XbbSlbA2FrmiNxjjBhalGRTFHBglcMcfIyDBtIYoTPycOdhf4bvWcE7h7Cd81AoHAQQnzRiAQOCh3w7wRBLTnKKPxDj/w4z/HF//y1K7LlZT8xD/6W7zlW1573XX1+zlsbu267HodZsV1lg9uUkALBAKBQCAQuJ0MsxjZOcUmVcvadQS0urW0xuIcJJGk1F4g2C41Du9EqbQljyP6aUS6Tz5bL1GUrWG1l7IxqZg1hrTSDNKIizs1y3nCrNZ7CnBzxkXDaNZwcq1HGitOrt28o2XO6VFB3RrOjUvW+smBxbM5K72EtUpzblyynEecHhX00ogL215k2S5bHjzUY6WXcGarWHRYCSGIrxC5ykZTd66aSHgFysfULbxN2M4elkSSSErKRmOMQ0nv+RJIhICqMSjBVeLcHCHAGbvIVpTSxzoump2cF36ccxjthaBIClq8M87Yq2MV566z+WtF9zfCO9tW8phjuaZvd6CqMMqylMZYA5WSGOtojLtCRPWxgDkl/7X8GN+tPsKqmB5on6y7FX7dvIHfsa+hFRnWgcLRYFCJF5X6SUSjLQhY6eckvSXW24yNmWW7aImUYCmPyRPJsWHGg4d7KCmZVF7wyhJFP1FsVw5rHFZcjkrk8kfxuo3wnXCDNMJ1/YBRJEmVZG4UnHU9ZbLLvmy0o9YObf14xErinCNSgkgKLzYaS+3EYl+abkcoKRBCLl4XSYnDuw+t9du/ksdEUjJtNLX2HW7GOIZZdM1xs102KClIY0W6h4N1re/P5UmlSZRiKYvYKlqODjPG5fXnnd343Pkd1icVG5OanUrz4KEeR4ZZd7xfTRophlnMch7zhQsTGt2yOatJuozYI8PLLjPVHWs+TnT37rzbMecEAoFAIBAIBALPJEFAew6yfmnEP/hnP8uTZ87vujyJY37qR/4ej7z2VTe0vvtOHOVLp87tumy0vbPva0fjvZcPBz1WlsMvEgOBQCAQCNx9rOQxkRKs9mIubHvHTLyHOwnAOrcQSKQQVK1GG8O0alFC0hiLEoJeKpGdSLIXSkqGaYw2jiT25VzTypDHiq2iodWGsjX7CmjjouHUqGC1F3Oon/CiY8NdhaGDYK3j7LhkNGtwznFi+en1V5xYzhY33JWcIaVgc9awVVwWz6xzjIt2IZzFCqa1ZjmPsdYyqTWNNrTaLmIki0aDkj6WT0BrLUnXEJbFku3SYXBIvCjQSyIqbQDHrPGCZxopnqo3WADhRRiBX6/DO9FMty6HozYGhxdchHBY63B0ziTbRSxyObIRfBdVnvhYz9WoJjcjiknFRtMQCcEwj1ntSU4s5zi8UKuN9vGJAg6zzXepD/M29fv0xME6hr9sj/FO8wjvt1+L6UbKfxLfE2asF6RiJVnOIg4Pe9hkwPkmZTKFnUpTa+OjJ7u4yUO9lOcd6SEQbExqprXf1l6s2IkUsbI464UpBCgJQkrvxHP2qkjLsjVESpBFikj5iMxerGiNo2g0jbTY7uTT1tBoH9UZSdm52xz9RC3ERiUlaeSXzUVLAcxqTdttUz+NkGLuIOyEcemdWw4vtjrnUJ1AlydXn1vWWmpt6af+OMr3EMyVFPRSxbQyLOduMXdY525IuH8qZ8clF7Yr1ncqytawnMes9pNdxbMrSSPF8w73ObNVcm675MJOhRCCLJaLecZ0YywEyF1K9G7HnBMIBAKBQCAQCDzTBAHtOcaZ8+v8/R/7Wc5fvLTr8l6e8XP//Ad59de99IbX+VUPPcBH/vBTuy5b3xjt+9r9lr/wefff8DYEAoFAIBAI3EmkFNy7klO1hvWdmvPbFffv46aQnbAC/oZ9axyTSmMsmM6vEUeCVCmyWCGuE7+YJ4qiFWRKohS0xjKatfQSyeas4fjy7i7+1ljOb1eMZg2rvZj713ocX864d+Xpu/7HZYs2jq2iZTmP9xUBb4RYSZbzmK3Cr7eXqGucbbNad24iLzTEUrJTadJI+hhA6yhbQxxJkk6kaK2k1Xbhamq1xcZenLCdMKQ6AUApvKsJaIxBCUmt/XqVkkRCIKTAWteJNO5yVGKHFxRY2MpMJ4vFnegzazTSOZy47DqbRxZK4d2Oh3PBqqqQzYjZTsOlrkfYAbrrbRtNa+8IchLjvND3oLzIO+QH+Rbxx8Ri/2j1p/IZ+yDvNI/wB/YlnZzoX2/pIiW5winnoJ8lRMMVJnLI+sywMW2wzu83hySWPjJROBjmMbW2TCvDpGrZqVqq1tJLIk4sZygh2JzVC7eZ6M4f50BJ5cVJB422qFiipCKOZBdB6EWZJBK0VlK2msz5nrVYim6MBVI5MKCdFzN7iSJRkqIxZLFc9K8JvKMwVjGtiShb7TveIonuXH7Oy5Zo64i6bj3THSPauGs6EieNH8te7B1e7HO+57GiaLwo7fBjULaGWX2w/Vm1hsfXJ2zOGqrWcGIp49KsodWO9Aau+odZzOGBt0qe26nYmPgfDrz4+JAkUjTaC9KJkqTx5XP/ds45gUAgEAgEAoHAM00Q0J5DPPHkGX7gf/w5Lo3Guy5fWRryP//kD/PVL3regdb74oce3Ps9v3x639d+8Ut7L/+qh4KAFggEAoFA4O7l5FqPM+OSe1ZyTo8KlrJoz8jCNJYkykcBNtpinaXU1rug8K6XPFZIKegnN+bK6MURSax9D5SQXCpqRjNNFhecWMo4NEhQQmCco2wM01qzXXq31sm1Hof6CceXM156z9ItGY9J1WKs7yE7Mkiv/4IbYJBGbBU+FjJW4hpnW9l6N5HFcXSYUbWWxli2ywZtHNr5WMUrBYw8Vugul2/uCpzVGoRjWpmFauJdShFaW7JYLlxMkRTEkY9JrLv1lI3pov666EcniIToXGjzqEALQqGdIxYQSYlxjkgKrBO4TpmyzosQwzzicGoZUEA7Yzapabr3U50HzMdRQtVatoqWojG01vEC+5d8d/QBvll8FimuUPNugI+br+ad5hH+3O19TTAXH5UULOcpIhuyLfqcLySgkQiWspii9XJhL4mwxjHIIh9X2mhGU8G0NoxmNVXnxnLCUTSdQ0x5H9Nc+BSAUhKBwFpL0Wha62itI8e7pObi2ZX7emIsRWuJpPB9c/iYxkhJkJYYSSRF16fm3aAW6CdXXwonyru+UqWotaHq1pMoQWMcaexfG0lJ2RqkEN6VBld1lVWtoWoMS1mMkpKlfP9L7iSSXiw09qrjdn483ihXxqseW/LnynalKVvNILuxy/7DAz+/1caxU7YUjeYL61OOLaUUtQbhxxgEm9P6ts85gUAgEAgEAoHAM00Q0J4jfO7xL/GDP/HzbO/s3nVw7Mgav/TTP8KD95048Lpf9fKXkKUJVd1cs+wzjz1B3TSkye43k/7ozz6353offs3XH3hbAoFAIBAIBO4UWax40bEhxjimVcupUQGwq4iWd66yuLu53mrvVKpbS6R8dGMSKYZphJQ35txqjGMpi+klEZESIBwXpzXawplxibvC1SK67q7jyxlr/YS02/Zb6QKZ1b7HzTkfhXgryBNF2VqkgO3Scv9a7ypn25Xdcmv9hJ3SRwG2xjIuWlpjya6I5wPvBoyUpG0tjbW4zqU2f9xBp6wJH6soQDeGuBNB5v1XiWIhbEhl6ElJo72QU2nrfYUGQHQuJQn4yEYZSxwCbS1dRRtKCnKl6GeKQ3FDbrepypJx1QA+ipHOmWaFd93NFUBjHWWj+Tr7ON8j3s/L5BMHGmftJB+wX8+v2jfxJXv8qmVXRkkK/LGkhGCll5H2B+zQ52Lh2CpbEinI04jVXkyWeKFx1mjyWNII70abVprTWyVmVJBHvs8vSxRN6yiahqq1TGuN7mJRYyWQeAdhEnsnm7GWNPL9g9Y5Gm3ZLtuuy+zy8SGFQElBUWlW+wmNtotjppdEaCEYZn7dUkjq1pBG0gux0i7Eu/m68jjCWB+hWNUtWazIlELbThC1jqqLDF3OY+9mVGoh1FatYadqyWJJnijW+ulV27sb82PXOTpxqnM17uJas9YxLlsmVcus9kKkFII8kTx2YcJO6Z1szz884AvrUwapYqtoWbMWdQPzjhCCI8OUWAkeX5904r2PrFyf1PRTxbmxd/oJKW77nBMIBAKBQCAQCDzTBAHtOcCffOYx/vG/+DfMymrX5c87eQ//9qf/CccOr93U+vu9nDd80yv5Lx/6/WuWFWXFez/8Cd76ra+7ZtmTZy78/+y9aaxk2WHf9zvn3L2qXtXbep2eIWc4Q4pDUVK0hKJES6RkyNYCRYYExf4g50McwEggwFDgCIbhwAocREkMJ3FiILCV7UNsyYIt2ka0ULFESbFWiNTCITmkhsPu6fX1q1frXc+SD+e+mvd6mekmh90znPMDenrqddWte89d3q3zr///zyc/9dl7LvPc/i7f+P73fEnrEwgEAoFAIPCouDjJOeo7vy5PS14+LNmpNefH2SmhZ5BGRFIwzBRH6w7nHHWraY0hTxKK2Ec35smD3X4b62P7hlnEIFVcmGS8dOCYVi17g4R37A94x+4A10fg5bHqBSIfPXlpp3jD+4dO9ryp14mgfFCUELTaECtJre/udbuzW+7YIVN23pm3bg2iM0i8OKak763qtGXRdEghemePQ4hXxQkAi6PVhiyJcM5R9kJenkQUiSSSikprWgNZHCGAOHKkSuLoKFuHkL6/DBwOwXEuoBC9OOcc1lkGScRWJhiLGtHNKJc1h20HffxjJH28pPUvxzjfQ+a70gzfpT7Jj8pf4xl5747j+1G5hH9jPsDPmz/HAdv3fM5Jn5MUMBlkpPmQpRhwrVaUTYeU3sXVGUdkLNbCKI/IY7+N69YQ9dtsne8NqxrNke2Ipf+5kH5fV62h6SxS+vi/dQNnt2JGWUwWK8a9i23RO5uWtT+ftDFMVy2DLCKWAimPHZ9eUNXaxyoaHLKPk9wbJgyziKQ/V2+vvBCprWNRtQzSiCT2Api11jvejEUKH7+JA2MtsfS9X8Y46k77OMlEEivJqvG9a2XvPMtiyTiLGWaK0QM4v46dZsfu1ePzeZC+ev7WneHKtOTqrEIbHydadWZz/mvj+MLtNdfnlXeHCsHuIKEzhlnZMS27h3KNToqESzsFs7KjSBRKCs5uZZzdStkfppyf5I/kmhMIBAKBQCAQCDxugoD2Fuff/cEf8zf/3j+kuYc7DOD5557mf/ipn2CyNfyy3ueHv+8j9xTQAP7h//5zvO89z5xyt5VVzU/9g3+MtfeOHvlL3/vh1+3+CAQCgUAgEHgzcBxHJoRgmLVcm1XMypZxHjNMI/JEoYQgTxSsYFF3HJUtrXEkSpFGgjyJGD9gjBrAqtF+Ij3yHUqxUgzTiN0iZW+U8tROwbNnRhsHyiD1z5vk8ak4uTeSkz1v5j7xctY51o2m6rxIcrx+aSx7USA65awxfV+cEBaBuMvZdme3nBCS/VFK2WrmpXc+RVJSdwbdaJzzooy2XhxTUhBJwShTOOsjAlMnMb0IIaTEWh+WKPECxqxqsTYiVhbtoEgUUngnWqsdXe/mSSNH1QqUkmSxpO402vZCmHXESjDJE0ZxR2FLTLtiUbZobTZOL/Dxf9b5rq6To5rS8hfl7/Ej0cc5L167d/hOZm7AL5hv5xfMtzFnAPSxjK/BMEsYDrbo4i2ut4rDdYu2mlj5mMI8kqytoe0ss6pjkEjyJGKURejSx4haOoyFqvPiXyzFJh7TaOvdmcYh5XH3mBfmGm3ZEvhzRPjzpTWOHUAKx7RsiZx3YRpj0QacM2jzqpBknGNcxF5ww5GniguTvBfmJNN1SxZLbi0bFpWm7AzTdUukvBAme8Nfnkg67aMKlRA+klFbjsqWQarYymJAkSgvFtWdZt1oBmnEVhaTJ4phph5YsDrZLaato+jPkWMx+eqs4sWbS5p+fY/Kjrrf5mMWle+Zm1ctRaL47I0l+1sJsfIuuNurhqI//x6UYRrRaMtOEVN2lmfPDhhkEe+7sEUeR4/kmhMIBAKBQCAQCDxugoD2Fuen/9H/dV/xDODKtZv86F//Ww+8vPd/zbv47/72j9/1869//jm+5zu/9Z4i2vRozo/9+H/JX/jwt/KOSxeYHs35pV//bW4e3PuD/qULZ/krP/Q9D7xOgUAgEAgEAo8TIQTvuzhme5Dw4s0l4zzaTGTPqmozka2NZVZ35Ili3Uhs4rDWT86PUvWqYvI61J2h7gxbmY9u3MoijLVU2pAlkiKJeHpvyHsfcc/QIFV9VKXv5DqZZNkZy8GyYbpu0b3zqu2jF4/FASG8mLUzSPqYOEnV+g6tWEqccnc52+7slkv7Dqw0kr3gAEK4PsrPj52x3olkrSOJJKMsZtxP8mvjOFw3gBfmIukdNDhotO8zM8YxrzryJCJWEiPACbERoIokwlrLrI+PBL/vcT4McRArdoqI7aQlbheUq5LDusX0/VwntYZXYxvdJr5xizX/gfr/+CH1W0zE+qH20Q23zc/b7+RX7L9PJxPa3sUGnPrbntqvMUVRsJYFV7qUqrRY1/VfdvOOMuMsaS80dcbSacO6M4zyhHGRcLBqkBKs8Y6tpHciSeEjMdkcBwLjvEPwWKBptI9cbDrDvNaMcy8cbfWC8/GX7nzsI7gIskj59TCOQaLQ1jFM4r5TTbE3TMiUokgi9ocJDu8gO1w3PtrR+EhNbWy/DhopZB/FKYiVPy68eOaFunWrGSaKzjq09evbWYeSCrDsDBISJdkZpA/kPDum6gxx75jTxnFxO/bnfRrxp1fn3JjXHK69cO+cY5zH7A9TslhuOhBfOlizrDtWjeFg2SCFj5uUEkaZou4UB6um39+vsW7OUWlLqw3rxnBrUXO4anhyp+D8JOebntrm0k7xwNsWCAQCgUAgEAi81QkC2lscdx+H1zGL1cN96F4s7//8v/HX/jK//0cvMD2a3/VvVd3wL3/x1193+UopfvI/+6v37UwLBAKBQCAQeLNycZKzO0i4Mi3J4oozo+yuKLWn9gZcPaoQwM1FjchjEiVZtoZx9vodRHVnmFfHHUoRO4OESEk/+e2giBW7/c8eNaMs9tF2se+m2hn4+7nDVcO1eU1nDMtas6oNnbWnHDJCeJFsmClaYzhct1wYZ6waTRZJpBQkiLucbXd2y40y7zC6tWyoteFYdbIOOm3QvahinfPLjBRpLIkj363VSUsRq41wAg5jBdY6hBA467DSj/P2ICZR3rWTx5JZ2bHuNMuyI44UWaLQ2rvs4shHeI5iy4gK0U0ppw3TTvsNcT6qEQECL/YZ6xBO4CVEwR5Tflj9Bt+vfodc3P8LcvfiJXuef2Y/zG/Yb8CgUHJT87YR5vq3R3gjF3kSUxQ5lRrxhSZiUdYo2ZH2vWAC7wC0vRPL4cUwbb3Db11rqtz4KD8EVvgIyp1hyiCN6LRlUsSoXjE0DtaNxhgflXhmK0Vrx6L2EYPTsqOzjkh6UU8IwTiPSZSP4eSEQ7HqDI22RNL3sEnr2NtKeXInZ91oXj4s+33qmJYdq7rDOHDOkUaSSRGxbmFWWqwDa0E7A5zuHvPiXu8mLGLOT3KM8+6szlrGWcyq6Thct0jg4nb+up1nJzHWUTaG7UHMvNLsDRN2BgkXJzmfubnk+qzi8rTkqOzYHSScuyM69phRFrE7TKk7Q5FG3F411J1mf5jSGOvdcKuGW8uGYWfYKeJTnWjaWhaV7jvnvAg6XbccLFt2BjHWOY5WLX92sKLuTIhrDAQCgUAgEAi8bQgCWuCB2d0e84/+67/JX//J/4aj+fKhXy+l4O/+xF/jW77++a/A2gUCgUAgEAh85clixbNnRzyzP2RWdSzrjnVjTkUpXj2qOLuV8okrM/7klRkKQdloUiXvO+lsrGPVaOrOdyhtZT4ecpTFrBvNqtYM0pjWGC5s56f6kR4Vk9w7Y7aLmBvzmkYbbs4bpmXLsu6YrlucgyJVbMUJSeQdPdY52j6+72jdMSu9+NZqw1HZcWGcoa0Xve50tp3slpuuWm7Yuo8BtKwbjTaWREUMEu+MU30coBACbS3O+WjBRClcBJEQxJGgSCLS2GGtJVISYxRVZ7AKYiVIY0WqBPujFIuj6XyPWtUeCzeSQaKQWUQMDFTHkDV1tWKxbmi1wwnv/joWsiT+fljixaS+Lo2nxA1+VP4aH5F/SCTsPUb+/vyxe4Z/qj/C77t386rHzPexWeuO9bNX3WcCijgmLzIqNeRym3K06GhNi8TRm8U2z5dCoJ31y3OgJEghAUdn/bjUrRdMYykZpIpL2wWtsdjEsTdMSWNFrARJJGm6XphZNSgkRS57G55gUXVUjeGqqdgfWrJY+XjFSLJdRNR9d1kk/TGYJxFp5OM1lYR37g15creg6gyRFHzh9pqXDtaM8wgL1K3F9J16vvPOYKwfL+Nc36Pno1jT2Md8Vq2hsz7Gc3+Qcm6SIRA02qBry84wYTJI2BtlHK5ams4SpQ8uoE3XLUL4cTY4Lm4XpLFCKcGNw5rL05J51fGO3YJJcf8vIB5HnUop2RkkaOO86L5q2B+mKCXZH2VksWa6bnzkZOJ7GVvjmJctnbGsGr25Dh13+BkHi1pTdpprs4q6M7wyq3ju7IiLk/xhDtdAIBAIBAKBQOAtRxDQAg/FM089wf/603+Ln/oH/4Q//eyfPfDr9ncn/Bf/6V/lOz7w730F1y4QCAQCgUDg0SD7KMJjF9ZJnuwjzm4uGm4vG26vGjoL1+cV20XCII0Qfd+SNj7qsO4MQvjYujyJGKYRe8OEdaM5WDUMU4UDLgxzsr4X7VEjpeDiJKfuDDcXDZ+8MiPp3XHrxjDKIraLZOM4Oknar7MZOKbrltur1kcyxhIH7A1Tlo1mUbXESpzqUGt7l9e0bJFli5DCi2KRRIiISEmccwgEnXXESmFxKOf7tRxwVLYkkUQJiJTfDm0t69YLBQBK+Ug/10cMLmpDo0uyWGGc86KCcSSxQAjH2UKxE7XYdsm8rDCAxBFHEouh0wLnXO86A4fY9GxZ53hevMyPqv+XD8oXHnpf/JZ9Hz9vP8JneAfauY3o5Y6FuT4u8hjX74PJMKeNRlztEg5nmko33ml24ommF6ngdOqo622WUtC7thxVpzcurSIWbBcJ24MY63zM55lRinZsIgHrzrBsNJ1xrFpNFicbl5mx3hWYRJJV4+MRjw2JxvptHKUR24OYs1sZzgn2BgmV9h6+d50Z8qHn9jlcNRwsG1qzouoMi1pTxIpRHlEoL8ot6w5jHVp7Z1saKZQUpJFESdE7SgV5GjGJFO+7MOLpvSEIwa1FjbGOM1sZR2XLu/ZHzKuOpjMPFpPYs+7FqiKRHJUtz5/fYneQ8NROwRcPSw77mNjXE8/g7qjT4+vDrWVDFhsmheTcOEVJwSCVvVNUc3VeU7emF7i9WzKLJXtD/9yqNbzr7JB37AxIIsmNec3NRcOFSY4xjqN1y/MXtkK3dSAQCAQCgUDgq5YgoAUemnc+eYGf+ft/m3/9sd/ko7/8cf70sy/5D9T34OK5fb7nOz7Aj/3I9zEowjcUA4FAIBAIfPUjhOADT+9yfV75SDRrkdJPkt9c1MSR9LF3/aSzd1hF5JEiUl6YKxLF7XXLqtYMU8VOkXBUtTy1WxApwSR/9AIawKWdgldmFXmi+PytFaoXU86M0gcSDZT0ri5w/Nmi5tw48wKW8CLLZ2+suTjJkUJsOtSsc1yf16wbzVHZUSSKc1sZVWcoO03dWnBsOrGs8B1OSkkwUCiJxrGsOoxzjNKYYWrYLlKKxG4ElkNatPOutGPBpjWWuHdOKSmY5BEj2TKQa2Rbsy47VrUmiQRIyTCLiaXkqGoBQ92xyU8U0veyfROf5i9H/5b3yS881Nh3TvEx+438M/OdvOLObrrUXvWdvfrn5M/iSDEqUnS8xQ2TcbjQVG2LPRErKfH70eBjJU8ugxPLgj4CEu8sXFXa94AJUFJyaacgVopIwcGy4YtTi5Je4DzuxvPOQcO67tDWMkgiikRxcbvg6lGJEj6qcW+QoF0vNFuLFLA7SNkfpbz77Kg/juDT1xecG2dsDxJ2ioTLhyVS+qjR6ar1XWHKu9ySSNFqQ2ccjbef9TGpXrRtO0NrfF9aFvvz9PwkZ3eYcW6SkyjJVhbxqWtzyr6/7+qsYlJE941JdM5Ray9SdcaPQd1ZZlWHEA7nIt51ZsjT+8PN+dB0hmuzip1B8rriGdw76nSQRgw7w3TdMEgl1sK7z424vWyIVUtrLFt9DKkWzhPYCQAAIABJREFUgr1hyjj366wEtMb5vsJhxrlxxiiL6Yzl+rzmyrRkVXebz4Dvuzh+qGM5EAgEAoFAIBB4qxAEtLc4/+r/+PuP5X2llPzg93wHP/g938HB4RGf/vzLHB7Nmc2XDIqM3e0JTz1xnne944nHsn6BQCAQCAQCjxMpBe9/YkISSYx13F41jLIB61azqHzPUKIEWSJJlCKSgqKPVKs73xEm8M6sURbRaMPZrWzTjyTv4fJ6FGSx4qndgk9eniEEXF/UPL03eCDx7Jh1o1m3hgvjDOOgs47P31qRKMGq1nzmxpJBGm3cR9ZaDpctq0bTGUvTwazyXV2pUpTOUrWaxlgEXvTqrMNhQcpNHF1rDMYJWmuoO0tj7EYoub2q0dZ3WyEUy8r3cY2LmLPjjCJyJLqEdkndtKzKmqNa02hDpCRSKBIlMdoilUAKsenF8/1nho/wCf5D9Wu8U954qDEvXcq/Nh/g582f4zYT4EQkI/5Yc7zq0jomiSTDPKOLR9wyGdOFodZN/0KBFK5fxqtFadaCEw6cuEtB28RR9v9vLDT4sc2TiN1hwtktH8d5dVaxbjStMYDo4wD9a5vOj3+tDa70b111hlEasz1I6LRjK48ZZNFGgCpb33f3xHbO02eGnNvKALg8LRFCbM6L64ua6dr3x22lEXI7p+wMiZI02lC12kd1WkejvXgnpaDrMzWN871naSRpjWWnd4Rd6MUzgEmR8PyFMb//8hFZ7I+vupUY59gZpGSxF62WZYvFu0ylFAgHtdbMa03VGqQUDBPFOEvYG6bsDlO+5tyI3/z87T4O1XF+nD3QMXIy6vRo3WEGDiUFO4WPgF3Wmli1nB9nfltiyarpWFaaJJKcGaUUabSJ2oyl5JWjinEeE0mxOb9jJXlyp2Ari7g8LTfjv92PfyAQCAQCgUAg8NVGENACXzb7u9vs724/7tUIBAKBQCAQeFNx7Nb62icmXD5ck0SS6bql6jSrxlC3FserwkLVWWptiZVku4gZZRGxUgzTiHkFFya+H+lSHxH5uDDGbTrYtouYVWNANBvHzX1fZy3T3rE1TBV7g4Rri5pXpiWjLOLKtPbOM23JY8WkiJFCcLhq2RkYlk1HJCXGwazsKBIf/6iNodr0WYF1PgYwVt5B5PvVII8jL6R1jnVryBtDHElabai0wVrQ1os3Z0YZWSJ5x0ig9ArXrrm9rMhjxSgRNK0ii70rTVsfM5kogRQSbbzYY60jo+F71e/yw+rjnBWzhxrnqRvyL82H+Kj5IGuKU+KY47hbzXvFIuldU9o6pJSMByki3eK2zjhYWhaNF2RjJVBCICW9aCSIlUA7L4h5pxgI4Y/DkyETou+zA3yXmHVY51W27UHC0/sDGmNxFsrGsGo0qvPi1iCOUMrHP2obc7BskC2sGo2xjlEW41zvyOrXM4sV49y7r24tayIpKVLfdwcwK1um65ZLO/68ODNK+cMrMw7XLc7Cs+eGaO14+XDNzWXjRTRn0NayrDVKSmptQBvAuyMHiXeBrmvNVpYyyWO28ojdO6JaJ0XCc2eHfP5gxc4g7o8zmFcdrTbESjAvNWVnKVvfKdZq72wUvcNuECmKNGKcR0RKMK87PnNziTaOo7JjnMfE6sH61KQQTIqYedVRtpqXbq+Y5LHfZ9ZxuG7ZymJWrSGNJNdnNdr4ffrM/vAuAfxg2SAEjLKInUGyccue3H6Alw9LhlnLizeX7A6S+3Y8BgKBQCAQCAQCb1WCgBYIBAKBQOChsNYxqzqWdce6MVjnkEIwSH3H0SSPH5s7JhB4M5HFiufOjjDGsao75lXHe85v0WnL4brtXTluE1UoBH2PkUBJwe4gIY4k12cV20XM7iDhubOjxzpJbXt30TBVDFPF9nZB2XrHzbrRDHoXne8bE5i+w6zuDOvWnHLV1dpwZpTywrUFy6ZjnCec73ul1q1haCKKxAtcTsDuIEFJyaLuKBsvQmpjNh1cXe8GS2NJJP37t9qBcOSxF0aUEn3vFUzLlkmmmFUaECS9++ZModjLNK5aUE4bmr7nS0lBq2FlrI/aHKY+ftI5GuPotEVbg0IwZs1fUr/OD4jfYizKhxrja26Xn9PfyS/ab0YLLyJKHOakmLX5DyiJ395IUGQJrRoyswVHK8ui7rC82oempCCSEgTEveMKAYkUWO2NZz4O0wuRx29jHehjZ5/z6yJwSARbecyT2wV5rEil4KBsWDZdL4o5hml8qhdPSb8vYyWRQlC2hkXVkaeKVEkaY9GF8wIf3llXNobtwatuqFnZcnlanjovbi2bU9GHl3ZyLk9LEIJJkXDlqORgqTHWn2fDLEIJ797DObTzomIWKcYT/3ss64/ne3FhkjOvOrJYoq3jPedGTNcNL1xfcrhqmdeastU4551bwzSiSCNGaYSSftx2igQhBTcXDUr6c33daKpWsz8cPNDx0hnLwfLVvkWH4+aioWoMWaLojGHVGKQQxEqylUd0xp+zwyy6Szw77mbbGybESm2iMu9kUiTs1Jprs4pxHnFlWvLs2dEDrXMgEAgEAoFAIPBW4U0poB3NF7xy/RbzxYrlusRay7vecYl3P/PU4161QCAQCATettSd4cq05OqsQhuHdY6qM5uJ/+NOp0gJLk5yLu0U4dvogYfiq1GcvTjJOerj2C5PS64e+cn9d58d0hjnowc724scgjSW5ElEqgQ3Fg23jrx49uROwblx9thj0mZV1ztkNM+eGTHMYq7NKgapZFl7UWvdtnc4l7jLVZcnCmrvLALvDru0XZBGkkiKTZdUogSdsdStJe0dSUWiOFy3zKoWZwStcWhjsIhe6HFejJSiF4wUSvr3SCLJGo22vi3sYN2SSMn+MGErtjw9sth2ynxecWtR+y6w/pAbphFGOvJEkUcSKSWjLMI6OFq3zKuOC+KID61/iW8xv0kiu4ca28+7i/yc+wi/pr8W4xQO300m+p65k71mov8j8aLIzrAgyre41aVcXxoWffmakgKc2yQyKgF53MciWv8YRN9hBkjhIx17IU1b1wto5nhvIgX+D5LtImF3mPJk7wI7WNaUneWJSU7dWW6vG1aNZnxHZ1+eRLR9H5iUgqoxrGqNiSXWQdkZJtZSdZob85plrcljSRlr/viVOVVrOD9ON+fF+a2M3/jcwanoQ4Hgye0CQcmy7pjkMcu643Dl94vWYKXdCNZFLBmmikESAYJGW7LYRyKeH7u7XFixkozzmFpbnj0zZH+UcmvZsJ3HtFupP5ZVQZFIvx8EREKyN0q4uF2w3TvETvaKNdpf91a14bkHEKMOVw3X5jWdMSxrTastq8bQaMO1WlMkCiUFZatJI8nVWckXDu1GONwpTu+XdaM5WDaba+6FcfaaLrjz42zjBMziimf2h2+5a3Qg8NXGV+O9VCAQCAQCj5M3jYB25dpNfvZffYzf/cSfcvnq3b0AP/bD33dPAW2+XPHx3/7DzeOnLp7j655/7iu6roFAIBAIvN24Oqt48eaSpjNM1y1HZUfdi2fHCOEdN9tFTN0ZXplVPHd29Ngn/ANvfr7axdnnL2wBPi5tmLVcm1XMypZxHjNMfXfUsVurag3TVcO86hBCcGmnYHeQcG6cbZbzOFnWHcZ6R9n+MGVnkDDKIm4vG2LVMs5f31U3LmJeOlhvJvfOjTOqzuKcY3cYU3UKhCCLNVemaxZVx7ozbOcxnfHxjDuDhFXdsdAG5xyRksRA0h8XifTjLYV3laWRX4dWWzprWdea3WHKua2UgobCzRgJTWoiSu3FhiKJsFishWEWMc684CGE75wa9r1TAO9013h29i947+p3UNiHGtNP2Gf5efcRPiGewxrRi2P+4uoc+KBPz8kYRyklkzwlH22xlCMWNdxeNTTaIvoeszgSSCt9H5zzx9hxFKMUko020gt0SgqUlAjhnV9SghISIf3ylPQdc5EUjLKYSzsFZ0YpSomNgHpmlPZiTcUojVjUfjzvPGfHmf8oKoQglv7186pDANdnYIwlXTbMyo4kkrwyKzkqO7JEsTtIWTWGzjretT84Iez66EMHXJtVG6dnFisabbGuF8sSRaSUv75EklEW9112MMp8bON03bKqDePcsW40o+y02AReVJ1VFUr6MT0/zlhUrReELxYM0ggpemE8VpvHJznZK/YHX5xSd95ROS87iuTeH9etc7wyrZiWLcu664VDGBcxcSSZdD5Cs+ossldbV43hylFFESvKvnNO9etirPPb22gGqfLndi+OvhbHIuJR2XFmlDGrOnbuiLsMBAKPhq/2e6lAIBAIBB4Xj11AW5UVP/2//J987Dd+D+fsqYm4Y8RrfDlmNCj4mX/6UW4cHAJw8dwZ/sU/+W+/QmsbCAQCgcDbC2sdL1xfcGNec7j2E//OOcZ5zP4wJYtfjWmrO8uy7rgxr7m5aLgwyTHGcbRuef7CFuK1fqEH3ra8HcRZIQTvuzhme5Dw4s0l435y/qjsmFXVPbf13DhjZ5CQ9jGQb5ZtXTeGWvt79iz26kuiJBcmOefHGavW3NdVN0wUQgiuzao+Qq5lmEZs5RHlrKY1lqZzPLUzYJj6603VJbTGsmw0lba06xaAqvWxi5EUyDiiiCWVtgzTiDxWGOcwfQSgNhbdF6RJIdhKI84WkgtZh+iOqNuWo7JluO3H+Pw49zGSjUYKSWstO4UXCuNIkSnZO7Qc51Yv8P6bv8Cl5SceahytE/w73s8/dx/hs/YSQnihykmL8/mICAcWH7N40gMkpWCcp8T5kJkruLyUtLohjb3w6B1qAiH935EQWNmLcc5Ra4PE7z/nvPNMW4sFpAPV96Qp6d1hzjocXnhyDgop2BumvHNvwBM7Bctas240s7I7FQm4M0iwzgtu88q7vk5N1grBOI9JlGDZeDGmNY5F1eKApjObbckTH7mYxhZrJaum4+xWihTw21+YUiRqI+xGUvDZG8uNK2vVGDpjWbcG3PE4gLWWOPIxkp2xTAYJ+4Nk8+EzjxVl6x1tVWfuKaDlicI5WNQd1+d1L9Q53v/EeNMT9qBMCh9h+okrc+rO8EevzCg7Q9LHkp4U4F6ZVhyuGw5WDevGMMoitouk30eO26uWJFJUrWZWdRgDSSY2QlnVGWIpePmwpEgVZWOQAvaGCaPMR0te2nmwa86xiGidY1kHAS0QeBy8He6lAoFAIBB4XDxWAe3zX7jCT/xX/yM3bt3e/GK/c27tXoLaSaSU/MgPfDf/08/8LABXb9zijz71YnChBQKBQCDwBvDC9QXXZxWXp/6b/8dOmHtFOhWJnzA9GUe1qjtc/8v8fRfHj3r1A29i3o7i7MVJzu4g4cq0JIsrzoyyt9w3xK1zm/vzY/eKc+6ewlkeq1PC2fHrp+uWZe27oXYGyeYacey2At+RNcoims4wrzR1Z9kdJLj+/azzMY2IGGshkoI8idgZxF446MfUObfpvBokku1Ek9mK1WqOXlsQIJ0jVoLWWtaNZtILJVns4+9yYG+Ukhxf95zlqdkf8P5bv8CZ8nMPNX6tU3zMfjMfld/FLbXfr7vD9t1iOC+4Cuc2UY3HH4eEEGwXKVE6YC4GHKxhXnVEUpBECqe9UCgFCCmIpaSzDiUhlRJjHdpA1RrSSJFGkCYRAkfVepFOSoG1fnyPxTMhBFmkSCIvwIyymPOTjG94aofz44x/+5lbVJ3v2DoZCTjKYureWQi+A7DpRc6TnWh54qM1by0bRB8P2fYi7f6WdznuDhLObuXe/ZdExJGkbDSfvr7kwiT3nXit5taypu5iWu2YrhscMEgU4ywlVt7phoBJFqGdo+ksTe9qXNUaHOwPvYiWRF5g9MLuvV2Fx+fA7WWLlDBdt+wMkocWz457zI6qDm0st1cNsZI+ZnGQbFyckfQRmmVrmJYtZe/4O9ljJoRgf+SvodO1P+c646MqnXV01rLoBc2qP6/ObKWbeNUL4+x1nWcnORYRq86wbszrvyAQCLxhvB3vpQKBQCAQeNQ8NgHtxsEhP/53/ntuT+eAnzBw/TcCpZSMRwOO5ssHWtZf+M5v5R/+bz+7efwbv/uJIKAFAoFAIPBlcnVWcWNec3laMq863rFbPNCk4Mk4qsvTksvT0k/8DpLwLdfAhrerOJvFimfPjnhmf/iW7CiRfYQhQK0th+t2E5P3etGNe6OUpjNo6zueitQLVI324oQQvtPrmERJzm5lGOuwFiaDGIGg7rwLzjrY62MUD1ctUSSoO8t2kTJMIzrjiJQgi2AoKhK9RHcNTdNhjSaJFAhonCOPJa22FLHv36o6Qxp70SkSAolA2o5njn6L99/6KJPm6kONW0nGL4tv55+bb+e2GREJQeK8UOqco7HGC1d4weN4PI5HY5inxNmQpRhwWMG66dDWO6k660BrtPHnzqAXqKQA22mMFRSxwCpJjYXekddoQaQsSgriyDveJF4gTSKFRBBF3iUWSUHVWbIILm7nfOjZfb7j3ft88vKMIlFcm9VcnGQoefr83Rsm/bYIEqVZNpq6M2SxIlGSSPnjaV52tNrSai/0SCm5tFNsIiKf2i0o0viUGHvyelB3mturhturFj2y1Nr1rqx4s061NkTKO9SSWDFQEps6lo1mUev+2PVjvz9KN1GLx869e2GcP+5nVUvcR1+eH2cPdWyc7DFbt4bOOKrOcm1W0WhD1RpkL4jmiWJeveoseWq3OCWenWSUxeSx4uVDyyiLe4ead8vhfFznMFMkkY9hPDPK2B+lr9l5di/UA4xTIBD4yvB2vZcKBAKBQOBR8tgEtJ/8e/8zt6fzU46zD3/wG/mR7/9uvu69zxLHEd/yff/Ra8Y3HrO3M+G9zz7Np158CSHg9z/5wlduxQOBQCAQeBtQd4YXby457GNgHlQ8O8nx818+LBlmLS/eXLI7SN5UbprA4yGIs97pszNI3jJxZ9Y6ZlXHrGy5vWz44uGaK0clw1T5XjHj0NadSo8Qwu+zYarojOFw3ZJG0jtirGUr9tvuRRM2UXUnSWPpO8xiSR5FDLOIedXSakPdGYaJ77tSUpMoQWcc61ZzbpwxVJYBFbQr6qZFGx9d6HvMjj9k+L+zSFH3Asp03SCE78lyFmy75msPPsbXHf4/DLrpQ43bUo359ey7+aj+ABU5K6dRwiKFxOF7yI5Fx86+Onix9BGMRZKgsgELN+ByJVhUHVIIlPK9ZMp50a2zoIQjjbxnrUgUjXGkcUTbGbSDWAmGqaLqvPjUGoNtHBLvsmqdj3BMI0UcSbJIspVFG6FuZxDz5HbOu8+P+fpLEy5tF7x0a8UgidDWboTQk9zphkojRaUNdev3n9//hrL1cYvaOnb63xPnxxnPnR3y3Nl7d/+dvB785ucOuLlomNcdSgie3h/eJSzFyju4hABjHLE6jsOMSSPJoupY4LsHs/64Oz6O7+wtO6ZqDY22pJGk1oZzW/eeuL4X9+4xc33HX0zVGsZ5zO4wQQpB1RmuzirWTUerHVt5TNkaihOi4t3jD5GSPL1XUCQxcSS4PqvQBhLlX7M3TNgbplz4Eq+h5oTge79xCgQCbzzhXioQCAQCgUfDYxHQfvU3f48XPveFjessSxP+7n/+n/DhD37Tl7zMb/769/KpF1/COXjxpcvUTUuWvjUmJAKBQCAQeLNxZVrSdIZrs+pLiqM6ZlIk7NSaa7OKcR5xZVry7NnRG7y2gbcSQZx9a1F3hivTkquzCm0cs7LlT6/NuTarsA68xiBQSjBMFMM0Rinhu6ZwGOc4WnfMyo6dQUqjDY02G6Hg+D3i3q2WJ6c/nuRJhBCCWEmqTjPMol6s858jVC8CpLEkUZK9ImIr6ti2U6K2pmy7u1wxnbFEUoDwLi0A1Ucglr2z59J2Qa5nfOPiV/iaw18it+VDjdssOc/nn/ghPjP+EJ+73WKP1rjORwWiQUkvoGlrvQBxYhUlgiKNKYYDloy4UgrmdYcxrhdEBFEksb3gJ447vZyjM+DwcYp5ooj62L7tQYyUkqrVOJ8TSdP52M0Tuh0OHymZKu8FXNQaIWCUJZzbynjX2REfeHqH5y94UWuc+1jNURrRaB+BeS9H1LEbalFrorpjkETeeacN07VDCoPAcXaUUCS+x25/KyWPX//j6iCNSJRk3XRUjcEOuEuIBe+qO3ZENsaQ8er14vjaMa86EqWZrmGcx/cVdo9ZNRr84Y5z3LMn7X7cr8dsq+pQc7h6VFH1IuMoixmmEetas2o6qlYzTCOWtY9i3B/dO3JxWnYIYCuPObeVE/XnZmsc23nCUdmirWNWdlyYuC9JAKtas4mfHaThGhwIPArCvVQgEAgEAo+OxyKg/d+/8MsAm3iXv/M3/uMvSzwDePadlzb/73B88ZXrvPuZp76sZQYCgUAg8HbEWsfVWbX5NvzDxlHdyflxxqxsma5bsrjimf3hmzKaLvBoCOLsW4ers4oXby5pOsO0n6S7fLjmlaOKWdmxajSDJCKKBInyEYiH645BGlEkqnf7CBwOZxw3FxWmV2sqbXhCFBhrWbemj9rzItxJhomPeRymiqOyY8dav7xe9JEC0lhxbhizm7bEeklbV9w4ahhk3ll0EmO9aFOkEc56Ea/qvHjTGYepNc+kM/78rV/luemvo1z7UGN2M3+Gjw++l+m5D7I/Krg0jLkyn7KVxyxqH8lnrCOSXtDptN8Q40AgyJKIoshp1IiXm4RZ31UVS4kUliyKvFhjLW0/lq4fh2MdLo0UUSSJpGRcxDS9CJPFkr1hwbI2TNcNaxxV57fbOrCANpZ1K6h1S6oEgyxhlEZMiohJkbI7zNgepBvHU6QE57YyXjmqyCLJwbIBuKeIFinJziBhu/DdaG3f9RVJH0m4PUx4YjJgf5gwrzVKyE0n3mtxsGwYZtFGCLTOsqj0Xe7OPJJI4cdh3RistcgTkZNZrGi0Zdloslhye9WSx150y+8xodwZy7zqyGNJpx1ZJMnuI7TdyeGqYVq2HKyau3rMtvKI6VqRxxGr2rCoOsZ5Qq0NCB/luD1IaI1lUb/qmLtTvFs3mlWt2RumxEr5CNU+IjNWktb4GNVVbRjnjnWjH0oAPGbVaLK+u/FLeX0gEHh4wr1UIBAIBAKPjkcuoC2Wa1747EubaMZvev97+e4PfcuXvdx3PnkRYLPcL75yIwhogUAgEAh8CcyqDm0cR2XHOI8fug/lTmLl+1WOyo4zo4xZ1b1lYusCbyxBnH1rYK3jhesLbsxrDtct12bVpiMlixVbWUTZaIxVSOkw1nHUeCdToiTLuiOJpBfRlBcVilihjXf4SCHQ1rGoNBaHAEZZxO4guSuKTgjfn9YZw6zsekeNQEn/mjOFoHBrluURkXG0xndcxZFfjzZSDBK1OS7K3i2TKYlKhO8dc4551bFff4Efcr/K1x/9AfIBhJuTvDL6Ov74zA/y+fg9zGrNWaFYNh2LpmOQ+C41HGjtXXmVs2gL2vrYwyKLGOY5pRzySpNwtOzoTEMcCRIlkEIwjBOw0FpLhxcnYykQQiLxUY7GWjpjSa1knEe02ve5nRml5IkilorhVkQeSw6WEtE7kASOrjUMBwmJlBRp5HvKIsnuMGWcRwxThbGOT19bcLRuef7CFlIIdoYJwzRilHmH2a1lw7A17AwS1D3OR9G742Ij+GKjqTrLMIu5tO0dFIMsYt4730524t3zWHWO6bqlM5aidy8uas2sbNkp4lc/HPo3ZpTFXrRtDMvWMM5O/34bpRFNZ1g1mqaz7J0dEUlxT0Hw+rxGCMEwibCJY9WYTR/Ya9EZy7V5vek/PCmeAUTSj/ntVYuSMC1bdgYp2nrHoXGOUeqdmScdc3nszzfw4tnBqmGYKkZZxIVJTqIksRSnBOlJHlO2vgOp6sxDC2DHIuK5cUakBJM8CGiBwFeacC8VCAQCgcCj5ZELaH/86c+dKsb+gT//oTdkuePR4NTj+XL1hiw3EAgEAoG3G8u6w1hL3Rn2h/eOhXpYhmnErKqwzrGsg4D2diWIs28NXri+4Pqs4vK05Kjs2B0k7AwTXjpY44Cqj1xMY1jULWmkvAPIgHYOJb0jTThwznG4ajlwjiKOaLRh3WpSJbkyXTPMIs5u5RuHzL3YG6Ucrr2IMK9atvOIrSHU6znpuvVCVd2yO0jYGyZ0xnlxqfPv1ZaGJJK9SGAZphEOR6IUt8uap8pP8Re7X+Frzacfapwsgi9MPsifnPlBDot3AlD3Ys7NZc12EaOt5eaipe4sthc/QGAtGGHJ4ohBntPGQ27qjJuLlrL1Li4lhHfMOUgjSdP5aEacF8qSSJJFikEqSSLvAFo3mrqzKCU5XDe0xgGOW0u4OMm4MC64tarp+t6u85OcQaKIhePg4JAz+wM65wXOcR7z5E7BxUnOhUnO9XnNlWnJqu42guoo6+MWRwlKSrI4Yhn7Pq91oylSRd4LcVIIrHO02lJ1htm628R3DtKISZGwP0xYNvp1oxOPWTe+N23dWHaGCUkluL3uWNSaStu7nGNbuY89HKUxi7ojVfJUXJmUgjSWHK07skQR9665O6MNjyebL+0U1NowTBSrptz0gb0WB8uGznhX5zCN7inOFYkiSyRFpEAIbi0bH/fZ9wxGShIruXHMpZEXL8d5xLTsWNWaYarYH6ZsD2J2++vinYL0uvWRpa2xNN3dHXavx7GIuNN3Jz3qSffjbsZjMdI6H0M5SBWjLGaSx0EICHzVEe6lAoFAIBB4tDxyAe3waH7q8fve88wbstxBcbrstKzqN2S5gUAgEAi83Vg3hlpb31P6gHFUr0eeKJzzE+/rxrwhywy89Qji7Jufq7OKG/Oay9OSefVqr8q1WUVnDC/fXiMRxEqwarwAJIFUKZLUxziuW82i1igJWRwRS8G6tdxuGqSAWltmpWbZaJ7aGfCOXblxyNyLREme2i0YxBV7UUW5uk1TNyxXFQvn0M6hjWPV6N75FlEkIHCkUUxmhofoAAAgAElEQVSlLatKs24NkRJUnSES8HT1O/yV2b/hSf3yQ42RFjGf2/kwf3LmB1im5zY/N8ZxsKyRUmKt5WjdsmwMzlqUEMSRYi9WdNZiLeRZiolHXNcZ86Wh1S3W+u1tjcU6UAIiKTbCgHXe8TdMI4ZpzO4w6Z1ekqo1HK4allITqdMdZ0JYytby4s0lSgoc/rq8XSRcmOREGOziNs+eGZBn2cbBtG40R2XHMPNi2lYWcXlacnlaIoRAiKzvW4vIIskwjbg29wLGstasakPZtpzUlYTwkZRFKpEy4XDdcm4r3fR4vVYn3p1UnRdNOmvZH6Zo40gbv92zsiUfn/6MGEnJziDFuobWGBZ9h9hJEc05R60Ne6ME69xd/WKzsuXytGS78MLUKI+Ylx1CQN1ZXitJ7dgxt6w1znHf61WrLeMspkgislgiheQLt1csqo6y8wLj8XGxrDs6Y5mVDdv9sbA3TH2n2iDmie2cZd1RdYamszTGn3+RkszKFoGP/7yzK/D1OCkiprHi0k7xUK//crizm9H2Drrjioi8j5SMlODiJOfSThF6nQJfNYR7qUAgEAgEHi2PXECbLU47w3YmW2/IcjutTz0O3zMLBAKBQOBLw7pX+4UeJI7qQThezpcySRf46iGIs29u6s7w4s0lh33f2bF45pzjcN1yY95QtYZYCehdJ8Y6ys5QtprOSiQCa71Yo6SgbA1p7z5yDlatptG+/8ohWXeGedXBPa4LAt+xFaMZJyWxOODQVKyamlemK1rtHTlCCpJeQCojQ9v3PAFYJ7DaIaV33oxiwzc3v823Hf4ik/b6w42PLPj90Xfx2bPfjyh27vr3yzPfSRMrh5OSNI4oYslR5Y/7c1spwzRBKkkXD/n8QvHFo5ZZ2SCljyv0fjFHJCVC+DHQ1qEktAaEc+SJYqdI2R0mjE+oNXniXXyttbTat4flfTeWlP0+wAsMSgouTgrOjVMvvtWnz51jV9StZUMW+36cURZtenZePiwZZi1S+Gv6dhFzY15zYZKzlcccLBsS1TLOHc45v797cSPpxbGjdUskDfTbNK866k5zY95snGKuj9i80wF2TNP5yErn/PafGaXMqw4lBQfLhq0svsvhNcoiaq3BxczrjnnV0RjLKFG0xlG2tnd4eYHx2N3RGcv1ec103bJdeEHx3DjjwiTnD794RBar1514PnbMrWrfP3aviEvw52ISKc5uZewMYg5XLXmiOFw1rBtDZxrAuxEbY1jWmmEaoZTkie2cYao4N86w1vHpa0u0Pb0fnKMXWL0Trkgizt7HAXov7hQRnzs7emQC1b26GetePDtGCC+K+r49wyuziufOjrg4ye+/4EDgLUK4lwoEAoFA4NHyyAW0JD6di962HUX+5WU2g+9WO8l4a/hlLzMQCAQCgbcjUohNbcyDxFE9CMfLEYL7ToQGvvoJ4uybmytTLwBdm1XsDJKNWLJqDY02XJ9XALTGx/ulkWRRa4QQNEIzqzTa+Bi4VhscUKQKgSCNFEparPMiRaIkrXbM1g3WDblyVLFuDJd2cpQUREqSmArVrnBtiTaGnUxyMLd01kfzrRrNstabDjVHxFHl3U6CV+uvlBQ8UWi+rf4433Dzlxjo2UONS5Pu8Zlz388fjT7CzUZRNoaClnEWbwSQ26vWu5DwgteF7ZRl5d1b87pjp0i4sD2gGG2jigmfvlUzrWZY50VCnBfOlBRIBEr5yEklBbU2WAvWWR+JmEQg8WKbc6d64yIlkECioGote6OM7SJhlEVcn9fEStBoy9N7A86NX1tMGKQRw84wXTcMUsntZcOFSc6kSNipvag2ziMi6cXUm4uG6/OaJ3cKLkxyzo29k+3Y+XQshKWxJI8VNxLF5w9WHJYdTgiUEEzLlqazZLGg1ZaXbq83y98fpXdFlZ28pkghGOcxWazI+0nl+/WxbVwbQpAow7xuOVo1WLx7KVWSJJLESnC4alg1mnnVIYTg0k7B7iDh3Djj+QtbfaSi2IiInbH3jVQ76Zjbiu8ttBlrWbeG7cIfX0UScUhLrMQmjtD1wjH4a6A2vh9NGx8Rumw05cGKPJYbJ2Bn7SmRadF0NNpgnOPavEIIKNKIs1v3/2x+PxHxUQhT9+tmHOcx+8OULJY+9tQ56s6yrDtuzGtuLvxxa4zbdPfd2bUYCLyVCPdSgUAgEAg8Wh65gLY9Hp16fPtozuSOn30pfO6lywCbbzaOR0FACwQCgUDgS2HQd9Y8SBzV/8/emwZZmiVmec8551vvmmutXVXT3dMzkmZkJCFGIIFAC2JzBNiAHP4BAeYHxgZ+YEwYcNiB8BbGYYxxOAgcYcAmHA5kg4iQhQSSB5kQ0iDNCI1mX3qpvSozb971W8/iH+fe25ldWVWZ1VXV1d3n+VNVmZX3nm/N+533vO97WsrGrGOVummIUfqwEsTZFxdrHbfGJaNFg3OOi8O3J9HLRjMpWhpt0cbR78Rrt8kwj0mU4F6jiZWkNd5dJgUYB612OKcBR6Qkg05MnijGRUNHCoQQXB8VOCCWgsO54FrfoooZRje0xq+Ed85xe1LhrO9rcYBcupmcc+BY9pyBXXaEGevYkTN+j/00v+Xgn5O58kz7pOhe4fYrf5i9Sz+IlRH5uGIrakkjw7hsKBtDHiu0cdwcF8txwvlBwrhoOVw0FLXm0kaX3a1tXDbEphmldmSxYqsTUzSGaCkY4hzaerecw//ZWpBIDM53iSm1TtqoWoNYikYrnPUOKm0tWax4aSPn3CCjl0bMKh9rmEQSJU/nWtjqxCyWQmWsGi4OM4QQXBxm6wi/3X5KHPkYzhujgsHSqSaFoJ/F9LP4gdc9mNfcOCyYlq13QbmaRjsWjaaTRIxLTSRbqtbSyxSNMRwsGi4NM7aPRJYdvaesJn0HWUQaS9JIkUbyoX1sgyxGG5iWXvhcdfc5lp1gjeHGYUml/b68MMzY6iaksTrmZhICLm/kVK05JiKexFHHXBKdfAxGSyG2m0Y02nDzsGReG1rjyCLJII+JpKC3dNZpa5mW3oEWKcHtcUm0FNe0dfTTiG4WMYiTY110OzrhK3enRFKgjWNStvzi6wdcGGR8dLdLJ43WglTZmEeKiM+Dk7oZLwyzE8XKTuLjMVeC3zu7+z55efhcxhwIPAvCZ6lAIBAIBJ4vz11A293eAN5eEfrFr36Tj37kpXf9ur/8a8dLv1+5dvldv2YgEAgEAh9G+lmMFOJUcVSnZV5rsmUnyUmTqYEPB0GcfXEZly3aOA6LlmEeH5uUrlrDYdFQG0OsFP3kwf2cxoqy9dGJg9Q7Z1adRFmk6KWKOPLHfiOPkVKwqDVpJOkkithpVDNCHzYclpJBfvwx5fakYlq0jIqGRlt2ev7kKWPvdFNS0E+jtShxztzje6c/xXdMf4EI/c7hPpL7ndf4xpU/RHv1txJHEc55USqLJfNa0BhDFsulYFIxKf3EfGsd3WVn16I2DDopGxubZP1t2qyDkpLa+H6Zea1xeHeR70eTRFJQaUurDVIKpPCCSw2gHWkk6SYR3VRRNJYCL6AlSpInCmste/OaqtXEkWSzEzPIE/pZTNkYuknEvWlFHEnKRuNc8lAnjlu6eBpjlyKOpjWOXhax003ophHDPOawaDnXz7gwyHAW5lXL9ZEXEzdOuMCtc9wclYyKhqo1jIuGWvu4TydgZxlLudVJSSJ/Dh0uWsZFu44MXTkVxdLN5iMhfW8YgJSCS8OcbqqotXtsH9tmN2bTxRjnRVnf72e4splzadmf9bg+rStbHW6OywdExJO2/6hj7p0sas280uz0fBTlMIvZm1XMa8NG7q+rbqNZLP8tpURbi3OCzY7vbKtbw515DcB2NyFPIs71H3SVRVKw28+4MMiZlC1ZLLHWrR13O0eEylUk4sNExGfNw7oZH0es5IndfZvdJMQ5Bt63hM9SgUAgEAg8X567gPbJb3mVJIlpW1/Y/DM//0v8/t/129/Vay6Kkp/+57+IEH7V587WJlcvX3j8DwYCgUAgEHiAjTw+dRzVaWiNZVK2XBhmREqwkQcB7cNKEGdfXGZVi7GWqjVvx9stWdQGY72brJ9K5BH3krGWWe2jG6WA3V6CFBLtLFL6yb0skWRJxCCLiZV3nQkgiyRX+4JzyQJRl9w4rGgHKXUnIU+66/vOYdEyLb14Nq81kRJYK3hps+OFK+OdcYvGcKl5gx9c/BM+vvjlZaPY6Zlf+M28ee0P8Vb6ce7Pa9r7Bc46GmuJpB9zoy3awqxsmdUaHERKIgV0peCj53qkcUy/H3G/zWijDoPc7xMAbSyjRUPZaIyFXhr5aD4hlo4pw6z2E//GWFQiEa2hwdFYR2QsiZWkse98E2habeimEa11zCpNligiKdjuZewuhcbGWAReXLLWYRxU2pDHxx8HtXWMFg2zqsW6t4W0aaW9U04KJkVLtBT4VpGEvTTiwjDDOcf1UcGbBwVblebiOxxCN0clB4uavXnNrNIkkSSJBI2xbHcThllML4/YXo67n8WYrh/T/rxZirL+uF7d7iwnkQWxlJStQeD3nRCCixsdskieqo8tkv53Xp5GvHWwYF5pLm3mfNvFIZc2MvpZvBZ+TyJbCkrGuEeKiCc55lYsas3evKaXKsCRKMVh0bBoDOf6Kd00QskGnBcRZ41hmMm1IFfrZQ+YgETKdSl42RpmVfvA/XHldLu8mfFvXBlSNYav3psTR5LtbsJ2L2Gzk6wn1R8nIj4rHtbNeBbe2d33tXsztrvJc9uGQOBpEj5LBQKBQCDwfHnuAlqaJHznJz7GZ371iwB89vNf5nO//hW+69u/5Ylf83/+e/8Xi8LntgsBv/m7Pvm0hhsIBAKBwIcOKcWp46hOw51JhRC+w+byRv7QCcjAB58gzr64LGpDpb2wkMXHj0ljLOCwzj1wvIrGYKyjbA1xJEkiPyEdoYikxLmWNFIky06pNJJ0YsF2bJmNx2RNi3WSYZYwto439xdcGlqUgMubHe9YOiwYLVoO5jXp0qm12YnpphGDPMY5y+D+5/jE/j/iSvHFM223E5LZlR+i/71/gt7Oa+zOKub7CyyON/YWTOuWeaWptY+EXIkVkRTkiUIJQdl6IW2rl3N+awObDpkWEYuDOVuJWotnANNKo41jVmt6qaI2Foujagx5oshVhMVHauZJ5IVLa0miiEb7Y1DUq7hMQ9kaOonCCcFGHrFQXjjxzpt8HfvRGou2jlj6BybnHI22HL1kauPv10rFlNpQNQZtfazkvPKLH2ttWdSGXuajEO9Pa84NMl7a7Kyj/IQQ9DLfUTUuGoZ5TC+NKFvD/VnFvWnFtGrpJIpJ6VDL/rN+6sWzdwq4Sgp2+ymdRLE3q9mjRghBN1VsdhMfZ5gpDuYNDu9iU1LQS7y4dpo+tm4aIYWgNRYlBB+/0OfSRs73vLx16t9ZlzdyDpcRqA8TEd/pmEsjhbGWUeHPs16q2OwkTMqWJFLM67fFM4BBHjGtWtLYx6C2re8wW9SautUksQIHO32/DydlS6I0o4UXwaLlOI463SIp6acxeax4dafL6wcLFrUmUpKXt7vs9FP6WfRYEfFZ8bBuxrPyzu6+G6OC186/+yqJQOB5Ez5LBQKBQCDwfHnuAhrAv/17f4DP/OoX146x//y/+9v8L3/tL3Ph3PaZX+sf/tSn+fGf/Ln1awkB/+7v/5FnMOpAIBAIBD48nDaO6nGsOnKubHVIY8WVdyHEBd7/BHH2xeVotJx6Z7Tc8uvvrFpxzgtnK0dP/g43x+pVlBB004hzXUnHFah2wWi6YDRZcGWzw8bSdfRq1OWNg4JZrWlGBY12TKqWWdkwKlo6ScRu38cHRkpyvhvx6uwzXH79x+lNv3Gm7dUyYe/q7yH6jX+E3Ysvr7++20vZn9XcGTuklFjrt2uQxSSRJF5GDbbGC1BVa0ijCFRCOjzHSG4ymWtao7FOHOu5cs7HN5ZLp1Avi5GNxlhHLbwY1k0iYikojcVYvwfzOCKSYJ0mVYos8f1eHRsxqzXZUph0DvJEMcxjtHVER5yC1jnfGyclOO80a41bj2t/0bDQgqwx1NYfzzSSxEpgrKNqBKv52doY5lNNJLygduuw5OvdGd96sc8nLw/Z7CZ87d6MYR4xWrqG9ucLbh6WLGrNtNJsdGIipTg/yGiNZVQ0REqw23swanDFSkS6P6uZxS23J4JBHrPVTWiM4a0D7/p6ecf3cx2Np3xUH9tR3u095XEiIoCxfr8fzGuq1rBovHNup+eFKm0tm92YG6OSXhatt3vVdVa1Xtw0xrJXG8Chje8YXCx7+Vpj6STKO1RqTRopppVmq5usnW557DsL57XxPYRLd54E7k4rslh5J51gHbX6vO+xj+pmfBKOdvdlccmru73weyPwviN8lgoEAoFA4PnynghoP/C93823fPQjfPWbbyIE3Nsf8Sf+/H/BX/ozf4zv+02/4VSvMZ7O+Vv/+//NP/onnz4mnv3WT30HH335yjPegkAgEAgEPticNo7qUYyLhuujgs1OzHY34WPn+yEuKRDE2ReUo9Fy5h1KmReBBEp6h86K1njRrdWWOJIPdDqlsSJTcLFr2VJj0qJmXrVUWjMpWrSxLGqN3Mg4P8ioG8O81tTaca6fcm6QYqzDWucj+YY5SSTZTCzfOvk0V7/8D8nKO2fazkJ2+fWt3834tX+L7//218iT449D37g/Z1w0aOvIIskrO126aURjLONFy7zRKAR5JBlkMbVVHJqUb04Vr981pAcjOrFaC2dH90nVWqyDqjFksUJJQSdRlK0XPYrG0EiLlBLnDHYptEgBnSTCWrx4Fis6SYTD+e4wHHmsSJVks5PQGEuCwDi3ftiTy9jM1XOTW8YzAuzPG+/OsjCvDd0sRuBjFa3zsZO1dkTakCgvwCkhmJQNk7Kll0XszzO+eHvKJy8PubyRs91NuDEqyOKSc/2Mm4cFjbHcPLRc3cq5OPQdZs45JmXLTi/lsGhZ1HotGJ1EN43oNYbRoqGbekfabj/lrYMFkRSAoNFu7cA6C0/jniKEeKiIOC7LtSA0rzWLWnNR+q66fhYRK8XFjYw744rRosYBWx0v+M0qzWhRY6xFW0utDa1x1NqwqDUCHyUaK0EeK+ZLt103VlQOSm2QZYO23kEo8F1pQoCScOuwoV0Kp9ZaDhYNtTbszWuU9DGKN8flA71n1jrGZcusalnUZu3s66bqqTjWHtXN+CTESh7r7huXTyf+LhB43oTPUoFAIBAIPD/eEwEN4C//2T/On/wL/xVlXSME7B0c8uf+yl/n469c44d/26d47ZWrx/5/WdV87fXrvHH9Fr/wy5/n//vMr1JW1Vo4A9gcDviLf/qPPf+NCQQCgUDgA8hp4qhOojWWO5OK0aJhsxNzdavDhWF2bNIt8OEliLMvJt1ULfukvNBz9HB0UoWSEEeSSlusdUgplhPuDmMd6Sq6UQo6aUQ/MiSmoC1niLnmvjawFG/sMhLQWt/PtKg0d8YlUgp2+inTUrM7SMiTiK1eQq0Nm50Orw4ML9/9KS699RMkzfhM27dIdnnjyh/g8/3fgVUZr2z0qI3j6F3p3qxif15ze1Ixq1pe2swZLCfbx2WLlKAEVNoSxzGl6HOrTbgzaRkVNZ0komw1UwFKSrJIcWnjbcdMYyxuGYnYSfw9VElJP428EGkdRaMfiNCEZV+WgEh58WywdFIl0nAwrylqTW+QMezECHy/VasdKy0qVpJIifX+99H3glnVMq81s8qgre8Ea4zDWkttDK32QkttLLKOgBZtvXAn8PGKdyYVG50F17a6bC4dDFmseO18n1d3e4yKxu+fOGKzE/PqTo9uFpEnEb1EMSpabowKWmPZm9fL8/Hhj6krF9Ws0iSqIYsl1jl2+ykO764rak3yHt5TThIR7dKx2c9i9uYV96Y1eazY6qZsdxN2+uk6KnReG7rLiNC9ecW8MpSNYVb7KM1hHvu+otL/Wy97AFFyGVVplw4zR6MNVatZJBEb2pLGCucECChbS9lYOqliECckSyE8ixVFa1BS8MZBwf1Zw6WNHGMch4uGV3e73DwsuTUu0catt231bP60OtMe1c34pPTSyIuZS0doENAC70fCZ6lAIBAIBJ4f75mA9vFXr/Fjf+Hf5y/81f8Rh1uvhvzKN9/iq6+/tf5/qwWwP/6TP8uP/+TPPvD11c/FUcR/+Z/8B+xsbTzPzQgEAoFA4APN4+KoVh1AxjnKpXtkUrYIIbiy5WO0Lgyz9esEAhDE2ReRfhavJ87fOamcx76XaW9Wo63v7xrmMcY6jPVRjb0sYphK+rIhsTN0WXA4rylbjVxOqBscWjuq1tBoC8LHA46KFm2hk0jiSHJYNFzezOmmiixKMdO7fOrgZ7j2hZ9GmfJM27XofYTbr/xh9i/+DpyMGC4a7s0qrHMs6nbd9VJrwxv7Cw6LlmnZcnkjp59F3BqXTEvvrplULZ00ob8xxCQb1E4QtRWd1FC2EXns3WSToiGNFbNKc+uw4JXdHiDWPWQAkXrblZMnEY1xOOcogEVj0cbSTX2Hl3WORvvnJbV0DIEXwopGs2g028v4v3ODjLq1zGpD2Wp6mX/c871bXvTS1hJJgRQwWjSUjabUBvAinzVeDMFBFPljEkeSXhYzzGMUgtp4F5ixjn4Wc2dc8flbY5SE7W6ynoSVUiCFYKuTsjdreO1cn2vb3WPHaLubMK9b/1A3r7k/q+m1hq1OjJIP3g+UFHRSxaRsaYxjVmle2vSuCYc/H1+Ee8pREfGoS+vKZodfvzVhu5tysGh4aSNnc3m9jYsG6yytsQyzlL1FzbzUTKqWqrXkiaKXKKSUVMs+N4kXX1ttiJRa96uVjUYpyepU2+6l6/Nu9QzdzyI2O74z7iiDPKa1jt1eyvlBira+i2xetewvan7lrREXBtnaXVctxbMVQvjt3+zED3WvnYZHdTM+CdY5jHOMi5Zv3J9Ttd6R97Qcc4HA8yR8lgoEAoFA4PnwngloAN//Pd/J3/irf57/7K/9LQ4ns7WT7J39Cid97ej/3Rz2+W//0z/Lb/i2157tgAOBQCAQ+JDxuDiqkybMLgwztroJ6XJ1bHggD6w4GvclBCwagxQ+xu7upOJwUbPRSYI4+x6wkcdESrDZibk7qWiNXU/A5UnERsd3gEnrlr1fkkh6J8xOZtlNC2S7oGpaJq3GWse0apaij6BoNWLZiiaFF0CUEOwOUrY6Cc7BtNIYa2k03J1UROM3+Y2j/4fvvftzKGfOtD2TzU9y+5Uf5XD3U28/OABZonDOu8jK5u04yjuTikYb7s8qhnnCII+9eFa0HJYNDsXO9g5Rd5PKRjTaIvCdY3kTkcaGTuIFA2MdB4uGWAnuTir6ecxuL1v3kMGxIQEwWApdQgis9WJJ3Qqk9DGHjdUkSmIcaOOYlA11a7HO0Ul8R9sgi/n4uR5fvDOjlyoOi5Yta70bLpZI4eMgjXU+SlIbtPGCqLVefFo0BofvbluJYDNjSWNJJAXdWIEQJFZSNgYhfNRjB8nrewt6acRLmx1eO99fb9tpXETr/h4hyGIfV7ioNd1lj1cSyfX9oNGWotbcm9WcH2Rc2+pwbbvL+UGKEHB3Ur9QCz6k9N1CR0Xp88OML9+e8tbBghuHBUJ450jd2nU0am0s88oLt7W2a9cZ+EjFSdkyyCOcU9StYVJBN41RAoyDVhvK1oulK4dYN45II0ndWs7104c6/ZJlp15jLMb649NPIz57fYR1vpfvrYOCfhoxzGN2eylZ/PYxqlrLrGq5O/FOu6PutU9cGhzrp3sUj+xmPAOtsezNakaLhqr1rk3w7tlVBOrTcMwFAs+bsNAtEAgEAoFnz3sqoAF8z3d+gr//N3+Mv/m//gP+2b/4DGbZq/C4z8fO+Yfv3/n9n+JP/3s/yoXd7ecw2kAgEAgEPpw8Ko7qaUc2BT54VK3hxqh4IO4LQEgf4xcpmNWaeWPIInnMeRLE2WePlP66rVrDvWnNnUm1FjV6iSKJFBeHGbfGJf0sIlOOvmyhmTGZz5kV7tjn92ndYqzvQ0I4sjhCLuMP00hhnGWjm5BHio08QSyFnf15w2D8BX5o/M/4WPE5BCesrHsEo3O/mVuv/CizzU+c+P3VHcm5ZSwi/s9704pJ2eKcY7efcFi0zMqW0jhkNiTrb2FUwqKxwNvCWxJ5Z5daCkl5EnF5I2dRa2pj2Z837C5asiha95Ct3v8oQgiGeUyiBGWj6Wf+77X2/WOzuqWfxlC3RBIiKelmilgKxqVmp5dwaSNHSsl2N6E1hnHRMipadnspQgg6y763NJIUdUskE0ptqFuDFNBaL87183jd4bZotP8Z5SM+Vwd5VmukFOz2EtJIUWnLpGi4MSr4/K0Jr+721k6e07iIBIJrW116qZ8A7qaSWaWZ14ZF0zywWINlz9b5QUo3i/jWS4P1/WCzW77wCz4e5hxpjf+daqzfn1Vrqdq3xTMf76ipWkMW+x4+bS2dJAZq+nmMwztDHYpe65jVDcYJWu1jQKvHiGfwtljlHNjlNTitW/JI8fW9OYmSXBhmfOeVjfV5dZRO4qM2V06XlXtt1bv3ycvDU+2nR3UznpaDZSxrawyzSnNYtNxfuml9j5x9ao65QOB5Exa6BQKBQCDw7HnPBTSA3e1Nfuw//pP8qT/6B/mJn/l5fuXXvsSXv/4m2py80vTVa5f51Hd+kt//u76fV65efs6jDQQCgUDgw8nD4qis85PkIQIpcBK3xn4yu27NQ+O+jPOTxDjIEy+ebXUTNjtJEGefI1e2Otwcl1zayLkxKhhkERudBCEEu72UREFGQ2oXuKZgf1xQNdo7kJKIeBkPVzY+Wg7AOUc3i3Esu8OUBAexlAyziE4a+Qly57g2/1V+391/xOXiK2cat0Xxja3fxlcu/AGa4UdIY0nWGDqxfMDpsnq6EI9V97AAACAASURBVMJPzsPK+eaYlF64AphUBpIeYzKSrENpBc5a3kkWKZSALJEsKoNNHZGSbHQSJmVD2RruTSuSSNLLonWEnjaOk07hNJKksaKzij7sSu5PKxrtXWC7vXR9TNSyxyyWajkZ6sWpnb6PBtzqpuzPazqxoptGmGV3WT/3TqeyNZS1RluHsw7jfIzmSjxrtKXV/thK6Z2i4AXxqjUMsgglvZBStZavV5r7s5rrBwX3phUXl5OyZ3ERbXcT+lnE/qwmVg3D3EdbNsauF2skSqKt4/YYdnspnzwinsH7Z8HHSc6R+9OKSvt7ZSdRTCu9doNNSn/vFMI7FvMkopdGgOOwaEEIYiWPR7dlfntvT0pSJbg/rXj1XP+R4hm8LVYJARLBwaLhcNFStN51qKRgoxMzLtoTBbQVsZJc3eowyCKujwqujwqEEOuuvMfxqG7Gx2Gd4+aoZFQ0zKqW0WIlxDqGeczVrZyXNjtsdZOn5pgLBN4r3i/3vUAgEAgE3o+8EALaiovnd/hTf/QPAn+Qqm64tzdiOp8znS3IspSNQY/drU0G/e5jXysQCAQCgcCz4aQ4qsCz5Wj04ftFtLTW8aU7U+5OKg4WfnLYOffIuK9x0VIbSy9VsJzw+ehuj14WvbDb+UEiW65GN8Yxr1qujwoiJdjpxLzc19xcHKDiGd+8PyNWkiwSzCtLoy3OtXTTCG0dk6XTxC0F0cYs4w5jBQi0tWz3EqSUDBLBq6N/wbff/8dsV289bojHqEXKr3R/B/+y9yNMom2YgpyNfXRV5l1UG3nMVjdZiwpV4wWILJLkydJlVbfL6EjDuUGHkoQ6G/L1kcEBO+LhPjgvfngX0KI26364QRYxr1u6ScRh0bDVjYmXPWSRXLrVeHDictYY1NLZNcyTZV9Tw7lBhraWrZ4XlpNIkkWKvXm9dOmI5f71AtOljRxjHVWr2ZvXFI2mbA1XtjpejIss+7Oaee2jIeetRQnW+6nRlrLVxJEX1Pqp7yOrWsO0bMliSZ5EbHUTlJR0U8lGJ+betKJuDV+7N1sLaGd1Ea3Gf3GYMW8MZaN9XCUOiVgKhYJYCi5u5OTxg4+0z2PBx7u9L5/kHImk4Bt7Mw7Lhknpoxf7WYw2LZEU9LKIPFJEyv8e7mex702zjlp712ESibXIFUtJogTaWMrWIvAxrY+jWbqyEiWREm6Py7Uj8OXtLqNFw6zSJKrhwjBbi9EPY2OpfL15UNDLGr52b3asK+9hPKqb8XHcHJUcLGr25jWL2qz73kaLmjjyrthhJ6GTRE/NMRcIvJeEhW6BQCAQCDwbXigB7ShZmnDtpQvv9TACgUAgEAgE3jMeFn34qNXELwpfujPlzrjk+qjgsGjXPRsnFduvJi8vbbxdbJ9Gkk6scMC17bB46nmxipaLJByMZywO7xFNa4appKc0cwnn+imHhT9GgyxCCE1RG7RtqVu7jJBzJJEiUYooksRSLGMTfd9aXxm+r/x5fuOtn6Lf7p1pjHPR49PZD/Fz8W9nanPMzCEo/LUQCUaLhjiSnOtlaGMZly3n+hmbnZiiNSSRWk4meiGhbCwGSd7pEw8u8LWx5fa0YFZrrmw+3iUzzCNmVUs/jZhWeu0iy2OFAKa1Y2/eIIUgjyOyRDGvNL00Qh2ZxKxaQ9UYBpkXq+JIMls0XN3urq958PGNeewdZUVt2OzGvp9s6Spyzi1dZMvovaLhjf2WzU7MuV6f3kbE/WnFeNEwrVrSSAGOWHrXzqLRtNoSR5JurMgSSRrJtQNqFR3YS6O1Yw/8eXFvWnFYNLw1KrDWIaV4YheREIJ+GtE/wS11MK8R0ouG3fThIsyzWPDxJPflRwlFR50jrfGi3FZeM61bNrKYYZYQKS+KSeFFJX/dwWjRcLCoGZe+J63RzVpQVNLvw2nV4ICisWx1UlpriU64D79zG1eCb9kYWmMYLWp6WcQgj6m0YV4ZhrljUetj58HD2OgkbFWa2+OSYR5xY1Qc68o78Wce0c34KA7mNaOi8eJxbdaRlcZaFo1hsxOjpKCXHD8u79YxFwi8CISFboFAIBAIPF1eWAEtEAgEAoFA4MPMaaIPT+pt2U2frCfmaXJrXHJ3UnF9VDApWz6y3Vk7EB5FmLx8AXCOT+xI3qindOIJ+7Li3qTk/tIJIyT0UoU2EbNa4xBr94lwPsrQ+TTOpTvJf88635F2Lir5gerTfM/ez9Kx8zMN7UDu8P/mP8IvZd9LYROkgGEkiZd9ea31bjhjQRrHnUnJYdFweTPHWsesaigaw24/RUnBIItASGSS4boDDiuLbBWzqmFaGbqJOtbF9zBWkaPWQWMs09K78ZJIoaR3X2kH41JjgVRJFgLmS7caeMFiWnlnV7qMUDyYN/RSxW4vpTaWVEn25jX3ZzW91mCtdwn1M+8E09axP/OOT2MdrbHcn9VMK0OivHvsG/tzLg8zpmWLXDqUylaDg0aDLFriKCKPFXEkEUsdbn9ePxAduNs7fk3Hyo99Xhta7YXLlUvqSV1ED2Nea7KlUHUa8eZp8aT35cf1DK2cIy9vd9mfV+zPKuZ7LdvdlEHu3YuJkmTLWNJVJKGxlro1zKqWujU0xtIax0qXFWLZY+ccZasRwtFoS/6IXXZUZJISytYyq7S/ppfutTxWFI3vcCtbc+pjcHGYMS4aRouGLC6PdeWdxKO6GR9Gayy3J9XafXO0721UtAj8NbPdTR4azfikjrlAIBAIBAKBwAePIKAFAoFAIBAIvEA8SfTh0d6WQ9dytxTr6KnnTbWMbztYTi6fVjw7Spi8fA8wLdQzaGYIo3llIOiKDGsNvdS7jyalxlmYN4bGOJwTsIxq7GcRjfEimVBeEEhj6bu1rGPXjfidzc/xm4qfJ3HNmYZ2Q77ET8gf5oudT5FnCdo4eqmiE6sHJt+ttSxaLyrESmCt48Zhwfl+xmgOUsJHz/W4MOwg4wzyDXTjmC1mFM2crNJYZ2mNZZilpx5jP4upWotzjint0hFkuDTMSCNJ2Rp6qVrGY3rhYVo2CBzaOsrWEi/FqnnTspEn7PRSHzvXjbm6mXP9sAQhyGLN7XHBuGw5P8goG0ttLF+4NaHWhsPltTevNQB5otDWkiwFroOipaw1+7Paiz9AJMD6t0cAjfFRkiiJNo5u5vf3Siw8STCxzvl+MuO74lZi2ZO6iB5GayyTsuXCMCNSgo1HqUFPiXd7Xz5tn1YUSS4Ocm72S25PKrJYstN7+zx0zrG3jN4sG82s9uJnN41IlGDReOdgHisvGtctjXas3nHRWO5Pa4ZZ/Lal8R0cFZk6sWJeG+b1cUF51cvWGLvuOzwNsZIM85jDwrtCVyLro3hYN+PD2JvVS8dcQy+N1uLZotbMK81OLyVWip3+o6/vJ3HMBQKBQCAQCAQ+eAQBLRAIBAKBQOAF4kmiD4/2tsRopi189f6C3e3N5z7+G6OCujXcHpd+8vyM4tmKMHn5nGgKaGZQF+BWEornfD9jI4+5M6m4N63Y7vq4ukpbJkXL/qwGOowWNXvzxrtgtO9bAR8xeNnc5oern+Y7yn+FwpxpaLd7n+Dnst/Nz8xfJosUrXaIxrLZTdYurXcipaSferfOvG5JlCBRinvTCoBXz/UxMuXCpZeguwFCkCYLsshHDE5LTWu8KBhHZ+uIWTmyhBBYW7OoWyZFy2bPi35SSDa7MY0x3BpXzCrN/rwmjST9LAHlYxtf2szpZxGxUlxaxvsBXNvq0ksbvn5vRhxJdnspsRRrV1rZGGZ1C3iX4NXNDhvdmFRJtnopZWPWXVY6kvSyiEpbnHVsdBRKl+x0EzppTJ74eMlILvu0BPSymGEePdSV12gvjK1ch4vaLI/J2V1Ej+LOpEIIH1F2eSN/Ll0+7/a+fJY+rXODDCUl/TSiaAyLWq9FoP3ldTatWqrWkieKXhLhcBwsGoSwFI3GLselhGCQxZStpjW+125Rt+zNG3ZPEJDeKTLlScS0ah8QlFeuUx/LerbFGr00YlyWWOdO5Ug8qZsROPF3i3Vu3c/mHOvXXtS+C7CXKvpZxKWNnOQUIu5ZHXOBQCAQCAQCgQ8eQUALBAKBQCAQeEF4GtGHX7k14rAR3J813BqXzzX60FrHrXHJaOEdNheH2bt6vTB5+YywZuk2m4NulsLZyaSR4iPbXa5udZhWfvK9bCx202Gsj3ab15qDecMb+3NuHBaMC83H7Nf5PbN/yrfWv3amoTkE++d+C7+0+W/yhnyZu9OarK4Qwp9fnPLwe4EtZla1OOcjFDf7HWTvHEW2i0sHawfO0YjBw6IG57+uHuEUOhEh2O17N9J06azJE4VE0BhL5hSF1sTSi1eJEtTaYoFeonh5t8dmx8debncTdvrpsUn+1lgWtSZSgqubHZJYUjSGRAruTCoa6b++20+JlCRa9uDs9tO10PMtF/qMy5av3Jny2estkRQ4JdjpxsSl49XdDlGc4JxDCEGsBEkklwLjo/dH2RrSSGIcpLE6Jqyc1UX0MFb3gytbHdJYPZfex+cdSZvFiovDjFuHJYkS7M1qwItD81ozrXzX4DCPj7hyBf00xrmW1kpmVYNDkCe+hy9WMcY4tHbMa7uMwJTHnIQniUxFfbKgvDq2Qrwtpp2WPFE458+Xlcj6OFbdjM45ro8K3jwo2Ko0F98hYi5qjbaOeWXopL7bb2/eLDsHfRzqZjdei9KP40kcc4FAIBAIBAKBDxYvpIDWtC3zRUnTtE/8GhfObT/FEQUCgUAgEAg8W55W9OFLGxlf1nBYtM89+nBctmjjOCxahsvenndDmLx8yrS1F87aORjDUbfZ45DCR+WdFJdnnWNStvzslyxXp5/lu5t/zEfL1880NCMU13d/gMOP/Tu85c6xP68ZTyqkgDSWlI2hnyo6ie/RaiL/d/UIQTWSAiklVsX0B1s0SZ9bleKaUsccjUcjBm+OCvLEXy/GuSd6WOokEf0sIpIxUgp2el4U2+knnO/nXNrMMMbx5sGCUdEi8eKYkl6sOtdP6SQKZx2F0ZSNYV5rJmWLEIKXd3q+v0nCZNHwzb0FWay4tt1hmCeksY/w66bRA+KGEILNTsL3vLLNaNHwVW2YVhrrBErCMI/JzxBducJYR1EbuqmiaPyfR9/7LC6ihzEuGq6PCjY7XgD52Pn+M7+3vReRtN1UcXkj56vZjCTy3XV3JyWLxiCB6gHxzJMnikpritrRWlgVs2WR9OeXEmSxRDtD2WhGC+gsz/VR0Z4oMs3rdt3vdlRQbrTv30uUJI3Pdp9XT+he+8SlAeDP4V7mYzTHRcMwj+mlEXmimBQtZauZlg2dVHGjMQg4Hod6RtH1rI65QCAQCAQCgcAHixdCQPva69f5J5/+l/z6l7/BN964QVnX7+r1BIJf+sm/85RGFwgEAoFAIPDseVrRh4M8phM57k5rLu+Y5xp9OKtajLVUrWG3d/ZJ+JMIk5cPx1rHuGyZVS2L2kcnSiHopop+5sUuiYN2sRTOqke6zZ4UaTWbb/0Mv+8Lf4fO/K0z/WwlMn5944eYfOwP09m66MW4+3MWtcZZP7neGkcWKza7CYmSxK1h0WjqwpBGahkb6N0wzoGxXhpUUURnuMl+m7LQio1YsJXGHMxrWuOIlPBuOueoGoOxDosXeISAVjvSJ3haGi0alBS8tJVzrp9hraPRjmtbHa5ud7i80aGbKn7wW8+zqDXf2JtTt76z6bBouTUuOaorCAGp8m6hLPaCirGOu+OKRa2ptOW7rm6yeYZrQwrB1e0O48K/58GiwWqBtk/WnThaNGtBJcol3SSimx4XeE7rIjqKdY5J0fLWqGB/6Y7ayGMcbt3z9Sxdqe9FJO3KEfnSZs64aBlkMXVr2JvXTEpNN4lwzouuq3NeG0djrBe2pGBrOU5tLcY55rUBJ7BAHkeMyxbrHG/sWyIlHyoyScS6Ku2ooFy2hlhKhBDkZxQxzRO614QQfPLykM1uwtfuzRjm0fqaGZf+mtmf14zmDdNak6cRm534xDjUs/AkjrlAIBAIBAKBwAeH91RAe+vmXf6b/+nv8rkvfGX9tafSdy+exosEAoFAIBAIPB+edvRhPwa37IJ5ntGHi9r4TiUH2RldCQ8jTF4+SNV6YfTWuEQb30tWtgbnQAroZxGpMKS25FzacK6rSN+lG/BEmgK+9BO4f/33EfN7nMXXMaHPP41/gF/p/yBpd5PhYcwrqiKNpXczNd4xU2mLNpZ+mrDbS5BCMC69UFMZS9Maav32eaGkpJunyHRAFfdpjaCua3LE0lGj+dz1MReHOY22REp4AcJa7s9qQPDmwWIZW+ijFs/CovaRlju9hFgpzg8ybo9Lzg8zrm13+a5rm8dE4FXE4o1RQRaXXnA7cjxXMZmHRYuuNbGK6WURb+wv2JtX3JvWdJOIm+OSsjUPxD4+isubHV7fWzDIIsZlQ2ZgVmn6Z0xFPLrNjbZcGGZIIY7FA644jYtICUGlDbcOS+5MKma1BqCfxoCg1BZrHZ9765BI+X61K1udp+5Ge68iaVeOyK2u35+r86ObRNStJY0k0+rBpJZICnpZzG4vozFeKE8jwazSHMxbhIR51ZLHikXtO9H6acwru10G+ckiUxr7PsGjgvLKbbjZjYmkWPeznZayMQjB0iV59mN2eTnGk66ZNJLESqzPiyxWJ8ahnoUndcwFAoFAIBAIBD4YvGcC2i//6y/xH/3Y/0DdNGvRTIh1FcETEz7TBgKBQCAQeL/xtKMPlYBBFj336EPr3IlxX++GMHl5nFvjkq/dmx1zLFWtIZKCVEk6oqIwBcpWdCJYZBG3IsXLO13O99+dALCmPITP/5/w+X8A9fS0tWQA3Be7/NP0d/KZ9LdQ2AhdO1JbUWuDNo48kVjn0NYSSUGzFMeSSBFHiiySpJFi3mhUrenECucc1kEnSyAZUEY95o2PmetnEb0s4s6k5MZhSSQFk7LBWMe0bBkciaSc1y1Na3DOMV5G2mWxOrXraFFr9mb12gF4aSm4TMqWC8OMSIkTIzCzWPHa+T6v7vaOOQrvTituHBYoKeililpbDhYNe7Oa66OCWa1Z1JqLw5zRoqY1hoNFc2qnzWYes9NPmZQts7JhruFg0XJx0z227+ykbe4kCilYdrCdvK2ncRHNqpbRwh+jdumIi6VgXrckkY/z/MLtqXcldmKq1nBzXPKx8/2n2vn4XkXSSunFn6o13JvWTMqWi8OMea3Z6CYMshjnHNo4HL4WMFICIcRSQI8ZZBEImJaaeW3Y6HhRrm4teazWCxM2uwmdVHFhkJ8oMuVJtOzCk5StppdFa7dhP4vY6iZn7kDz/WvqoSLraXjYNSNgHet6bbvLbi859bn8MJ7UMRcIBAKBQCAQ+GDwnghoN27f48/9lb9Ovew4W30ODXMigUAgEAgEPow8i+jDbhoxbsxzjT6U4njc19MgTF56rHV86c6Uu5OKg4V37uAcO/2Uj2wm9EVF1E5p2oaiallow71py/2ZWMcIToqW1873EGeSvI4wvQ2/+vfhyz8B+myR69fVVX6+93v5cudTSCXZEDB03o0yLb1gUraG3rK3q2otG52ISluiSBAryJaT+ytxZpjFNMYRKYWOu8xFl8JIrIWNjly7IG9PSialpjEOYyytdWzk3v31ym4XJQTGOarWrvuu5k3NvNR84c6Uj+70uDBIH7rSz1jv9pzXmu6yQ2qrk7DdS7k+KhDCu4kub+SPdIJK6f/fRh7zpTtTrHVkkeL2uMQ5xzCPOdfPfCyfddwcl/STiDyWXoAqWra6KcY65nXL1a3OI4+1EIKXt7vMq5a744iDyot9t8YFF4edR/bLnbTNjbEM8uRU23qSi0hbyzf35lStpJtGzGtNKgT9LOLSRs6ljZwskutjNata7k68C+/SRo4xjsNFwycuDd61aALvbSTtla0ON8cllzZyvnBrghTejXu5kxErRWMsrbHr2NZYeadYFstj255Gkn4acW6QcrhoSWPFtGroRIrWWs4PUq5sduhlMeOioW4tFodEkMaSLFJICb1UcVi0pGVzzGG52z/bfmmNfaygfBZW18xqP3ZTRRYryuWigqdxHrxbx1wgEAgEAoFA4P3NeyKg/fd/+/+gbtpjwlm/2+EHf+t3813f/i1cvXyBbicnjd/dB+pAIBAIBAKB9wNPM/rQOUdtls6QueHr9+c02sd5rXuxnlGcYzdV5LFCCKhayxPWBR0jTF56vnRnyp1x6Z1HlebiIOOlviM1BbQFWmuccyQSkk7MRiemNSl7s4a7k5Ki8d8H+NhZO/H2vw6f+7vw9X8G7mwxml+UH+dnst/N6+kn6KQRWaSOCTNxLkljxaRswMHerCZPfLfV/ZkGB4mU9NKYo1qQALI0ppv2KKMBtZZIbem94+lmb1ZT1L4zTRvHVj9hKAXby76nTvL2D3QS+J6Xt9jsxnzm9RH3pzUHsxpnLJMy59JGRhJJpBBY52i0pWwNRW2QAnZ6Cf0sZquTcGUrX8f1XdnqkMaKK1uny0Y8eqwPi5btbsKFIz1h92fV+hreWr2ntYyKlv15TdXq9crEa1vdR77XTj/l4jDn7qDgYDIjVoJpqdGmoLO8nk+zzfFyPJc28lNv6ztdRJ99a7SMYfSLLF/e6XB1q8tGHj8ghHQSL4C2xnJnUnFjVDCv2vU5/snLw1Pt60fxXkbSZrHiY+f7GOPIYsn1gwJtHekwI40UOY+/F/rfATW9LGK3n/HRc33mleb+TDEpW5yBadny5TsztroJzvkeNedY99kJ4R2bjbEUtV674VYOy7O68u5MqlMLyk/Cqj8ui9VTWzjyNBxzgUAgEAgEAoH3L89dQDucTPnFX/n8uvBYCPjB7/tu/tKf+eMM+o9+wAsEAoFAIBD4IPI0og8bY9mf1dzYX3BQCwbzmtHCx+A559aT4M+yMyhMXj4bbo1L7k4q7kxKqrrmSseQ1WP25zVGG5JYkEU+lu2oSy9WkksbGb1UcXtSchvvOhp24sfHOToHtz8Hn/t78NYvnGm8FsFnxHfw4+6HuBt/hEwqIutwjabShm4SHxMk0kiSxxGNMXQSybzWGOuQYtVB5siPiKdpEqPSLpXqs7ARVWUB+8A4ZlXLfDnp32rLuX7KRhZTa/tQR6MQgo+fH6Ck5LNvjrh5WLBoDAeLGmst2RHBTQiIpWSzG9PPlh1Sw4ztXsq4aLg+KtjsxGx3Ez52vn+q6211rK+PCiZly0e2Ow9ESNatdx85B0nk96OSkt1eSidW7M1rmNcgBL20eWScY6Iklzc7HM4K3rgNlbZcSCM2OjHzylAcidt/2Db3UsWs0mx1kzNt6wopBWVrvFvOebH8pa0OiRLMK820ateOqDyJ6CVqLajFSnJ1q8Mgi7g+KtaOv82lQPNueK8jaS9v5BwuGs73M/ZmFTcPK0aLhnP9FCUfLlyZpZg6rzS9pTtwsxtzbavL9YMC53x86a1lb95mJ6FszfqcWiEEa2fbrUnJtNSkStCJ1dpheRaeVFB+GNa6Y/GNq/05KmoSJRkXLZc27LuK3nzajrlAIBAIBAKBwPuP5y6gfe7Xv4p1bu0++7bXXuG//ov/4VOJVwgEAoFAIBB4P/Juow9XkX6tMYyLhrEW3DysmLeAA20dtbbPvDNoI/c9O5udmLuTitaEyct3S9Uavn5vxr3RIft7+wxVw7Sw3G/1ejFaLCVC+O6fYR6z1U2O7fdVz9etcUkniXhjf8FGHpNGJ4gczsLr/9wLZ/e+cKaxahHzufz7+On0h/lGvQmAdA7jwGhLox1ZHOFcS2u88LJ6BugmiqYwCCmQQjBrNL1UgLPkaYSzjiSOiLIutRowsTFVbXAnCGewFBEWDWWjKRpNN43oJl6MW7lr0ke4ij6620Pg6CWKr92fo42ltpbLvZhEqWMOnWgZI7eKs7s+KhgtGjY7MVe3OlwYZqe6zqrWrCMkD4uTxTM4Luy8UwTspv7x7v6sJos1t8cl/Sx6oNvqKNvdhI1ORC+CC30fxWgsXBimSCFOdCVFUjDII7RxTEp95m09abvvTku+ubegkyj2Z/VDHVFKCra7ybHOrtV+evOgoJc1fO3ejO1u8q4WCbwIkbSfuDTg9b05u7OMaWlY1Job2tJNfFRhEsl1BGmjfdzkovFdYDtLl+Vm1x8bgMubGXcmJdZ5MW9v1jCvDZeGGcM8oZsqIinQ1rGoDZOyYVy2tMa/p5KCO5OKb7t4NhfrkwrKJ1G1hhujglvjEm0c1jnK1qzPk6I2HBa1/761fPtLG488/x/Fs3bMBQKBQCAQCARefJ67gLZ3cAi87T77I3/o9wbxLBAIBAKBwIeaJ40+dM5x/bDgcNEyqzSjRU1VayIcvSwmTQTXtjqcX0ZuPevOICm9u61qDfemNXcm1Xri9kn40E9eGs1X37jBnbduc3NvQt22VFKi7YNOkUhKOomkNZZx2XKul7J5xHk0yGPmteH+rKKfKe5MKj6yfST9wTTw1Z+Cz/1vMH7rTMOsRM6Xd34XvzT4Ee61HUZFSy9zKKDU3i2lpEAgKFuNtnIdtdfP/OOIlN4dOS01rbWkkcDhiJWkm6ZEeQ/b3eHQJZSNwR2JknTLTqyjvVCzSlPULZNK+wjQpWvJuJXgKMgfM4H/ym6PSEniSHFnWqGEYH/WcGkjoxNHDPKYXhqRxpK6tdwel0zKFiEEV7Y66+jFT1wanGo/3hgV1K3h9rj0XWgPuREcFXZOcjF104heaxgtarqpZH/mr/dHcb6fkio4P0jZHnRxzlE2hiTyjqMkkkRSECmJWL7vuHjybX3ndt8Zl/yrN0dkSlJrvyjgYY6oXqpojeFg0XBp2aUGXkTbqrxoOMwjbowKXjtrXOkRXoRIWiEEv+HKBovGcHdarRcRzGvD4iR3oJJsdo44Io/sH4BbhxVJJDHGC9sXBynbPe9oq7ShbM2x1+ulMbv9wgJ15AAAIABJREFUjNZY7k29GNtNIj57fcLH/3/23jRGtvQ+7/ud/Zzau7r7Ln2XmeHMcEhx0S6ZtgNFlk2JtmE5cRLISALBUAIEsIDECOJAEBQLMBInthHAQWzA/uAYiRNAUiIQsiREVmJRCiNaUihSJDWkZp+79e2turazv0s+vFV1e1/u7e47pN7fp7t0nTp16py3uv7PeZ7nhuLmKTGO84jNpxGUj+LhMOeNjQllLRnMhOZiJp7NkUqxOSnxHIf3d1JqqXn1evtEJ+ZRXLRjzmKxWCwWi8XyzcmVC2h5sb9w/BMfefmqd8FisVgsFovlA8XTRh/e283YnVZsTUumpaQd+ywnLtkOeA4EoU8YePSbs56kS+4MArjTb/BgmLPWS7g/yOjE/rFCwEn8sR1eag11hiomvLO+yR+8tcXDnZTH44KlRogfOLSigMB3cXFQaGqhKIRinAvGhaCXBCilyWvFzW60EEdX2yHjomKU12yMjbjp1il87RfhD/43SLfOtasTr8fnW5/m/es/gp+02R7l5ML0lq02Q9JaguPgu67p5ZpR1AKlPDRz8c+hloqsUtRKkQQ+oQ84LstLPWq/w706ZrlwcZwnA34hFeNCMClqlDZCmpAajWYnrSiFpKgUOCbqUEiFg0O7EVALRVpJhlmN0hrXmUUEBh7NyDciFQ4v9JvEvkfx7mAmSjj0GiGlUOxmNbuZ6etyHNNbdaMb02+GRLMOq7MKBUppHg5zBmmF1pqb3eMjNqPAnbmxoBLqSCdhvxGQloJJIQi8ipvd+ESRvBSalq95oZ/QacV0k2CfQJHXc6effObXuhchFL/99g5vbU5IC4nwNVlt3E7dOCLwnYXDqhaavBbsZjXDrKbfjJBKMy1r7vYbODjc7MaLtSMOcl5ebT218P48ImmPiiWcFKa/8FYvQStNHPp0E30uhx7AzrRkkJnPi0pKXlppstKKaM0cisdtb+6w/M67Pb7yYIjS5v2/v5sxzCq6MyE5Cb3Fe5VXchGfehEiq1Ka19fHPB4VC8e11ppuErDaioiDJ068ojbO53e2Uyal5N3tFKk0t/vJ4jw5jYt0zFksJ3HUNe86Ds3Iu/TeWovFYrFYLGfjygW0Tmt/z1mzcXGxQRaLxWKxWCzfjDxN9OFOWrGb1mxNS9JKcq0d0Yx88qJAachqyY1mjO86i1g3uNzOIDCD1Q9fbyOlZlrU3Btk5jWeQ0T7Yzm8lDWUU6imIGveejzivZ2Ux8OczWlJOw5Y6zU4fFo4hJ5LMwKZwCifiR7iiXtnrWfEmMBzaccBo1xwwx9Qff5/Jf76/2Ge8xxMk1v8v53P8I3un2ZYulyLIkopURqqWpm+PdelHbkEriKtanzXp1IKIUzo4rQUlEKRlpJW5BH4xlnku9BrRPSX2gxEg3cLn1C6CFWjtbOISZwUNYO0QkhNLiRFJRHKvGAhFdNSkNcSpSD0HaTSbE1KgllnmNIO68P8RMFgtR0ReC7XOzHfttZhY1zQiQNu9RJzre2JjUtmosjTdgwO8xohNbtZTTcJTrz+jSvKIXBd8loeKcR4rksz9JiWkm6imVaSdnT8V7+0FPieiXP81KurM6En51o7PhSR96yvdS+/896ArXHBg92MWsJqO2KpERzq+PKByIdW7NOfdXxtT0sjzM5O9Bf6TQLPpZsE7GY119oxw/zpha+zrMtKa9LZuVbW6lgxFqASkvVxQTcOeDTMudaJeDwqaEYeoecyLmrWR8WhWEKN5vGoIC0Fo1zw7bcj2nGIUMo8J/rYjrg5tVQ8GhVMippJXhMFHtc7Ef1mxLfdbJNV8kyv4Xte6PPVh2Nc18SuLrdCpqVkmOeH3HAXJbICvL4+Zn2Yc2+QsZvVCzHuqOukEUK/GdKKfN7emvJwmPPm5oSsFAipeHn1aFei1kbIeH8nZXta0Yp8uo0AjSYJPJTSVsiwXBinRZFe5DprsVgsFovl2bhyAe2lu2v7/j4aT2kkp5SYWywWi8VisXwLc97ow0qauLhJIZiWT8SzOZmENg7t2KffDI/s2rmMzqA5t3oJuzMnzb1Bxns7Gf1CXHnc1weemduMcgJVbvrH0GxMCranJfd2MrJK0Ah9rrfjI8Sz/XiuGRzHgWQ3rRhQzQZx7iLOcUVscuPdX+C1wedwVX2u3S2XP8pbd/4Kv+d8glxAoIGyxMWhFBKtNVJrYu/JORQHLoEXUNQKV0i0B1p7pJVEKk0SeiSBT2sWOaf9kN7yKqM6pNKSnXRCvxHSSXympSAJXPJ6JpBVgklpuuDiwKMRuvieiYkEKCrjVnMch+1JCZjerrlAMC7qwxF4rksr9qjmEYHdmOVWxFJiHF0fvdnmZjeh1wgu1C0wKWqkMh1Wq63oxJ9tRj6+69CKPXbTGtnUeEc8Zxx4s5g/TV6JYwW0eubka7ga33W43om56Tq8vNq6VGfEw2HO+zspG+OCaSl5cdk4ok7Dc11WWxGNwGNrWsK0BMehFVUsz4STYZ7P3FtPL6CdtC7XUrE1KY2Iq453g/muQzvxQcPbWymTosZ3HULf5Z2t1HR2VZLHowKlFa5jOgDNNp/sy25WMS0F06Lmjx5PuNlrsNZLuNM/2/forUlJLU3socQM59uxz3IzxHNd2rF7pBB7kF4j5IXlBjvTkuVmiO+5vHa9canD/4fDnMejgnuDjFF+fDfgQV5aac6ibX3uDVLWxwVpJUlLya1esnDMFULxcDdjfVQwKQQ40JpdK0UtUUrz++/vWiHDcmGcJYp0LkJfZm+txWKxWCyWs3HlAtrHP/IyzUZCmuUA/OEb73Dz+spV74bFYrFYLBbLB4rzRB9uL4ahJa3Y3y+eVZJKGtdE4HkLx85RXHRn0F7mMV2O49CKTeTWVcV9feBZuM0mIMVMODOUwkSO7WY1w7yik/hMconvn12oaIQeEDJIK1JfsDktuVG9xwvv/QLLjz+Pgzp1G/u4+ynUd/04X65eYnNaoiYlyw2fnawCQKERSi+G/gfFHM91aUbGEVUrPes48xiXRkxoxD53ry+hgi5vjx08FZBEHtpxaIQelVRIpWlGHm9vpYSeQykVRa0WDpm9z5nXJhJSomnHPlJDWQOOYpQLHMchrxVrvdi45RwHpTWVUOS1ZDedRwSGSKVJS8lyK0BrKIVxIb2wvD9V41lJS7lwDcbByUqpO+sFrKSJoByk1ZHXeei7aG0E97I+/j2fdw02ArjRiRaimDtz4s0FqL1RY49HBY+G+VMLakUteWNjwsa4ZJQLOnFAr3G6gLOX+bq3OSmJA7OOtWOztmgNeW3EkmfhqHVZKs2jUUEtpbmJoZDUR/QSmq49c84UtSCtBN0k5OEwBw2TvGYrLUlLSS0VtVDEgUc3CXhxpcnNbrxYIyeF4GsPR0yLmnd3MjTOofjK41BaM0grJoUgryS+59JvRgSex8oJnw/HMY/JjAKPm92ET9zukpbiUkTW+XmyMxMZziqegfnsubvcoBl5uA48Gpr+t4fDnFopPMdddIdKpalnDtbAdUhLQeS75JXia4/GVsiwXAjnjSK97N5ai8VisVgsZ+PKBbQwCPjMD36K//1X/hUA/+dvfIE/+29831XvhsVisVgsFssHirNGH2pt+p0mhUBjuo7mpKVgO60IPU0r8lg7xfEFXGhn0F4cx+Hjt7osNUPe2JjQTfzFndaXHff1gaVKD7nNDrI+KqiEZHNS0Ix8tIYJEvcMvT17aYQeReWyNPgyP5j+KrenXz3fvjouvPLn4Lt+HFZfY5zXyEcjRrmgHQfGWVYYgUAIfej9PHqbDoHnmHMygCjwCaOIuL3MyO8yKQTjsmSpGXK9EzHKXbpxQOA7C8eaUIrttMbB4Xo7onHAVaWUYlIIssq4eUqhEEoTB6bjyXWNMzOcRTnu7Q+LfDP0l00jOGxPq5mrRlMJI8RobQSJi0bpJ8fQO8NgdLUdsZNW9Jsh29OKRujtE9L3bkdrI3Iexfzav9GJGDtwq3fY0XQZUWP3BxllLdkcmwjDSuojnbKn0Yx8WrW5maAZuWxPjDNq8bqf8b3auy5P8or/7/1dE+c3E6W0hkbk0QnC/WJsrXg0ztlNa9LKCFeN0KMTB3zsZoe1XsLDYU4pJNlMfJovu6FvhJ3ArbjTT4y4GRrX4Xs7KW9tpry7nVLWErRxxL3QP17QTUuBUJrtSUkpFMutkHbss9ZL9nWknZWDMZmu41y4oDxnfp48Gub0m+FT9WkutyK+Jwn4yoMRj0Y5t7oxq62IrDaOz1YUMClrItehHZnjstaLiX3PChmWC+Vpokgvu7fWYrFYLBbL6Vy5gAbwE3/1R/n13/pdxtMp/8/vfokvfPGrfOq7P/E8dsVisVgsFovlA8NZog+nMyFhWkqaoYfnukhlhrkm4s6j6UM3CVg+QxzaRXYGHfealpsh9wfZlXQqfeCQwnSMlRPjPNPHO4GU1myMC0a5GZItN8J9Li/OKKI5WvLC6Hf5SxufZTV/53z760XwbX8JvuM/gO7txT+npYkYrISk3wgJfBfHKfFdl0LIfaLZaZqF73k04pgJDR4VPlHh03FqKiEJZtF3SWicle/tpHTigDXX4Q/Xx6SlREiF77oMi5pi9hgwsXqFUKRljeNALTT45vwC46ZqRx6jwsQ/DlIjNB7s2/Jc07XWCD22JiVblFRSUQmF4/BUQs9puI6zOIbyDKJP4LmsdWOkMtfS1qQE2CeizbfjOBwpwO7tGlyKYCXSRP7+Y3EZUWNKaR4OcwapObeXmiEb4/Kpxa5+w8RrTgpB4BmX6+J1X8B7NV+X399JUUrx5mYGjsPNTsRKKz4yPnNc1PiOQyUl06LGd42zbCkJCT2PvDb9f+NCoHF49VqLOPAOCbcAd5eNSLbcimZCm8P9Qcb6uKAQkpd1m1YULITDg0wKwea4YGtacbMbsdqKWGoe//Nn4aJiMk9i73miteZm9+lrHwLP5ZO3u/gudJKAYV7Tjn1Mw5zmpeUmd/sNuo3g0DljhQzLRfC0UaSX3VtrsVgsFovldJ6LgLa81OVn//P/mP/ib/8PSCX5qb/zD/n7P/Of8j3f/tHnsTsWi8VisVgsV8reKLSDsVc3uzFa62OjD9NKUApBVgm8KGBzUpDN3AsrrRAfSeZrbnXPHs112cPQOPB49Xr70juVPlBUuYlorDJQkqPcZgcZFwKp9LEur/AUTdFTFa8MfpNPbP4S3erx+fY36sAn/l345I9Bo3/ov/NKUUrjkooCl9h3cV2HRugyLsSil8txQCrNUfqn77kkUYwI2wx0wm4u2U4L+g2X0BfktWKpEeC5Dq3QiAnX2jFrvYStScFHb3T4yoMhoAk8l1IqstIcs7lYEvgOke+aqEXfoRWZzrNr7ZBew1wTpdRMSkEcuIxycez5vjciUCrTceW75ny9aJqRRxJ4OA4UteIsRpu5oKK1ZouSzUlJq5L0myGe6ywEv9BzifbEQh7VNZi4gu09z3mZUWPDvEZIzW72ZK1xHKiE2ucIPAvGHajRSvNwt6CcxXAWlURITRKe32F1FL1GYPRrxyHyTSRgXisGaUkceIT+k+MxSCs2xub41lJxt98gDnwqodBoNqcF5VChFIc6LA8Kt85sfZzfDHGnn8yOl0MUuLy3k/HGxoRhVvGxW106sX8oGvetzSnjoqYTB9zoJiy1whM7Ns/CRcZkHsfe86SbBKe6qU8j8Fx6jZDNSUnguWSVohH6fORGxwoZlkvlWaJI51xmb63FYrFYLJaTeS4CGsCf+t5v5+/81F/nb/39f0yWF/zkT/9dfvSHf4Af+9FP89Ldtee1WxaLxWKxWCyXxnmi0JLAZakRHIo+3JqUDFITu4aGRuiz1Axoxz6B59EJNOOQc8VKXcUwFA53Kn3LoeTMbTYFUZ7oNjuK01xejWOEm0CmfHT7X/KxrV+hIUbn2+fmNfiOfx8+9m9BeHwM276IQcz51UsChFSMC0FZSxzHwXNM/9jeoZ7nuiRxhArb7NJgWmoqKRHKHB8NDHNB7Lu0Y5/lZojjOExLQRx4LDdDIt/l3k7GSjvm47ciJoVgN6uQar4FAAfPNdeEcdyUCKm50YkW4hlAO/Ipa0lWS/yiZqkRHHu9NCOfViVZH+UsNUO2JyVCad7fSS9UBG7HxvkSB965ROy9gsokMH1oaSloRB5ZKcBxEMq4F3em5bFdg9djxet7tnveqLFeI6CT1bw/yPjSvd1ZhGzC+ijnu1/o7zsuk8Kc50UtWWmZKMrAdclrSTs+Ww/a/LybFDVKQ1oLRrnAc2E3rWhGPu9up4S+i5D6mVytRS15c3NKKwpIAp+XVgJC3zH9Z6UkrarFtSGVYietEMrEhd7pNGhGPv1miOs4bI4LJkVKLhRCKBqRT16bayH0XWLf2yfcToKaRyOHzkxA2tvrZZxv5n3NasHX18cs7RnKz52B/VZIHHpsT0ru9pvP5OSasy8e9BIiTWH/ebJ6Bjf1WYh8l0ejnKVGiNaab7/ds0KG5dK5iChSuNzeWovFYrFYLMfz3AQ0gB/41Hfxz/7Bz/Jf/4N/yh+8/iaf/bXP8dlf+xwr/SVeefE2nXaTwD//LjqOw8/8Zz9xCXtssVgsFovF8nScNwptPnBtxQFx4C2iD9/cnOK7Dmh4od8gDDz8mTC12o7I8xwwzoxJaaLqylqh0LgY10IS+rRCbyEaXMUw9FuaujQRjfUU5MluM6U140KQljV5pRYCTBK6bE1KSnG8y0sqvS8uLql3+fjWr/CR7X9JqPJz7XLeukv0fX8N97XPgHe6aLEvYnD2b/1myDCv6SUhg9QIS2HgkpcSpTS+75JEEURtxjSZVJpSPBFo56daKcx1sNZNCDyPlXZELRWjvOZGN6YUknbkE/gun7zVZbkdkVeCvJZkpaQSCmZOq2bkEXgOv/22oJaKQVYf6gZzXXMdFJWiGUIhJElw/HeObuLz1pYgcB2+/GDE9a7pfbrIGNJeEuB7DkuNgMejglqqMzlu9goqj0ZGyJsURiTbmJTm34cQuA6O6xzbNbg9GC62eZ6osVqqhagvlEZrjec43Bvk7EwrdtKKQVpzvRMtjktaSgqh0BqWmgGjvKYVe+ymNbKpj4xE3MukMEKhkJpcGLdZIRTTokYpjZCKa50Iz3W42Y14e2t6aqzkSewdfr+w3OBGN2Z7Us7iIs1rrqR5PaNZ5OpOWtGOQm50E7qJjwbGuWBSCtZHOaHnIjXcmsU2Gvemg+dAKzY3TrQic/NEMzKOtLU9+77ciugk5ue+fF/SiQOWGiEvr7ZM2Ouec/LRKKeoJJHv0k0u5uv/vnjQS+oA23uexMHFOAnTSiKEicp9sd+0Qobl0rnIKFK4vN5ai8VisVgsx/NcBTSA4WhCEps7yuZford2dtke7D7V9uZfYq2AZrFYLBaL5YPAs0ahuY7DtdnweVoKEwOmNUJprs8G4c3IXwwxx1IxquEbGylRJPYNd+dxbo7j4LkOy82QlXZ0JcPQbzmUgjqdCWfFqW6zUkjWRwUb4wKpjPtwPhx2HIh918TqTSumlUDNYjz3urxGRU2/EdIpHvHJzV/ild3fxNPiXLu92fwwWx/+MZqv/RleXDn7wDcJjaDnOFDWiiTwCDzXCLsqpxQ+W9MSz3FwPQfX82l0+kwcI5wV9WFno5CaWigyNNfbMe3YZ62XEHruIh6t3wxJAo+ilgsnSjvyaUfHf42ZFDVLjYhBWhF4DplQdA9EA4aeSylm14dQJCdoiOujgqKWTByHRuTz1YcjXMd5ph6wg7iuEd6KWrIxLlkfFeeK2ZsLKluTktCrqKTmeifmesd0Xt3sJWcS+UqheGP3bFFjO9OSR6OCWkrjxioktTLntFSa+7s540LweFzwydu9xXHRe9yMgevSb4ZUUjLMjDC22j7abaS1Zntquh7zyohRRlzx6M4ElsB1aIYet5caNEOfjXHJ5qQ6NVbyOI4afgeey1ov4WY3ZlrJxU0KUmmyWhIrxVIS8qHVJr7nMikEg7REKkUtFVklGcua0PcYZhXOTJz2HIc4dBHKfA50kwCtTYdZ6FXcmAm3c0ykYBOlNLszsfl6J6YV+/tckS9nTd7cnDJ5KM4cD3oaeSUXIt1lRJrCAdfrBXwuKa0ZZTW5kISeS791NrfjcVghw3IWLiOK9DJ7ay0Wi8VisRzmuQloQkr+3j/6X/jsr30OADursVgsFovF8q3IeaPQ+s1w0VF0f5AxLWr0zKX08VtdAMJZx1M7DvZFnu2kFW9tZUxqh2FWIXIzsD046A88l1bkUUvJTlqRhN6lD0O/ZRAllClUYxPZeAbH3sak4N3tlEpIRnnNKBdU4rD7cFoISqFIy5p3tlJuLzX2ubyS3W/wA+u/ysuT38M5Q6faXt5pfie/s/QX6Xzo+1huR7zSO18HUjMyEYOh75FWwnRCAUuNgKwSoEFpGJWSVqPHtm6wlYdofVg401pT1or1UU5WSZYaAYHnAJrQd9mdRZTe6TeIAo9uEjDM6zM7UfJa0op9lIZeEhr3jefuE4t8z0VrEEpTy2OOpdbc281YHxVEvvtkUKmZiU9P3wN2FHf6DR4Mc9Z6CfcHGZ3YP5dDZi7sxIERbV7oN2jGPh9f65AE/pliJh8OC8raOTFqTGnNg0HOIKsWbjCtoRF5dIKQ0HdNXOGkZJLXuA68sTFhkBohKysFWW3ES6k1q20T49hvhmxPKxqhd8g1CLA9Nc83LmqKmYjbjHw818SGKlVTw8xhF/HajTYOHFpLgcVaehonDb8dx9kn5k5KwTCvySvJUtM4g7emBdNCkleSSWlcx4HnIKRDJ/YX0YxCKiqpSAsTo9uOzPlbCcW0EHSTkLQUR0ZctuOAUSFYaUVc70Z0k3DRMzkpBJNCsD0t0VozvqBh+zxe1XWcM8dunpd9rtcLcEanpaBWiqKSLPUCQu/ZPuuskGE5C5cRRXrZvbUWi8VisVj281wENK01P/3f/iM+94UvLgYHe79T2uQgi8VisVgs3wqcJwptL8ZZ0KAT+9wbZAs3zlIzPLIrSc8G/btpzbgQDCuHVi7otwO6cUTgO4tBfy00eS1Mp1pW029GrI9y4sCIaJc1DP2mRmuo9rrNztYTp7Tmrc0p29OS3axmc1KgtaYdB/QbIVHg4mEiEcta8Ujl7GYZg6wmDmp8N6cT+3xb/Yfcuf/zrE3/8Fy7rXD5o+6f4tejT7Ob3OVWr8ELzZCXVppE/vmGx53YCBXdxGdrUlLLaCEmrPViwiCg0elxPw/5+lbF5rhAU7HUCGbimxGrJnnNtBQUwogKzdA34pLjoLTmK/eH7KQVa13jSPvw9Ta7aXUuJ0pZG5dmOzKxiFklGBc1wEJEm29GaxaiykHu7Wasz/oKmbkB13oJK63o0MDyJPEbzibYxLNIRSk106Lm3iADOJeINswqHuzmrPViXlhu8tG1zokuOKU0w7zmwW7O49zh994fUmiXUSa43UsWEaN7eTDI2UlLtqalEXtin6VGeCh68UYnWvThdZKATmyi7rTWaDSDtJ45onzWujFSmU7IrUkJsE9EmxTmvJmLZ90k2CeIpmVNXguutSN6jWDhZASOXUvP4g48z/A7rwRKm5sWunHEVloyzY1ztKgVSegRug5SQVmXBDMRN/BcAs8lAVRkonfHhaCSisB12Z5K1nrJsR1xSehRC8W72ymPRwVrs/dtHjGq0TweFYzymnuDHNeBG3uOz3nZG6/qe+a6uAyakUcy+1y6COdcXpu4TzlbG6ILiIW0QoblNC4jivSqemstFovFYrEYnouA9ou/+hv8xm9/kdl3ZeBJ9OKtG9e4e+sGzYb5Im6xWCwWi8XyzUhRS97YOFsU2nHMf/69nYxWXPHGxoTvf7F/qCvp0Shnd1qxNTVdRJGrudWLaTX2d234QORDK/bpK9MPtTEuSMuaF5abPBoW/NBH7O9fC0QF1RSqCUhx7ru83tqcsjUpeDQqGM9cZCvt8Ej3oYlEdGaDb8VgkvGx9Av8yeEvs1y8d67nrd2IN/p/hj9Y+Yu8Pm2SloK10Oduv2FcKu3zd7C4jsP1jukj255WbE0q1noxvu/jhA2udbs8ziHYTllpzeL20orNSYmf1XhAKRVKgcJEBWpt/hx6LkWt+OrDMbVU9BshOLA5KRbPfR4nyjz6LQk94sAhcB1GRc0orymloj0bPgKz7yP7hR+pFA92c9ZHBUJqAs9htR3hOMZZdVJP4Eni91kEm1u9ZCYYau4NMt7byegXYhEdeBxz4W6QGtHybt90dR33nEUtuT/IeDgTCIeTjEcZlKOCUQVJ4PL+IMMfPulXDDyXnWnJIDNrTVZKrrWjI91iAJ7r0gw9pqWkm4T0WxHdJOAbGxPGeU0tNQ92M/rNkOVWRFpKtNZsUbI5KWlVcnGDwCCtyCtxSDxTyghOg6yeuRVDrrVjlg8IGUetpcvN8NSeuvMMv8taUUtz7pVSMS0ko6KmFE/2eVRUCxFYaY1U+88l13XoJgGR7zLOa4SrEAoGacXKMQLeKKt5OMyppKIRekxKcahfczcz0ZfTouYbj8eMCsFaLzl0nM7C+qhYxKve6iWXFlt41M0iz0JZK6alwHOfdIE+K1bIsJzGRUeR7t2O7a21WCwWi+VquHIBTSnFP/25f7FPOIvCgP/wr/x5/vKP/ADXVvpXvUsWi8VisVgsF879QUZZyxOj0M5CrxHSLwSPhjndxOfhMN/XlfSNxxOk0sYNUklWmiGZzyE3yEE812W1FZFXgkGqKGtp4s7GxZl7m74l0fpJt1l1drfZQTYmBduzjqhJUXOrl9A5xamRhB6JW/Np+Vt8x84v05db53rOwmvx1eUf4UvdP8eIFtNMMCkqbnQSVtsRd1cavHq99VSvB0znz+NxwbV2zCCrqZwYp7lM5UTUUtOO4LUbbfrNgD96PKEZBaRVzfqwoBAE3q2PAAAgAElEQVQaxzHDPqU1Lg79dki3EbDciMiFJPZNXCMwc2w2+fqjMRq96F87ixNlr+DWb4aMPQGOQ+iZGL2yNtGb8z5BB9NRVwnjNBoXYtGfBi43u6ZL7NGoPHNP4NMKNgAfW+sARthrxaY3cZhVdJOAVuSThN7CUZpXkmkpGOU1juNwp99YxMTOt3OQh8OcNzYmlLVkMBP4B+OUzcKhnpSMS00nDhASWrFHNYt6vdaOTCzjLB7wJPFsThx4pJURBPNKcK0d89q1Nr/15haB5/DeTsor11o0Qp87/WTxuieBiYacx+6Vs/cl8l081yGvjEOrqCRCaZTSNEMPqTWN0GNzUpCEPq3QWwikB9fS+4OMV6+f3AN4nuG3Qs/63xSjrKKo1SHBz8EBZ75tjg1inf/8IK2QSjHIKiq5v2dxHqW5Ps5JS3M8+o2QV66Fh/o1J4Xgaw9HTIuad3cyNA5SaaZlzd1+w+zXGRikJQ93c5ZbIRuTktV2xOuPxmeKBz0vvSQ4dLPIs/RHVVKRVpI4MI6/VvjsccXPImTM3Z/z62nu9ryMY2l5flx0FOne7djeWovFYrFYroYrF9C+9kfvsLWzi+M8Ec/+4X/zX/LJj75y1btisVgsFovFcikopXk4zGfdQJqb3fM7fvZysxszzEwvVBzkfP+LfR4Mc1bbIb/zzoA48MgqM9B2tTjzdtNSIBW8sNygqBWu65xr0P8thaxnotl05jZTpz/mGEoheXc7ZTerGednE8+8esLt9/8F3/veZ4nq0bmeb+gt84XOZ/hS6weo3QinBt/VuI4RkK51Iz5+u8dHrh8tqJyVyPf40GobL5JUScg3Mo9VF7qNJ0PB0HO51Wuw1k24v5vx+/eGrLQUg7Qmr8Ri4NeMPULfI/SMwHGtHdGOfQLP41o7ohTGBZaWgqVGyG5endmJEgUuoWcEt0poVlsxsS8YpCVx4JDVkp1pRSUUu1kNOIwLsegHDFwztN9Na252Y+4uN5kUNY5jXt9Zo9+eRrABIyB9/FaXpWbIGxsTuom/ELqGeX6oOy8OvFnvV0g0i4E8SgRXSvP6+pjHo4Kd1AhzWmu6ScBaN+btAFabIZ6nWW6FSKXZTedRr+EsutNEb7ai4FTxDExfo9ZGvChrc00tNUNuLyWziEqHr69P+O4XlnAch7vLDZqRx6ORERLGec07WxmTsiavFJ3Ep04rlNYUtUQqRSWMaNUIPRzgvZ2UduzjOkZsW26GrLQjQs89tJa+vNo6UaQ4z/DbxfxsVkki32VS1sSht28t9VzwHMBhId4eRxx4RL7LTlqjlGKU1fv+fx6luT4smJSCD7WbfPRmm7Uj+g0boY/vGsHyrc2Ud7fTmZBsfvaFfvPE11ZLxdtbU97YmJAEHnHg0og87g/yRX+m6zj4nsOtXjLrCHy2zxDXdfbdLLI+KrjbP19341520grXgUbg0UuCM/USnsbTCBkH3Z974zYv61hanh8XHUUKkFfS9tZaLBaLxXKFXLmA9uY79xZ/dhz4q3/5h614ZrFYLBaL5VuKYV4jpGY3q+kmwTPdNQ9mqN9NAnazmmvtmFwoPny9zf2djMh3eX8n5UY3oRn55MXZBLS0FGxNSpqRx7V2jOc6bE1KVlrhmQf93/RoDXU2E87ymWj27HeIr48KKiHZnBR0k/BE8SzMt1h77xe5fv9X8WRxrufZje/yB9d+lLd7f5JKu/RmA9jAdclryW6meGm5wUurLT5xjBvpzDgO+BHXbt5gECnag4xBnfHuLGLwRieilMZlVNYKhWacCzqxT1YKmpGiHftIpfE9l07s04p91roJjuPgu/ujAoFFDKLWmmkpCX2XUV6f6kQxw0pncRzacUA79klCl3EuIK9IfbkQim8tJbiOY0Q34P4wJ8BluRlwe8kIUXktCVwXx3FIzjHMPq9gs5dbs4i9+4OMOMi51o6fadj++vqY9WHOvUHGblYvnGqB5zKepvgueJ5D4Dl04wDfc5FNE5+4NSmZlgLXAangzimCy5x9Dp0919ZHbnZ4OCzwXYcHuxkvrTToN01E4XIropMEbE1KpDSCm9SaZmh60YZZNesmM2J1WSuiwGOUC3BKtqdGKGknAdfbMfXMQTePLNy7lg7zkwXZ8wy/o8Al8ByKWlLP3GLtAy6nwPWQul5EgZ7mFI59DzRUUpNVYuFS2hulOcpNvONqO6adHL+D85hM13G4P8hYHxcUQvKybtOKgmPjHDfGBV97NGKYGhG5chTbaYXjOGxPKuCJkLvUCChqyYNhfqyQex7u9Bs8GOas9RLuDzI6sU+vYWI9p5Xct964PIlm3Os8BNMNmFeSa52Y3ayicQbx9yycV8g4yv15MG7zso6l5flw0VGkANNSEM/Wfttba7FYLBbL5XPlAtp4mgJPOs9+6E9/71XvgsVisVgsFsulYoa7Jg5u9ZjemvPSinyGeY7SmklRc2epYaLtZi6FWki2JiWJd7IAJJUZiE9LQTPyWG1F9BshN3sxX18fP9Wg/5sOKfa4zepncpsdRGnNxrhglNdorVltHz0sS6b3uPXOz7Py6DfO5RoEGC19nEcf+vcYrHwvtdBcqwVVrRdD5EpJKqX4yI0Ot5cSXr7WIvKf9i51B/wA4h5EbXAcXruhEcr8Mh8FOd9Yn/Dl+0PiwJ1FLZp4uEejnLySDLOayDd9WDe6IY3QpxX5rHVj4tCbDZ/9Qw6OvTGIoe+S1QKtONWJ0oyM26YVe+ymNbJphArfdek3Q6RSyJZmpRXRjX2W29Fi+C61RgOPRgWN0MNzXaTSZKVkqRngu86ZnFdzDorfpwk2B4kDj1evt3l5tfVMcW8PhzmPRwX3BtksHvNwJ6MxRjmARmqNj4mCXW1HuK5mc1JS1JJeIyCrxJkGt/scOnv8Vs3Q58XlBvcHOY3Q482NKa/dcBb7FHgua7N+rUoqsqrGxWGQVhRCIJQmLYQRU33jGkwC8wyOY/a7qARvbU5pJz63e41FZGHzwFp60vtxnuF3EvqUwrwv01LQTQJcd7/QG3oOUilC30UobdxoJyC0Jgo9ylrhuS7pbHA+j4ad5Kb7baUV4rnOqbGEe2Myo8DlvZ2MNzYmDLOKj93q0on9RexjWgre3kp5PC7IaxNlm/gey+2QV6+1SYInUaJFrZgUNY9HBRvjkrVegpSa3bTiY2udp3Z7xTNHpZSaaVHz9nZKKyyopOmP01pTSbWYLRjnqbPPeZiVgnuDjGvtkFJoksAz7rsL4KxCxknuz4Nxm5d1LC3Ph4uOIq2lYpTX3OjG+J5D7xR3u8VisVgslmfnygW0INj/lLdurF71LlgsFovlnNieBovlfKSlpBAKpTRCKTYnhblLfnbtRIF7rGhwHEnoobVxwqSlZJjXrHUT3t5KWeslxIHHIK0YVBVTYQZ7ri8XTodKKPJakpUS14GVVkg7Dug3Qu70jQvoWQb93xTUxUw4S0FJLsJtdpBxIZBKM8qNwHBwUNbafZ1b7/w8y5tfOPe232l/D1sf/jHktU8ARvBohtCcDc1rqdiaVGSlEW7XujErrYjr7aeJEHXA8yHuQtSBPULAPGKwFIo/XB/RinymZc36qFi4KfJKkNeKvDYD5k7i00p8HBxeXGnyyurZutjmMYg703LmzHAZpNXCiXIUrmPcbJU04t0grVhtGyE7LQXTUnKjk9BrBLx2o0245z3anBRoNLVUdGPzmEFa4TjQjn36zfDcnTMHxe+nua7cmUPvaR5b1JI3NibszBwvR4lnAL6jCTwHx9HUQrNXJ/Rd4xoc5RVSmUjJJPDwTxkEV0IdG315q5ewMSlZbpgB8NfXJyShRzcx66LrOAyykloqamHWUqEkk1xS1BLPhX4rpB0FJKFHK/IphCIrBePSiNJx4DHKKqaF4G4/Aa0pIrlvLT2J8wy/W6GHVIo4cNlJJcvNwzdPSG2un0bgUUtNIRXHXZ1SmZjKVuSjtCbyHfJaMikEtTQOJolxP7Vjn+VmeKq4sjcm07jfjJstqwVfXx+ztOe82J6WlLVEKU3kOfQaER9b63C9c3iPG6GJi62lYn1UcH+QMS3MTQQAH7/VPXG/TuJWL2E3rdhOS97cnPL+djUTydx9HXXm9RnxtRV5FLXgG48nBJ7L3X7C7aWEx+OSwHOuXMg4yf15kMs8lpar56KjSNdHBc7sM+7W7CYDi8VisVgsl8uVC2jXlpf2/V2Ii7n7y2KxWCwXj+1psFiejqKWrA+N20Mq43456i75o2LrjmNfFNpsEK9md7C3eglZJWlGHltDzbp2GKQ10/rJYGUe7bfUDBZdU2vdmOU9DrmLGPR/4NDaOM3KiRHQLtBtdhRpWc96mST9+TBaa5a2fpe1d36e7u7XzrU9gccXo+/ns+4PMQ3vsLoT8SITrncSIs9BAkUlyWo56+lyuNFNWGoErLQiXr1+NqHqCQ54HkRdiDvgHl7T526K3bRiuRnxjfEYpWGtGxMFHlpr1ocF01KQVUbYEFpTzhyZ00Lw/iDlbr8xczydzDwGMQ5cSmHOedOfxbEi2mo7Yiet6DdDtqcVjZnIuDUtaUVGcFjrJfvEM4CyVtTSDOUD35kJboKVVkjgeQsh7jwcFL+vmvuDjLKWPBrm9JvhsccscI34GHgueS1oxU++KtbSRG8GnkspFEJqxoU4dY0oakkwW++ScP9XzyT0WEp8cqGoaoXvuby3k1ILRRK6JIFPXgse7uZsjMvFjQBKQyvy6CQhoe8Seg6+Z+I91UxM8T2XopYM0po4MK/p9fUJk0JwaylByCdr6UmcZ/g9F8bma3kp5CG34rQUM5cmtByXslYUvjzyd6dpaXr52pFPKRS10hSVZFwIJoUgryS+59JvRgSex8o5zs15TGY38fnyfUknDlhqhLy82kIDu5np79yalkgNr11v8dJq69D1chAjVjUW8av3BhmO47A0G/Y/DWrmNMsKSeR7lFIzySsi36WXhLRjnzjw0GiqWjMuKt6blJRC0klCbvVicODWUsJLK03e2U6vVMg4i/vzKC7jWFqeD8dFkZ6XeRzwnX6DKPC48wznr8VisVgslrNz5QLaR199ad/fH2/t0Ov+MejYsFgslm8ybE+DxfJ0PBzmfPXhiK1pwaQUPBjmAIfvknddWrFHNe/nOSBmHWRfFJrjLFxuWhuBIfBctiYldVXTDTS3l2L8IDyXaPe8B/0XiqxnbrOJiWw8ZVB+UeSVopwJMLGnWH34f7H2zi/QnL53ru1UTsQXWz/I5xqf5kHVYlIKEqnZTWuUSnlvJ6OXhDQj088U+kbc6SYBoe/x0krz/M4z1zdus7hj3GcHmLuRv/j+gHuDbCGSrbZDPnG7S+C6FMJ8ZpQzoaPfDLnZTQg82M0Fu5npMJu/Hy+coUtrHoNYCEU39uk1A1zHRDv2C7E4/w8+Zq0bz2L7BG9tTQk9l5VWyGorYql5dOeT4omjpagku1m9cFuvHeMYOY2D4vdVopTm4TBne1qSlWLRqXbQDau0JvTM2tKKXHazmr4ysYFm32fn9EzoyYXEL2qWGsGxriepFGklWWoER8YLjrKah8OC1XaE5zlMyxqlNKWUjMY1UhUMs4pxXs/EJIfAdeg3I3oN43z3XYdaaUohKKWkFnqfK0lrzTAXhJ5LHHo8GGbktRGePnm7cyY34XmG391GiOuanrxSmBjf+TErauOc6ybmmAWey7SsGRc1wD4Rbf6zndjH91w810VrSCsTX7k9KSmFYrkVHisGn4YRaJoopdmdOamud+JF12Bz5uj73hfaLJ3zZoq98autuOKNjcmic/C8zKMPTbiq5no74pXVFlklmBaSSSkY7+n+NCJTgFQBShnRtRn6gMPd5SYPR8WVCRlndX+exEUeS8vz4WAU6Wk3gBzFMKu4N8hYapjPrg9fb9tzwGKxWCyWK+LKBbQ7a9d55aU7vPXufQC+8MWv8pFXXrzq3bBYLBbLMdieBovl6dh77aSlYGNckpaCdujTbxmnxME4xd20ZpjVs14mTVrKRZziQfJKLpyfzchjUojFkNibDWPXegkNT7LxvuZmJyYIo3PFRj7PQf+FUeVQjaHMZm6zKxYstMYRBd+29at85zd+mbjYOtfjU7fN7y/9MK8v/zAq6tDHIakF721nOC74roPrOjRDH99ziAKPF/oJnuviuQ7XOzE3u/H5Os8cz/SbJV3wDseQ7XUjb8ycFI+GOWklWW2HKAX3B/mid6gdG/dbVkmWmyHJTDhZbXk0Ao+taQnTEhyHVlQdKWQdZO6OfGW1ies6dOKAVmw+o4ZZZZyYkU8SPullmu/7vO/I/JNDO/GPdZ64mGt0lBuhr9cIFj2BJwncJ3FQ/L5KNiYF93YyvvJghOfCxrg40g1bliWTGu5GHoF2TfRlVi86HB3HWey/7zoUlaQZ+hS1Wry/BxlkNQ4cihdUWvNgkLM+zklLQSUV/UbIq9fb1EKRVmZtq4Tia49GZJVEAx5mEO265qr2XYdaaiohTUeXBt93iVwX1zUuL62hrI3IUlaKHE0tFK0o4I2NKd/9wtKR+76X8wy/Q89lqRGyM63wXYdxXi/+b5TXxIFLEvqstEIKIfEcGBU1o7ymlIp26FFJve9nO7HPuDButLySbE8rtqYVN7vRiWLwWWnHAaNCsNKKuNmLqYTieifi6+sVt3rJucWzOfP41UfDnG7ic3+Q8er18904e9C99YlbXZqRz9akZJBWdJPje9B81yQkZKUgLQWPRwVLM+HhqoSMs7o/T+MijqXl+TKPItVac2+QnXgDyF7mUZ6DtGKpEXC33+BGN7Y3K1osFovFcoVcuYAG8OP/zp/nZ/7ePwbg537p1/mxH/00Sfx0X0gtFovFcrHYngaL5enYe+3spBWtyMftJiSBSzveL0pEvnG0yKZmkFZsT6tZPKq5du4uHx7uT0vTJeU6Du04IC2NoAZPBvRgBtyRZzrOOq3zxfs8z0H/M6HUk5hGUV56TOOx5Lus/OE/58U3f5GwHp/robv+Kl/s/wXev/ZnwY/2/ZIe4bHUDFlthzRDD6FMxBpoYt/FdR2+ba1LJz57px4wE86aEPfAP3qwu9eNvDEu+MqDEcOsYpQLuknAMBOMcrHoHaqlZJgZAURrCP39nx3zSLvNSUkcmIFwO/ZPdc/M3ZGFULx6rU23EfDGxoRu4i9c0sM8P+T07DUC4sCdRRCb8yItJfd2skOCW15JttPSiExCcqMTca0dL3oCn5aD4vezctZe0ofDnM+/ucWjYc5OWhL6Lml12EkeuC4+knHtsJvX4AX0mxHb05LGTHQPPCNImLUBKvlEuEg4/JrSUjAtjONNGG1r4XzbGBdklTmfxkXNy6stPnqzzVrPrFdaa6aV5P3tlJudiI1xQSPwAU3ke/iuQ15J8kqCA7VQhL67WB/34YAf+eBAVStiz2GYCzQOj4Y5D3ZzXlw5Peb0rMPvKHBZboY8DM1+lkKyPsrRwFISGuE38mnHAe35Ve44hJ5kVFTsTksUpk8tCTySWW9cUQmGWUVeKYRSdOLARLW2wmeKIYT9zuNJIdieGnFKa83N7tP0Jz5hHr86SCviIOfl1daZO5tOcm+t9RJudGPSUpDX8sSO0WFW7XNvfepDy9zoxpcuZMzdnx+EY2n5YPCxtQ5gbkg47QaQvJJMS8EoN9HMd/qNxXey+XYsFovFYrFcDc9FQPvhf/NT/Ppv/S6/9TtfYnc05m/9/X/Cf/fTP2mdChaLxfKcsT0NFsvTcfDa+cj1Ng+GOYO0PBSFthfPdVhtRzRCj61JyRYlzmwQvtftUkvFaBax5XsOvSRgUtQkgYnvK2rFU97Yvo+LHvRfOqKCcmocZ0peWUzjIcbr8OV/Dq9/lr4ozvXQx8Fd/u/GZ3i39yeIoxBfOARIIs9bCKS1UDNnhUe/FbHcjBjnNY9mg3kHM6h3ncPusSNxXAgbEC9BcPRNbEe5kbenJS5m+He3n3CtHSO1phaavDbxjMOsNq4fociF4LZzeGjcjHxatWSQljQjl+2JcTCfxEF35K1esogjjIOca+34xJ7OwHVIKyM2nSS4OZgbQ+Z9X3eWkqd2ns05KH4/LWftJXVd0+WmgUfDgnd3UiaF4E4/oRMHR7thpzXDyiGrFHFknqsZusYtiBFCHcfBmz0OQEht4jgPkJaCx+MCrTW7WUW/GbExypmUgsG0ZpCVZJXp7GsEPrXUhHscPI5j4h717Hlj38MFhIZW7DMtBGK2D77DogvtJJLAQ0iF6zm4joMQZk3dGBc8HOZn+l3lLMNvd9Z32QhchplAak3gumjMOl4rReTPr1fjpBQSxrlx63muY8RkxyGvFYEnGRclUik6Cq51IjSwPSm5228+sygD+6+tUV4jpGY3q+kmwVNFlu5lHr+6m9Vca8cM87N3a94fZOSV4O3NKaHvMimMmHBQJDvtmjrKvXUeISOrJJuTku1piZCalXZohFrHiFpK6SOFrOEH6FhaPhg4jsPHb3VZaoZnugEkDjxudGP6zZBo5oS136ssFovFYrl6nouABvC3/+Z/wt/42f+e3//qH/Gb//qL/PWf/rv8V3/jP+LG6vLz2iWLxWL5Y43tabBYno7jrp28ljM3zv4otKPY68qZBDWPRg6dPQO39VGB45juslu9BNc1g3jXcYgDj0lxMYO0ixr0XypaQ53N+s1y0M+xq237TfjS/wxv/Nq59+O9+KP8q8Zn+H39Go0oIJQORVbPXD4OrgONyKcd+ZRC4c8i6eLAnCudxLw/D4c5jdDn3e2UXhKcHN3ouBAkxnEWnjyEO+hG7jcCpFKMcohrxfVOguc6+EDkG2GjrxSDrObRbk4tFUIqNiclt3qHHTL9RkBaCiaFIPAqbnbjE2+mO8odGQcer15v8/Jq60yOrLkAdZLg5gBffzyh31TUQi2O89NylPj9NJynlzSf9WQNM9Md1gg8nFbE9XaMf2CIP3fDNjzN5mMjLi65HqBxcGiGHpuTklZk/i0OXcaZAMe4yvZGvcrZ+781LhHKRDxWUvFgN2NSGjFhnNdUs24wMILRvd0U8ZbilWttXr3WMt1glUQqzaiQNCMPoTS+0ghlxOSqMo8PIhNlehpGSHVJC9OHFs1cVxvj8sy/q5xp+K01j0cmJtN14UYnRkgw7jkXrR0GWY3W9Z7twlIzYEkHSG0cfkuNgCjwEFIjdc5qq8FKK6LXDKhqReS7dJOL+Sq/99oqKolU5v056TPrPMzjV5XWZ/6sykvB77434M2NCdvTitu9xNwwcI5Oz70c5d467b0USjHOBdOyxnNcmpFHEroUtYKG+Sj60r0hvudwq5dwp9/Ydw5NivoDcSwtHzzOewPIUeeXxWKxWCyWq+O5CGiPN3cA+Kmf/Gv8j//Tz/Gb//pLfPErX+ff/om/yQ/8ie/k+7/r47z60h067RaB/3S7eOOaFeIsFovlPNieBovl6Tju2llpR+yk1aEotONoRj6tygzHm5FxpK31ksXQ706/QRR43JnFdfWSAN9zWGoEPB4V1FI90x3uFzXovzSkeBLTKOvnF9OoNax/Gb74z+D9z5/voTi83/s+Pt/+C3ylvs32tMJzNU4963Di/2fvzWIkyxLzvO+cu8eekVtVVld193T3rE1yOCStxdpMmbKogSTTEmnalkhJfvKDYQMG9ORHATYsAYYtAzJgm6YkmqAogYJMiTIskZJJmzRlzZDDIaene3qmu2vJqtwiY737OccP50ZUZlZukZW1zPT9Hnqpirhx8sS5NyLPf///txtnjhD4nkRpzSQpyJVmox0gpaDhPX6PO5HHNFPsTlLaocPDUcprq80nX1hIcAOIeuCf8vcnOM2N7Ei78T9NFY3AwTnFceFIyXoroFSajw5mxIViFJd0wpJ26D7x2KbvMM0U3chG9rXPOT/Oc0fKahP9os3kywpud1YbfLA/452HEx6O0qeKyNseJqSFRmlDWii+9nB8qrh3Fsv2kt4/tJF0o6TAdyStKr5QCiuUnDXDjhS0XBv9OskUjUCChNB1CD2XwSxjmpWUpSYrbYzgSsOjVLYLNS1s3NgkLXGlxJWSg1kOVL19QpAVJUpbd6KudLdJWlIqgyslRWl4OEr4nld6aGPQRpMVVoibpCWeJxnFBQbr8gIItWGWlbQC9+I0kypystfwF8LL/cOET6w3l/quctHmdyfyGMxyHgwTmr7HmxtNjKl+Vn1+Z9dKwyMKXEqlyQrN9ihhtRnwqRttPnOzw2rT5xu7UyYPymfiPEbYmFRjIPSezjE152hE5Cy7+EaDB8OEL390yIPDmAfDlFIp7g95Qiz2pKQVOuRKcTDL2eqGZ7pFz3JvnfVebo8StocpkS+RwmOWK8ZpQct4dELJwXQuxjmsNDzSQnF/mPDJzTY3O/b47+9O+ebejN1JSsNzKLUm8l1avnPl5J1l57Lm5WXZG0BqampqampqXhwvRED7M3/5v+Dod8Z5wXOpFL/y6/+aX/n1f/1UxxcI/t9//L8+5ShrampqPj7UPQ01NVfjvHPHdyRbvajaOC8XUWjniWj9pr9w5fhOTuhJ7h8mrDQ8Vps+n9xsL+5AltLelZwWip1x9tQb/ae53F4K8gTyCeSxjWnkBcU0Gg0f/Cp8+e/Ao68s9VQtPD5c/2N8uf9FHrDBBwczkrzAkdBv+HiuXHwfVtrG4iVZ1fFU0Y3sRtrJjdf1ts84zRdxdHf6jcc9UEJY4SzsQXBxzxOc7ajcnaRoYyi0puOdv2vfi3yGUcEkjZmkBYNZRuRbUeUooecwy+25k+TluQLadbojLxLcGr7D9ihlqxdxbxDTCd2lbyoplOabe1PefTSh3wzYnWQ0fIf3d6dLuQsu00s67wxLCttfpbVmmpaEvl1XbhVfWZSGc6Z48bOHgcvuJGOt5VeirUMziBjG1umotGacFOy5EqVtH9p8PE3fYcu2fkMAACAASURBVJKVZIUm9B0cQdW7ZjCA5woCbXv7mr6LlDY2c3+SM0kKsjLgt4yhG3poY2xMpFaU2qAq4SkvDWA3meOipNAarQ2+KwlO60ED63orDY6QeFISeJJ+0ycpyit9Vzlv8/u11Qbv7kzY6IQcTDM6oUev4aONuVRn15xhnBPMHN7caLPRCXj7Vpc4V8/UeWyPWwKPox2flpPxq2dxVCy+N4i5exAzjHNutG2E3anRozMbG9tv+ihtmGWK2/3oVIHqLPfW0fdyMMv5rXuHGA2hK9mflrhS8Im1BuvtkMaRaMe0sOLxo1HKzjhjve1z7yDGYNjqRnx4EPNwlDCYFkReyjQrbQyqFKw2fdbawYXdj1edy5pvHy57A0hNTU1NTU3Ni+OFRTie/L43/457Ld8DRf1lsqampmYZ6p6GmpqrcdG5s9r0mWaF/YIzzWwUWqHoN7wzO9EagcMoKciVYZKWbPVC7vQb3OiGT3Rf3O43uD9Mjm30X+XsPcvl9sLQ6rHbrMyvxW2mjWGclsyygiR/vHkd+ZJm4Nm5O23DWBXw3j+1wtnhB0u9ZuFEvLP6J/j6xhcZOysM4pxxkuM5Dng2Uq5xQtHwHLuhq7VhmOQME7u2ssr5cxLPkbRDj1FSstq0P2Mv8sH1IexC0IYlNsLPclRmhaaoXDMX9U2FnqTh27vn7fXfY5yUT3wO+K7EGMgrt81ZnOaOtPPzbO7aD6uuGaUM07Tg7iAGuLSIdjC1sYAPR7YPb5wUCAEf7MeLx8zjFk+6V46e4xf1kuZKsz/JOJjlKG04mNqepv1pTuBJGq7D/jQjLzWuI9mZpLTCi4XUo27Y2/2IfsvHkxLPcfAcyfu7U6QUSClZbXnc6ERMs5LBTKMwaAOd0CVTmmmuiTynEgoKe7MB1kkT+Q6d0CPyHeKsZHeS8nCckSvDrKHIS2U7r6TteytLg6piHKncW6XWaA8coVDVWoo8d7FGtbHOv7zU+I5AIvEcK1q5jqDtPN13lbM2v9c7Ie9sjzHGHFs/7dC7UAA2xvBglPKtvSmBK5lmBZsE7IxTmoGLI5/eeTwXXSdJzvu7U1ZbPtvDhJu9kDgvwZhFtOPTclr86mkcFYvvDmJ8V7LaDLjRC5+Ipp1Hj6qmjR3dn+aVA9C+1p3VJz/DLnJvSSl4NE6hEqe0gbc2Wk8I1nMavr3ppVCarz+a8JvfGhC4ktBz+ObejLzUDKY5h3FunYau7VVsBQ7F3DVXOeCuey5rampqampqamqujxcmoJ31fe9pvwfWN2LV1NTULE/d01BTczUuc+4sXGFCEHolg1nGLCtp+g6h5+C7jyPY8lITZyU7k4zNTsir/Qavrja50Q353FbniWOfttHfX/IUHsY5dwfxqS63506RWdGsmIK6HrdZVioejlJ2xilK2434eUSZENZlICtXwGYn5Ga32qzNZ/B7/xC+8rMw3VnuRRurTD79o3yt/0P83oHm/mGCwPbqNAMXVygOCkV0zsZ3oa1jpxd5i++3s6zkMC5YaRzfgG9UbhSEINUSmqtWPFvyi/V5jkptzGIcF23cisollpeaUZKzP8vxXYd+wzs2pmNuinPe66PuyLVWwDf3pjwYJpTKPLPemFu9iMNqHu4ObCxiPy25ecZmOtg5+nB/xjf3Z+yNU0pt6IQuq22PT250nohbPOpe2epFKGU4nOV8bqtDVupze0nncY6FUkxS61rdHiXEmSItNEK4KF25tLIS33P45t6UXuSdGXN3lONuWIfPbnWsuzwpOJhmdBseStvoRaW1jR9s+twfJESeQ1bacXQjb+GWmuUlSW7jFpueQ+hLIt++N43A5YaM2JtkjOKC/WlG4DokhXVDFaXGcwRRJaRIAaUylAaUMsQoCq0JHIdSFTiOwJOCQoEQhobvIqUgLxWR7yAR+I6NEU0Kde3fVa6yfnKleTRMeH9vxigpaPgSz/FIciskvvtoghSCnUlKXtiOuGWdxydF191xyigtiKp52BlnPBwm3DuMCTyHNzZaS7ukTnJe/Oqck2LxjW7ANFVkZXquE86RgvV2QMO3scd7ZIhKSD+5zi9yb10kWJ+GqeIelTaEnsNHBzMC17rP+w2fVuAgJaw0fQLHrufDeO6aC1DaMM0K7vQbCC6+Xl9mLmtqampqampqaq6Xl8aBVlNTU1Pz4phl6oV3XtTUfDtymXNHIHi136QV2A3vZiCZpCXTTFXxdUceK+w/moHDZiegGbp8ZqvzhPPsKCc3au8NJgxzKNX5rq1CaR6OUgaznJWGd6bL7ZmjNRSzSjhLr7XbbGeS8sH+bOFkGSUleamemHPfdehGLlmp2N97yKd3f4nWu/8QsvFyL9i9Dd/7E/DpL9J2A1rbIziw3b+7k4yNTmg3/qsBnLYvrbVmVtjup8CVtAMX6Qi0tuttd5LSCpxjm/CNwCXMQ4pghbG/wY2ot/RcwfmOSinEQvu6THRYJ3SZpAW9yGOclsSRIimtG2nOMTfFGZvHR92R08w647SxrpPD2HZvnXw/L3J2XZa5aC2EoBXa83cY53Qjj1bgEh2Jc0tyxTd2pzwaJYzSEk9Ktnohr681+MR664nN8aPulYdVZN00LRYOmsCVpzoBjTHcPYw5nBVMUivIG8AV0PY9jDa0Q9e6c5QhU4qRlExS24n27s6EtzCV4H++MNEIHKap7aibZSXt0GOSlryx0aIZuISuQ+A5fPX+kMEsZ1z19YWeQ1x12hljGCU5h7OcrNAErkMz9AgDh+4JJ1boOXQaHjujlLQoiTNFVipaoUsrdFHanjPKGIQUuI4VIoW0s6sUTIoCKSuXmevQDq0bzZFWUPMcgTEQVD1UvaZPPEyfyXeVZdbP9ijlo/0Zo7QgKxSuI0kKkEIRuopv7EwXa7sVOBzMcmZ5yf6jnLxUBK5zYSTkSdF1f5qzP81oBy57kwzfkexV4lpSaO4OZpTaLO2SOslF8aunxcZO0pJZlgDnd/fNmUcj704yJl7B9kjQOXENO8+9dVZ07UXcPYw5nObsTTPiXHGzG5GXitBz7LilJPKsmN1q2nXc15pBJRKnRbnYGHm1f3E/5XVG2dbU1NTU1NTU1FyOFyKg/aOf+hsv4mVrampqas7gqLPgeXde1NR8O7PMubPa9GmHLvuTDM/J6UYGU3X6zN0zviMptWF7COutgLcvEM/mHN2oRRW8qwTv7c64WcpTN/qnWckoKRBCcLvfWPQqneZye2aUOWRTyMc2svEarxPaGN7fnbI/zTiMC3YnKcYY2qFHv+ETeBIHUNhowllekuzf5c3dX+STg3+Bo/PlXnD9M/B9Pwmf+EGQjwWihu8sNnbX2wHGGPYnBYVWFEqjDEit0Ue6z/JK+GwFno1CDBz6DZ9BnDNMciJfMpjlbHZChBC4roeJmsxKwZgWq/rq1/DzHJWBJ/Ed26mVl/qJSLWTuI5cuJimuWKU5Axjj6j7eD3npV6s++AUAXrujuxGHtOsoOW7HMYF28MEYwzdyGO9FSzl7DqtG+kshBC8favLStPnvZ0J3chdCHfDJDm2ZKeZFWi1gXbostWNeGuzfaHw4DmSO/0GndBdRNcZqHrE1BNOwKMb9tNM0Q5dVhoe00yRlxkGQeS5eI60caBYp+t7OxNKbdifZKxE1Zpsnd93GnkO8byjrnI8zcXMjU7Aq6sNPtifsdK0788kK5FScDhK8By5EF0dKQh9B9cRxLmiUwl8p2FHZiir7she6IERBL7DKC5wKrdo4Dm2H00ZfMfGMfqupCztNdWpxDJHClqBS8N3mWYFwhiyUrO14uFKsejdexbfVS61foxhb5Yxy+w1oSitANmNPF5ba3KzGz6xtndGKQ/HKZOkJC0VD4Yz7vRbNHxncT4JIXDl3LXp83CcHhNdbQ+bWrhu76w06DY84lwxuzdkGGs+OogJXHdpl9RRTotfPclpsbG50ovrzWW6++B49GgzsI60rSOfn+e5t86Krj2Pg1nO4axgb5oxyxUb7YBmJUYOZjm3ViJmaUkrdDicFaimwZECR0rWWwENz7HdqNMMhKAV5OdeLy4zlzU1NTU1NTU1NdfPCxHQbm6uvYiXrampqak5g6POgufdeVFT8+3MsueO79hop5vdkGmuSPKSrNBoDBJRiQjWKXGzFxF5l/uqdnSjdhbHbEaGjbZPWuonNvrnLoYb3ZB+0yeoYiCfm/Msr9xmeQLm2bhT39+dsjdJ2R6ljJOCXuSz1vZPjU5bTT7k1oc/z9qjX0Us6367/fvgC38JXvmBJ+IStTHsTjIavsNKw69cuQZjEvanirRQjOIcp+rpmgsNke8QuRIpJb3IX2z0dkMb5TbLSjzX4VbfRQQdcq/NKDOM0gkblQPlqpznqIw869jxpCQp1KXcD+3Qo9vwbI+VEDwYJqS5phHYjf5hnGMQpIUmOOJMO+mONADGui8O42Ih+F7US3Sas+vtW92l5+VW5cC5N4gJvYSNdngsOrLUVmwwBgZK8+kbbV5fXy76br5h/+FBjBBJNWcccwKetWFv56yg1PZndJ3jayBwHTbbAQezgkJp7g8TEJLQdWmHZ19jjnbU7U8ySm2ORb3e6kVErsODQcKDw4RO5OEIwEC/4eM4VsQRQjBJC0qlcaQ8M1JTacPsiKPQdxyElJRa4woXAQuBWQiB5woCJfA9B78S0IwLpTbkpcJ3rBOt4bsIrHCmjcEVkrWqt2x+aXyW31XOWz93D2I6gYvW9maMtW7AGxtNbnajJ9Z3w7cOxMEsx5WSYVyQlqXtv5sdstoKaPsOjiPxpKQVOuRK8c6jMb4UpKVmlJQYDJ4U9HsR662A1WbAzer63/BdPnOzQyfyeOfhmA8PZtxS4VIuqaMcjV+91Yue6CU8KzY28l37HjuSpChpnbNOj3I8ejTnRjdcvK9nubfOi649i1xptofJwk1+9Fycj2GWlSCgFTgMY9v/t95+fGPCUddc6JVsDxPrmDzjunHRXNbU1NTU1NTU1DwbXliEY01NTU3Ny0MzcKrNUUgLzSVuvL2Quqeh5uPAVc8dIazzoX3KbfUH0wwhxZXOnVu9CO50+d3fNtzohDQajWfWEbUUWlWi2dQ6z64xpvEkO5OU/WnG9ihlkhbc6kV0Tt6pbwydwe9w61t/j5X9Ly33AkLCG38cvvCTsPGZMx82Tu3G9igpudEN2WgHDGY5Sa4WzpPIt/FywEJoEKJyUgQu7pENUkcKGr4DwsVv9hj5m3huQKkMkzS7luvteY7KZjWek26Ki+g3PD46gELZGLbdSUI5AteBOFP0Gh4PR0kldDgErmSWq4U7EmCWlmijGaflpaPVTnN2CWF7uq4iFoeew1ubbd5YbzFMCtvpldnurPuDmI12QFZqPn+7x6ury4kMc3oNn35a8tHBjMhzmGQlNyvH3nkb9lC9d9V/n6YDtUOPWa5oBpI41+xNMgql+dSN9pluQikEWlvxbJQUfGqz/UTUa640m52AlYaP5zqVSOCw0vQQWBeY79pIzcHMOudKpU8VP+PcnjOl0nhS4Ho2ltCtRNuocqFpYzDaADbK0ZOC0LeC4ONjCQql0cYhzks01vHoSsGNXoDvOqy3A8ZJ8Vy+q5y2fj7Yn9HwHcapdQ2+vdXkZi86Vciz6yxhEOdMs5K0UPQaLgczQ+RV13Up0ICLoVCK3UnJvcMErQ1JXlJqez42A5eVpr9w5N7uHz8f1tsBB7Oc19ea3D9MOJhVjtxLuKSOcjR+NfCcxfl87DFnxMa2fKdyDzocxgV9bcXXizgrevQ899Z50bVnsT/JKJRiMMtohe6xc/HoGG50A5S2otr+ND/mSobqWl/Y4zQDyf4J19wyc1lTU1NTU1NTU/NsqAW0mpqamhraoYcUgtBzmKQF/afouphT9zTUfBx4Gc+dwJWsh/D7X+/hhs1jG/2y6ldrhx69yHv2d7CXWRXTOLEFRVxvRNpJslLxwf6Mw7hgnJwinhlNf+fXufWtn6c9ene5gzs+fOZPw+f/IvRuX/jwWWbjEPNS0W9Y99tmJ6Tpu3xjb7pwC3UbHgIroHmuQ+jIU6upAt9jxW/zMA9xTBNizUbbHuO6rrfnOSpl5XzIlTrVTXEak7RgZ5xC9fNlhcJzJIVWDGYludJVLJ0iLhQNzyHyHd5Yb/KJ9RZSCMZpQTN0uTeIzxTPjDFnOjoj3+X2SoOPBjGtMOe9nQmrTf/KorGsYvHm57rWhv1pZmMKXXnq5vd5aGM3+W2knqZQmp1xihSgDPiVm+y8DXuo3rvFfByfm3k06PyPXUeQKcU4gXcfTazjRitKY4VOWSryUjNOCvZnVjC5s9rk1dXmE1Gvc9dirgytwGGWySqu9uQ6NAghcIQgV5qTszSPicxLjZASD4PvSRuB13ApKvHLdSVxXpIphSMfx0S64rjoEXoOeWnsz6ELlLav3whcbvYitioH4/P+rjJfPw3f4Vv7M1qhRxBbcfI8Yfj+IOFglln3YRXd+cpKg9uF4qODGUIKQk/SDX2SwsZBGq3ZG6fMMkWprSs59B1e6Ud4jsNWN2S19eQ57DmSrW6I0obVlmIwzdmf5oSee6FLas48fvWoY/G0c+6s2FghBKtNn2J+vYmLJ2Jlz+Jk9Gg79M51b50XXXsaxhgOZjmTtMRgRcmzxiCFoB05xIUVgfcmGcCx87ff8BauOc/JudkNj0XNXnYua2pqampqampqng21gFZTU1NTQy/ycB3BSsPj0SilOOPu8MtS9zTUfFx4mc+dueBxHaLeUhgDxTymMX1mMY2n8XCUkpeK3UlKN/IX4plQOevbv8ytD/4B0ez+Uscs3SbTT/4Ivd//E9BYvfTzklyTKevoOtrv1Qgcmr7DWstnnJR0Q5/zlozvubhBk8ztMMolj4YzhFfSCuzPdp1r5iJH5dyZcpabYo4xhv1pvujam6TW2bHViwhch1FS4MmCVmBdM53QI1caWfVVZaWdt62ejbp75+Hk1F6iebTgwSxH6dM7BUXVmaW05u7BjG5kxbi3NttXnqejXMW9AvZ9m3cllSfGnhWKcVoihOArD0a81m+wO8nO3bD3qh4wgFIZHKGZ5TYqVFcxk2mhafqSyHWY5SWF1oziAk8KjFGMc8HDUYrv2266QmlagcNrq022eiGfOaWTce5aLJTGFTbyce6qPEroOjgCQl8ySxU6MMdEjEI9Pk7gCkplXZCBJ3GFxPUFWalxq/c1yRWOfBwHetINKYV1v80y62oLfMlmO+T1tSYbLSscHT13pLRi6EcHs+dyw8EynVsH04xBbN178Qn3YTNwWe+ETJKCVuDiSOtENsawO05RYP+tDY3AxRGC0LVuuPPW6morYJapRfTp9ijlg/0pn7nZPtMlBU/Gr550LJ7kvNjYtcX1JmB/mtHwTr/enORo9GhW6AvdW+eN4TSmuap64RRN3znVGXd0DGt+QOjZ6+IeGbuTjFau6Df9RSda03eYZtY1N80V7cBdei5rampqampqamqeDbWAVlNTU1ODlDbKLS0UO+OMh6OUO08RD1P3NNR8XKjPnSPMYxqzCajimcY0nvryxrAzThkltu9qve3jFDM27/0SWx/+An42WOp4WbDKV1b/FAevfZH+Sp8fiPosI40ei0M88udSCLqRjRQbpyWjJD9V5PQ9F9ePyL0uh8YnyRVFtclrDMz9RNe5Zi5yVB51ppzlpgDYn+ZM0oJxWjBMCkLPYa0VcmslQmuD0ppew7URcs2ATuSilWGUFiSFphW4SAFfunuI58hTe4kOZjnbw4RCqUWsYVEJUHOEsGNuBQ4N3+HBMKUZuISewxvrrWs5v5Z1r4AVRLZH6eOxp4pCPx77NFMcxjmuI9mtHHz7k4xcaXqRd/qGfSUWulIwSXMmQqC1IVOKojQUypDmJeASeVacSnJNKxAgBY4WBI5ho+PTCEN8R7I3zVDaZasX8UfeWl/0ZB1l7gDTxixci6dFEAohaIUepdbMMsUkK+keEXtt3KJBaYPvOoCqRDBJ4Ak86dDyDduFxpUghCIvDb5jULJyzkn7nhsDZamYZiXTtKQVOKw2fG6tRLzWby4iCx+OrLCUFopHoxSth88l8naZzq1C6UUc7eyU6E547GDyHclK0+e1fpOkKDlMCoJCsdLwWW0GTLOCXtNHXdIIPJ8nIQS+I3lvZ8J7O1PGSYnvShq+gyMEyhiSXC0E83n86ryr8Khj8Ym5OCc2dt4Zat+jkr3p6debk8zXnzEwSnIO4/xc99Z5YziNJLeRsoXSdMPTz/mjY9DGLL4XCCGYeNbBO8tKGtVNC1IIkqIgLUoeDmMG1Y0Gy8xlTU1NTU1NTU3Ns+HbQkAryxLX/bYYak1NTc23Lbf7De4PE7Z6EfcGMZ3QvVTPzEnqnoaajxsf+3OnyKxoVkyfS0zjWRztHFuTU954/x9w4+4/xi1nSx0nbr7C9us/yt7WD3J/YmP1utowTsul3F3H4hBP/F2/6TNMCnqRx2FcEHrK9psBnuvgBxG51+HQhKS5QlcuvrlAIQRIxLWvmcs4Ko86U05zU0zSgmlWMk4LklxVm/oeUsI0LZhmilbgst4KWGn5vNo/3hc2jyt7d8fG+RVKs9EOFuMwxnD3MOZwVjBJSwazDAM0fYduGOC5YrGpX5TGCglxwTAuMAa+sTMl8CTfdat7anzdsizjXjnaYzVJi0pAsa7EjufjuzaS0HcFaaHIK5dakisM1vHiO5KFunOE0JMIrPtsmJSEnnVsYcB1JT5gfJdu5NEKHLQ2DJMCz5VkpaLrC0AgDNzshjZyU2leX21wa6XBZud0kad5RAAo1eOf8zS6kcskLWgHLuO0JHDlQsxQ2lClmiIwdo0LkBIrtAmBJyWuI/nW3gxtwJWPrzbTzLrzjNaUBpS2An4jcOg3A3pNn++9vcJa9Z4P45yPDmZIKRBxznor5N2dCWklns0RwsZBrjQ80kJxf5jwyc32U7mAlnEt7i2iO3NagUvDd0iKsjo3rHNRVGLpwSynE3oIKWgEtt8syRXtrst6O2RvIjmc5bQCh71zXGSPf3bBndUGzcD2kb1aKIZpSVpo3t+dHhOi5vN0oxvSb/oEnnOpeTovNhZgtekzzQq75qfV9aZQ9BunC8lg15/WmsEsZ5pJ3tponeveumgMJ7FRq1Z089zTBTd99FotxLG53B5ZZ+NcPI/znLy049XaCui3q/EuM5c1NTU1NTU1NTXPhpdKlZrGCb/2m7/FV772DX7v3W+ydzBkMo0pVYnnurRbTdb6Xd7+1Jt8z2ff4g//vs/TbNRfJGtqamqug7D6BV0pwzQtuDuIAZYSAuqehpqPIx/Lc8cYyKuYxiJ57m6z05hlBd7kPt//rZ/jrcG/xDHFUs+fdD/Fg0/8+ww2/wBUfUoNzwodtqeqWEpAi3xJ6EqEsBuu0ZH303MkG60ArQ1pqTmc5XhuRLfVovTbHJqI5IhwNicv9SKaMFOKw8H5zopluayj8qgz5aibIvAkw7igUDY+UFAlepaamSlxhGCtFdAOXVaa3qnHnp83X7k/RACHSXHscXcPYw6nNs5uWnVBrZyyme4CgQut0KWvNYO4YG+ckaucg0nAl+8e8kOfvfFU8wXLuVdO67FaafhPxA92Qo/Acwg8STt0caVkZ5KRlTaScW/6ZP+cEIJSGzSGrFRkpaEdeot+r1le4mO76CLPRQjIlaHX8GwvWVmiqaLngFJD03dZbQXnOhvnrsVW6DKKc3vcUhO4T65FR0r6TR9dRduNE3uOhp5jhbBqHktt4xOtSObgSslqy0cKSV5qug0r9CaFQmuD1gZHCgwgpCQUEHgunpTEhWKrF/H5272FeDaYZXz57hBjDKHnMMsUkoxu5LHeCgg9uRBhbUdfwaNRys7Yik5KGQ5nOZ/b6hzrqrosl3UtamMYVF1bqlIX7w1ilLFCso3+pIrbVEyzx669lab3hEuq3/QXXVu+k9voykuMf7UV0Ik8HAHZ3pStXsjNXkg79J7aqXdRbCzw+PwXgtCzovksK2n6DqHn4LuP36+81BxMM/ZnOZuO5M2N1qndfcuO4Siai8/5o9fqoxG+87ncm2T4Tk43siJonJUYA5udgDv9Jq+vNa/V9VhTU1NTU1NTU3N1XgoBbe/gkL/99/8J//if/RpJZqMZTt78lRclB4cjDg5HvPetu/zCP/0VojDkT//QH+Ynf/SLrPV7L2DkNTU1Nd9Z3OpFHFaRQncHMR8exPTTkpvd8Nw7pOuehpqPOx+bc0cVkE0hn4AqXwrhDIDdd+j8+v/M1v1fRbDcmA7Xvp8Hn/gxxv3vftLV4zsYA2mpSfLljtsMvMpNZPumeid6q1aaPkmhkVKSKMmIJoO8jW9sfN1ppIXdIN+f5qSlZqsbXmnNzN1H81i4o31PrcDFc+W5jsqz3BTbw5RhklthxAgMhobvog3c6jXoNVw8x2GrF7F6Tjdfr+HT8Fw+HMyQCKZZySY2tvFwVlgBKj89zu40HClZbwW4QvDe7oSHo5T1QcKDYfLU59pl3Svn9VidxHPsMQPXoVCGlaZLUii2h9bd57sOoSdph4/X1CS1YlRaqGpTX+BKWQlRhqLUhL5TxVqKxw4ZBL2mh1SS+xr2ZwVGJmgDn93qXOhsnLsWN9sBj0YpUkBSqGNjO0o79EgLjTGGMQWjpCAr7f8jQBvQynablVrT8T0bTSkkcakWHV+zXGG0QRvrDnWlIPAcPCkQUuDN+/SU5pV+hO/IxfX23UcTTHXtSkvFpzc73DjjWt3wrfA0f+69Qcw0LRbdYG/f6p45N2dxWdfiLCsptWF3nBHn1t0bF4o016gjwi1YB1+cW1ff9jBhd5ItxN25S8qRgkbgME1t19YsK898n07iOZLX1ppkpWZrJeJGO+RmL3rqrriLYmPBrtFX+01agY1tbQZyEds6y/MnHIOzXNFr+NzpR7zSj07t7lt2oWC5wwAAIABJREFUDEeRHD/nTzuLk0LhSRurGp0Qv7wqmvJGN2SWlSSFYhQXzArFzW7EJ9aafO+rK9feu1dTU1NTU1NTU3M1XriA9n/9xpf5a//dTzGeTp/48nsW88fFScrP/+I/4//4F7/Bf/mf/xX+6O//wrMdbE1NTc3HgPkduravxG5WDOO8in1yia6h86Km5juR7+hzJ4+taJbFlWj2YmIaj2EM3P9X8KWfhvv/ivYyT0Wyf/OP8OATP0bceePMx823Pec9NsvQCV0cKehGbhXDFhzboBdCcGejy6PE52HuU0xzdsbpItIvqpwVcwEkyRXbwxS3Ele+d8M6apZZM2mhuDeIeTBMKJU5s+9plBZkhaIdOOc6Ko+6KTyZMYwLlHbJCo2Ugobn0G/6rLdDepVTbq0d2BjCC+i3PD44gETZzeW0VGwPk8XG+WXFs6O0QpdO6C06xt7bmbDa9J/K3XEZ98pleqyOP97Q8O1x81IzSUtCz6HhuySFJslLBjNsB5WUqCquLi8VjpR0IkmhdSW6QKEfu2HsWG3kH9j3XWCFlZZrGMYFsyJmvW2dghc5G+euxTgv+d3tMaUyxJlCNc0Tzro56y2/em2B75RMspI0V5RakxQlnpQ42GulwIqDNtZRsNmJaIcuvciKirsTu+5GlZutFdpuvU7gEueKbJqRFYr9acZhnDPJ7FwmhUEK+L5X+6xcwi3sOZI7/Qad0OXuIObuIEYIwUrVPbgMl3UtznLF7ijlYJbjO4K9qQIDgSdpOA6uIxedb3mhSEvrQns0TulEHlmhSQrFK73H8ZuR5xDn9maP84TO03CqKMKm77LZDfnsNXxWXSY2ds5q06cduuxPMrwj7q286j4Uwo7x/mHCWsvnlZUG//anN2lccJ1YZgxg59+v5r4oDScPr7Q9B1aaHq4UZ57rUgjaoUc7tC7QuFC8udHizc3WhSJeTU1NTU1NTU3N8+OFCmj/4J/8Mn/9b/3dxS8QR39/OG+P4uTjRpMpf/Wv/ff81f/kJ/hzX/zBZzPYmpqamo8JQgjevtVlpenz3s6EbuQymOW2QyZJTu0GqXsaamq+A88drSCf2pjGMn953GZawTd/Gb78t2Hv60s9VUmf3Vf+HbZf//NkjYvj++Y+sHmPzTJIIdjshGSlYn+aszfJ2eqF1k3jepigQ+62aYeCZJISF4bbfXmsF+fomhmnBaXW3Flt8eZ6k81uuNSaeTBMeG9nQlaoxbo8t++pVMwqAeY8R+XcTdEMXMZJacU0R7LW8ivxLOCNjTYt31kq7s53HJqBw3hYUGjNvYO46oLKaIXu0uIZWOEi9BwCV7I/zckqQfGtzWXk1+Ncxr1yssfqorGnhaIb+Rhj6DZ8dsYJErGIgrMikGSUlPSbPqOkRGnNJCttXxiQ5CUxinFSoIymG3nWgVR17ZXKimquFHiOQGlNrkEqg5GaXsNDwKXW17wH8o31Fu9sjykrQe9kzOQCIVhv26jEwcy6sIZJwaNRRlZocAWHcYHnSHKlaYQuK5V4ctLBuNGxNysUSj12JWUl09TeoFAqjedK2pHHasu3cay5IvJcvutWZ+m+yvnjPzyIaYVXE2Ev61q8exBzmOTM8pLSdWiHLi3fPdOV1PTdRSTnKCkoqg7B3WnGrZ51EfqutIKb0naul+BYB+MVoitP47KxsXP86npzsxsyzRVJXpIVGo1BIjiYZWytRHzv7R5vbrQuFM+uMobIdxFVVGZSlLTC468xmNko03bo0m/6l5qraSXszkW1mpqampqampqal4cXJqD92m/+Nn/jb/3MsQ7s+e8P/V6H7/r0G7z5+m06rRaNKCBOMsbTKe9/eJ/f/fo3OTgcAcef+9f/x59hc73PH/o3Pv8CfqKampqa7yxuVRtU9wYxoZew0Q7PdCvUPQ01NY/5tj93iqzqNpuCsrFhLwVlBl//Rfitvwuj+0s9tfBaPLrzZ3j46p+lDC4f+53myopKriTyL3ZNneRmN+TROGWjHbIzTumrkHZnhdxrkxsHpQxgzuzFmTsrklxhjGG9HbLa8vmB11d5c6N1qTWjteFrD8c8qpws28PECjMX9D1VKYBobTeYh3F+rqPy7iBmd5KijOGN9RY3uuGi50yw/GZ74Enagct9Y8gK66rRxmCAfuNqG8zzXqKNdkCcW0Er9Kzwc9WotIvcK0d7rIzhQmeJ0rY/bqXh4TqSpueQFooHh4kVAF1JoWyUn5sW9Bou07QgLqw7qR24i9+PCmWIUYAgLQyRZ8hLg+tYZ5LBvufjtCROMwoteKsXkGqJKwWhJ9HaXDg38x7INFc8HCbsTlL2pxkN3zlXLGyHHg3fYZSUdlwyp9fwKJWhETist0O6kcftlQjfdU51MJ7lSkoKRaE0K42QzU7I27e67E0zVps+xuSstoKlxbM5vYZPPy3ZHiZ0I3dpEfYyrsWDaWbjUNOCstRstkOagWuvC6Wm0Bql7c8qhKBQmlIbfClYrdb3Rwcz4kIxjks6YbEQe+Fqrtqkuh5GnhW3r4u5AHtebOxJhBC0A5f2kfU1jHMOZjlvrDcJ/fOjR59mDC3fwZGCVuBwGBf0tV50MM6ykmlWstby8RznbBH5CIXSjJKCG90Q1xFLdW3W1NTU1NTU1NQ8e16IgJZmOf/1//DTaGOOCWDf9ek3+Cs//mf4A9/3XUh59iaFMYbf+NJX+amf+9/5nXfet9EjArTW/Fd/86f5hf/lvyHw69iDmpqamqcl9Bze2mzzxnrrzL6cq3Re1NR8p/Ntd+4YA/msEs6Sl8dtBnZMX/378Ds/B/HBck8N19h+7c+xc/uH0e7y7r64UPiuU71ny29qBq7D62tNpHTQfpu7RcRK0aApJSeFydN6cbJCM0pyZlnJ62tN3txo8f2v97m9cvmN4a89HPNwmHB3EHMYF4uo0Mv0PQ1mOUKCwVj3S+Ce6aicZtaJYTCstf1FLOlViXyXwLMb1fvT3EbSlZpmFVt4Fea9RK4jWW/bze+Ndsgwubj36Cwucq/Me6ymqaIROGfGGs4ZxAUC61650Yls1Camcg3aOMJ26JLmmqaPdZ8ZSHNN4EmkFKgqntFgxZrQc5AIHCkYpwXaGCZpQeBJBAXdyKUXekx9w0rDJwoDAs9BaS49N/MeyO+53eO37h7yYJjw/t6U11cbdKILRENj8F3JK/2QWabZm2T0IhuNeKff4GYvOtfBeJor6aP9mNWmzxvrLd7abPG5W12+en/Ew1GCIwU3u+Gpx7osN7shwzi/kgh7kWtxHvmZ5IqsNES+iyNtlOX8RgxjDOrIZTorS7SBvZkgCmyMZTfymaQx46xgMHNo+M7j7rsruMielUtqLsAqZZimxbmxsWcxjHPuDmJWqqjYi6JHn2YMQghWmz6FUgzjgkFcsN4KmGXWgTv/fN+6oAN1zsNRihCCfhUH+lJ8J6ipqampqampqVnwQgS0n/tH/yd7g+Eis10I+E//8o/xF//8n7rU84UQ/MHv/27+4Pd/Nz/zC/+Uv/lTf2/xd/uHQ37uH/0zfvJHv/ishl9TU1PzsUNK+4t93clQU7McL/25owrIprbfTJUvl3A23YOv/G/wu78AxWyppx6Gr7Dzxo9x+MoPYuTlN3rnXWNpqRauqn7TZxjnaG0WAuilEZLNtVXGvkc8UezuzfjG7ox+0z81DhEe9+KEnsPDUUqp4c2N1kJIWEY8ezBMeDRKuTuIGSUFr602LrUpfbLvqeE7hK6NPvzUZvtUR+W9QczuJMORkk/daNO+guB4lJbv4DmS0JOM04LQs86rbnixo+M0TvYSrbUCtkfpQkx6mnP0PPdKUljhvNCajnf+a8yjB9daAZ7jsNYO8KrN9NsrJY6EB4cJB7MCzxFEngNoCmXIlEYKySix0ZxC2K4x37UigisFBiu8DOKcVuCx1vJYa4WstgKyLGPsGd5cb4Djc3+YLD038y6+OFMEnsMH+zPeeTRhpeGx0Q6PuRbzUpMWNiZUAP1mQFq4lCrhs1sdjDbc6AZ8cgln19yVpKrYxs/fWWGjE/D7PrFKnCuUNhzGBd3Iu5SwcR6eI+lG3pVE2Itci/PIz1lW0vStyLY3zXGlIFeaotQLkRRAG0gKK25lhSLOSrJSQxUjOIzzRdSnV3Uo+o5cRIJehmftkpoLsMYY7g7ic2NjT45rLvavNKzj9UY3vFIc8jJjWGsHHMxy+s2AnXFKkpcobQXr9VZAv+Gz2rr4WjUXYW/3GwTecq65mpqampqampqa58MLEdB+6Vf+n2Pi2X/2H/84/+GP/MkrHesv/Hs/jCMd/tv/6WcXx/wnv/x/1wJaTU1NzTWitfn2cNHU1NRcjDFQxFW/WVyJZi9JTCPA4YfwW38Hvv5LoIulnpquvc37t/8c/x+fox0GbF1SPCuU7WwaJUUVi2Y3seOiJPId0kLz9UdjHGl7zW52QwL3HHeDkOAGEPXAb/Jmy5Btjyk1tEIbo3heHOI0s/1NQoiFk+tGN1wIFJeai0Lx3s6Eg6rv7LLi2VGO9j2tNANWGj6f2eqQl/qJz4JO6LE2TvnG7hTnGvqRhLCb9A3PYViUDOOCyHfx3Ksd+2QvkY3DswLXLFMXH+AcznOvZIXtoTLG9k+dxSwr2ZtmtALbdbXVixZRhXdWG/ieZJaV0BPsTFLSQnOYFAxTe0pP0wITeoQutEKXyHVwHSvgt0MPU0V0DpMcL5Ws9Wxs6KdutOmELqpwGd63wpDrOxgDs7xke5hW47v4s3/eA9lrePzzd3ZoBQ6PRikPRymH8YTAdfAdiesIpARXSnznsTNure3z5uY607QkLZR1wMX5tTiRdsYpSlvRbv0SwsZlaAUuw2R5ofE81+LRyE9HCIyBrBLM5r/req4kcB2ktGJYnJVo4xC6EmVgf5bTDlxKbazwY+BgmhM4ktBz8KREiLkAezmeh0tqfn0TQjy36+TTjCHyHR6OEmZZwWCmeXW1wUY7pN/wud2/WMB7WtdcTU1NTU1NTU3N8+G5C2iP9g748N7DRezi5z71xpXFszn/wb/7J/jnv/abfPXr3wTgo/sPebR3wI311esYck1NTc3HlrRQ3BvEPBgmNkbq26nHqabmJeClEp8XbrOp/e+XyW0G8Oir8OW/Dd/6lywt6L36h+D7/hJi47uZ3huyMc15NEpoBQ6dC5wSh7Oc3WlGqTSzrCTO7b/HaUEr8DiY5niOJC4U3cglK20f1+trTTbbJ2LghADHh2gFgtaRP7bCwkrT572dCd3IrSL5To9DDD2HG92QftMnqMSZZR0V9wYxWaHYHib0m/619T1N0/LMvqdxWpzb67QsjcDFcSQrLY/hrEAIdSVx7rReIj2PObxCF9RpnOVemYtncHpkntKaQVwwTUtalXtlpek9EX95oxPyA6/3+dr2mEIpdicZ7cDBccTidNloB3iORAobE9gJXdxKhBNCoI0hKzVbvZD1dngsZnNc5ovX0tqKOMVDXYk5xVKf/a+sNPjxH7jDlz4c8KW7h9zohoyTkmFSkJf2uiOx4lCpDd2Gz9urTTY7NjoSA6XS1+pEmmWKtLTvRbiE8+o8okpovIoIe5Zr8WjkpxFm0W0WZyXdhkfDd4+to7wS1zqhR+BJVho+ca4Yp9ZtVmqD50rGSU7oShDQi3wOphn9hkdSqKrTzD3TXfu8XFIv4jp5HWN4dbVJVijSQtt40F54ZtwoXK9rrqampqampqam5tnz3AW0d9//CHjsPvuRP/nHruW4P/LD/9ZCQAP4+jc+rAW0mpqamqfgwTDhvZ0JWaEWmwdptYE2Z755sNLwSAvF/WFyLRsYNTXf7rxU4nM+e3ndZsbA3d+AL/80PPjScs+VDrz1J+ELPwGrbwIQAK+vNdHaEOcl26ME4FQRTRvDo1G26BgbJoWdmkqPuNkNWW0GrHcCQtdhltt+m/1pzkY7RGvDKC54a7OFQILrQdiFoANnbJ7e6kWsNn3uDWJCL7HHeQZrQ2vDg2HCoBJ0nkff00W9TlchKxRb3YhRUmC0YXeSM8kKVhqXdxCd1UsUqxK4WhfUWZzmXtkdp6SF7eVKCxtXeFqE4VoroB26rDS9Yx1qR7nRCclKRcOzwogx4AhJM7R9ZSsNj1bgEXry2Ab+ZUU6gMO4YC/OOJzlC8fWMC6W/uwPPYd/8611vnBnhd97OOZb+1NmqaLUVhTyXUnDd+g3fVwpj633wJX83vb4Wp1I2pjFz3AdDsmjx7mKCHuWazFXGm0M49TOuTJW9Auq68JJ8SwpSjxX4ruSduBV0ZKSwJWMkwJlDKXSTLKSpJjR9F0izyFQkofjFN+xa8Wt4obXKxF2zotwST2v6+R1jEEI2B6mCKyzcG+S8c7D8XN1zdXU1NTU1NTU1DxbnruANhiNj/3/9779yWs57uc/9xbweL/i5OvU1NTU1FwOrQ1fezjm0SjlYGY3rowxdCOP9VZA6MnFZkBaaCZpwaNRys44Y6sXoZThcJbzua3OuXfg1tR8p/KixWchBO1GgFNMYDh5Od1muoT3/7l1nO2/t9xz3RA+9yPw+f8I2jef+OvNdsgoLjDGsI19P6aZYr3tH9sYfjTKrCgU5yS5IvQkBkFWKFYaHv2GT6fhcaNjxadew6NQAXsT626LcyvAuF7AJ165acUzebGzJfQc3tps88Z665m5E4dJQamur+/JkQLPEXxrf0ZW2L6mlYZ/bKwX9Toty7xz6dXVBjvjlJWGyzgteTTMKBX0mz7OOfOjKhfVNCtP7SVKcrXYBG8G17Pxfpp7xZXwzb0Zk6zk3iAh8p3qsVTz6NEOXTzHYavatD+PO/0Go6RgvW2dN5PUuroMBqUNUtqfXRm9lEinjeEwh+1RyjAz7M8ypLRdT7dXGlf+7I8Cl+9/rc8X7qwstd6vw4mkteEwtg66D/dnPBgm7E8zdiYeK82Alu881fcUVQ3kqiLsaa7FXGnSwjpgbcSioB3auNE4L3GlxnUESaEoStv11vQcQl8u1hbYOUkLxe4kpdSGrNBkwjr+5MgKPmmh7TqUklbokCvFwSxnqxvSibwX6pJ6HtfJ6xrDH/+0x8Nxyns7E9Za/nN3zdXU1NTU1NTU1DxbnruANhpPj/3/Svd67rY6eZzxZLmy+Zqampoay9cejnk4TLg7iDmMi8XdsadthDZ8u4k5j6O5N4htD0u1Y/D2re7zHn5NzQvjpRCf8xgn2aeR7WFm++CcHrX3wigSeOcX4bd/BsYPlntu2IXv/nH4rh+z3WLn8NamjU8UQtDwXXYnKeM0px3aTq2s1BxMMw5mGdOsJKr+DFgIQ53IY6t33LnlOZKtXkg7dBkkin3VxJg+YR6y1VhOLJKV4+M6nFonmaTFtfQ9FUqzN8mqDeGcvWkGxqCMYb0dPOECWWsFp/Y6XYWjnUtvbbT46v0x6+2cQmnivGSWlTQCh8hz8F2JrCIKrStHEWcKKWCtZTvATvYSTbOSsBp/O7xcV95lOepeKZQmKx8LLavNACFYOH8cKVht+qy1g0Xn2XkIBN3Q41YvIvQc3lhr8v7elHFasjPOSIrHYvkyIt32KCMuBXvTnEGiaAced/pN3txo0w6O/8p4lc/+q6z3qzqRAL6xMznmAN4Zpwymdi1/uB8zmBVLz/1JrkOEPela/O27h3w0iG1sZl7SCj0CRzJKrWA/iHM8Ca4jafguvisJfUn3yBo2xjBOS3tNMzBLbJRoK3BZb4WsNDykIxb9c8oY9id55dR0eTRKEEKw0Q5euEvqWV4nr3MML4Nrrqampqampqam5tnw3AW0RnT8l/hpnNBsPP1dV7M4Ofd1ampqamou5sEw4dEo5e4gZpQUvLbauFRvjudI7vQbdEKXu4OYu4MYIQQrVdl8Tc3HgRcmPquyimi0bjOdjEiTmGO3vr9o0hF89efhKz8H6XC557Zvwuf/Anz2z4J3ueuJQPDJzTbdhscH+zPaocMoKRglJYeznEfjdBGn1Yk8HClp+JJmYDujNtp2k/k0PNejv7qCURHv7WUkXkHOhH7TP3cz9Hn24V1H39PBNGN7lFIoxSQtOYwLdscZpTJMMxvrd9JJKYVgmqknep2W5WTn0ttbXWa5Ii1Lvv5ows1uRJyXTFNFnOdPuDw8KVlpHhGNuuHCeQaP3W03uiGuI+hd0JN3FebulddXm8AjAleyPUxYb/v4jkPgSSLfXdoFddSZt94OeGUleiyuzHI2OwFSiKVEuoNpxigpmJUQZYrQc7jZDfFdScs/e00/j8/+ZZ1IZzmA40zxaJwxTgqSXLHWDmgFDsXcdXUJ999JrkOEPela/MR6gwfDhKzU5ELgu5pSGfLSdqxJAcpAKAWeK+iE3jHnGcA4LUnykmleEheKEmxcZsvnZi/kjfUmk7RkeuQ6YYBpZueiGbi80otohS4bnaB2SV2Sl8E1V1NTU1NTU1NTc/08dwGt1zl+59qHd7fZXOs/9XE/uLsNPO5WO/k6NTU1NTXnkxaK93YmHFQbTpcVz44yf/yHBzGtMOe9nQmrF2wq19R8J/BCxOc8tsJZHoNWvFTdZnMmj+C3fxa+9gvWfbYMq2/CF34S3vwhcK62Ob3ZDulVUWQ745TVprHxglrzaJSy1Q1Zb4c2gk1aIaXf9E8VPV3XRfhNCr9LblxcaWiFiu1hQjdyuTeIeWvzScffi+jDe5q+J20M9wcJgyr6zvaoQeBKOqGNtLzZs1FupzkpMYZpXtJreItep2U+S07rXIoCt3o9VW1IWydXNzIYY8iVXsznRZ1OcNzddqsXPdPNbNeVfPpGG8+xvWWe4yxcUlfh6NhfW/3/2Xv3IMmyu77zc+775ruyurq6q6e65/3QjEbSSOjJCiQkBAJhDAIBiyUZFu/iJWDXjl3DH/YGONaGDe9C7G4EYRbbiIfBMkisV0gggRDiIYTEII2kGU3Pu9/VXZWVz/s+9+wfN7OmurteWZVVlV19PhETCvXNe+pk5s1z7j3f8/19y9w3X8VA8JVLHb5yoYNtGByvuxiIHYl0qcy51Inox5JEFqU6bduk6lnMlp0diXsHMfdv5wLKc8VXL3Y2dQA7lsC9YlBxTZb7CaYo8t7aQUqz7CJzRT9OOd0sIdj+PU9ahB05mAZRSs23cboGVc+iWXZRqsi3CxJZCGtZvvYbT2QOCVhmIZqGcUYnzOjFKXFSiKG2IUhzRcN3eNUddSqujW0mG/5+0ixnuZ8gc4VnmZxplrR4NibT4JrTaDQajUaj0UyOAxfQFheOAy9nlX3qs5/nDY89sud2P/XZz1/3/+84eXzPbWo0Gs3txPlWQJwWi8HNsrMr1wAUC2nNKNt2UVmjOSocqPicy8JplvQhS6Yv22xE6/ki3+zsJ4bi3hgsPFYIZ2fe8vIN4x5wLZM7Z8ucbpZohyntMMG3TOq+zemZEr5r4tkWJdvYUCywTBPhlsnsOomwSaViJFaerHtrbinPDrlnrnKdGHNYeXgjBxK8nNO0Uy60QlYGMdf6MYNYFplZJYcsz4myHNc28CyTkmNt6KRc79yr+zYvrgQ0o4yTm7gxR4za2CxzabFZ4kI75PRsmfOtgIVG0V6YSuI0X3N5uLYxLKlnbZhLdaO7bS9i1k4Z9X3SzrxR388cK3OpG/GKhTrnWwF1z95x+9d6MamUrAYphihy1ObLLrZpcqy684oehz3378QBfKLugVAEicQ0DBZnXFpBynI/JkqzNdfumWZ527+3HyKsZ5ssNsucnvG50gmL0qNlB4VCIDhhCpJMEcQpWQ5hJokSSZQWY2yuFL0oJc1y0lxR823KrkUvSjFyNcxDLMp4nqx79BNJmGTF7we1JrreKRXL3QjXNnmpFbAwLBeq0Wg0Go1Go9Hcjhy4gPbgvXdSr1bo9vsoBX/w6b/k+7/rndx/9+ldt/n0cy/xsT/5S4QonntqlQqvuP+uCfZao9FojjZ5rrjYDodOA8XJurf9SVuw3aKyRnOUOBDxOY2Gwtlget1mAJe/XAhnL/zZ+Ofe/c3w2AfhxCsn3KkCQwgMIWj4Dq1BypnZ8pYilWmamI5fOM6Ee51wNsI2Deq+zWqQcrzq0Q5TmmXn0PPwysNsMCEgSnO2uySVUvQTyeV2wLlWyEo/Js5y5qouZdfCFBBk+ZrDy72hLOSNTsqaZ2EIg7JnUfFsLrVD2kFC3bepuBa+Y669/1EpzU6YIoTYNHPJs03un68ipaIfpVxYDTndLHG8uvP5aiN320EIAzf2fVLOvFHfd9t+rhStQUIvyohSSaYEvlO4zxYa/ti5YIc19+/UATxXdVkZJDTLDsv9hJJjMldxKdlmke/Xj0EIKm6yZTnH/RRhLUOQK6h4Rb7ZTKkoMbuerGTTjTKsKKXsWCilyKSiF6dI22KgMnzXoOJauKaBVAqZFyLz6CsVQlB1rZvy7UbkudIboTQajUaj0Wg0Gg5BQBNC8JbXv4qPDwUvKXP+yc/+Ir/8r3+axYX5sds7f2mJf/pzv0Se58P24Rtf/6pJd1uj0WiONO0wJZOK1SAd7lDeXWbOiM0WlTWao8Z+ic/dKGW5F3JPLcdI+pDF0+s2Uzm8+BeFcHb5S+Oda1jwwLvhNe+H5v5vfhrEKTLPSTJJcxNxwTRNDMtFug0CwyeVOWoLwbLiWrTDcM390Sw7h5eHN6Tq2RhC4NnmWp82IpE5y72YlUFCnEourAZ0o4xumFH3LcJEEqURhigcYo5VuPR8Z+NHiPVOysVmCdOAmmdT9601B147DDd04J2oezTLDu5QDNpI3DzV8Fkd/tbOtYKJudsOgv3u+27aH8QZcSa5sFpkbrkmHCvbzJTtsfPA4HDm/nEcwLZpsFD3kHlRRvVaLwagPBSRrvZiPLvYxFD1rA0FxP0WYRXQKNmUbBMFtIKUucr1TkDLNGiWnaFrNSeRxZgWphLbUnjK5HjVw7MNunGGKQSWWbgyd7r1Qm9BjVUxAAAgAElEQVSE0mg0Go1Go9FoCg5cQAP40R/4Lv7oM58jz4udrFeXV/ng//Cz/OMPvJfv/rZvxtzBwq2UOR/9wz/llz/0e/QGwZr7zDRMfuQHvusA3oVGo9EcHXpRsagcpfKmhZrdstGiskZz1Jik+CyAkmNypmZC2MIyFd0Vn4Z3KLdr2yNTeOaP4PFfh9Zz451rl+Dh74FX/xBUxt9AtVvCJCeWRXbQjS4qwzCwbBfp1gmNEqlUKLm9aOk7JkpBOMznOpQ8vBto+DaWKZgp2UXmm8xvujZHzrhUSnpRxqV2RDtM6IYptmkwSARBKjENgWMaDJKMumcTpBkVZ3PBYL2T8qGThRDmWAaeHXK86u05A27kShNCUPGSibjbDor97vu47Z9rBZxbCejHGSeqLq2BojEU6XbLQc/94zqAZysug1iilOIaMVd7MZVE0iw7VDyL1iCm7Bos94aZfkMOSoQ1hGCu6mIaBhXXphullIYlSW+kELNNfEzCxKDmS1KZ0yg5+I5JlBYlHiuuRZhK6r6NsYN8N9AboTQajUaj0Wg0mhGHsiKzuDDP97/nnfz27/8RQhQPz71BwP/2y7/Or/zH3+ed/9XrefSh+7j3rjuoVcr4nksYxXT7A5594QJPPPUMn/rzv6Hd6a49fI/+9/ve845dOdk0Go3mdmYQS6KsCJH37L25z0bcuKis0RxFJiE+m4bAEgo7j7DiHkna48Jqn9iuMIjM6RPQ0hCe/Ch86begd2W8c/0ZeNUPwiPfB97BCxi5Umvup5FEYwiBabvkbo3QLJPmkMudl8g0hyUWi/EuY2kpOpg8vC0wjEKMilLJUjfmcidaE0WUUpxbDVgdpPSijNYgJleqcJiZxaL9XMUBIZBSEUvJcj8mk4qqZxMlOedWA043S4hNFuOvd6+YvPW+Oe6Zq9AOU3pRyiCWa5llZdek6tk0fHtHDhchBI+cqjNTdji71JuYu+0g2O++j9t+P86oeBYKRbNkIR3FHQ1/0+91Jxzk3L9bB/Bis/gMhRD07JTWIGEQZ3i2QZBIVvoJIKj7RS7hQYqwo9/DbMVFKUXFHZaXhA1FtBGJzFG5IssVJccgSiXdKMWzDSxDUPNsfNu8aePAVuiNUBqNRqPRaDQazSEJaAA/+SPv46ULl/mrLz6xJqIpBavtLv/5Y3/Mf/7YH295/ugBcH0sxJtf+yg/9aPv28deazQazdHkukXlXeTtbMT6ReVcTWlek0azR3YrPgvAMgU2GVYWIJI+MktI8hxD5OS5IspywmSKyjaGq/DEf4InPgxxZ7xza6fgNf8AHnoPWHsrc7kXDCHW7h1zIbBtB+XWiazKUDgbv005HN+EYK0k3L7m4e2QxWaJC+2QhYbP+WEuWaPkFOJZP+FaP6YfS6qeNbx2BSv9mLJrYVuFWGebQFoIOaYrGMQZSSZZ7ScAnGmWN/zbm7lXRv9NglMNn9myw/lWMDF320Gx333fafvnWwFXezGmYXDvnEswph6+EQc599/oALYMQS/OCJOMOM3JURgIXNvAdywqjokQAiEEp2dLlF2TS51CxO1FGf1IEmeSl1oB/VgSZzklxzxQEXZUfnWu6rIaxFRdF/pDp1wqaW6QiQaFQy7LFblSBGlGJhWebVD3bJI8p+LaW5Zf3Qi9EUqj0Wg0Go1GozlEAc00DX7+Z/57fu6X/h1//Od/syaiAezkWWv9+q5S8M63vp5//lM/irHBA4VGo9Fotmb9orKc0ILX+kVlY0KinEYzbYwrPhsCbENg5xFm0ockIJNyLe8KXnZGTY343L0MX/oNePL3iyy2cTj2ADz2Abj3W4q8s0PGdwx826TkOeRug6TcJFEGcgzH2Y2EiUQIcC2DbpiS5WqieXi7zSDyhgv9Uir6UbqWx9YJU671YwaJ5HjVpexadML0OvfKiCiVdMOUkmNS9x1KjkGY5oUjRggqbrJpVtZBuFc82+S++erE3G0HyX73fSft1zybY92IZ672J/b5HOTcP3IA9+OUPLf46qUucvj7S2S+JhY6ZpHdZxqC2bLDsaqLYxrMVlxqvs21XoxjJtR9RdUzWerGnKi7LDQ8FmdKByrCri+/GqWSimuCEHh24RYdxBnloajnWMZaSc5+lNKJEnpROrxuijKOvm0gMkHFNTENsWX51RvRG6E0Go1Go9FoNJpDFNAAPM/lX/30P+aNjz3Cv/2Nj3Ct1QauF8c2Y3QPPzc7w4+//3v5znd84z72VKPRaI42ZdfEt02EgCjN2aVp4jpGi8q+bVJ2D3/Hv0azH+xUfLYMgS0ktgwwwsJtlsqNd/SP/vXQxeflZ+DxD8EznwQ1pvvg1OvgtR+ExTfu7MbugKj4HnbZRWYmlxKTBSmAvS0M9+MMzzYJ0yJn7Fo/2nMeHkwmg+hUw2d1WN7uuWt9nrhQ3GunshD4RiXhRu4VKJyRea7oxRlRKvFsg5pXZGjNVV0GccbVXoxnFw65qmfhbPBeD9K9Yhhiou62g2S/+75d+90oXZv7J8FBzv2DWHK5G3GhFXK85pJkOf1YkmSSJFOkuUTmxS/cMQQ1v8gUW+7HnJopSjHapsFCw+dE3WMQZ7QGNolUzJQc5qseD5yoHqgIe2P5Vds0WWy6XGqHlF2jcMrFkkGSXLfptBdlyLzIdpwt23i2SbPsEmUSkeVUPYvZsoMYYzweRwzNc3XLidgajUaj0Wg0Gs1OOPytwMB3fetbefe3vIVPffbzfOqzn+crTz1Hp9ff9PX1aoVHX3Ev7/qmN/L2b/wGLFMvzGo0Gs1eGJUM8mxzYk6B0aKyIQRVz55ALzWa6WMr8dkQYJlGkW2W9iENyLKMbJud/NFwAdqzDHzngJ31SsGlv4PHfw1e+ssxTxZwz9sLx9n8w/vRu90jDHBKVGsNkqCHYQVc7UTMVb09CV2pzOmEKSfqHqmUVF1rT3l4NzIJF9cop+lyJ6JRsjl7pY9jGwySjFwpHMsgyXKSvBAeelFRFk8IqHlWUfrOtYpcNIocpkoqaQ1iyq7Bci9mYYNydtq9Mv2iwvq5fxCP6S7dhIOa+/NccXapx4VWyCCWXGqHgECpwklpCIFrmqTkpLkiGGaCXWyH1H2b5X7CmdkSd8+VEYi1/jqmwWqQcsdMiTuPlTkzu3GZ0v1ko/KrD5yostyLsYdOuRtddmFi0xokXOtDybE52fCI05x+lHGs4mKbJseq441LOxFDo1RyvhVwsR2SSXXLlFHVaDQajUaj0Wh2ylQIaACWafLtb3sz3/62NwNw/tISy6023f6AIIwo+R61SpljzQaLC/OH3FuNRqM5WqwvGXSlE5HKfGKLypYpaPhaQNMcTTYSnwu3WY4lA8ygt6XbbCOCVOJY5nCh/YB+OyqHF/4M/vZDsPSV8c41bHjwO4uMs5kz+9O/3SIMsH3wGuD4GMB8LaUfZyx1Yy53Ik43S7tu/nInQojC4YOCWI6fh7cVk3BxCSF4xckaT1/pYgjBbKXIZgsTSTB0sXTDtMiOSiWOZVDxLEq2iWkYNMvOTUJIs2QziDN6UYZtJpysezc5W27nMr63iqiwfu5/vjtgD5VMgYOd+5+83KXVj1npx3SjlGOWg2EU+ZJZnhOl+bCc48vn5ArSTBKmGUGc0Y1SgkTyylP1tddMw3W7UfnV080SCw2fk3WPfiJvynnL8hzXNnEtA9syiIelViuuSdWzWGj4GzpFt2I7MfRiO+TsUo84lbQGCatBSjS8zkcIUbyfUUnKC+1wXzPkNBqNRqPRaDSaSTM1AtqNLC7Ma6FMo9FoDogbSwZNclH5VMPXZXs0R5bRAvRs2aYdpLgqxstCSAZImZHk45VFS2VOL0qZq7qYhqDm7fOtmkzh6U/A330IVl8c71ynDI+8Fx79QajM7Uv3do0wwHLBbxT9XMdG7o7GLurWjvLJFpslXNuk7tmcawXAzvLwdsKkXFztMKXuF2X8fLvIT8rWZUWVHRMvSLAE1DyHimtS8WzqvoW5Qb6waRiUHZN+LKn7in5SuO/Wc7uW8b2VRIX1c/8LQtBL99beQc39F9shVzoRK4OEOMsxBCSZAhS9uHgTrmVQti1MU2CIQjyTUhFLSS/KuNaPSYcCm0LxylN1BGJqrtv15VfPtQJeXAloRhkn6x5V17rp95YrxSCWhInk/GpA2bGo+xZzFZeZsr1pVuFmbCWG5rniycvdte/gUjtEKUXdt5mruHj2y9lsUVrMaVc6EUvdwq0qpWJ1kPDwQm2skpIajUaj0Wg0Gs1hMLUCmkaj0WgOlv1aVF7cgxCn0Uw7hiE4M+PhZD2M3jKrSxnHyru/vbrWSxBCUPdt5mve/jkgkgF87aPwpd+CwdXxzi3Nwqt+CB75XnCr+9O/3SIEmE4hnG3St43cHcBY4107SDjXCpgpFQvT989X6QTpjvLwxmFSbphelCLzIufs7rkKjaGDLEwlcZpT86xC7BCCkmNwR6O07cK2Z5vDHCZFmGQ3LejfbmV8b1VRYTT3n6i5PJkJumFKrTJ+Owc190ep5OxSj5VBQpTmWGZRfrE1iLFMA98xqTgmxg3CrwnYJniYVF2LlUFKa1CUrRQCyo7FPXOVqbpuR+VXhRBUvOKaagcJdb/IJPQdc+2aChNJlEraQUKS5jR8wVzVY6Zs72pD1FZi6JOXu1xuh5xrBawGKbNlhxP1jcvhlhxolh1SmXO5E3G+FdCPUtRwbHtknftPo9FoNBqNRqOZRrSAptFoNBpg/xaVddbF7cW0Z/5MlDSGuMeC6HItalE2Uq50QhzDp7aL0mXdMKUTJpyo+ziWycm6N/k+By144nfgKx+GuDfeufVFeOz98MB3FO6uqUKAZYNXB7cG2wgQW7k7tipfO1oEbg0SZkrFwvSJusephk8m803z8HbLpNwwg1gSZS+XlxyJAyOBIFcKmYNtClYHKbkCc5ufqWMZKAWJzInT652WR72M70bj3AvXBnTjhJV+SpJKZivuLSEqjOb+1U4fz4IL7YhKOZnauf98KyBOi8yzsmtytQeZzBkkkjsaDiV3+8dbwzCYq7qAYjVIcAzBSysBFdeaqutWCMEjp+rMlB3OLvWo+9aaq7Edhje5Gn3HZK7qMltxaAcpdd/mTHP8DLetxNCR++9cK6ATptw5W9rRtWKbBqebJWqexblWwLlWgBCCmaFAp9FoNBqNRqPRTCtaQNNoNBrNGvuxqKy5PbhVMn/2TJ5DOijEpzQCleMKONP0yTJJkGRc6oQAY4lo3TDlUiek5tvMlGzuOlbGtSb4+XQuwN/9Bjz1/4GMxzv3+CvgsQ/A3W8DY9q+MwGmCW69EM82KDe4GeO6O/pxRidMEUKw2CytuS5G7WyUh7dXJuWGydXLWVAblZc0hk6TREraQUprkAwFhs25rrwk1zvujmoZ383GuVY/4VKnuH7CJOdE3cM0BNv5EKdFVDjV8DledZhxFFXPmtq5P88VF9shrUFCIovSjYYQ5EDZMUnz8Zyfs2WXOM3pxBlXezH5pQ6zJWfqrttTDZ/ZssP5VoBnhxyvepvOsZ0wYRAXc1EvSmkHkxND17v/VoOdi2frGb3+xZWAipdwdqnHbNm5Ne8HNBqNRqPRaDS3BVpA02g0Gs11THpRWXP0uZUyf3ZNFkPch6QHuYQbSvTNVz06QeEguUTxmfRjyVzV2XYB+lovoRMm1HybhbrHsYrLfHVC7rNrT8PjH4JnPwVqvDw2Ft8Ir/0AnPqGbR1dh4JhFW4zv74rYW8jd8dKv8iAfKk1IMkUCoVA4FiCmmdzsu4xW3Fxh66d9dfvKA9vpmRzpRORynzL7347JuniMoTYtrzkXNVlZZDQLDss9xNKjkl5CzfPdeUlefn6OKplfDcb59Is52I7ZBBn9OKMYxWXOJNc6YasDBIWhuLHVkyDqPDA8TI1GxZnfFJhT+Xc3w5TMqlYDVJUrlBG8TupuBaWIehGGa5l7PhzMwxB1S9cZ9d6EUopTtW9qbxuPdvkvvkq98xVtnV5ry+xOEkxdL37r1l2dlXmG4rrvRllXGqH1H2L862A++anrBzwbcptVUVAo9FoNBqNZodoAU2j0Wg01zFuySDPNjlR92iWnQ0XlTVHl1s182fHKFVkhcU9SMNtBaj75ovgICEEJcfiai+iGyVUPZuSbeI5JiYggSiRBKmkFxUL0CfqPjMlm2MVd62dvfT7ePQs1T/+Xbj8xfHOFQbc+86iVOPcg3vrx34hzCLfzK+DufcSa6caPhXH5AsvtlgZpICg4lj0ychzgWFAxbEAwcogZb7m8dhig/oNi8eGUbgro1Sy1C2EuN1kD42YpIur7Jrblpe0TYOFuofMC2fLtV48PHfjx4UkyxECHNPAtYuF+aNYxne7cW41SJC54vxqwAnXo+SYxXwZpDTLLjJX9OOU080Sgs2/w8MWFYQQnPAV9x8vcy0WUzn3j7L8wiQjkTlpkmMYgtPNEqtBSjIUnYEdX3eOWci/gzhjpmST5XDvXGVqr1vDKMaErRyu+7ERar37Tym15xLDJ+vemtju2SH3zFW0MHOI7KaKgEaj0Wg0Gs3twsQFtD/4k7+YdJO74ju+5RsPuwu3DcutNk898yIrq21WOz3KJZ9jM3XOLJ7knjN3HHb3NBrNLhmnZNAtX5ZPsyvW73JfDdK1Rbdpz/zZliyBZOg2k9lNbrMbyZWiG2UM4nTo9BEkUjJTskmynHgolN24AO1YRV5N3bdxLJO7jpX35jzLJTz/GWpf+Pe8beXr451ruvDQe+A1P1xknU0jwgS3XJRqnGAG28hZlOWKZtnmcieiH0uS4SKikQv6SlL1Bc2yTZYrHj/f3lAwWGyWuNAOWWj4nG8F1DxrVy6NSbu4dlpecrbiMoglSimuEXO1F1NJJM2yg3nD4naUSmzTQAiBbRqcawVHsozvVuNcrhSX2iFRJrEMgzsaPkmuMA3BSj/hueUeJdvieM0liCUPnqhuuVlgGkSFEzWXe6vVqZz7R1l+YZpjGoLVQFJ2TBolh1Sq4XyS0glT4qxwpl133SpFIhVpLpE5yDynH2W0w5SyUzwW1z17S+flrcB+bIRa7/6r+/ae3LVQCPZ132Y1SDle9WiHkyl7qxmf3VYRmHPHK5mq0Wg0Go1Gc6sy8aeDn/0/fnUqqvzcjgJaFMU89eyLfO3s83zt6ed58uzzXFpa3vT1X/j4h3b9t5RS/JdPfpb/95Of5atff25tAfRGFhfmeedb38D73/tuyqVbfxFFo7ndGKdkkN45fHtxsR1ypRNxrhXQCXeehTItmT83odQw26wPSQhKbntKnEkudyKWuhEyL8SWKMtRCkq2ySCWDBKJABq+Q8k1MQ2jWIiyDAwhMA3BfM3jZN3bfeaZTODrH4PHfwM658a7uXOr8Mj3wat+EErN3f39/UYY4JTAmwF7csLZZs6iZsnhTLO8oYPyajfmWi/Z1EHpDRefpVT0o5RzrQBgYhlEu2Wc8pKLzeJ3KISgZxd5aIM4ozR0sTmWgVJqKDqYrPRjBIUz5qiV8d1unBvEGVmu6IQpWa640A7JVXGfrChKW17rxwzilNVBymqQcOdsmWNVF2eDz39aRIVpnftHWX5JJvFsg1Tm1L1iTDhWKT4nIQSOWZTTjFKJZ5uYoihRGGU5uQIpc2KZk66VaQUEdMMMIRTL/fhIiDmT3Ag1cv9FqWSuMplxuOJatMOQXKmJ5UZqds5eqwisqpQrodh0HUCj0Wg0Go3mqLBv2+sO8z5qGgS8g+Tjf/KX/OZHPsHzL11E5mPmm+yCF85d4l/+0q/yla8/t+1rz19a4t//zn/hY5/6c/7ZT3yAt77hNfveP41GM3l2UjJIc/sQpZKzSz1WhjuVdyqerWcaMn+AwmEW99a5zXY2jy71Il5YHpBkkk6Y0gkzkuzmHduOYeDYJoYBYSI5UbeZq3j4jkHZtal5FsZub1ziHnz19+DL/xGClfHOLR+HV/8QPPw94JR39/f3G2GA7RXCmTN5cXW/HJSnGj6rwzJnk84g2i3jlJcUQnB6tkTZNbnUKcSSXpTRjyRBkqAUdKKUOJWYwqVecjjZOHplfHcyzoVp8fu/3ImoOCZRVpTIlLlaGwukVFyNYoK0KD1omWLLbLRpEhWmbe4fZfmlUmGI4jO2rWL8FEIwVy0W/VsDcC2TMJN0gpR+nJLnkOb52maH0QYGQwhSmWOIolzrhXbI555foexaR+I6npQYOnL/KQWevTf32QjfMVGq+B0N4u03rWgmy17nQJuMbgpPXx0wNztzCO9Ao9FoNBqN5mDYNwHtsESs23ED1FPPvsgzL5w/kL/1/LmL/Hf/7F+z2umNdd7VlVX+53/5f/Jz/9N/y7d+0xv3qXcajUajOQjOtwLiVHKpHdIsO7sqUQeHnPmThIVoFg+GotnObiBypXj2ap/lfsxqkHK1F6GUourZNEsOrm2s5ZzFac4gyYqcs0RwvOqhVNHGQsPfMg9pSwbX4Mu/DV/93SKjbRwaZ+CxD8ID3z6R/LB9QRhFiUa/Ds4e8+A2Yb8dlPuRQbRXxi0vOVtxqfk213oxjplQ94sSee0gJclyFhsljlUdHjpZo+SYR66M73bjnFKKF1YGLHUi4jQnyxWWIXAtg7JtYZoCQ0CuYDVICOKMDnD2So8zs5VNs9G0qLA5oyw/BcRZsdnBvOGhs+rZ+LZJN0wZdDJMQ+BZJoMkwzIEvm3gmiaGaWCKYuRPspyqa9JPJBdWQ8qOxVOXutOd0TkmexVDR+4/uPkz3y2jdkbzoubgmMQc+PWLLVYTwdVewsV2eCQEZ41Go9FoNJqN2BcBTd//Hk1WVjv8+M/8wtji2QiZ5/yLf/MrNOpVXv/qhyfcO41Go9EcBHmuuNgOaQ0dNifre8js4oAzf/K8yDaLe5DFO3abrefZq32u9SIudSK6YUrDdzhWdTbcse3bJo2STSpdrvUSrnRCgiRbcy3dP65Y2D4Hj/96Ua4xT8c7d/6V8NoPwF3fVAhU04gQYDrgN4rSkvvEQTgo9yODaK/sprykbRosNHxO1D0GccZSt3DInZn1OdUo8YpTNe47Xj1yZXx3Ms6dWw3oDFI6UUKQZByvedQ9C8O4/vdlAsfKLsuqEMdyBdd6EVFqrT00nWm+7ALVosLmrGX5WQbdqBgDpVI3PdBapoFEUbFN4lSigHrJwbcMTMPANIrcPtsUdKMMx8yp+jYlJ6fsWFztxby0MpjOjM5DYuT+g+IznwSjdoRg905szdhMag68o+HxVAarQXp4VQQ0Go1Go9FoDoCJC2i//PM/Pf5JSvHjP/MLazfl3/pNb+S7v+2bJ9ovzd75pV/9bVqrnQ2P+Z7Lu775jdy1uMBKu8snP/PXXLl2czkpKSU//39/iN/55f8Vx57Sne8ajUaj2ZR2mJJJxWqQUvftLUvS7YQDyfzJ4mG2WQ+kZKdusxtZ6kUs92MudSJ6Ucqphk/N334uK0QIj4prcqkTcolCYKmXbOarOxAgl56Ex38Nnvv0+H0/85bCcbbwmimucS3AssGrg1vb934epINykhlEk2C35SVlXvzm+7Hk3uMVTjdLnGz4R1ZY2G6cWxkkrA5S2mFCIhUlx6Li3iyejTAMgWsbJFnObMWl7ll04wz6MQhBxU3WyjlqUWFzRll+xyouy/2YXEGaKdwbnmhHJUe7cUauYL7mbfibkrkiSiUVzyLPFZ5jcrLuUfUsOmE6PRmdU8DI/SdEUaZ0l8PmdYSJXBsDy64WXg6KSc2BNd+mZCmudGNOHZMHW0VAo9FoNBqN5gCZuID22lc+uOc2TszNTqSd25Fmo8Yr7r+bh++/m0cevJt/+Yv/jqsrq3tu90tfO8sf/unnNv6bM3X+7S/8DHfecXLt3/6bH/x7/NQ//zf83dfO3vT685eW+K2P/CH/8H3v2XO/NBqNRnOw9KIUmedEqWSu4k6kzX3J/FEK0sEw3ywCtbdSaHEmeWF5wGqQ0g13Lp6tZ/T6i+2QkmPxwvKAhm/jWhssHCoF5z9fCGcXvjDW31HC4CX/UWbe/hPU75zm7FEBpgleoxDONhEfJslhOCgnlUE0KaaxvOS0sdU4l8icS+2QXpSRZIoZ36YbZWRSsZXu6ZgGcVY4UE1TMFdxudqL8exChK16Fo5paFFhC0ZZfsv9mLNLPYIkI0wzKt7Lj7RZntMaxISJJEpz6r69qSDdj7Pis7ZMchSOaSKEYL7mIXN1+BmdU8Sa+882JzZP9+MMb7iBoOrpjZUHwaTnwKpdlLM9kCoCGo1Go9FoNIfEvmWgaQ6ON732lTz60L08/MDdLMzPXXfMNCfzoPd7H//0psd+6kfed514BoUj7V/8kx/jvf/op5Hy5kXLj3z8T/ng93/nkcgU0Gg0mtuJQSyJshylwLMnI3hMNPNHZi+XaZTprso0bsTlTkSSSa72Iuq+M7Z4NqLm2/Tjop2qZ3K5E3Hn7Mvl28izwmn2+K/BtafHa9xy4aHvpnPvd/P5v32Jd87cc93hXCm6UcYgTgmTfE3A8R2DsmtT86yDc7yYViGaeXUwDm5R+jAdlHvNIJoU01hectrYapxb7sWkUtIaxMMSrYogkSQyx2fza9kyDZSCLFekUlH3LSpp0U7ZNVjuxSw0fC0qbMNis8T5VsBc1aUXp6wMEpplB3MowHfDDJnn9OIUzzE3Fb2iVBKlkppnFW4/Jah4JpYhKLvFWHhoGZ1TyMj9N1OyudKJSGW+p/EzlTmdMOVE3cMyBY1dzqma8Zj0HGgKqHnW/lYR0Gg0Go1GozlktIB2BHjz6x7d1/YHQchn/upvNzxW9j3e8dbXb3jsjpPHee0rH+RvvvS1m45dubbC3z7xdV73qocm2leNRqPR7C+5UmsL7OaExJaJZP4kYVGiMQkg332Zxo3IlWKpG9EJU5RSzFX3tjg0V3XoRgmdMGWpG3G6WcKQcZFt9vEd9TQAACAASURBVPivQ/fieA26NXj0fcV//gx5pwu8tHY4ziSXOxFL3QiZK3Kl1sQBIcCzDAwhMI3CeXGy7m3sipsEwizyzfxGIaIdMLeMg/IAmLbyktPEZuOcUoqVQUIvylDAiZrLxXaE55j0o4yKa2Fu4r4YNaMUa9lazZLNIM7oRRm2mXCs4mhRYRs82+SBkzUurIZ0h2UWL7aLcZThbzBIi40YVWdz8awTpni2ge9YCIpoyKpn0Sw7axsJDjSjc8oZuf+iVLLUjbncGX7mu+RyJ0KIYlPBqYZ/236uB81+zIFl16KdyFtuDtRoNBqNRqPZKVpA02zLF7/8FFGcbHjslQ/du2WW2ete9dCGAhrAZz//uBbQNBqN5hbDEGJtIVjuVuy6gV1n/uRy6DbrFzlnE3Kb3Ug3ypC5ohNmVL3JuJaqnk0nzDju9Ij/+iP4T34YwtZ4DVXm4dU/DK/4bnA2Xshc6kW8sDwgyYoF406YkWTyJpeRY5nUfYs4k1zpRtx1rLyzfLadIkxwy0W5RuvwFtem3kF5wExbeclpYbNxrp9IZK7ox5KyY2KZxeeTScVAZPTjjPomoteoGSFYq8BgGgZlx6QfS+q+4vnlgRYVdsCpYf7etUFMlBUlNUHRLLvkqsjoci3jpky64rvLiFKJZxvUPBtTgFQwW3awTZO56suiwoFkdB4gea729DtfbJa40A5ZaPicbwXUPGtX+VkjUXKxWcK1TRb3IMRpxmM/5kDPNlBxfkvOgRqNRqPRaDQ7QQtomm35+nMvbnrs3rsWtzz33js3P/70c+d22yWNRqPRHBJl18S3TYQoFil3mT1/HWNn/iRhIZwlg4m7zTZiEBc7tpNM0pzEGwZm8jbzL/0eD638MZYMxzu5eQ889n64711gbr5Y//xKQKKK0nxXexFKKaqeTbPk4NoGJiCBOM0ZJBnXejHL/aRwIuWKTpBy33wFwR4W8YVRiHveDNiT2e2+F6bWQXnITEt5yWlhs3EuTDJylZPKnLpXXM81z6IXpVRdi26U4VrGhi69TOYIAZYhsM2Xrz3PNhkkCf0opRMqHjnV0KLCDnjN6UbhCh7um7jSiVjuJwiKkpoznk2WF0JBJhWJLFw3YlhyznesQjzLFWXPourZLNS9mzZIHIbDdK9C141EqeR8K+BiOySTatdOU29YwlVKRT8q3H/AWCJaO0g41wqYKdnMlh3un6/eFq7WaWE/5kDjCMyBGo1Go9FoNFuhBTTNtjz93EubHps/1tzy3Pm5zY8/84IW0DQajeZWo+rZGELg2ebEFhN3lPmTyyLXLOlDluyb22wjwiQnlsWik7vHHdt+/xwLL/wucxf/BENl45188tXw2Afgzm8shKktWI4FM/2EbprSDVMavsOxqrOhe863zWGWk8u1XsKVTkiQZGtl5u7fTe6PMMD2CuHMmZ68rKlyUGqmls3GuTjNSYdjgW0V37VlGjTLDrmCZJjrBNwkCiQyxxQCIQSO9fLv0LEMwkRyWRYl8bSosDOEELztweMoFIYA3zJ4YSUgSDKiNMcQgkH6shvGMgQVz8K3CmFUUDjPyp7FXMWlWXKY3aCk3UE6TCcldK3nYjvk7FKPOJVrWYdRerML2bNNZko2USq50A43zTo81fBZHSQopTjXCnhxJaAZZZzcQHxcTypzLnciWoOEmZLN6WaJE3XvyOcpThv7MQfmeg7UaDQajUZzxNECmmZbLly+uumxZqO25blbHe/1A9rdPo1aZdd902g0Gs3B0vBtLFMwU7K50olIZb6nkobpcMF508yffcw22ynX7djeZRuV1ac49cKHaS59DjHue7jzrfDaDxQC2g5Y7icMMrjSjZHC5FTDp7aDLCXbNFhoeFRck0udkEsUi9T1kr3zco7CAMsFvw7O9M3vU+Gg1Ew9m41zORu7N6qeTZTmQ9E5pROmxFm+lomW54o4zSl7JqYAb5gxKHPF6qDIQ7xjxme+5mlRYUze9sBxGr7DVy92iPOc862QOM2xDYFrG9imwDaLzzvPFTkKQwkMA2bKzpord7G58Wd+UA7TSQtdea548nKXK52IlUHCpXaIUoq6bzNXcfFsA1MIpFJEaU4vSrnSiVjqxiw0fKQsrs2HF2prJUdHPLxQG/ZHUPGKtttBQt23qbgWvmOutR0mkn6c0QlThBAsDkXiE3VvrR3NwbEfc2CU5noO1Gg0Go1Gc6TRAppmWwaDzUtL+d7WC2q+t3W5pv4g0AKaRqPR3EIYRrHzPUolS92Yy53CNbFbLneimzN/ZDYs0XjwbrONuG7H9jgnKkVj+Yucev7D1FtPjPlHTbj/2+E174fZe3Z8WpxJzq1GhBL6seSe+cqOxLP1jF5/sR1ScixeWB7Q8G1ca4uFMSHAdMBvgLsLx9oBcWgOSs0txWbjnMH17o31D1LHKsW1JITAMTN6a1lbJlEqkUrhmAaOZdKPM8JUEsSSLM+peRZzVZf5qhYVxkUIwWNnZpive0ilqLoWz14d4FrGsHwjKFUIoK5t4JgmFc+k6lnYpslC3dvQeTZivx2m+yV0PXm5y+V2yLlWwGqQrolWG214KTnQLDtrLrHzrYB+lK65kB85Vb/u9UIIHjlVZ6bscHapR9231kS/dhhuKPqdqHs0yw7usAykFokPh/2YAwdxhue4eg7UaDQajUZzZNECmmZbBsHmAppjb30JOfbWN9Fbtb0V7U6P5VZ7V+dqNLcSrdUOQRjRWu0cdlc0mjVKIieOImq24uJKF0MmY4s0AN0w5WI7YnHGhyylpga0L11DpQOUzGAfd/uPQxpHZElMFCe0ulDfZoFIKMn8tb/gzvMfpTZ4cay/pSyP+L7vJHro+8jLx4t/7HR3fP6F1ZBOb0A7zDmpMow8oz8Ys1QkYACOyDl3rYOR+zx9IeOOmQ0WPIWBYTkot44yyuQDCYPpnZ9zpQiCAFulXG4lVK0caw8OykzmXG4NOF51CIKALHJYjoMJ9lhzWGw0zqUyJ0sTkiShO4DKDW6Lig3kijTNqTmCKMvpBhG9SOLZBlelJMsyOoMiB63sWGAKOjLneMlgsSpYOaT5/la/33CBh485DAKL5Y5Bo2RTcoxhyU2FEMVnbgiBIRQVC2bLBjYZ3f7mY+RqkBJGEWlskYQGy63Jbuj4+lKfpW7MhXZEN8po+DbzVQfLBFRKlsCodxYw40LVMlnqJZy91KLmWXR6Hu1ujwfni02JV7oxZ68OOL8a0osy7mh41BxFGIZs9+TVcMCQcKHVox+E9AY+pBEnajeLjC5w/4zFxXZGEuV4ZYNcCeI0L5x+FC5AQwgsI6fpKE41LNw8ZrkVT/BT1OyUSc6Bvf6AIE5Zag84M2foOVCj0WzLrX6vodFoDp7djBvHmo2J90MLaJptieJk02OmuXWZBmur3epAGO3u4enTf/lFnnjq2V2dq9HcSgRhxFPPvABAyd9hCTWN5gDoJHA1ErQSwdMSGo7CH6NyT5RDjEPTN+j0Ylwz4K++GpKmydqu92khlLAUClYSuCSgtol+ZqmER+Mv8g3RZ2nkq2P9jcgo80z1zTxbeRPJoARffAF4Yaw2lILzgWA1TGl1+ly5IGlfvTJWG+vJFawkcOVCIQwsltSa+8YwTVzPRzpVgtwhSlKkPFyn4E65FkErESyFgpdeUDT2sAG/nUAoBau+4pqjuPL1yfVTc/jcOM6VTMUgE7QzwVUKEWYjcgWRhEEmCCRYAmQCWIpBBOYwg6snIFUK2xCcDa4weElROqSns6NwvxFkcDEQhJEgbCnKJmSqKPwrKL4H2wDHgLbY2Qi7mkCqBN2LigulyX4/66+veDiPdk3YaUp0KOHpRPCECU1H8TlPUbbgpYGgl0InEcy4is7F8fsWSngqFjztKD5vw5mywtpCZ1GqOCeWkORi7TN3DIVrgm/CFQFfGr8rmgkzqTkwTlKevbxKIzaJVgw9B2o0mm05CvcaGo3mYNnNuPGPfvjvT7wfWkDTbIvnOgzCaMNjmdx6V3uabX18uxKPm/H2t7yOe+9a3NW5Gs2txGiXxbvf/maaM/VtXq3RHCyb75zffJVNKUU7zMjikBk7Zs7JqHs17pyZ3ocopRRfutBjuR+zMki5c9bHMl5+j1ba4/Slj3P60h/gpDt3iwGE3nHkK3+A5N5v55TlcWoP/exFGc2lAU9faZOpizz64F2US7svrwlwpRsRy5wzMyUemC9T9WyEZYFbQzk1ciZf0my/ibOcL57rsNxPuNSJWGx4u3ZQnm9HLNQ9jlUcXne6jrvVCrPmlmT9ONcJU9phxrxS9GLJqYaHadz8G5C5oh2m9KMM0zSouCYl22Su4iCEwLUMPNvAMQXPXgs4XnU4UfN4412NfSkTuBOOwv1GrhR//UKbK92Iq72E+4+X9+wwPXt1sC/fz2gcak54HJot28x1Is5eDXjIszjV2P3cenE4t99/vMSZZom7j+1tPtFMB5OaAy+tdLkSPc9bHr2LM8cbeg7UaDTbchTuNTQazcEyLeOGFtA021Iu+ZsKaGm6dRpMkm4toJVLu6t/36hX98WSqdFMIyXfozlT19e8Zup4y0ydr13qUq++nN1yoSep+wYV18J3zLXslkzmZGlKGvWpZgPqJUHVERyrlLhvvoKYciHmHmlhtwYE+YBAmixUPZzwKgsvfpT58x/HlBvPk5vR8s+wdO/78F/xbdw5N5kbwVAF+H6GYdqUHYtyqUSlvLecmVlMlnoR5bKPU6rQnDsOfh3MWzznxPF56lIXzAGtMKVStmmUdr4Nvx0ktOKUhWaVM7NlHlqo6UyfI8qN49xXLrRpBQmRzFkOc07WPQwhyJUiyfJhtlmOIUxOzfpUPZtmyWGx6V+XUQVwrhVQLvmcPl7lnrkKx2cPNz/wKNxvPJRZONf6DGSPvjQ5Xd+96LOf388zSz1cz6O7mnJqtsYdu8wSrVUgNwM6YcpJ1+VcNwVh43su956sbZh5tlN83+epy11SYRMoi2ajXuSUam59JjAHthNB1TO541id1917Qs+BGo1mRxyFew2NRnOwTMO4oQU0zbaUyz6sbFyKarsMs2Cb45VdCmgajUajOXyEEDxyqs5M2eHsUo+6b9EaJKwGKe0wxBw6LUoiwckHOHlExYJK2cSxDO46Vma+Or3Os/WcrHtc6UYcr3pES2c58/wfcPLqZzDU1htJbmSl8Uq+0HwP8o43MVt1uXumMrE+hklOLIvyl5PaBO45Jq7tkDs1+u4JqDQn0/Ahc6rhszooyoWeawW8uBLQjDJO1r0tF5xTmXO5E9EaJMyUbE43S5yoe3rh8Ahz4zj3hrubfPHFVWSuuNKJCBOJZ5vD14JtGMyUbaqehW2aLNQ9Zis3V1xoBwmtQcJis4RrmyzuUkDRXM9is8SFdshCw+d8K6DmWWMJAyP28/vJc8XFdkhrOAadrO9tHjxZ92gHCRdXQ/qxxDYEdd/ek3gGYJsGdd9mNUg5XvVohynN8h5q3mqmhknMgVXPYsZRHK86eg7UaDQajUZzpNECmmZb7jh5nBfOXdrwWKuzdamqVnvz49VKiUb9cHfaajQajWbvnGr4zJYdzrcCPDtkoe5jIsmTPiLukWcxllAYwsY0BPM1j5N1D3ebnMxpwrVM7s+fg6c+RPPqX491rkLQmn8zZ099D0+p01Q9m1Nlh7uOlSf6GeRKMYqPm4RHwLIsfKdKLE26Zo0Zdet8Xzvh4YUaUAgkFa9wULaDhLpv3+SgDBNJP87ohClCCBabJWbLDifq3lo7mqPN+nEukYrqtQE1L6QbZtQ9i7Jn4ZgGQggsQ9AsO8xV3Q0Xo9tBwrlWwEzJZrbscP98dU2E0+wNzza5f76KlIp+lHKuFQCM7a7Zz++nHaZkUrEapBMVui53IxzTYBDnHK9NZnNKxbVohyG5UvQiLaAdJfY6B9oqpWPDA8fLh/xONBqNRqPRaPYXLaBptuWBe87w55/fOPJ56Vpry3O3On7fXaf31C+NRqPZb/Jhjk0vShnEklwpDCEouyZVz6bh27qc0RDPNrlvvso9DUGv2yHodwhUijTBEB6+Y1B2bWqedWgZP7tC5fDiX8DjH6J5eeO5cDNyYXHt1Dt46cz3ci4/TidMqPn2MKvGnbj7zhCC0Uer9tCOaZqYjk/qNOimJqtRl9lc3Vrf2w7YzkGp1PrXFtf4ibpHs+zgDhfp9a7724u1cW6uwueeX+HF5QEvrgzWFpXnax5Vz6LsbjzO7beDUc9ZBdPuMO1FKTLPiVLJ3AbuxN1QcS36UUbFNYmzHM+ejA3Zd0yUgjCVDOLxHNea6Wavc+Cc67Dsq5tK02o0Go1Go9EcNSYuoF25urLnNvqDcM/tnDg+u+d+aAoevOfOTY899+L5Lc995oXNjz9wjxbQNBrNdBKlkvOtgIvtkEwqcqUIU4lSxSKCb5sYQmCZglMNn8Vm6fZ2D8gMkj7EPQyZUhc59aoD1Vt4p7pM4Zk/gsd/HVrPjXVqZvpcvOPdPHPiPawaDXpBihApJ+o+MyWbYxWX++YnV7pxhO8YeMPajVk+/vmmaWI4HtKuExg+qczphDEMr/myezSv8RsdlMernv7Na7bEMARvvmeWum8zX/PWMiCX+zGpzEmy/EAdjEd5ztqtKDjNDtNBLImyHKWYqNCVK0Wc5aRSYU5I1Bi1o1ThctYcPXY7B/Z7vcPuukaj0Wg0Gs2BMHEB7bv+4T9lt/fro3vyj3zi03zkE5/edR8Egr/+2H/Y9fma63ndqx7Ccx2iOLnp2Fe+/hxxkuA6Gy+SfuHLT27a7lvf8NjE+qjRaDST4mI75OxSjziVaztxo+EiwojRTtyZkk2USi60w9vTjZIEkPQgDgqn1p58T1NCEsCTvw9f+k3oL411amjV+drcu3lq9ltJrAoiAcfKmau61H0bxzL3Nfet7NoYQuBYgmQMAc0wDCzbJXMbhIZPKhVKFg304wxvuHBW9ex96fc0sN5ZpB08mp0wLQ7Gozpn7VUUnJbvZyPWl9udpNA1cj0qFHJCYteoHSE4ci5kzcvsZg7sH3KfNRqNRqPRaA6KfSnhuNf79T3f74sjsIA3RZRLPt/0ptfyR5/53E3HgjDiU5/9G77zHd9407GXLlzhS197esM2T8zN8tpHH5x4XzUajWa35LniyctdrnSiNTeBUoq6bzNXcfFsY223epTm9KKUK52IpW7MQsNHSsXqIOHhhdrRLmezzm2GTIfC2REgXIUn/hM88WGIO2OdGpVOcvGu97K08A4CZXNiuMDrWQaGEAeW+1bzLExDUHMt4hyyfOvvxjAMTNsld2uERpkkVyj58j1U4UBLOVH3sExBwz+6AtoIY5hdpXN+NDvlsByMR3nOmqQoOI0O0/XldicpdNmmgWMJUll852PEvm1KmMi1z+ioupA1L6PnQI1Go9FoNJqb2RcB7TCfwXRlif3hvd/x9g0FNID/6z98mEcevIc77zi59m9BGPFzv/j/kOcbfyHf8+63Td3Dukajub158nKXy+2Qc62A1SBdK9+0UV5KyYFm2VnLSznfCuhHKWo4CT1yqn7Q3d9/kqAQzpIAcsmRcJsBdC/B3/0mPPX7kMXjnTv3ADz2QZy7385sovDilDDJ13ZsH3TumzHMYGp1i9u7lUFKo3rz64QQWLaDcmtEVoVUQi5v/j4vdyKEKBbTTjV87bw6otwuuVn7+T4Pw8F4FOes/RIFp81hWnZNfNtECCYqdLmWgTvcuNGL0omIILeLC1mj0Wg0Go1Go9mMqXSgacbjk3/2ef73X/mtDY+1O91Nz3vXf/2TG/77D3/Pt/EPvvfd1/3bqx++n3d985s2FNFaqx3e/5P/C9/2tjdx5+ICrdUOf/iZz7F0rbVh+4sL8/zQ33/Xpv3SaDSag+ZiO+RKJ+JcK6ATptw5W6KxgxUt2zQ43SxR8yzOtQLOtQKEEMwMBYdbnlwWTrOkD1lydNxmAMvPwOMfgmc+CUqOd+4dr4fHPgCLbwAhMICGz1Q4tE7WPZ69bFKxoBtldMOU2rBfQggsy0a5NWKrSpJDnm3cTjtIaA0SFpslXNtksVk6wHehOQiOcm7Weg7yfR6Ue+P8asAzSz2evdqnNUiYr7kArAbJ0Cm0sWi/1Zzl7muPd8Z+i4LT4q6pekW5Xc82Jyp0NUo2mVQ0Sg6dMCWV+Yaf3U65HV3IB8HtsmlBo9FoNBqN5qgwcQHtx37o7026Sc02xElCa3W8clPApueE4cY78P/HH/tBvvDlJzc8L4xiPvqJz2z7N03T5Kd/4gObZqZpNBrNQROlkrNLPVaGZaJ2Kp6tZ/T6F1cCKl7C2aUes/8/e3ceH8l533f+81R1dVdf6EZjMMAMOMNjOMNreA0jW44sy5EjK7YsS7IsWSfJ5OVkd52Xd7PrbJx4nWycV+LEa8dxXvZm45W9JkVLZuRYty0rsi7HOmyLQ4qkeIx4YjgHOINGA31Vd3V17R8FgIMhZgYN9In+vv/hjNRV/RSmUQU83+f3e9LxkZxsBqBZX602q+6uarMwhNPHo+Dsxa91eLCBQ2+EY/fCzM29GF1XJGI2ByddkjZkEjanl+tRFVk2CfEsTSdLM7QJNqk4W1OqNZkv1phMOUyl4xyZyY7uZ1k2tVv3zbrYbrtOzw945uUKX3rqZRYrTc6VPSZTcSqNgGqzTty2oqB8NSiaziY2DVA2e2YdmezJusotG6eFLPmkQ8w2TKYczi57XQ26QqCQivPU2RZnlj0O7mDxg6qQu2tcFi2IiIiI7DbdD9De/45un1KGxNRkjv/0y/+E/+mf/juWlssdH29Zhl/6ub/P99xxSw9GJyKyPSeLNRp+wOlSnUI63nF4tiafilPwWpwu1cklY5ws1jg8s0n/vGHVDlb3NqtErQx3U7VZ2IbnvwoP3Q8Lj3V2rOXATW+FOz8I+YO9GV+X7cnEScdgdiKBR5zFwKXSmmQikcIEhksFomuVHMVqk8mUw8FCitmcO7ST0MNg1CoJdvO+WRca1eu83Oep0mixsOzx4mKVhRWP585ViK0GZqW6D0ST8I5lkXFtmkHAYrXJ/pzLVObV9WUXP7NOlS5RjtoH47aQxbKigMTzAxZWGl0Nug5Mpni5En2OTxZrTLixbf1coyrk7tptYb6IiIjIOBnsUkMZOYeuvorf/pVf4F/9h9/h8aef3fJx01N5fv4f3sMbXnush6MTEelMux1yqlSnWG0ShiH7cu6Ozrcv565POrlOnUPTmaGaPN/Ubq02Awh8ePpP4OEPw9ILnR0bT8PRn4Tb3wvp6Z4Mr5f2T8SZ3buHmrOHs9WQFxarhKVlckmHTCJGMm6vBwj1ZkCl0WK57mOM4UAhtd467Zb9E4O+lKE0qpUEu3HfrM2M2nVe7vMUErJYaVKq+VQbLV5YrNIOQ2KWxTWFFG48+qy1w5Bmq03dD1iq+pRqUWvAoB1SbQQcKCRfFQZe+Mxqeu2BteEfx4UsBwopXirVux50HdqbIZ+OEwQhFc9nvlgD6OjcqkLunlEN80VERETkFQrQpGPXHtzP7/77X+QzX/jvfOrzX+Xxp59bn2S42NzsNG9+w2u5+11vIZ3S6jkRGS6luk8rCFmq+eSSzo5aKEHUSiqXdFiq+ezNupTq3dnbpOt2c7UZRGHgdz4Oj3wUqi93dmxqCu54P9zyE5AYzonXyzIWViJDO72Xq+auxjNxvIUyN8Wz66veS/X6pqveZ3MuhXSchGNvuup91KqtemVUKwnGpUXeqF3nlT5P58oNKg2fajPAb7UxhPjtkOmsS+6i60rEou/FIB1SrDY5X2muBnHRyQ5ObawiuvCZ5aYt6h1uB9kN47qQxV29z/Yi6JrLJ1la/XrOF2u8sFij4LXYd4kQeY2qkLtv1MJ8EREREXk1BWi7wFvf9Hre+qbX9/U9LcvibW9+A2978xs4t7jEk8+8wOLSMqXlMumUy9Rknquv2sf111zV13GJiHSi7PkE7TaeHzC9SYur7cgkYpTqddphSNkbsgBtrdrMr0Kwy6rNAGqL8O0H4fE/hEaHrYZzB+HYB+GGt0CsO5+FvjJWNO5kjsAKWKo9QRiGzE0mmUrHOVms4Tp19mbdjqulRrXaqttGuZJgXFrkjdJ1buXztFzzabQCqs0WQdAmJKoya7Ta1BsB58oNpjPx6BvxArZlmM4mSMVtzpUbnKOBWQ27L27n+Mozy9AYQIA2tgtZoKdB11r1sDGGjBt9vkq1pqqQ+2jUwnwRERER2ZwCNNmx6alJpqcmBz0MEZGOVRsBXitqW+U6O5u0W5OM24Qh1P2A6iBmIy+226vNAJZfgocfgCc/A0Gjs2P33gLH7oHrfhCs4QkCtswYsOOQzEM8A8YQVkobKsNdx+bwTJZD05mOK8hGtdqqF0a5kmBcWuSN0nVe6fPkB23OV5s0V59R1+/NUvF8XirVWar5VJstEl702uns5qF/OhH9qvdyuUHZ8Tm9bJi4KKRae2Y1/DbNdv8rtcZuIctFehV0GWM4OpdjMh3nxEKZXDK24ypk2bpRCvNFRERE5PIUoImIyNhqh+H6JJLdpYqQtfOEYXT+gdnt1WYA556C4/fDM3/WeTB44LVw1z0w95pXVW+MBgOxGCRy4Oa2dA2WZSik41uaTB7laqteGOVKgnFpkTdK17mVz9O5cgM/iILrTCJGOhGj5rfIJByqjYBm0GbFi4IU17HIus6m75VOxMg0o/OkE1FF2v4LPntrz6yovq3/xmIhy2X0Ouiay++8Clk6N0phvoiIiIhcngI0EREZW5Yx67lD0KWwa+08xkTn76txqDYLQzj11/DQ/XDym50dayy4/k1w7G6YvrE34+s5A7b9SnBmdWfC+WKjXG3VbaNeSTAuLfJG5Tq38nlqh9EeZmWvRRiy/r6G6JkVj1mkEzbVRkDcblGsQipuY1/iflBIx6k2WpS9FnG7paYpZAAAIABJREFUyWzOXX8+rT2zLAyDiEF39UKWDvQy6NpJFbJ0bpTCfBERERG5MgVoIiIyttIJm6RjYwx4fpttLhDeoN4M1ie60ok+reBeqzZrVqMQbTdWm7UDeO7LUcXZy090dqydgJt/HO74AORGeG9OKwaJCXAnwO7dj3CjXG3VC6NeSTAuLfJG5Tq38nmqNlq02iEVLyCVsLFXJ8sd2xCzohAtZixcB8qNVrRfWr11yfHZliGVsKl4AblkSLXRWq9YW3tmJRyLuNX/Z8euW8iyA70OujqpQpbtG5UwX0RERES2RgGaiIiMrazrYBmD69hdmxytNFq4q6vEL9VSqyuC1mpoVoFWc3dWm0FUSff0H8PxB2B5vrNjE1m49d1w23sgVejN+PrB2NG1JHNg9/AzxehXW3XbbqgkGJcWeaNwnVv9PNX9KDTx220mnFe+/+IxG2MMtmVoBAHZhEPDD6j5ATHPZzLlXLJlatKxqTWj9637wfrz6cJnVr/WfFxo1yxk6SIFXaNtVMJ8EREREdkaBWgiIjK28kmHmG2YTDmcXfbwg/aOVgr7QZvlus9sziVmG/LJLocdYQh+bbVNY201NNuF1WYAjTI8/kfw7Y9CbbGzY9N74Y73wy3vgHi6N+PrB2NBIg1uHmLdmYS7klGvtuq23VBJMC4t8kbhOrf6eWr4bfwgCgPjsVdek4xZWCYKCKuNgGwiJOFYeM026Th4rYCks/mvd/GYRRhCM2jT8KMFFxueWVab5ACyppFeyCKyiVEI80VERERk6xSgiYjI2LKsaB8Rzw9YWGlwZtnjYCG17fOdWfYwJlo5PpdPdq+ypNV8pdosaO3eajOA6jn49h/A4/81aknZiclr4M574IYf6XmlVk8ZC+JJcCfB2VnFUyd2Q7VVt+2GSoJxaZE3Cte51c/ThWHghvddDYSCdptqI6DcDIjbFo1WizAMabbaXGrdhrVJGHjhM6sQDzk7gH/KkVvIInIFoxDmi4iIiMjWKUATEZGxdqCQ4qVSnf35JCeLNSbc2LaqbtaCggOFFAnH5sAOgjggmiVpVqFZhqa3u6vNAErzcPzD8NRnoe13duzsbXDsHrj2B6LwaVQZKwrM3DzEd/j52YbdUG3VbbuhkmBcWuSNwnVu9fN0YRh48WT5RDJG2fPJJhxWPB979fPUaof4waWfEe2LwsCLn1lz+RiP7PgKOzcyC1lELqPdDtf3rXvhfJVTpTrnKw0Wyg6T6QSZuH3J9qpbMYyLFkRERETGhQI0EREZa65jc2QmSxCEVDyf+WINoKMQrVRrMl+sMZlymErHOTKT3f5+T60GNKrQXIF2ALt9pfHCd+D4/fDsl+g4ILz6dXDX34V9d8AoTygZE7VoTOYhntnWKS6cvDt1rsrZuuHEy1WqoUPWdcgnnStOJO+Gaqtu2w2VBOPSIm8UrnOrn6eEYxG3LYyBZqtNIvbK8yRmWRTSCdphg2YQUG60aAXRecPLfJ6arTbGsFqxFrBUbG54ZiXajR1f33YN7UIWkSvw/ICTxRqnSnVaQUg7DFlY8ShWGhSrTV44X6NY9bEtw1Q6zp5sgvg2FqcM46IFERERkXGhAE1ERMbeXD7J0mrbuvlijRcWaxS8Fvty7mWrcPygzZllj2I1mog8WEgxm3OZyyc7G0C7DX412vfL93Z3i0aIkoOT34yCs5f+urNjjQ1H3gx33g17DvdmfH1jIBYHNweJ7LZCwM0m784t1TjvwfPna1SCaPI/ZkdVHgcKqUuGu7uh2qrbRqEt4JWMS4u8UbjOrX6eoko6g2NZ1P3gVeFd1o3htVoQOrSCkJV6g0rDJ5+69K92dT/AMnC+2sTz2+zPuxueWeeLgwvQhm4hi8gWnCrVObFQpuEHFKtNlmo+nh9QawScXWmwUvepNwP2ZBNkEjZ+ELBYbbI/n2Sqw4B/GBctiIiIiIwLBWgiIiLALfsnADDGkHGbnC7VKdWa5JIOmUSMZNzGNoYgDKk3AyqNFst1H2MMBwopptJxZnPu+nm2xG+s7m1WHo9qs3YLnvkiPHw/nHu6s2NjCbj57XDHB2Bif2/G1zcG7FgUnLm5bVfPXXLyru6x2DA8t1jjbK2N69hMphw8P+ClUp0jM9lNQ97dUG3VbaPQFvBKxqVF3ihc51Y/T+lEjJhlyLg2S1WfIB1iX/T+a1WidT8gFY/RaoecrzTXq/DiMWvDM+tMqU7MtjDGcMeBPNOZROfPrB4a+EIWkS1qt0OeOLPC2WWPxWr082IYhuSSDtOZBPGYIXHWIpOwOV9pYhtYqvmUaj6FdIKgHVJp+BwspDBc+b4yrIsWRERERMaFAjQRERGi4OzoXI7JdJwTC2Vyydh6KFGq1zdkW8ZEK+Zncy6FdJzE6ur5LU3YtduroVllPKrNAFoePPkZePgBWDnV2bGJHNz2U3DbuyE52Zvx9Y0B246uyZ0Aa3vhyZUm7/y0RfFkyHV7Ujhxl7Lnc3bZY2Glwf58kiAIWao2uWX/xIY9WXZDtdVWXNjustoIaIchljGkE/ar2l2OQlvArRiXFnnDfp1b/TxZq8FdMwgo1XyK1SbT2YvbqhqmMy7VRkDaD5hMOaQTMZpBSLXZ3PDMWvF8Wu2Qg1NJDk2nmc25W39m9dFAFrL0USf3nmF+j3H3xJkVzpTqzBdrLNX89c/dhUHvbM4FE1JrBtiWxYHJBMWaz/lKA89vrS+YurqQvuL7DeuiBREREZFxoQBNRETkAnOrrXVOFmu4Tp29WZd2GFL3A8KQ9cqRrbbFWzdu1WYA3go8/ofw7QehXuzs2MwM3PkBuPkd4AzXJO+2WDFITETBmb2zH7+uNHm3EvrErOhzOpGOU0jH16s0ThZrVDx/fa+ko3O59fPuhmqry9ms3eWVvq9HoS3gVoxLi7xhv85OPk/T2QSL1SaFdJzzlSapuE06sfHeEbSjBRjX7slgWzCZjtNuR3uhNYP2avvUFmEYMp1NMJWJ873XTnFob2bo/u2gjwtZ+mw7955O/3368R4SVX6fXfaYL9ZYrvtcM5Xa9P6y2ffvdCZByrE5V2lApQHGkEk0L9vOcdgXLYiIiIiMAwVoIiIiF3Edm8MzWQ5NZ3a2knscq80AKgvwyEfgO58Av9bZsYVDcOweOPzDYO+CNkXGhkQGkvmuXM9WJ+8u5tgWBwspJtwY88Ua88UaxhgmV1e0w+6pttrMpdpdbjYhv1m7y2FuC7hV49Iib5ivs5M2k45tsT/nErSjIORcOdqj7MIQrVjzMUA+FWN2Ism+nEulGVBvtmj4bZa9JtVGi2v3pLl+JsvfuHpyJCbge7aQZQB2eu8ZlveQKKQ8sVBmcfVrfLnn75W+f18uN3CdFqdLdbJujPgm96ZRWLQgIiIiMg4UoImIiFyCZUUT3R0HCX4DGmXwKz2vNmuHIStei2rDp95sr4d8ybhFOuEw4cb61zqv+Dw8/GF4+k+i/c46se+OKDi75vvBbL/CZ2gYCxJpcPPR/m1d0Mnk3aWsvf6FxRoZt8mJhTJT6TiuY++aaqsLXandpeu8sk+U57c3bXdZSMdJxKyetQXsZ8u13d4ib80wX2cnbSanMgmqjYAwDDlHg5fLDTLNgEI6jucHVLwWezIJHNtmTzaBMYZsIoYbsziz7NEK4Pq9GQ4WUuxbDZlGRdcWsgxIN+49m7Xa7fd7yCtOFms0/IDTpTqFdPyKz4HLff9m3BjFaoN0wuJ8Ofr3WDNqixZEREREdjsFaCIiIt3Q52qzRivgzLLHwopH0I7aNXmt9vrqfDdmYRmDbRlmJlz25VwSsR6tXD77GDz0e/D8Vzs/9to3RMHZvtu7P65BMBbEk+BOguN29dSdTt5dSj4Vp+BFK99zyRgnizUOz2Q7qo7ZimHYt2Ure9WsScW5ZLtL2zZMpeNdbQsI8N2Fcl9bru3WFnkXG+br7LTN5IFCcv2ayk60H9pipUGj1SaXjBGPGfZkErSCNuW6P7Kh56VseyHLgHXr3gMbW+32+z0k0m6HnCrVKa5Wt+7Lbe35vtn3b7XRwnUsas2AxUoTMOSSUWXgbvv+FREREdkNFKCJiIjshO9BoxJVmwUB0Pu9zRbKHs+fr9JsBSzXfZbrLZqtV7drisdscskYjVbA2RWPa/ekmcl2KdQJQ3jxa3D8fjh9vLNjLRuO/EgUnBWu6854Bs1YUWDm5iHe/SqP7U7eXcq+nLteEeU6dQ5NZ7As01F1zOUMw74t3Wx3efVUGtsyHCykutIWEOAbzy0OrOXabmqRdznDep2dtJk0xnBwKkU6YTNfDKk1A8qNFjE7etqseD4LKx4LK6Mdeu4mvWy128/3kFeU6j6tIGSp5pNLOluuzr7w+/f0clQ5WfZaVLyARivgxWKNSiOg0WqTitv6/hUREREZQgrQREREOtUOokqzRgVajb7tbdYOQ555ucL5SoOlms/LZY8wDMm6DoVUnIRjYQMB0PDbVJstzpUbnK80o4njdshyzefwTAbDNquBAh+e+UIUnC0+09mxThJu/gm4432Qnd3e+w8bY6IWjW4+2uusR7Y7eXcpjm2RSzos1Xz2Zl1K9WjPs06rYzYd6xDs29KLdpfT2ThTmcSO2gLunUgAIU+eXhl4y7VRb5G3VcN6ndtpMxmGIYmYxXV7MqTiNrmkw95sgpDdE3qOul632u3Xe8hGZc8naLfx/IDpTOdtmacyCSaSDufKDeJ2k1wyJOvaLKw0mM0l2J93OTCZ0veviIiIyBBSgCYiIrJVvre6t1m1b9VmF3rm5Qrnyh6nlz1W6j75ZJw92fimYUrSscmnHPwgwblyk7PLdWrN1nq7prUWclvm1+GJT8Ejvw/lM50d6+bh9vfCre8Cd7e0iTIQi0fXk8hGs9c9tNPJu81kEjFK9TrtMKTs+est0jqpjrnQMO3b0qt2l1k3xkzO3XZbwKVqc+haro1qi7xODdt1bqfN5FWFFIV0HCdmMTvhkknEhiIMlFf0utVuv95DNqo2gvU22a6zvQUsjh3tpTmbc6k2WhSrDs0gZDIVZybrcsNsVt+/IiIiIkNoKAK0peUVvvDnf8ljTz3Ld587SWmlTKVWx/f9bZ3PYPjmZ3+vy6MUEZGxNKBqs4stlD3OVxqcXvYoez5z+SQTSeeKx0UTNi6ZhM3p5TqniSZucylna+0c6yV47GPw6IPgLXc26Ox+uPODcNNbo+qzXcFALAaJXBSe9Tg4W9ONybuLJeM2YQh1P6DaCDb8f9upjhmWfVt63e7yBw5Pb6st4GK1qZZr8irD2mZSOtePVrtAX9r5ykbtMFwPte0dPvctY8i6DnHbYqnmc9Vkimv2pLl6Kt2FkYqIiIhItw00QCtXqvzG7zzIn375G7SCFsCG1ZbbZvpbESAiIrtQsx4FZwOqNrtQoxXw/PkqSzWflfrWw7MLrb3+VKlOKh7j+fNV8kmHROwSk7ArZ6Jqsyc+CS2vswHvORLtb3b93wZrKNbqdIEB234lOLO6E2JtVTcn79asnScMo/NfaDvVMcOyb0u/2l120hZQLdfkcoa1zaR0ph/3HqAv9zfZyDJmfb1M0JUJi1fOY0x0fhEREREZTgOb1XrxpbP8zD/7d5xfKr1qEmYnuvTzrIiIjKMhqTa72Jllj2Yr4OWyRy4Z7zg8WzORdKg0ovNkXZszyx7XXLziefEZOP5hOPGnEAabn+hS5u6CY/fCwe/rW2VWX1gxSExAMgfWYMKKQU3ejWJ1TD/bXW61LaBarslWDFubSelMP+49QN/ub/KKdMIm6dgYA57fZpu38A3qzWD9GZpOaCGEiIiIyLAaSIBWrlT52V/8Vc4VS8Arc2xhqABMREQGYK3arFmNQrQBVptdrB2GLKx4LNejvY+mszubtZnOxlnxmizXfRZWPA4Wok3rOf0wPHQfvPgXHZ7RwHV/C+66B2aO7mhsQ8fY0f5myRzY2wstu2WQk3ejVh3T73aXV9KPtm7D8HUXGXf9uvcM0/1tXGRdB8sYXMfuWshYabRwVxegZN3B/owhIiIiIpc2kADt9/7LZzl7bnFDcAZw9Ibr+J47j3Ldwf1k0ikSCa1+ExGRHmkH0ChHwVmrOTTVZhdb8VoE7ZDleous2512TVnXYbneYioVUHv6S2Qe/wic/XZnJ7JicONb4M67YfKaHY1p6BgbEmlw8xAbjp9FhmHyblSqY/rd7vJK+tVSUoZPux2OROgs3dGve88w3d/GRT7pELMNkymHs8seftDe0b3cD9os131mcy4x25DfZmcBEREREem9vgdoQdDmE3/6lQ2dna7at5d/+XP/gNtuur7fwxERkXHTrK1Wm9WGrtpsM9VG1BKq2QoodKPsCEjbbWZO/Rm3P/lZ0pX5zg520nD0nXD7+yAz3ZXxDA1jQTwF7iQ43WmN1S2avNu6Ydurpp8tJWU4eH7AyWKNU6U6rSAc+ran0h39uvcM0/1tXFhW9L3q+QELKw3OLEcV/Nt1ZtnDmGhRylw+qSBdREREZIj1PUB7/KlnqNbqGBOtcstlM/z2r/wzpqcm+z0UEREZF0FrNTQb7mqzzdSbbRpBtKo9scN2TVarzszJz3Hs+T/CbZzv7ODUFNz2Hrj1XVFbw93EWOAko4qzeHLQo9mUJu+2btj2qhm2lpLSW6dKdU4slGn4AcVqk6Waj7canq0xJmqNOply8PyAl0p1jsxkmcsP5/1HtqZf955hur+NkwOFFC+V6uzPJzlZrDHhxra1n+VaC94DhRQJx+bADp7lIiIiItJ7fQ/QXjx1dv3PxsAH3/kjCs9ERKQ3RqzabDMbWkJt8xyxRol9L36K2flP4/iVzg7OXRW1abzxxyA2XFVZO2as6JqSeYinBz2aK9Lk3dYMQ7vLCw1bS0npjXY75IkzK5xd9lisNjldqhOGIbmkw3QmgetY2MYQhCGe36bs+Zxd9lhYabA/nyQIQpaqTW7ZP4FRFdBI6te9Z5jub+PEdWyOzGQJgpCK5zNfrAF09Bwu1ZrMF2tMphym0nGOzGRVfSoiIiIy5PoeoJWWywDrLUz+5mtu7/cQRERkNxvharPNbGgJ1eGxidpZ9j//X9n70uex283ODp6+EY7dA4d+CKxdNrljTBScuXlIZAY9mi3T5N3WDFu7y2FrKSm98cSZFc6U6swXayzVfKbScWZz7qafvVQcCuk4ftDmzLLHyWKNiucTrv67Hp3L9Xv40gX9uvcM0/1t3MzlkyxVm4RhyHyxxguLNQpei32X+F5fs/a9Xqw2mUw5HCykmM25qjoVERERGQF9D9AuNrt3atBDEBGR3aBZg2YZGrXV0Gx3VGUk4xZuzMIYaPhtklsIO1IrzzL33MfYc/bPMZ0GiFd9D9x1b/TfXTcxbyAWBzcXtaEcwevT5N2VDVu7y2FrKSndd6pU5+yyx3yxxnLd55qp1JaCbce2OFhIMeHGmC/WmC/WMMYwufpZk9HSr3vPMN3fxtEt+ycAMMaQcaNq01KtSS7pkEnESMbt9WrTejOg0mixXPcxxnCgkFoP19fOIyIiIiLDre8B2lRh44rKlt/q9xBERGS3WKs2a5Qh8Ee+2mwz6UTUEioes6k2W+RTl1gdHoZMFB9l7rmPMXn+W529ibHg0Bvh2L2w96Ydj3n4GLBjUXDm5kYyOLvQlSbvWn5Aqx3tj+VXGmM5eTdM7S6HraWkdJfnB5xYKLO4ut/ZVsOzC629/oXFGhm3yYmFMlPp+K6rDh0H/bj3DNP9bRwZYzg6l2MyHefEQplcMra+32GpXt90v8PZnEshHSexWkmugFxERERkdPQ9QLvh0DUb/r5wvkg+l+33MEREZJQ1q6vB2e6qNtvMhBvDtgy5ZIxz5QZ+kNhYaRS2KSx8g7nnPkZ2+amOzt22HMxNb8XceTfkD3R55MPAgG1DYjU4s7bf5mqYXGnyrlb3eNkzPHe+RirZHsvJu2FqdzlsLSWlu04WazT8gNOlOoV0fFtBBkSfzYLX4nSpTi4Z42SxxuEZ/Y40avpx7xmm+9s4m8snmUrHOVms4Tp19mZd2mFI3Q/Wt6tIri50iNlRdeKBQkpfZxEREZER0/cA7fprrmJudppTZ88B8K1vP8kNh67u9zBERGTUBD40Vvc226XVZpuxjGFmwqXRCjhfaXKu3GR/3sUETaZPf4n9z/8hqepLHZ2zaaU4e/WPYW5/LweuOtijkQ+YFYPEBLgTUfXZLnSpybtzSxbn5kOum0oxPZkd28m7YWl3OWwtJaV72u2QU6U6xdXP2b6cu6Pz7cu561VBrlPn0HRG/74jqB/3nmG5v40717E5PJPl0HSGUt2n7PlUGwHtMMQyhnTCJus65JOOvpdFRERERtRAZpTe946/w6/+Pw8A8F//+Iv81NveRMwej8kcERHpQBiCXxubarNL2ZdzObvisTfrslhcpLDwFa499WkSjcWOzuPFCzy650dZuvbHyeXz3Dmb79GIB8jY0f5myRzYu78yZ7PJu4wd8KwL1+5JMTedHevJu2HZq0Yt13anUt2nFYQs1XxySWdHlYUQ7YmWSzos1Xz2Zl1K9e60/JT+68e9Z1jubxItlCik4/p+FREREdmFBhKgvfNH/xZ/8sWv8Z0Tz3F64Ry/9Xsf4x/99HsHMRQRERlGY1ptdimJmM2htMdVT36EvS9+hnhQ6+j4evoqnp17B99Kfh/pVIq5iSTX7kmTiO2ixSvGhkQa3DzExm8C68LJu7TxeTwZcmRvmj2F9KCHNlDDsleNWq7tTmXPJ2i38fyA6UyiK+fMJGKU6nXaYdi1PfPWtNvhJatk/Lq/4ftBdqYf955hub+JiIiIiOxmAwnQLMvi//rFn+Xv/+//htML5/mDT36eMISf/XvvViWaiMi4CkPwq6vBWX1sq81epXQSHn6A6ac+A0Gzo0PLuRuYv+ZdPJk8xrIXMJF02J9z2ZNJMJPdWauxoWEsiKfAnQSnOxPYsvsMw141arm2+1QbAV6rTRiC63Rnj8Vk3CYMoe4HVBtBV87p+QEnizVOleq0gnDTz36lWuO5SrR3YiarcLZb+nHvGYb7m4iIiIjIbjWwTUGmpyb5nV/7RX7+3/wmjz31LA9+6vP89798mJ/68Tfx2mO3cvVVs4MamoiI9NN6tVkZgtbYV5ute/lJOH4fPPuljr8m56fu4rtz7+Sl1E2UGy1Ms81sLslkymFPJsHhmUxvxtxPxgInGVWcxRUkyJUNw141arm2u7TDcL3Kxzbd+cysnScMo/Pv1KlSnRMLZRp+sF6d5K0GK2uMgcBvstKEF4s1quGiqpO6qB/3nmG4v4mIiIiI7EYDCdDe9vf+8fqfgyBaWRmG8NKZl/n1//cjADixGBPZNI7T+f4lBvjk//drXRmriIj0gKrNNheG8NJfwfH74eRfdnRoG8Pz+b/Jo3vfRjF1LcZAPAiZzibIJR3iMZtr96RHv/LMWBBLQDIP8fFuTyjbM8i9atRybXexjGEtNwu61P9w7TzGROffrnY75IkzK5xd9lisRmFtGIbkkg7TmQSuY62HtZ7f5myxRbllOPFyjbadIAhClqpNbtk/gelSODju+nHv0V5cIiIiIiLdNZAA7czCeYxhvaUEvPLftd89m36L88XlbZ1fv+OJiAypwIdGeXVvM1WbrWsH8OwX4fiH4dyTnR1qxVm46s28dM07WY7vJRNC1oAbs7CMwbYMMxMu+3LuaO95ZkwUnLl5SOyCCjoZa2q5tjukEzZJx8YY8Pw2HWxpd0n1ZrD+759ObP/f+4kzK5wp1Zkv1liq+evVi5u1C03FIRYmecENmXBjnCzWqHg+4eovZkfnctseh4iIiIiIyCgbWAtHeHV4dvGft0ObX4uIDBlVm11aqwFPfRYefgCWT3Z2bGICbn0X3PpTJK0J9jd8Jpvt9XZNybhFOuEw4cZ2VMUweAZicXBzkMhqlYzsGmq5NvqyroNlDK5jU/b8rlT9VBot3NXwNOt23okDoraNZ5c95os1lus+10ylyG8h3bMNzOVd2pbDfLHGfLGGMYbJdFyVjyIiIiIiMpYGFqAp6BIR2eVazajSTNVmr9Yow2N/CI8+CLXFzo7NzMAd74eb3wHxFBaQB/LJ7U20Di8DdiwKztycgjPZtdRybXTlkw4x2zCZcji77OEH7U0rvLbKD9os131mcy4x22zrvu75AScWyiyutgbdanh2obXXv7BYI+M2ObFQZiodVwWkiIiIiIiMnYEEaP/if/3pQbytiIj0mqrNLq9yDr79UXj8j6KvUycmr4Vjd8ORHwF7t4VlFzJg25BYDc6s7U9Gi4j0kmVF7TU9P2BhpcGZZY+DhdS2z3dm2cOYKFCdyye3VXl4slij4QecLtUppOMdh2dr8qk4Ba/F6VKdXDJq63h4Jrutc4mIiIiIiIyqgQRoP/a3v38QbysiIr2yXm1WhiBQtdnFll6Ahz8MT/0JtP3Ojp29De66F655PZhdHiZZsag1ZTIHliodRC7Wbodj2e5xmK/7QCHFS6U6+/NJThZrTLixbYVWpVqTYrXJgUKKhGNzYBtBXLsdcqpUp1htEoYh+3Jux+e40L6cuz4u16lzaDqzKz9fIiIiIiIilzLQPdBERGSEhSE0q1Fo1vQgDAY9ouGz8Dg8dD8892U6rsS7+vuj4GzfHbu/faGxo/3NkrldXl0nsj2eH3CyWONUqU4rCGmHIXU/IAyj20Nydc+smB1VRB0opHZFu71RuG7XsTkykyUIQiqez3yxBtBRiFaqNZkv1phMOUyl4xyZyW7rOkp1n1YQslTzySWdHbWTBHBsi1zSYanmszfrUqp3Z583ERERERGRUaEATUREOtNqRi0afVWbbSoMYf4bcPw+OPVQZ8caG468Ge68G/Yc7snwhoqxIZEGNw8xTcqKbOZUqc6JhTINP6C4uq+VtxoirTEmCnImUw6eH/BSqc6RmSyEqyHbAAAgAElEQVRz+eTgBr5Do3Tdc/kkS6tVX/PFGi8s1ih4Lfbl3MuGWH7Q5syyR7HaZDLlcLCQYjbnbnv8Zc8naLfx/IDpTGK7l7NBJhGjVK/TDkPKngI0EREREREZLwrQRETkylRtdmXtFjzzZ3D8w3D+6c6Ojblw89vhjg/AxL7ejG+YGAviKXAnwenOJK/IbtNuhzxxZoWzyx6L1SanS3XCMCSXdJjOJHAdC9sYgjDE89uUPZ+zyx4LKw3255MEQchStckt+ycwI1TFOqrXfcv+CQCMMWTcaNylWpNc0iGTiJGM2+vjrjcDKo0Wy3UfYwwHCimm0nFmc+76ebaj2gjwWm3CEFynOy1/k3GbMIS6H1Bt6NkvIiIiIiLjRQGaiIhcWqsBjdXgrN1iw9J/ifh1ePIz8Mjvw8qpzo51c3Dbe+DWd0My35vxDRNjgZOMKs7io1sZI9IPT5xZ4UypznyxxlLNXw9YNqtoSsWhkI6vVzSdLNaoeD7h6j376Fyu38PftlG9bmMMR+dyTKbjnFgok0vG1ivnSvX6ppVzszmXQjpOYrUN5E4r59phuP4+dpfCw7XzhGF0fhERERERkXGiAE1ERDYKQ2hWVts0qtrskrwVeOxj8OiDUF/q7NjsbFRtdvPbo0BptzMWxBJRSBhPD3o0IkPvVKnO2WWP+WKN5brPNVOpLe2p5dgWBwspJtwY88Ua88Uaxhgm0/GRaOe4G657Lp9kKh3nZLGG69TZm3X7tnebZcz6lplBl8KutfMYE51fRERERERknChAExGRyHq12Qq0A1WbXUplAR75CHzn41H1WScKh+Cue+H6N4Ht9GR4Q8WYKDhz85DIDHo0IiPB8wNOLJRZXK1e2mqIdKG117+wWCPjNjmxUGYqHe9KSNMru+m6Xcfm8EyWQ9MZSnWfsudTbQS0wxDLGNIJm6zrkE86WFb3Qql0wibp2BgDnt+mwy/fpurNYD30SyeG9/MjIiIiIiLSC0MboDWaTcqVGq3W9iofZvdOdXlEIiK7ULsNfhUa5dVqs/agRzS8is/D8fvhxOeidpad2H8nHLsXrn4djMUKfgOxeNSiMpEdk2sW6Y6TxRoNP+B0qU4hHe84RFqTT8UpeC1Ol+rkkjFOFmscnsl2ebTdsxuv27IMhXScQroLSdYWZF0Hyxhcx6bs+V1530qjhbtaMZd1x2Dhh4iIiIiIyAWGJkD7+rce5S/+6hEee+oZnp8/jd/qcHLyAgbDNz/7e10cnYjILtNqRC0am2VVm13JmUfh+H3w/Fc7P/baN0TB2b7buj2qIWXAjkXBmZtTcCbSoXY75FSpTrHaJAxD9uXcHZ1vX86lVGtSrDZxnTqHpjNdrXjqlnG97m7LJx1itmEy5XB22cMP2pvuHbdVftBmue4zm3OJ2YZ8UgGaiIiIiIiMl4EHaF//1qP8xof+gBdPnQG6NIdrNBEsIvIqqjbbujCEF78WBWenH+7sWCsGR34Ejt0DhWt7MrzhY8C2IbEanFnbn7AVGWeluk8rCFmq+eSSzo7CD4j2BsslHZZqPnuzLqV6d6qSum1cr7vbLCvaU83zAxZWGpxZ9jhYSG37fGeWPYyJqujm8smxCCFFREREREQuNNAA7UMf+QS/+wefJiRc31R7p4vVVUQhInIRvwFNVZttSeDDM1+IWjUuPtPZsU4KbnkH3PF+yMz0ZnzDyIpBYgLciaj6TES2rez5BO02nh8wnUl05ZyZRIxSvU47DLvW1q/bxvW6e+FAIcVLpTr780lOFmtMuLFttcNcq+A7UEiRcGwO7CCIExERERERGVUDm+n65J9+hQ999FPAK8FZJ3O6FwZtmgsWEbmIqs0649fhiU/CIx+B8pnOjk1Owu3vhaPvikKkcWHsaH+zZA5stfUS6YZqI8BrtQlDcJ3uVHIm4zZhCHU/oNrY3t7CvTau190LrmNzZCZLEIRUPJ/5Yg2goxCtVGsyX6wxmXKYSsc5MpPFdexeDVlERERERGRoDSRAO18s8Wv/+ffXQ7AwhH17p/jgT/4ot954PZ/406/w8T/5MhAFZZ/83V/DazRZqVR5bv4Ujzz+NF/++kN4jeZ6+Pa2N7+Be971Y1jab0VExpmqzTpTX4JHPwaP/Rfwljs7dmIO7vwA3PTjENvZfj0jxdiQSIObh9h4VHSI9Es7DNdv23aXfqZdO08YRucfRuN63b0yl0+ytLqf3HyxxguLNQpei30597LtMYMQTpU8GqHPZMrhYCHFbM5lLp/s4+hFRERERESGx0ACtD/45Odp+q31AO2mw9fwn37550mnol/OMqmNv6Ttm9mz/ufbbz7MO/7OD/KPK1V+98FP8+An/xshIZ/6/Fcpl6v865//Gewd7psgIjJS2u3V0KyiarOtWjkDj/x+VHXW8jo7ds8ROHYvXP9DUfvCcWEsiKfAnQSnOy3WRGQjy5j1n4+DLoU+a+cxhqFdaDau191Lt+yPKqKNMWTcJqdLdUq1JrmkQyYRIxm3sY0hCEPqzYCFpTove4Ypr8X1+7JMpePM5tz184iIiIiIiIyjgcz8fe7LX19v2Rh3YvzyP/2H6+HZVmUzaf7RT7+X19x+Mz//b36Tpt/iS1//Fr/6nx/gn/7De3o0chGRIeI3Vls0VlRttlXnvwsPfxhOfB7CDlt6zf0NOHYPHPy+nW/YOUqMBU4yqjiLqwpBpJfSCZukY2MMeH6bbWxd9Sr1ZoAxkHRs0onhbMM3rtfdS8YYjs7lmEzHObFQJpeMUaw2War5lOr1DT8yGANBq002FnJkb4o9EwmOzGRVeSYiIiIiImOv7wHaqbPnOF9cXm+9+MbXvYa52eltn+91r7mdX/if/y7/8t9/iDCET3zuy7zpB76Xu269sYujFhEZEqo261wYwplH4KH74MW/6PBgA4feGAVnM7f0YnTDy1gQS0AyD/H0oEcjMhayroNlDK5jU/Z8CumdJ0mVRgvXsbGMIesO536F43rd/TCXTzKVjnOyWMN16uzNurTDkLofEIash4yVao3Febi6kOK2a6e055mIiIiIiAgDCNCefvZFgPVf2H7gtXfu+Jw/+sbX8cnPfYVHnvguAPd97LMK0ERk13ATcazQh8r5qNosCABVm11R2Ibn/xyO3w9nH+3sWMuBG98Cd34QJq/pyfCGljFRcObmIZEZ9GhExko+6RCzDZMph7PLHn7QvuyeVVfiB22W6z6zOZeYbcgnhzNIGtfr7hfXsTk8k+XQdIZS3afs+VQbAe0wxDKGdMLGr9ucezrkuj0phWciIiIiIiKr+h6glVbKG/5+/TVXXfGYRrNJIn75lag/9qbX88gT3yUM4a8feYJypUo2oxXzIjLC2gG2XyXHCmblNGR1T9uSwIcTn4PjH4al5zs71knDrT8Jt70XMtuvjh5NBmJxcHOQyI5Xm0qRIWFZhrl8Es8PWFhpcGbZ42Ahte3znVn2MMZQSMeZyyexrOH8vh7X6+43y4q+JptV+J0v+rrti4iIiIiIXKTvAVq5Utvw98n8qzemTsQ3rhJtNPwrBmh33HJk/c9h2Obxp5/j++66dQcjFREZEN+DRgX8CmG1hFcuEbY73K9rHDWr8J1PwLc/CpWFzo5NTcHt74WjPxmFR2PFQCwGiVwUnmkGVWSgDhRSvFSqsz+f5GSxxoQbI7+NTcFKtSbFapMDhRQJx+bADgKpfhjX6xYREREREZHh1fcA7eJpuc2CsVRy44bV55dKTFyh8qIwmYvOv/oGL515edtjFBHpu3YQ7WvWqECr8creZtrj7MpqRXj0QXjsY9AoX/n1F8odgDvvjto1xhK9Gd/QMmDbrwRn1vbbpYlI97iOzZGZLEEQUvF85ovR4rNOwqRSrcl8scZkymEqHefITHbo2/KN63WLiIiIiIjI8Op7gJZKuRv+Xqt7uImNvxhn0hsDtDML57nu4Nxlz9tqbazOqFRrl3iliMgQuaDaTHubdWj5JXjk9+GJT0PQ6OzY6ZvgrnvgujeCNYaTq1YMEhOQzI3n9YsMubl8kqVqkzAMmS/WeGGxRsFrsS/nXnZvMD9oc2bZo1htMplyOFhIMZtzmcsnL3nMMBnX6xYREREREZHh1PcAbXpqcsPfy5UahYvaOB6cmwVeqSb7ztPP8brX3H7Z886fOrvh77GYJgRFZEhdqtpMtub8CXjoPnjmC51/7Q58Lxy7F656zXi2KjR21KIymQPbufLrRWRgbtkf/XxsjCHjNjldqlOqNcklHTKJGMm4jW0MQRhSbwZUGi2W6z7GGA4UUkyl48zm3PXzjIpxvW4REREREREZPn0P0K6+at+Gv8+fOsvVV81u+N8OX3tg/c9hCH/+lw/zDz7wjsue94t/8dfrrzcG8hPjtoeNiAw934taDPpVVZt1Kgzh1Lfg+P0w/43OjjUWHPohOHYP7L2pN+MbdsaGRBrcPMQ631NIRPrPGMPRuRyT6TgnFsrkkjGK1SZLNZ9SvU4YXvjaqAXibM6lkI6TWG2HOIoVWON63SIiIiIiIjJ8+h6gHdg3Q8pNUG9E7baemz/F67/3jg2vyaRT3Hjoap5+7kUAvvv8PF/62rd44+v+xqbnfOb5k/zRn3wJY1j/pfqGQ1f37iJERLZK1WY70w7g+a9GFWcvf6ezY+043PRWuOODkD9w5dfvRsaCeArcSXDGbY83kd1hLp9kKh3nZLGG69TZm3VphyF1P1hfOJZ0bCxjiNmGuXySA4XUyO/9Na7XLSIiIiIiIsOj7wGabVvcdvNhvnn8cYyB4489xT3vesurXvfDP/hannr2xfVQ7Jd+/UOslCu85Ye+H8d5Zdhf+tq3+JX/+36aTX+9G9eewiRHrjvYr0sSEXk17W22M0ETnvpjePgBKL3Y2bHxDNz6LrjtPZDe05vxDTtjgZOMKs7iqsQQGXWuY3N4Jsuh6Qyluk/Z86k2AtphiGUM6YRN1nXIJx0sa/e0px3X6xYREREREZHh0PcADeC1x47yzeOPE4bw8ONP0/R94s7GvVje/uY38MAffY7S8grGQN1r8G9/6z5+43ce5OD+GWJOjJOnFlipVNZXoa799/3vePMgLktExl27HVWbNStRgKZqs841K/D4x+GRj0DtfGfHpqfh9vfB0Z+IQrRxZCxwXHBzEE8PejQi0mWWZSik4xTS49WKdVyvW0RERERERAbLGsSb/tDrv2e9WqzRbK7vX3ahTDrFz/2D9623ZFwLyGp1j6eefZHvPP0sy+VXwrM1R284xLt//E19uAoRkVWtBlQXYXkequegWVN41qnqefj6b8J9b4Gv/8fOwrP81fDGfw53fxqO3T2e4ZkxUXCW2QsT+xWeiYiIiIiIiIiI7NBAKtBm9hT4e+/5cc4tlgCo1xubvu6H3/BaiqUV/sOHPgpsDMou/nsYws2Hr+XX/sX/QszW3gci0mNhuLq3WVnVZjtROgkPfxie+mzUtrETM0fh2D1w3Q9GlVdjyUAsHlWcJbKvflCKiIiIiIiIiIjItgwkQAP4Hz7wE1t63Xve9sMcveEQ//F3H+TRJ7+7XpF2oYlMive+/c184J0/QiKu1i4i0kOtZrS3WXMF2gGb3pTkyl5+Eo7fB89+qfPw8erXRcHZ/mNjHBgZiMUgkYvCs7H9OoiIiIiIiIiIiPTGwAK0Thy98RAf+tX/g/PFEo985wTniyXqXoPcRIZDB+c4euP12Pa4Vh+ISM+FIfjVqNqs6UEYDHpEoykM4aW/gofui/7bCWPD4TdFwdmeIz0Z3mgwYNuvBGeWnn0iIiIiIiIiIiK9MBIB2po9hTx/+/XfM+hhiMi4CPzVarMyBC21adyudgDPfhGO3w/nnurs2FgCbno73PmBaG+vcWbFIDEByRxYalUsIiIiIiIiIiLSSyMVoImI9FwYgl9brTarr4ZmatO4La0GPPUZePgBWH6ps2MTE3Dbu+G290BysjfjGxXGjvY3S+bAdgY9GhERERERERERkbGgAE1EBKIKs2YlCs4CX9VmO9Eow2N/CN/+A6gXOzs2MwN3fABufjvEU70Z36gwNiTS4OYhpv09RURERERERERE+kkBmoiMt2ZtNTirqtpspyrn4Nsfgcc/Hu0Z14nCddH+ZoffrCorY0XhoTsJTmLQoxERERERERERERlLCtBEZPy0g9UWjRVoNVVttlNLL8DDH4an/hjarc6O3Xc7HLsXrvn+KDgaZ8YCJxlVnMWTgx6NiIiIiIiIiIjIWFOAJiLjo1mPQrNmNQrRVG22M2cfg+P3w3NfoeOv5TWvjyrO9t/Zi5GNFmOB44Kbg3h60KMRERERERERERERuhyg/fEX/+JV/9tbfuj7t/S6btvsfUVkDLWD1RaNFWg1VG22U2EI89+Ah+6D0w91dqxlw+G/A8fuhqnrezK8kWIMxBJRxVkiM+jRiIiIiIiIiIiIyAW6GqD90q//DsZs/N82C7I2e123KUATGXO+F4VmfgUCVZvtWLsF3/1C1Krx/InOjo25cMs74I73Q3Zfb8Y3SowBOx5VnCWy9PyBKCIiIiIiIiIiIh3rSQvHcHWe+kpzgmGP5rM1Fykyptrt1WqzsqrNusWvw5OfgYcfgPLpzo51c3Dbe+DWd0My35vxjRQDsRgkctHXRg8rERERERERERGRodWTAM2YrYVjvZg77FUoJyJDzG9EoZmqzbrHW4bHPgbffhC8UmfHZvfBHR+Am98GTrI34xspBmz7leDMsgY9IBEREREREREREbmCrgZos9NTWwrFtvo6EZFLWqs2a1aido2qNuuO8ll45KPwxMej6rNOTF0Px+6B698EttOb8Y0aOwbxCUjmoj3gREREREREREREZCR0NUD79H3/vquvExF5lQurzdqByk67pfgcHL8fTnwu+rp2Yv8xuOteOPg31ZZwjbGj/c2SOYWJIiIiIiIiIiIiI6gnLRxFRLpK1Wa9c+bbUXD2/Fc7P/a6H4Rj98LsrV0e1AgzNiTS4OYhFh/0aERERERERERERGSbFKCJyPDyG6vBWVnVZt0UtuGFv4iCszOPdHasFYMb3gLHPgiT1/ZmfKPIWBBPgTsJTmLQoxEREREREREREZEdUoAmIsNF1Wa9E/jw3c/D8Q9D8dnOjnVScMtPwB3vh8ze3oxvFBkLnGRUcRZPDno0IiIiIiIiIiIi0iUK0ERkOGhvs97x6/DEJ+CRj0D5bGfHJgtw+3vh6E+CO9Gb8Y0iY4HjrgZnqUGPRkRERERERERERLpMAZqIDI6qzXqrvgSP/hd49GPQWO7s2Ik5uPODcNNbIeb2ZnyjyFjR3mbJPMQzgx6NiIiIiIiIiIiI9IgCNBHpP9+DRiWqNgsCQNVmXbVyBh55AJ74JLQanR07fQMcuxcOvTHa70wixoB9QXBmzKBHJCIiIiIiIiIiIj2k2VER6Y92AM0qNMtRu0ZVm3Xf+e/C8fvhu/8NwqCzY696TRScHfhehUMbGIjFolaNiQl9bURERERERERERMZEVwO0D330k9083Y78/fe9fdBDEBFQtVmvhSGcfhiO3wcvfq3Dg01UaXbsHpi5pRejG2EGbPuV4MyyBj0gERERERERERER6aPuBmgf+eTQLM5XgCYyQO0g2tesUYlaCKrarPvCNjz/VXjoflh4rLNjLQdu/LFoj7PJq3szvlFmx6LQzM2BZQ96NCIiIiIiIiIiIjIAPWnhGA64wGRYQjyRsaNqs94LfHj6c/Dw/bD0QmfHxtNw9Cfh9vdCeronwxtpxgZ3NTiz1eFYRERERERERERknA3FDOGVAq8w3NprRGQAVG3WH34NHv4UPPJRqL7c2bGpKbj9fXD0nZDI9mZ8o8zYkMhEwVksPujRiIiIiIiIiIiIyBDoaoB259EbOq7+qtbqPP3s/Ppxa0GYMTA7PUU2kybpJqh7DcqVKmfPLW54zZobD11NKuXu/CJEZGua9Sg486uqNushU1/iaOnz5D/+r6OvdydyB+DOu+HGt0As0ZsBjjJjQSId7XOmr4+IiIiIiIiIiIhcoKsB2m//yj/r6PWPPfUMv/Bv/xPGRMGZm4jzwz/wvbz5B7+PW264jlTy1YFYre7xnaef40+/8g3+21e/SaPpYwwslyv8k5+5m6M3HurW5YjIxVRt1j/LL8HDD5B/8tNMBs3Ojt17Mxy7B677W9rDazPGgngS3ElwtPBCREREREREREREXm1gLRwfevRJ/tH/+es0fZ8whNceO8ov/OzfZXbv1GWPSyVdXnPHzbzmjpv56fe+jV/+rfv4y+OPc/bcIj/zC7/Cf/xXP8edR2/o01WIjIm1arNmNQrRVG3WO+eehuP3wzNfgLBNR0W9B14Ld90Dc6/RZpCbMVYUmLl5iKcGPRoREREREREREREZYgMJ0IqlFX7+l39rvXrsTT/wPfyrf/w/YttWR+fZN7OH3/iX/xv//Ff/M3/23/8Kr9Hkn/zr3+Rjv/3LTOYmejR6kTHRDqBRjkIzVZv1VhjCqb+Gh+6Hk/8/e3ceH1V56H/8e2afbJOEQABZZd83VwQXQFwAa1WsVATb3uuttZvtr9ba21u7WbW9tlprr1Yr4F53UVxAlB0Vwr6HNUAgQPZ9m98fhy0wkzDJzJyZ5PN+vXi9mnnmOfMFzamcb57nWRnaXMMm9b5aGjlDat8/MvninWEzt2j0+iRXktVpAAAAAAAAAMQBSwq0f770jopLyk6ec/bfP/pOyOXZCXa7Tb/68Xe0cetOHTpyTMWlpfrnS+/ovu/NCHNqoI1gtVn01NdJuz43V5zlbQptrt0tDZgijZhunnWGsxmGZHdJ3lTJnWx1GgAAAAAAAABxJOoFWk1NreYtXHZyd7FbJo2X1+Nu0TW9HrdumTROT856XX6/NO/TZfrJXd+Uw2HZDpVAfDm52qxUqq1mtVmk1VVLW9+Xsl6QivaFNtedLA25VRp6m5SQHpl8cc+QHE7J45PcKWxnCQAAAAAAACBkUW+YNmzNVkVllSTzmealo4aE5bqjLxiqJ2e9LkmqqKrS+i3ZGjmE7cyARlWXH19tVs5qs2ioKpE2vSWtfVkqPxrS1PqEDNlGTJcG3SS5EiMUMN4Zkt1xqjizNW9lMwAAAAAAAABEvUDbk5Pb4OvM9uFZQXHiOicWGuzJyaVAAwKpqz1emrHaLGrKjkjrXpE2vmFujRmCupRuWu24SL2vvUvp6e0iFDDeGZLdLrl9kidFstmtDgQAAAAAAAAgzkW9QCsubfjwuKa2LizXPfM6Z34O0Oax2iz6CvdJWXPM7Rrra0KbmzlEGjVTRekjtHvxV+ptd0YmY7yzOczVZp4Uc/UZAAAAAAAAAIRB1J82ulwNHwIfOJSn9NSUFl/3wKG8Rj8HaJNYbWaNw5ulrFnSzoUKuajsfpk08k6p8whzSW1RcQQCtgKG3TwPzuuTKBcBAAAAAAAAhFnUC7QO7dIkndpq8fMVWRrSv3eLr/v58tWSJL/fvHb79NQWXxOIWydWm1WVHS/NWG0WcX6/lPOFlDVb2v9laHMNu9RnojRyppTRJzL5WgvDLrkTJU+q5HBZnQYAAAAAAABAKxX1Aq3v+d1O/m+/X3rz/U81dfJ4dWzf/LN9DuUd05sfLJRhmNeUpH69urc0KhBfTqw2qyqR6mpYbRYt9bXmSrOsWdKRbaHNdbilgTdKw6dLKZ0jEq/VMGxmceZOlZxuq9MAAAAAAAAAaOWiXqB1O6+jevfsqp17cmQYUnlllX72u8f1t9/9TKm+5JCvV1hUop/+9q8qr6ySYZirz3r16Kpu53WMQHogBlWXS9UlUlU5q82iqbZS2jJXWvOCVHwgtLlunzT0VmnoNyRvWmTytRaGTXJ5JU+a5PRYnQYAAAAAAABAGxH1Ak2Sbv/6NfrNY8+eLLy27dynmT9+UD/5r9t1xSUjz/k6i1Zk6bFnXtKhI8dOrj4zDGn616+NYHoEc+DQEWXvztGxgiIVlZQqJSlR7dJ86t2zi7p0yrQ6XuvCajPrVBZLG9+Q1r0iVeSHNjcpUxoxXRpwo+RKiEy+1sKwmYWZJ5U/KwAAAAAAAABRZ0mBNmn8GL2/YJlWr99y8iy03Lxjuu/3T6jbeR018fKLNbh/b/Xs1lkpSYnyetyqqKxScWmZdu87qI1bs/Xxoi+Uc/DQyS0bT5RxFwwdqOvHX2bFb6tNqqmp1Wtz52vewuXasWtf0Pf16dlV140brdtumCin05J/7VqH6rLjxRmrzaKuNE9a+5K06S2ppjy0uem9pJEzpD7XSHZnZPK1FobN3NrS65NcSVanAQAAAAAAANBGWdZkPPzAPbr7F48oe3fOyRLN75f27j+kZ195t8n5pxdnJ77u07OrHvrF9yKUGGdavyVbv/vrs9qTk9vke3fsztGO517Tux8v1q9+/B0NG9gnCglbCVabWSt/t7RmjrRtnnneWSg6DZdGzpR6jDGLIQRnGJLdJXlTzeLsxM0dAAAAAAAAACxg2RNdX3KS/vHHn2vU0AFnrSLz+5v+deK9kvn1BcMG6Kk//ly+ZFYsRMPqDVt1zwOPnFN5drq9+3P1/V8+qtUbtkYoWStSXS6VHpYKc6SyY1JtFeVZNB3aIM37qfTyLdKW90Irz3pcLt38nPmr5+WUZ40yJIdLSsyQfF0kdzLlGQAAAAAAAADLWbqX3okS7c0PFuqZl95WQVGJpHN7dnqidEvzJeu/pt+km66/KoJJcbqde/frJw/+RZVV1c2aX1lVrZ88+Bc9/5f/0fndzgtzujjHajNr+f3S3mVS1mzpYFZoc212qc+15oqzdr0ik69VMSS73TzjzJ0i2SgZAQAAAAAAAMSOmDiM6uZJ4/S1ay7XgiVf6eNFK7Vx604VlZQGfX9KcqKG9O+ta6+8ROPHXCiHIyZ+G22C3+/Xw0/OVnlFZcBxX0qSrr3yUnXu2F6H8o7qw4UrVFhcclBCD2MAACAASURBVNb7yisq9fDfZunpRx+QwWoTc7VZdalUVcbZZlaor5V2fCJlzZGO7QhtrtMrDfy6NPybUnKnyORrbewOszTz+MziEQAAAAAAAABiTMw0Tw6HQ9dedamuvepSSdL+3MPKO1qgktJylVdWKsHjUXJSgjpkpKlLp0yL07ZdH32+Qms3bQ841qNrJ/3jj/crIz315Gszp07Wd+//Y8CtHtds2q6PP1958p95m3NitVl1qVRbzWozK9RUmNszrnlBKgltO1J5UqWh35CG3Gqe24Wm2RzmFo0en1miAQAAAAAAAECMitknmF06ZVKUxaA3P1gYdOyBH3yrQXkmSe3SfHrgB9/SXfc9FPh68xa2vQLtxGqz6nKpvk6sNrNARaG04d/S+tekysLQ5iZ3lkZMlwbcYK4+Q9MMu+ROMoszh8vqNAAAAAAAAADQpJgt0BB79uce1rrNgbe369Y5UyMG9ws4NmJwP3XrnKl9Bw+fNbZ203btz81Tl04dwpo15tTXmeeasdrMWiW50tqXpE1vS7WBtyENql1vaeSdUp+rzZVUaJphk9yJ5mo9h9vqNAAAAAAAAABwzngKjHO25It1QcdGDRvQ6NxRwwYELNDM667VtBsntihbzKquOL7arIzVZlY6tlPKmi3t+Oj4P4cQdB4ljZopdRstcV7fuTFskssredIkp8fqNAAAAAAAAAAQMgo0nLNtO/cEHevdo2ujc3v36BL8urv2NjdSbGK1WezIXSutni3tWRziREM6/0pp5Eyp45AIBGulDJtZmHlSJVeC1WkAAAAAAAAAoNlirkCrr6/X1uy92p97WIXFpSotK1ddfb2GD+yrC4cPtDpem7ZtZ/CiK7N9eqNzMzPaBR3bvmtfszPFFFabxQZ/vbRnqZQ1S8oNvmoyIJtD6jdJGnmHlNYzIvFaJcNmnm3mTZVcSVanAQAAAAAAAIAWi5kC7au1m/XKux8ra/1WVVRVnTU+45ZJAQu0gqJivfbegpNf9z2/m8ZddkFEs7ZV+3Pzgo6lp6Y0Ojc9Lfj4gUauG/Pq68zSrKpUqq1itZmV6mqkHR9LWXOk/J2hzXUmSINvloZ9U0pq5efxhZNhSPbTijO2uAQAAAAAAADQSlheoOUePqpf/en/tGFrtiTJH2DRTmPPZNN8Kfp8+WrtzjkgSWqX5tNVo0fJ4EFuWNXW1amyqjrouNfT+DlHXrc76Fh5RaXq6uplt9uanS/qairN0qymVKpjtZmlqsulze9Ia1+USgOfsxeUN10aNk0afIvkabwExukMyeGQ3D7J46M4AwAAAAAAANDqWFqgfbl2k37x0N9VWl4uv998BnviOeyJrwMVame69YYJevjJ2ZKkYwVF+mLNRl0yknOLwqmsvKLRcZez8X+VnE5nk9dPSU485zyFRSU6ml94zu9vKcOQDL9fRk25jJoS+Wuq5K+vi9rn42xGZZE8296Se+s7slUXhzS3LqmzKgd9Q1XnXyM53FKVpKrQrhEtRcUlqqisUlFxidVRJMOQYXdJnhT57cmqr5BUUWR1KgBnyC8oUnlFpfIL+P4EcG64bwAIBfcMAKHivgEgVM25b2Skp4Y9h2UFWvbuHN33+7+pvKLyZHF2oixr3y5N7dNTtXnH7nO61oQxF+nRp16Q//j2eUu/XEeBFmaNrT6TJLvd3ui4w9H4eEVVVUgF2sJlq7R+S/Y5v785bDabXE6HPA7J5a+UUV2m2uoq1dbWRvRz0biE2nz1L16inmWr5PDXhDS3wNlZW1Ku1P6EwfLn2qTctRFKGT4VlVXauXe/JMnrCb6SM5JsNpucbo/87hRVyqOK6hrV1lIgA7GqvKJSW47/N1SCt/EV4gAgcd8AEBruGQBCxX0DQKiac9+4a/rXw57DkgKtrq5e9//x7yfLM0lyOhy6ZfJ4TZ08Qed1bC9JumjSnee0M1hKcqJGDOqr1Ru2SpK+Wrc5UtHbLI/b1eh4Uw/Ta5oonRrb4jGQcZddoN49u4Y051wZOr7irKZMRnWZ/DUVrDaLAfaCnfJselWunIUyQjxrrqbjSFUMmiZ/p1HqbxjqH6GMkXBi5dkVl46QLyU56p9v2B2SO1l+V4r8hp3NSoE4cOKns64fN1rpaT6L0wCIB9w3AISCewaAUHHfABCqWLlvWFKgvfvJIu07cOjkqrPUlCQ99ut7Nbh/r2Zfc+SQficLtD05B1VWXqHEBG+4Ird5Tf1ZNlWQ1dQ0vlIo1H9Wqb7kiCzJVE2VVFVinm1mr5M8Nslz7ivjEGZ+v3QwS8qaLe1dFuJkQ+o9XhoxU87MgWp8E9HY5vW45UtJVroviue0GXbJnSh5UiVH4wU6gNiT4PUoPc0Xmf+vBNAqcd8AEAruGQBCxX0DQKhi4b5hSYH2xgcLT5ZnNsPQHx/4fovKM0nq07Nbg6/35BzUoH4tuyZOcdjt8rhdQbdybOqMtPLyyqBjXo9bdrutRflapL5eqi41f9VUSiGubkIE+Oul3Yuk1bOlwxtCm2t3Sf0nSyPukFK7Nf1+NGTYJFeC5EmTnNZsGQkAAAAAAAAAVot6gXY0v1DZu3NOnnt25ehRGjWk5Ruqde/SSZJObvmYczCPAi3MunTqoOw9+wOOFRQWNzr3WCPjXTpntihXs9VUHS/OSqT6ulOH8ME6dTXStnnSmjlSwZ7Q5roSpcFTpWHTpMSMiMRr1Qyb5PSYxZmL1bsAAAAAAAAA2raoF2ibtu2SZHYVhiFNvOKSsFw3OSmhwdfFpWVhuS5O6dere9AC7fDR/EbnHj4SfLzv+VFcJVRfL9WUHd+mkdVmMaO6TNr0lrT2JansSGhzEzKk4d+UBt0kuaN/RljcM2ySwy15U80SEgAAAAAAAAAQ/QLtWGFRg68H9ukZluueeYZWeUXwLQPRPP169dAHnwY+hyp7T06jcxsb73d+9xblOie1VVIVq81iTvkxad2r0sbXzVIzFKndzW0a+08yt21EaAzD/HPzplI8AgAAAAAAAMAZol6gFRWXNvjal5IUlutWnXE2l8NhD8t1ccrYi4fpsWdeCji2at2WRueuWre5kesOb1GuoPx+c4vGqlKppoLVZrGkKEda84K0Za5UF/hcvaAyB0kj75R6XiHZ+D4PnSE5nJLHJ7lTTu17CwAAAAAAAAA4KeoFWmKCp8HXFZVV8nrcLb5uYXHD1Su+5PAUczilS6dMDR3QW+u3ZJ81tj83T6s3bA14nt2Xazfp4OGjAa85fFBfdenUIbxBa6ukqjKpupjVZrHmyFYpa7aUvSD0QrPbpdLImdJ5F1D6NIsh2e2SJ9Uszmw2qwMBAAAAAAAAQMyKeoGWmtJwq7AjxwqUnprS4utuzd4r6dTZamd+DsLj5knjAhZokvTwk7P0jz/er4z01JOvHc0v1CN/nxP8etePC08wv988R+vk2WZ14bkuWs7vl/Z/JWXNknK+CG2uYZN6X20WZ+37RSRem2B3mKWZx8eqPQAAAAAAAAA4B1Ev0DLbt5N0agHJus071K9Xy8/A+mLNxgZf9+3VrcXXxNmuu2q03v7wc63dtP2ssT05ubrte7/U9eNGq2OHDB3KO6p5C5eftW3nCSMG9dU1V17SskC11ce3aCyR6mpZbRZL6uukXZ+ZK87ygm/hGZDdLQ28QRo+XfJ1iUy+tsCwS57jxZk96rd7AAAAAAAAAIhbUX+iOqjf+UrwuFVRVSW/X/rg06W6dcqEFl2zoKhY85d8KcMw+5POme2VmZEepsQ4nWEYuv/7M/Wte3+risqqs8aLikv1yjufNHmdBK9HP//+TBnN3YqvulwqyZWqWW0Wc2qrpK0fmGecFe0Lba47WRpyqzT0NimB7+FmM+ySO8kszhwuq9MAAAAAAAAAQNyJ+iE4DrtdFwwbeHKh0NbsPVq49KsWXfPRv89RdXXNye0bL7twWBiSIphe3bvoL7/5iTzu5j2Yd7tdeuzBe9WrewtWFlUUmOecUZ7FjqoSafXz0pwp0ud/CK08S+wgXXavNPMD6ZLvUZ41l2GTPMmSr7OU1J7yDAAAAAAAAACayZI9vabdOFGLv1hzcsXYQ397Xud16tCsrRz/Put1fbps1clr2Ww2ffPr10QgNU43akh/PfmH+/T7x5/Tnpzcc57XvUsn/epH39awQX1bFsBf37L5CJ+yI9K6V6SNb5jn0IUirac0cobU9zrJ7oxMvrbAsElOr+RNk5weq9MAAAAAAAAAQNyzpEAbNXSALhw2UF+t2yzDkIpLy/Xd+x/WPXfeopuuu0o2W9ML43bvO6jHn3tVK1avP1meGYZ07ZWXqnNm+yj8LjBsYB+9/OTv9drc+fpgwVJl79kf9L29unfRpPGX6bavTZTTyVlMrULBXmnNHHO7xvqa0OZ2HCqNnCn1vNwsf9A8hs0szDw+yZVodRoAAAAAAAAAaDUsazJ+9ePvaOa9v1FhUbEMQyorr9Cf/vGCnn35XV05epT69uzW4P1H8gu1aEWWdu07oOWr1mvD1p3y++tPFmeGIXXp2EE//e50i35HbZPT6dD0m67T9Juu0/7cPO3YvU/5BcUqLi1TclKC2qX51KdnV3XplGl1VITL4U1S1mxp50JJ/tDmdr9MGvUtqdNw85sWzWMYksMteVLNs84AAAAAAAAAAGFlWYHWsUM7/flXP9Q9Dzyqqurqk6vI8guL9faHn51834mz0j5cuEwfLlx21usn5qUkJeiR//6hkhK80fxt4DRdOnVQl04drI6BSPD7pX0rzOLswKrQ5hp2qe810ogZUkafyORrMwzzXDOPT3InU0ICAAAAAAAAQIRYupfekP699a/H/kf3P/Sk9h04dPJZsD/AopbTXzux4uzE6927dNRjv75XXTuzygkIq/paKftTszg7ui20uQ63NPBGafh0KaVzZPK1EXa7QzaHW0psZ5ZnFGcAAAAAAAAAEFGWH0bVu0cXzXn8Qc1+/QO9+cGnKi4tl9T48+ETZZrX49atUyZo5q2TWXkGhFNtpbTlPWnNi1LxgdDmun3S0G9IQ2+VvGmRyddmGDIcLtlTMlSf3FnyplodCAAAAAAAAADaBMsLNElK8Hp094ybNXPqJM1f/IW+WrdFazZu05FjBWe9NzHBqxGD++riEYN1zRWXKNWXbEFioJWqLJY2vi6te0WqOPv7r1FJmdKIO8xVZ04K7RazOSR3svy2NBVU7VK9WHUGAAAAAAAAANESEwXaCQlej752zRX62jVXSJJqa2tVWFyqktJyedwupfqS5fW4LU4JtEKlh6W1L0mb3pZqykObm95LGjlT6jNRsjsjk68tMeySO8lcbWZ3qr6qULW1dVanAgAAAAAAAIA2JaYKtDM5HA5lpKcqI51ty4CIyN8trZkjbZtnnncWik7DpVF3St3HcCZXOBg2yZ0oeVLN8+MAAAAAAAAAAJaJ6QINQITkrpeyZkm7F4U+t+cV5oqzTsPCHqtNMmzmlpfeNMnpsToNAAAAAAAAAEAUaEDb4fdLe5eZxdnBNaHNtdmlvteZxVn6+RGJ1+YYNnOlmTdVciVanQYAAAAAAAAAcBoKNKC1q6uRsudLWbOlY9mhzXV6pYE3ScO/KSV3jEy+tsYwzOLMk2qedQYAAAAAAAAAiDkUaEBrVVMhbX5XWvuiVJIb2lxvmjT0NmnIVMnji0y+NseQHM7jxVky58YBAAAAAAAAQAyjQANam4pCacO/pfWvSpVFoc1N7iyNuEMaMMVcfYYwMCS7/XhxliLZbFYHAgAAAAAAAAA0IewF2t33PxzuS4bOMPSPP/7c6hRAdBXnmqvNNr8j1VaGNjejr3m+We8Jko1ePWxsDsmTYq7is9mtTgMAAAAAAAAAOEdhf1K+esNWS3cm8/vZGQ1tzLFsKWuOtP0jyV8X2tzzLjCLs26X8o0TTobd3KbR65PsTqvTAAAAAAAAAABCFLGlJn7/qf/Nc3kgAg6ukVbPkvYuDXGiIZ1/lTRqppQ5OBLJ2i7DJrkTze0aHW6r0wAAAAAAAAAAmiliBdqJ0szvb1imAWgBf720Z4m0erZ0aF1oc21Oqf8k84yztB4RiddmGTbJ5ZU8aZLTY3UaAAAAAAAAAEALRXQFmmFIXTtnqk/PrpH6GKBtqKuRtn8orXlByt8V2lxnojTkFmnoNCmpfWTytVWGzVxp5k2VXIlWpwEAAAAAAAAAhElEV6D5/dL+3MPyetyacvVYXXvVpfIlJ0XqI4HWp7pc2vy2tPYlqfRwaHMT2knDpkmDbzHP40L4GIZkd0neNMnNPQ0AAAAAAAAAWpuIFGgnVp+d2MZxx+59euyZl/TEc69p7MXDNeXqsbp01BDZbLZIfDwQ/yoKpHWvSBtel6qKQ5vr6yKNmGlu18g5XGFmSA6HecaZO4UDHgEAAAAAAACglQp7gfbMow/ovU8Wa+HSr1ReWSXp1Gq0mtpafbZ8lT5bvkrpqT5dP/4yTR4/Rj27dQ53DCA+FR+Q1rwobX5XqqsKbW77AdKomdL54ySbPTL52ixDstslt0/y+CTKfwAAAAAAAABo1cJeoA0f1FfDB/XVfXffoflLvtT7C5Zq7aZtkk4t1vD7pWMFRXrxzXl68c15GtjnfE2ZOFYTL79YSYkJ4Y4ExL6j26XVs6TsBZK/LrS5XS+WRt4pdbmQFVGRYHOYW2B6fJI9YrveAgAAAAAAAABiSMSeBnuOn3s25eqx2p+bp7mfLNa8hct1+Gi+pIZl2uYdu7R5xy499szLuvLSUZoyYYwuHjk4UtGA2OD3SwdWS1mzpH0rQptr2KRe46WRM6UOAyISr80z7Ob5Zh6f5HBZnQYAAAAAAAAAEEVRWU7RpVMH3T3zFn13xs36cs0mvTd/sRatXKPq6poGRVp1dY3mL16p+YtXqn27NE0aP0aTJ4xR186Z0YgJRIe/Xtr1uVmcHd4U2ly7S+o/RRpxh5TaNRLpYNgkV4LkSZOcnCEHAAAAAAAAAG1RVPcjMwxDF48crItHDlZpWbk++nyF3p+/VJt37D4+br7P75fyjhZo1r/nata/52rYgD6afPVYTRh7kRK8nmhGBsKnrlraNk/KmiMV7g1tritJGjJVGnqblJgRmXxtnWGTnB7Jk2oWaAAAAAAAAACANsuyA32SEhN0y6TxumXSeO3ad0DvfrxYH32+QgWFxZIalmnrtuzQui079L9Pv6Rxl12gyRPGaNRQtq1DnKgulTa+Ja17WSo7EtrchAxp+O3S4JvMEg3hZxiSw20WZ27+jAEAAAAAAAAAFhZopzu/23m69z+n6Yff/oaWfrVW789fomVfrVdtXV2DIq2iskrzFi7TvIXL1DmzvX5+zwxdMnKIteGBYMqOSutekTa+YZZooUjtLo2cIfW73ty2ERFgSA7n8eIs+VRrDwAAAAAAAABo82KiQDvBbrfpiktG6opLRqqgqFjzPl2u9xcs0c69BySZz7f9fvO9Bw8f0fad+yjQEHsKc6Q1L0hb55rbNoYic5A08k7p/CvNLQURAYZktx8vzlIkG3/OAAAAAAAAAICGYqpAO12aL0W333Stbr/pWm3evltvf/SZ3vtkcYMSDYgpeVukrNnSzk8lf31oc7uNlkbOlM4bxUqoSLI5zNLM65NsdqvTAAAAAAAAAABiVMwWaCfs3Ltf85d8oaVfrpPfT7eAGOP3S/u/krJmSTlfhDbXsEt9rjaLs4y+EYmH4wy7eb6ZN1WyO61OAwAAAAAAAACIcTFZoJWUlumjz1fq/QVLtDV7jyRRniG21NdJuxZKq2dLR7aENtfhlgbcKI24XUo5LzL5YDJskitB8qRJTrfVaQAAAAAAAAAAcSJmCjS/368Vqzdo7vwlWvLlWtXU1JzcqtEwGp5/1rF9O02acJmuGzfausBom2qrpK3vm2ecFeWENtedIg29VRp6m+RNi0w+mAyb5PSYxZnLa3UaAAAAAAAAAECcsbxA27M/V+/PX6IPFy7X0YJCSWpQnPn95i+3y6mrRl+gKVeP1YXDB1qYGG1SVYm08Q1p3StS+bHQ5iZlSsNvlwZ+3VwNhcgxDHOFnzdVciVZnQYAAAAAAAAAEKcsKdBKyyv0yaKVen/BUm3atlOSAq428/ulIf17acrVY3X15RcrMYGVJIiy0iPSupeljW9KNWWhzU0/XxoxQ+p7LeduRZwhOZySJ1VyJ7PfKwAAAAAAAACgRaJaoH2RtVFzFyzVohWrVV1TI+nU2Wanl2bt01N1/fjLNHnCWHXv0jGaEQFTwV5pzRxp6wdSfU1oczsOk0bNlHqMNbcSRAQZkt1+vDhLkWz8eQMAAAAAAAAAWi7iBVrOwcN6f/4SzVu4XHnH8iUFXm3mcjo09uIRmnL1WF0ycrBsPAiHFQ5vlFbPlnZ9Jskf2tweY6WRM6XOIyISDWewOczSzOuTbHar0wAAAAAAAAAAWpGIFGjlFZVasORLzZ2/ROu37JAUfIvG/r17aMrVY3XtlZcoOSkxEnGAxvn90r4VUtYs6cDq0Oba7FKfa6WRM6R2vSMSD2cw7JI7yTznjK0xAQAAAAAAAAAREPYC7cH/fUYLl61SVXW1pIbF2YnSLC01RddddammXD1Wvbp3CXcE4NzU10rZC6Ss2dLR7aHNdXikQV+Xht8uJXeKTD40ZNgkV4LkTZMcbqvTAAAAAAAAAABasbAXaPMWLg/4ut1m12UXDdPkCWM05sLhstvZohEWqamQtsyV1r4oFR8Iba7HJw29TRoy1SxyEHmGTXJ6JE+a5PJanQYAAAAAAAAA0AZEZAtHwzj1v7t07KBJE8bouqtGK82XLEmqqalRTU0kPvkUj4cVKjhDZZG04XVp3StSZWFoc5M7ScOnSwO/JjkpcaLCMMyVZt5UyZVkdRoAAAAAAAAAQBsSkQJNOrV14/5DeXr6xbf09ItvReqjzmLI0Mr3n4/a5yHGlR6W1rwkbX7LXH0Wina9pZEzpd5Xc95W1BiSwyl5UiV3csNGHgAAAAAAAACAKIhYgXbCiSItqgwrPhQxJ3+Xeb7Z9g+l+rrQ5nYeaRZn3S+jwIkaQ7LbjxdnKZKNbV4BAAAAAAAAANaIWIFmVedgSWGH2JK7zizOdi8KfW7PK6SRd0qdhoY9Fhphc5ilmdcn2exWpwEAAAAAAAAAtHERKdAosRB1fr+0d6m0epaUuza0uTaH1O96acQMKb1nROIhCMNubtPo9bFFJgAAAAAAAAAgZoS9QPufe/8j3JcEgqurkXZ8Yq44y98Z2lxngjToJmn4N6WkzMjkQ2CGTXInmts1OtxWpwEAAAAAAAAAoIGwF2iTJ4wJ9yWBs9VWSetekda+KJUcCm2uN00aNk0aPFXypEQmHwIzbJLTaxZnLq/VaQAAAAAAAAAACChiZ6ABETX3h5LzQGhzUs6TRtwhDZgiOTyRyYXADJu50szrk1xJVqcBAAAAAAAAAKBRFGiIT9Wl0rkemZXRTxo5U+o93jzvDFFkSA6X5E01izPDsDoQAAAAAAAAAABNok1A69XlQrM463oJxU3UGZLdbm7V6PHx5w8AAAAAAAAAiCsUaGhlDKnXOLM4yxxkdZi2ye6Q3ClmcWazW50GAAAAAAAAAICQUaChdbA5pf6TzTPO0rpbnaZtMuySO9k858x+rvtrAgAAAAAAAAAQeyjQEN+cidKQW6Rh06TE9lanaZsMm+RONLdrdLitTgMAAAAAAAAAQItRoCE+eXzSpXdIg28xVz0h+gyb5PRK3jTJ6bE6DQAAAAAAAAAAYUOBhvg0+a9SL7ZqtIRhM1eaeVMlV6LVaQAAAAAAAAAACDsKNMQnu8vqBG2QITlcx4uzJMkwrA4EAAAAAAAAAEBEUKABaIIh2R3mtpkeH8UZAAAAAAAAAKDVo0ADEJzdIblTzOLMZrc6DQAAAAAAAAAAUUGBBuBshl1yJ5vbNdq5TQAAAAAAAAAA2haejAM4xbBJ7kTJkyo53FanAQAAAAAAAADAEhRoAMzizOmVvGmS02N1GgAAAAAAAAAALEWBBrRlhs1caeZNlVyJVqcBAAAAAAAAACAmUKABbZFhSHaXWZy5k61OAwAAAAAAAABATKFAA9oUQ3I4JLdP8vjMIg0AAAAAAAAAADRAgQa0FfYTxVmKZLNbnQYAAAAAAAAAgJhFgQa0dobdLM08PrNEAwAAAAAAAAAAjeJpOtBaGXbJnWQWZw6X1WkAAAAAAAAAAIgbFGhAa2PYJFeC5EmTnG6r0wAAAAAAAAAAEHco0IDWwrBJTq/kSZVcXqvTAAAAAAAAAAAQtyjQgHhn2CSHW/KmSq5Eq9MAAAAAAAAAABD3KNCAeGUYkt0ledPMs84AAAAAAAAAAEBYUKABcceQHE7J45PcKWaRBgAAAAAAAAAAwoYCDYgbhmS3m2ecuVMkm83qQAAAAAAAAAAAtEoUaEA8sDvM0szjk2x2q9MAAAAAAAAAANCqUaABscywS57jxZmdb1cAAAAAAAAAAKKBJ/JALDLskjvJLM4cLqvTAAAAAAAAAADQplCgAbHEsEmuBMmTJjndVqcBAAAAAAAAAKBNokADYoFhk5xeyZMqubxWpwEAAAAAAAAAoE2jQAOsZNgkp8fcqtGVaHUaAAAAAAAAAAAgCjTAGoYhOdzmijN3ktVpAAAAAAAAAADAaSjQgKgyJIfLXHHmTjaLNAAAAAAAAAAAEFMo0ICoMCS7wyzOPD6KMwAAAAAAAAAAYhgFGhBRhmS3S26f5EmRbHarAwEAAAAAAAAAgCZQoAGRYnNI7hSzOLPzrQYAAAAAAAAAQLzgqT4QbobdPN/M65PsTqvTAAAAAAAAAACAEFGgAeFi2CV3onnGmcNtdRoAAAAAAAAAANBMFGhASxk2yZUgedIkJ8UZAAAAAAAAAADxjgINaC7DJjk9ZnHm8lqdBgAAAAAAAAAAhAkFGhAqw2Zu0ej1Sa4kq9MAAAAAK9OXnAAAIABJREFUAAAAAIAwo0ADzpVhSHaX5E2V3MlWpwEAAAAAAAAAABFCgQY0yZAcTsnjk9wpZpEGAAAAAAAAAABaLQo0IChDstslT6pZnNlsVgcCAAAAAAAAAABRQIEGBGJ3mKWZxyfZ7FanAQAAAAAAAAAAUUSBBpzO5jDPN/P4zBINAAAAAAAAAAC0OTQEgCQZdsmdZBZnDpfVaQAAAAAAAAAAgIUo0NC2GTbJnWiec+ZwW50GAAAAAAAAAADEAAo0tE2GTXJ5JU+a5PRYnQYAAAAAAAAAAMQQCjS0LYbNLMw8qZIrweo0AAAAAAAAAAAgBlGgoW0wbObZZt5UyZVkdRoAAAAAAAAAABDDKNDQuhmGZD+tODMMqxMBAAAAAAAAAIAYR4GGVsqQHA5zq0Z3CsUZAAAAAAAAAAA4ZxRoaGUMyW6X3D7J45NsNqsDAQAAAAAAAACAOEOBhtbD5jBXm3l9ks1udRoAAAAAAAAAABCnKNAQ/wy75E42izO70+o0AAAAAAAAAAAgzlGgIX4ZdsmdaJ5z5nBZnQYAAAAAAAAAALQSFGiIT84EKaWz5HRbnQQAAAAAAAAAALQyNqsDAM2S2I7yDAAAAAAAAAAARAQFGgAAAAAAAAAAAHAaCjQAAAAAAAAAAADgNBRoAAAAAAAAAAAAwGkcVgdAfPP7/dq2c6/25+bpWEGRKiqrlJ6aonZpPg3u30u+5CSrIwIAAAAAAAAAAISEAq2VyDuar03bd2nTNvPXlh27VVZRGfC9kyaM0YM/+c8WfV5+YbFm/XuuPl26SnlH8wO+x263a8Tgfpo6aZzGjbmwRZ8HAAAAAAAAAAAQLRRoce6/H/0/ZW3YoiPHCqP2me99sliPP/uqikvLGn1fXV2dVq3brFXrNmv0BUP1yx9+Sx0y0qOUEgAAAAAAAAAAoHk4Ay3OLftqXVTLsxfemKff/fW5JsuzMy1ftV7fvf9hHTlWEKFkAAAAAAAAAAAA4UGBhnP2/oKleuJfrzV7fs7Bw7rnl4+qqro6jKkAAAAAAAAAAADCiwIN56SgqFh/eebloOPdu3TSd6Z9TT/+j2m6ftxoOR2Bdwfdve+g/vXq3EjFBAAAAAAAAAAAaDHOQGslbDZD3bt00qC+52twv16q9/v16FNzwnb9v896I+i2jRPGXKjf/fxuOez2k6/dPGm87nngEVVWnb3a7IU35umGiZfrvI7tw5YPAAAAAAAAAAAgXCjQ4txdt39dvXt00cC+PZWY4D35+ur1W8L2GaXlFfro8xUBx3zJiXrgh99qUJ5J0tABvTVz6mQ9/eJbZ82pqa3Ve58s1t0zbg5bRgAAAAAAAAAAgHBhC8c4N+3Gibpw+MAG5Vm4fbrkS1UFWEkmSVdddoGSkxIDjk2ZOFaGYQQc+3Dhcvn9/rBlBAAAAAAAAAAACBcKNDRp6Zdrg45dMHRA0LHMjHR17ZwZcCw376h27M5pcTYAAAAAAAAAAIBwo0BDk7Zm7w061rtn10bn9u7RJejYtp3BrwsAAAAAAAAAAGAVCjQ0qqikVIeOHAs6ntm+XaPzM9unBx3bvmtfs3MBAAAAAAAAAABECgUaGrU/Ny/omMvpVFITZ6+lp/qadW0AAAAAAAAAAACrUKChUaVlFUHHvF53k/O9nuDvKSsrb1YmAAAAAAAAAACASHJYHQCxraw8eIHmcjb9r4+zkfeUNnLtphQWlehofmGz5wPxIr+gSOUVlcovKLI6CoA4wX0DQKi4bwAIBfcMAKHivgEgVM25b2Skp4Y9BwVaC733yeIWFUFNGT6wrwb27Rmx6zelsqoq6JjdZm9yvsMe/D0VlcGv3ZSFy1Zp/ZbsZs8H4kV5RaW27NgtSUrweixOAyAecN8AECruGwBCwT0DQKi4bwAIVXPuG3dN/3rYc1CgtdCzL7+r3LyjEbv+PXdOtbRA87iDb8FYW1fX5Pza2uDvaWx7x6aMu+wC9e7ZtdnzgXhx4qcsrh83Wulpwc8UBIATuG8ACBX3DQCh4J4BIFTcNwCEKlbuGxRoaFRigjfoWE1tbZPzq2tqgo4lNXLtpqT6kiOyJBOIRQlej9LTfPw7D+Cccd8AECruGwBCwT0DQKi4bwAIVSzcN2yWfTLiQlJi8JKrvLyyyfnlFcHf01g5BwAAAAAAAAAAYBUKNDSqS6cOQcdqamtVUlrW6Pz8wuLg1+6c2excAAAAAAAAAAAAkcIWji307/97SPV+f8Su73Ja+4/Il5ykju3b6dCRYwHHDx/JV3JSYtD5h4PMk6S+53drcT4AAAAAAAAAAIBwo0BrIY/HbXWEiOvfu3vQAi17z3717tk16Nwdu3OCjvXr1b3F2QAAAAAAAAAAAMKNLRzRpDEXDQ86tmrd5qBjBw8f0YFDRwKOdeqQoT6NFG8AAAAAAAAAAABWoUBDk8aPvUhutyvg2GfLVwc9B+3djxcHveZ140bLMIyw5AMAAAAAAAAAAAgnCjQ0KSnBq2uvuCTgWHFpmf7wxPOqratr8Pq6Tdv10tsfBZzjdDh0w8TLw54TAAAAAAAAAAAgHDgDLc797PdPaP2W7LNer62pDTpnweIvtGL1hoBjs//6a3Vs3+6s179351R9tny1igOsNvt06VfauXe/Joy9SMmJCdq2c6/mL/5SNbWBM9xxy/U6r2P7oPkAAAAAAAAAAACsRIEW54pLypRfUBTSnKrqGlVVB55TX18f8PX01BTde9c39ZvH/hlwfE9Orp59+d0mP7tnt8761jemnHtYAAAAAAAAAACAKGMLR5yzyRPG6AffurXZ87t2ztTf/3CfPEHOUwMAAAAAAAAAAIgFrEBDSGZMnSRfSpIef+5VlZSWn/O8S0YN0a9+9G21b5cWwXQAAAAAAAAAAAAtR4GGkH3tmis09uIRev61uVq49CvlHSsI+D67zabhg/tq6uQJGj/mwiinBAAAAAAAAAAAaB4KtDj39CO/sORz01NT9NP/ul0/ueub2pq9RzkH85RfWKTKqmql+ZKVkZ6qQf16KTUlyZJ8AAAAAAAAAAAAzUWBhhYxDEMD+vTUgD49rY4CAAAAAAAAAAAQFjarAwAAAAAAAAAAAACxhAINAAAAAAAAAAAAOA0FGgAAAAAAAAAAAHAaCjQAAAAAAAAAAADgNA6rAwChqKquliTtyTlocRIgOgqLSnQ0v1DZu3N0NL/Q6jgA4gD3DQCh4r4BIBTcMwCEivsGgFA1977Ro0sneTzusOUw/H6/P2xXAyLso8+W61d/etrqGAAAAAAAAAAAIIa88MRv1L93j7BdjwINcaWwqFgrszaqU4cMud0uq+MAAAAAAAAAAIAYwAo0AAAAAAAAAAAAIIJsVgcAAAAAAAAAAAAAYgkFGgAAAAAAAAAAAHAaCjQAAAAAAAAAAADgNBRoAAAAAAAAAAAAwGko0AAAAAAAAAAAAIDTUKABAAAAAAAAAAAAp6FAAwAAAAAAAAAAAE7jsDoAAAAAACD66uvrlb1nv/bkHNSRY4WqrKqS0+GQ1+tRh4w0de2cqR5dOslm4+cuAQBAaPKO5mvn3gM6dOSYyssrVVlVJY/brYQEjzIz0nV+9/PUsX07q2MCiCGFxaXauDVbR/MLVVRSJqfDrvRUnzp2aKfB/XvJYbdHPRMFGgDEsOWr1utH//O/jb7n3ef/rM6Z7aOUCAAAxLude/fr1Xc/0WfLVqmopKzR9yZ4PRo6oLfGXDRcN113lZxO/goJtFZz5y/Rb//ybNiv+9W82WG/JoDYdDS/UK+9N18Llnyp/bl5Tb6/c2aGxo+5SNNunKj27dKikBBArKmtrdVHn6/Ua+99om0798nv9wd8X3JSgsZcOFzfvm2KenTtHLV8/O0HAGJUZWWVHnlqjtUxAMSQG+78qXLzjrb4On/4+d2aeMUlYUgEIJ6UlVfo8ede1TsfLQr6F9MzlVdUamXWRq3M2qjxYy5URnpqhFMCAIB49Na8z/T4c6+qvKLynOccPHxUL7w5T6+/v0DfmzlV026cGMGEAGLNzr379YuH/q7dOQebfG9Jabk+/Gy55i/5QtNvuk53z7g5KjtlUKABQIx65qV3dPDQEatjAACAViD38FH96Nf/q937mv7LKQAAQCheeGOenvjXa82eX1lVrceeeUkVlZX69m03hDEZgFi1at0W3fvgY6qsqg5pXm1tnWb9+30dOnJMv/npXREv0djMHgBi0PZd+/TyOx9bHQMAALQC+YXFuvsXD1OeAYg6O2coAq3ezr379dScN8JyrWdeekfbdu4Ny7UAxK69+w/pvj88EXJ5drqPPluhx555OYypAmMFGgDEmPr6ej30xPOqq6uzOgoAAGgF/vDEv3SgkVXtyUkJunDYQPXu2VUpSYkqr6jUobxj2rhtp3bszjnn7R4BxDe3y6X0NF/I80pKylRTWxtw7PJLRrY0FoAY98b7C1VbG/z5xXkd2+uKS0cpMyNNeccKtHjlGuUcPBzwvXV1dXr7o891/z0zIxUXQAz489MvqqS0POCY3W7XhDEXamDfnqqtrVPWxm1a9tW6gO99/f0FuubKSzSkf++IZaVAA4AY88YHn2rT9l1WxwAQR0J92OV2uSKUBECsee+TxVq8ck3AMcMwNHPqJN1562QlJngDvufQkWP65POVev39TyMZE0AMmHjFxZp4xcUhzamorNKkGT9WTWngAo3zjIDW78u1m4KOXTl6lB76+ffkdJ56BH3PzKl64JGn9Pny1QHnfLUm+PUAxL8NW7O1cvWGgGMup1NPPXSfhg3qe/K1GVMnae78JfrtX5496/319X49+tQcvfDEbyOWlwINAGJI3tF8PTX7zQav2WyG0nwpOlZQZFEqALHu45eesDoCgBhUW1enp194K+j4f//o27ph4uWNXqNj+3aaMXWSbr/punDHA9AKfPDp0qA/Qd6/d3eNGNwvyokARNuRYwVBx3723ekNyjNJcjod+tl3pwct0I7kF4Y1H4DY8tmywN/7knTT9Vc1KM9OmHL1WM1buFyr1m0+a2xr9l5t2bFbA/r0DGvOE9iMGgBiyJ/+70WVlVc0eG3q5Anq3qWTRYkAAEC8WrQiS3lBHmpdc+WlTZZnp7PbbbLb+esjgFP8fr9ee29+0PFpN14TxTQArFJfXx/wdV9KkjpkpAcc65CRLl9yYsAxto4GWrdV67cEHbvy0uBbPzc2Nnf+khZlagx/AwKAGLFoZdZZP4HVISNd35t5i0WJAABAPHvn40VBx/5j2g1RTAKgNVqxeoP25OQGHMtIT9XEy0PbDhJAfOqUmRHw9bLyCtUGOdu9trZWZRWVAcfO69ghbNkAxJ68o/lBxxr7/j+vY/ugYyuzNrYoU2Mo0AAgBpRXVOpP/3jhrNfv+94dSvB6LEgEAADiWV1dvdZv3hFwrFf3LurRtXOUEwFobV5995OgY7dMGieHg1NDgLbg0lFDAr5eW1unRSuyAo59viJLtbWBy7XLLhoWtmwAYk9RSWnQsTO3fG045gw6tj83T6Vn7OgVLvzXDADEgH/MeVOHjzT8CYxxl12gKy4JvjwZAAAgmOw9OSoP8pPdwwf1kSR9tXazPv58hdZvyVbesQJVV9coJTlRnTpkaOSQfho/5iIN7BuZswQAxLc9+3OD/rS32+XUzdePi3IiAFaZ9rVr9M5Hi1RRWXXW2B//9rzKyis0YexFSvB6VFFZpU+XfqW//vPlgNdKSUrUtK9NjHRkABbyetxBz08tKilVuzRf4LHi4MWb3+/X9p17NXJI/7BkPB0FGgBYbPP23Xp97oIGryUlJuj/fXe6RYkAxJtf//lpbd25V0ePFaqsolJJCR4lJyWqZ7fOGtK/t64aPYrVJkAbszV7T9Cx2rp6feenv9P6LdlnjR0rKNKxgiJt3LZTc96Yp9EXDNUvfnCnOrZvF8G0AOLNq+9+EvScomuvGq1UX3KUEwGwSqfMDD34k//UA4/8Q3VnbNlYVFKm3/31Of3ur88pKTFBpWWBH5pL5kP1hx/4vjLSUyMdGYCF2qX5ghZom7bt0vndzgs8tn1Xo9c9ml/Y4myBsIUjAFiorq5eD/3tedWdcejuPXfeovbt0ixKBSDezFu4XLv2HlBxaZnq6upUVFKm/bl5WvLFWj01+w3d+t0H9INf/Vl7cg5aHRVAlOQXFgcde/fjRQHLs0CWr1qvGT/89Tm/H0DrV1JapnmfLgs6fhurR4A2Z9yYC/X0I79Q7x5dgr6nsfLsouGDNOfxB3Xh8IGRiAcghgwb0Cfo2OtzF6iurv6s14tLyvThwuD/7SFJpWWR2cKRAg0ALPTKux9r2869DV4bMqA3W54ACCu/36+Vqzdo+g9/3egDLwCtR7Cf6myOgqIS/fQ3f9X+3LywXRNA/Hrn48BbtUnmQ/DGHqADaL2GDeyjl578ne66/UbZbef2yNlmM/Tt227QYw/+mB0zgDbiytGjgo5tyd6jn//hb8o5ePjka5u379YPfvUnFRSVNHrdxkr6lmALRwCwyKG8Y3rmxbcbvOZw2PXLH35LhmFYlApAa1ZVVa3f/OWfSvB6Gv2PVgDxr7T83P8C6fW4ZTMMlQU5M02SCotL9PCTs/TkH+4LRzwAcaqurl6vz/006Pi0G1l9BrRVX67dpMeffVXbd+075zn19X7969X3NHf+Yt1z51RNGj8mggkBxIIxFw3XgD49tWXH7oDji1ZmadHKLCUmeFVfXx/0h3bOdObuXuHCCjQA/7+9+w6Pskr7OP6bTEjvIRA6gVBC7733JiAIih2x7lpwddVdxYZdFBur2BArIKKIoFKl9957FQgkIb0n8/7Ba5wnM5PMBFL5fq5rr8vn1DvzTGbJc885B6Xk9Wkzbf5P4PbRQ1S/Dt/YBOAaT49KCgzwk7u7udC2ubkWvTD1U8UXcAAvgPLPzYkv4zRpGKEv331eq+Z9rD9+mK7vp7+qzm2bO2y/cfte7dx76GqGCaCcWblhm85diLFbV7tGuLq2b1nCEQEoC2bMXqAHn37TpeSZtYux8Xr+rU/05odfXeXIAJRFkybeJR9vrwLbpKSmOZ08k6QAP98rDcsuVqABQClYunqT1mzeaSirXb2q7ho3vJQiAlBemM1mtW7WSJ3bNFOLJg0UGVFLfj7ekqTc3FwdPXlGC5et1ZyflyorO9vuGMkpqfpizgJNvHtcSYYOoAT5/v/ngiMhQQF6f/K/FeD/9x+adWtV19vPTdTND07S8VP2z0xcsX6rWjZteFVjBVB+zPrpd4d1N40YwE4awDXo1xXr9L+Zc+3WhQYH6v7bRqlr+5YKDgpQQmKy1m/drQ9nztWF2Es27ecsWKq6taprzLC+xR02gFLUIKK2Xvvvg/rPq9OUknp1zi7zL6YEGivQAKCEJaek6q3p39iUP/XgnfL08CiFiACUF/ffNkqLvnpHH776pG4fM1StmjbMS55JkpubmxpE1NbEu8fpkylPF/gAfenqTSURMoBS4ufrU2D94D5dDMmzv7i7u+uGoY7PYt2xhxVowLXq4NGT2u5gFaq/n4+G9WPrNeBak5mVpXc++c5unZ+vjz6d8oxGDuqlsNBguZvNCg0O1LB+3fTplGfk72f/3yofffmD0l1YdQKgfOrctrm+eOc5tW7WyKn2ndo004iBPR3WhwQFXK3QDEigAUAJ27rrgGLi4g1lw/p1U/tWTUopIgDlxZC+XZ3+R2HThvX04PgxDuujL8bp5JnzVys0AGVMWGhwgfVNG9ZzWNekgeO6mEvxDusAVGzfzV/ssG7kwF7y9vIswWgAlAXrt+5WXHyi3bqRg3qqZrUqduuqVa2skQN72a1LTE7Rui27rlaIAMqwujWr6eM3/qtP33xaN48cqKjIugoJCpC7u1l+vj6KrFtTNwztqxlvP6v3X/q3cnJy7I5jMpnUqH7tYomRLRwBoIRZLBabslUbtmvgLQ877JOY5PisojseeUFu5r+/D/G/V57gHDUAkqRBvbtoyodfOzxM9/zFWNWpGV7CUQEoCYX9ARkY4FekOr4RDlyb4uITtWTlRrt1Zjc3jb2uXwlHBKAs2HvwmMO6llENCuzbPKq+w7r9R06oT7f2RY4LQPnSsmlDp7aJ377noN3yujWrFdsWjiTQAKAMSExOKXLf+MQkw3V2tv1vYwC49vj5eCso0F+xlxLs1ifk+/wAUHFE1K4hT49KysjMsluflWX/jETp8nZMjgQG+F9xbADKnx8WLnP42dC7azuFVwkt4YgAlAWXEuyvPpMkb2+vAvv6eDmuz/+cAwAOHDmhP89ftFvXprlz20AWBVs4AgAAVGAFrRbx9OTcRaCicjeb1a6l4+2hHf3xKUlnz8c4rKtSyNaQACqerKxs/bBohcP6cSMHlmA0AMqSgs5xvxATV2Df6ALq2RIWQH6ffjvfYd3IQb2KbV4SaAAAAOWAve1fC3Pw6EmlpKU7rK8cHHglIQEo44b16+awbvWmHQXUbXdYx5mtwLVnyaqNDlezN21YTy2iIks4IgBlRWgBf08sX7ulwL5/rN9awLhBRY4JQNmXm5vr0jOOOQuWaOWGbXbrmkdFqnFk3asUmS0SaAAAAOXALQ896/AfjPbk5uZq2hffO6z38vRQZEStqxEagDKqR6fWDh9sbdi6W7//sd6mfNvuA1qwZLXdPiaTST07t7mqMQIo+2bNX+ywbtzIASUYCYCypmUTx+ecrdm0w+Hnx/e/LNPqjY6/zNOqgHEBlH8X4+J1wz1Patb8xQ6/pCNJySmpeufT7/Tmh1/brTeZTHrgttHFFeblOSxF+TozAKBE3ffkq9q2+4Dduvkzpqh61bASjghASWs/5A5JUv06NTViYE8N7t1ZQYH2zyKKT0jSqx98UeC3Pnt3aac3nnmoWGIFUHYsXrlBT7/+od06k8mkbh1aqnWzRjK7uWnfoeNaumazcnLsn6fav0dHvfLUP4ozXABlzI69h3TPv1+2W1elcojmz5gid7O5hKMCUFbk5ORq6O0TC3wA3rRhPXVu11zBgf5KSErR+q27tXv/EYftq4QGa8HMt+XmxroPoKKKjonTsNsflSS5uZkUFRmhJg0jVDUsVN5eHkpMStWhY6e0acdepaSmORznxuH99fj9txZrrO7FOjoAAACuqqMnz+jtj7/RO59+q8i6tdQiqoHCQoPk5+utpORUHTx6Suu27lJGRqbDMdzcTJowbngJRg2gtAzo2Um/r9ygVRtst2W0WCxavXFHgd8A/0tocKAennBjcYQIoAwraPXZmGF9SZ4B1ziz2U3/vHOMXpz6qcM2ew8d095Dx5we8593jiF5BlxDcnMtLn9OSFKThhF6cPzYYorqbyTQAAAAyqHcXIsOHTulQ8dOudz3lusHq1H9OsUQFYCy6OUnHtCjL7yjLTv3Fam/n6+Ppj7/qMLDQq9yZADKsvMXY/XHOvtnFHl5euj6wb1KNiAAZdKwft20c99hzf995RWPNWpwbw3u0+UqRAWgImvZpIHeem6ivDw9in0u0vkAAADXkBEDe+qhu4r/W1oAyg4vL09NfW6iRgzsKZPJ5FLfqAYR+uq9FxTVIKKYogNQVn2/YKlycnPt1g3p01WB/n4lHBGAsshkMunph8frgdtHy7OID7M9PSrpH3fcoKcevMPlf6sAuHaYzWbdPmaoPnz1qRL7dwgr0AAAAMqBBhG1dPj46SL39/fz0cS7x2n4gB5XMSoA5YWXl6eeeeQujRzYUzPnLtSGrbuV7mCrV7Obm5o1rq+bRgxQn67t2EYJuAalp2fop9/sryYxmUy6acSAEo4IQFlmMpl0103DNah3Z/346x9avHKDzkbHFNovPCxUA3p10qjBvVUjnLPdgWtFUICf7r9tlNZu3qn9R04oO9v+Gcx/CQkO1IAeHXXTiAEl/llhslgslhKdEQAAAEVy7NSfWrZms7bs3K+9B48qIzOrwPYmk0mRdWtqWL9uGtqvG98UB5AnPSNTu/cf0YXYOMVdSpTFYlGAv6+qhoWqeVSk/Hy8SztEAABQjsXExevQsVOKjolTamq60jMy5OnpIR9vL1WtHKIGEbVUpXJIaYcJoJRlZmXpyPEzOht9UTFx8UpLz1BOTq68vTxVpXKw6tetqYha1UttdSoJNAAAgHIoKytbZ85d0Kmz5xUTG6/UtHRlZmXJ29tLfj7eCq8SqiYNIuTn61PaoQIAAAAAAJQ7JNAAAAAAAAAAAAAAK2xmDwAAAAAAAAAAAFghgQYAAAAAAAAAAABYIYEGAAAAAAAAAAAAWCGBBgAAAAAAAAAAAFghgQYAAAAAAAAAAABYIYEGAAAAAAAAAAAAWCGBBgAAAAAAAAAAAFghgQYAAAAAAAAAAABYIYEGAAAAAAAAAAAAWCGBBgAAAAAAAAAAAFghgQYAAAAAAAAAAABYIYEGAAAAAAAAAAAAWCGBBgAAAAAAAAAAAFghgQYAAAAAAAAAAABYIYEGAAAAAAAAAAAAWCGBBgAAAAAAAAAAAFghgQYAAAAAAAAAAABYcS/tAAAAAACgPHr+7U+0cOmavOuh/brp+X/dU4oRobjl5ORq5YZtWrVhm/YdPq64SwlKTklTTm5uXhveBwAAAEDFQAINAAAAKGULlqzWi1M/tSn39vLUj5+9qdDgQJfHTE1LV8/R9xnKnn30bl3Xv3uR4wSuZUdOnNF/X52m46fPltic9z35qrbtPuBUWx9vL/n6eCkoMEANI2qpUf266t21rcLDQos5SgAAAKBiYgtHAAAAoIxKS8/QZ9/NL+0wgGve2eiLuv/JV0o0eeaq1LR0XYyN1+Fjp7Rw2Vq9/fE3GjH+MT08aYqOnyq7cQMAAABlFSvQAAAAgDLsx9/+0M3XD1LNalVKOxTgmvX29G+VkJRiKKtVvapaNW2owAA/ubn9/d3UqMi6JRydY7m5Fq3fultbdz2rx+6/RaMG9y5iqKSQAAAgAElEQVTtkAAAAIBygwQaAAAAUIZlZ+foo6/m6aUn7i/tUIBr0oWYOK3etN1QdufYYfrHHTfIZDKVaCy+Pt4aPbSPbYXFopS0dF2MvaQ9B44qLj7RUJ2ZlaXXPpgpX28vDezVuYSiBQAAAMo3EmgAAABAGbd45QbdfsMQNaxXu7RDAa452/ccVG6uJe86KMBf9902qsSTZ5IU4Oerh8aPLbBNTk6u/li/VW9N/1oXY+Pzyi0Wi17/35fq3LaFAvx9iztUAAAAoNzjDDQAAACgDPLx9sr7b4vFomlffF+K0QDXrmMn/zRcN2kYIXezuZSiKZzZ7Ka+3drry3dfUJXKIYa6pORUzZq/uJQiAwAAAMoXEmgAAABAGXTL9YMM1+u27NLW3QdKKRrg2pWYnGq4DvT3K6VIXFM5JEiP3XuzTXn+7SgBAAAA2EcCDQAAACiDxl7Xz2b1yLQZc0opGuDalZ6RYbh2M5efP6N7d22nwHzbNR48ekrJqWmlFBEAAABQfnAGGgAAAFAGeXhU0r23jNRL736eV7b7wFH9sW6renVpW4qRlZ5Tf57X/sPHdSH2krKyshXg76sGEbXVrFF9mZ1IamRkZmrPwWM6fupPJSWnysvTU2GhQWrTvLFCggKKJebUtHTt2n9Yp/48r+SUNPn6eCssNFhNG9VT1XwJ0qshOiZOB46cUHxCki4lJMmjkruCAv1VI7yKmjaqV6xbD548c16Hjp3UhZhLSs/IkLeXpxpH1lWb5o2Lbc6/JKemaff+I4qJi1d8QpJkkkKCAhQWGqwWjSPl5eVZ5LEthTcps0wmkxpH1tXG7XvzyiwWi2LjEuTn413kcS0Wiw4fP62TZ87pUkKSUlLTFODnq+BAf0VG1FLtGuFXI3yD9PQM7TpwRBdjL+lSQpJyc3IVHBSgyiFBah4VeUU/T2Fyc3O179BxHTlxWvGJyTKZTAoNDlSzxvVVt2Y1p8a4lJCo3QeO6s9zF5WekaEAP19VDw9Tm+aN5OnhccUxxicm6/CxUzpz/oJSUtOUkZEpD49K8vbyVJXKIapepbLq1qomd3ceAwEAADiLfzkBAAAAZdSwft319bxfdeL0ubyy/305V907tnYqYVQU7YfcYbj+6LWn1LZFlEtjDL/zMZ27EJN3/eyjd+u6/t0dtj8bfVEjxj9uKJs/Y4qqVw2TJP3+x3rN/H6hDh8/bbd/ldBgjb/pOo0a3FtubravS0xcvD6f9bMWLV+nFDsrb9zcTOrStoUevffmq/bg//TZaE3/+kctX7NZWdnZNvUmk0nNG9fXXTcNV9f2La9oruSUVH374+9aumaTjp8667Cdn6+PunVoqQnjRjj90F+Stu7ar/ufes1QtnnRTElSVla2vl+4THN/WabTZ6Nt+vbs1KZYE2jL1mzW7J+XaNf+I8rJybHbxqNSJbVu1lC3jBqszm2bFzrm829/ooVL1zisX7h0jcP6e24eqXtvvd654EtIUIC/TVlCUnKRxoqOidOM2Qv0x7qtir2U4LBdjfAwDejZSbeNHix/P1+H7ZyxfutufTPvV23fc0iZWVl225jNZrWIitSNw/urb7f2Lo3/w8Llem3azLzrOjWrae7Hl9/v6ekZ+uqHRZq7cLni4hPt9m/asJ4ennCjw/f53kPH9Ok3P2n91t3Kyc21qff28tT1g3vr3ltGytfFJGBubq5+WbpG839fqV37jxTa3tOjkhpH1lWPjq01uE8XhYUGuzQfAADAtYYEGgAAAFBGmc1ueuD2G/Tky+/nlR0/dVYLl63R8AE9SjGykpGalq5n35yulRu2FdjuQuwlvT7tS23avk8vP/mAKlX6+8+ctZt36rm3PlZCouOEQW6uRWs279TmXfv19nMT1aFV0yuK+/c/1mvyu58rIyPTYRuLxaJd+49o4nNva2DPTpr06IQirUKZs2CJpn/1oxKTUwptm5ySqt9WrNeSlRt18/WD9OD4MXYTjs46c+6CHn/xXR09eabIYxR97mg98/pH2nvoWKFtM7OytHH7Xm3cvlcdWjXVC4/fq8ohQSUQZdmQkWn7PnR1JaLFYtHns37WjNkLlJFpP4ll7c/zFzVj9gLNW7Rcj957s4b27ebSfNLlxPezU6Zr8459hbbNycnR9j0HtX3PQTVrVF+Tn7hPNatVdXlOa8dPndVjL75jNzFsbe+hY3rgP6/p0Xtu1k0jBhjqPv76R302a75ycx2vY0xLz9C3P/6mtZt36qPXnnL6vXkuOkb/fuk9HTx60qn2kpSRmaWd+w5r577DSs/ILHPJXgAAgLKm/GzeDgAAAFyD+nRtp2aN6hvKPv7mR4crMSqKzKxs/euFqYUmz6ytWLdFb3z4Zd71yvXb9PjkdwtMnlnLyMjUv154RydOO17FVZjlazZr0pvTC0ye5ff7yg167IV37CY6HMnOztZL73ymNz/82qnkmbWc3Fx99cMiPfny+8rKsl0d54zomDjd9+SrpZI823vwqO7612Snkmf5bdqxVxMem3xF97i8+TM6xqYsJNj5LUuzs7P13JSP9dFX85xKnllLSErR8299oo+//tGlfidOn9Vd/5rsVPIsvz0Hj2rCYy9p78GjLvf9y+mz0brvyVcKTZ79JTfXorc//lbL12zOK5vy0df65NufCkyeWTt55pwenjRF2XZWrOYXeylBd//7ZZeSZwAAAHAdK9AAAACAMu7B8WMMW+hFX4zT9wuW6ZZRg0oxquL1wedztHXXAUmXz7Iae10/dW7bQuFVQuVuNuts9EUtXb1Js+YvNjzU/+m3lRrcu4tCggL07JTpys6+vK1ftw6tNLh3FzVtVE+BAX5KSU3TngNH9eXchdp36Hhe/4yMTL36wUxNf/0/LsccfSFWL079VBbL5Qfm9evU1KghvdW+ZRNVDglUanqGTpw6qyWrNuqXpWsM27lt3L5Xr0/7Us8+erdTc7307udauGytoczby1ND+nRR57YtFBlRS4H+vsrKzta56Fht3L5H3/+yVBdj4/Pa/7F+m979bJYev/9Wl3/W56ZM14WYOElSoL+vRg/po87tWqh61cry8fZSzKWEy+fVxVxyeeyCXIiJ0yPPvqWEJGPSsEposEYP7aOu7VuqauUQ5VosOnchRqs2bNcPi5Ybkqhno2P08KS39M0HL9rdXrBb+5YKDQ7Mu167aachUVi/Tk117WB/282WTRte6Y94VV2IidPRE8atT0OCAhQeFur0GO98Oku/rlhnKDOZTOrbrb0G9e6sBhG1FODvp0vxidp78Jh+XrLKJvH1ybc/KSQ4QDcM7VvofEnJKXp40luGbWAlKTDAT6OH9FGPjq0UXqWyzGazoi/Gau3mnfph4XJdiP37vRYXn6hHnn1L30x7yeWzBrOys/Xky+/rUkKSJCkqsq5GDu6lNs0aKTQ4UBmZWTp68k/NW7Rcy9duyetnsVj0+odfqWObZlq8aqNm/7xE0uVtE0cM7KlenduqTs1w+fh4KzYuQRu27dbnsxcozmorzMPHT+vreb/pzrHDCoxx6iff5f3+/SUqsq6G9uumZo3qKbxKZXl7eSorO1upqek6G31RR0+e0ZadB7Rpx167W9kCAADAFgk0AAAAoIxr2yJKndo214atu/PKZsxZoBEDe8jP16cUIys+f60869mpjV54/F6bs4EC/H3VOLKuundsrX8+/YZhxdeMOb8oLS1dqWnp8vH20itP/cPmnDE/H29V7RaiXp3b6r+vTTM8CN+2+4AOHj2pRvXruBTzll378/77llGD9OCdY+Tu/vefXP5+vqpaOUQd2zTTqCF99OgLUw0PzxcsWa3+PToWek7XvF9X2CTPenZqo6cfGa/gQNuVRcGBAWrSMELjRg7Uy+99rt9WrM+rm/3zEnVt39Kps8Gs/ZXc7Na+pV54/D4F+BsTUX6+Pi6ds+YMi8WiZ6dMt0me9eveQU8/cpf88r1HQoIC1LRhPd04vL+efv1Dbdn5d1Ln3IUYvfL+F3r1P/+0madf9w7q171D3nXspQRDAq1xg7p6aPzYq/VjFauPv7FdAdW7azun+6/dvDMvEfSXAD9fvfHMQzZnI/r5eKtW9aoa1Luzflm6Ri+9+7nhXLp3Pp2lNs0bq17tGgXO+cr7X9gkzzq2bqrJT9xv8/4OCvBTo/p1NHZ4f02e+qnh9zghKUXPTZmuD199SiaTyemf+ez5i5IuJwkfGj9Wt44ebOjvL6lySJA6tm6qL+b8omlffJ9XF3cpQZ9997PmLVouSYqoXV1Tn/+XaoSHGebw8/FWnZrh6tutvSY8/lLenNLl38nbRg9xeM5lYlKKlq3ZZCibMG6E7r9tlN32gf5+qla1stq2iNLY6/orKytbS1ZtNGx1CwAAAPvYwhEAAAAoBx68c4zhIW5CYrK+mruoFCMqfm1bNNbrTz9kkzyz1rJJA902erChbMPW3dq577BMJpPeeOZhm+SZNbPZTf99eLz8/YyJyEXL1znoUbhRg3tr4t3jDMmz/Jo0jNC0l/4tT0/juWfvz5hT4NhJySl679NZhrKBvTrrzUkP202eWfPy9NCLj9+nXp3bGMo/+25+gf0cad2skd6c9LBN8qy4rN28My9x95du7VvqpScesEmeWQsJCtDU5yYqqkGEoXzp6k2G1YcVicVi0YzZCzT/95WGco9KlXSrCytXP8j3fqzk7q73Jj9mkzzLb1i/bpo08S5DWUZGpqZ/Na/AfgeOnNDS1cbkUPOoSE15dmKB728/H2+9/NQ/1KlNM0P51l0HtGbTzgLndOSB20frthuGFJh8u2PMUJstdr/6YZFS0tIVFhqkj1//r03yzFrlkCA98cBthrKYuHhDsje/3QeO5K2slS4n6Rwlz+ypVMldQ/p2Vf8eHZ3uAwAAcK0igQYAAACUA43q11H/Hh0MZd/NX6yYuHgHPco3s9msZx+92+EqDGsjB/Wy+5B7+IAe6ti6aaH9A/391Kdre0PZ7gNHnA/WSlhokB65+yan2kZG1NIdY4Yayg4fO6Vd+x3PPWfBUqWkpeddh4eF6pmHxzu9wsZkMumpB++Ul1Xibue+wy4nki7fnwkFJgmvtu9+Wmy49vXx1tOP3OXUe8TLy1PPTpwgs9lsHHP+71c1xtKUkpqm46fO6sff/tAdE1/Q/2bOtWnz0F1jVbNaVafG27Rjr46cMJ5xd9sNQ9Q0X8LIkaF9u6lnJ2OyduX6bTobfdFBD+nbH433w93drEmPTDC8Xx1xN5v19CN3ycfby1BelHvcwM7vpj0mk0nXD+5lt+7x+25VUKB/oWN0adfCZkvNXQV8/sTFJxqumzSsV+gcAAAAKBoSaAAAAEA58cDto+Xu/ncCIC09Q59993MpRlR8enZqrepVHa/csFa1cojdVR7jRg5wer42zRsZro8cP+2gZcHGDOtn8wC/IONGDJCnRyVD2W8rHK9+m7doheH6llGD5OXl6VKMocGB6pNvG7+N2/e4NEa39i2dTsRcDfEJSdqcb1XO8AHdVTkkyOkxIiNqqXe+1Xcr1m5RVlb2VYmxJJy7EKP2Q+6w+79eN9yvsff/R6+8N0P7DxsTomazWY/eM043jXD+d2Lxyo2Ga0+PSjarPQtz980jDNc5ublatnqz3bbZ2dlasW6LoaxP13aKqF3d6fnCw0J1Xf/uhrLNO/bZJJ0KM/a6fnJzc+5xSetmjWzKwsNC1atLW6f6m0wmtWpmPDvv8DHHnz+V8iWtrbeBBQAAwNVFAg0AAAAoJ2pWq6oRA3sayn76/Q+dORddShEVn475tmIrTO0a4YbrsNAg1a9T0+n+dfL1T0vPULrVuWrOGtCzk0vt/Xx91LldC0PZngNH7bY9eea8LsReMpRZn9XlivwP/XfsPeRS/x6dWhdp3qLauf+wLBbjWV6De3dxeZyh/boZrjMys3Tg6IkrCa1M8/T00MCenfTdtJd08/XOb90oSbv2HTZcd+vQyuUzFxtH1rX5PdyZb9y/HDx60uZ3rkj3uG9Xm7L8P0thOrVx/kzAGuFhMudLtnVo3dTpBJxk+/kVn5jksG3+hOLG7Xu0cZtrCXAAAAA4hwQaAAAAUI7cPW6EvK1WHGVn5+ijLws+V6g8ahBRy6X2+c9Jq1/3yvpLUnJKqktjhAQFFHjekSP5z1A6fOK0MrOybNpt32M8/yskKMClFVjWwkKDDddnzrqWhI1qULdI8xbV3oPHDNdenh5qWK+Oy+O0bNLApmzPgWN2WlYM/r4+at2skUuruCQpOTVNJ86cM5S1iIosUgz5X/M9B+0niPcctL0PLaJs71dhGtarY7Plo6M57fHz9VF4ldDCG/4/Nzc3eedbdVq/rvPJe8n28yc5Nc1h24b1aqtmtSp517m5Fj3y7Ft6/u1PtH3PQeXk5Lo0NwAAABwruQ3rAQAAAFyxyiFBumnEAM2YvSCvbPGqjbrthiFqVN/1hEJZFeDn51J7j3zbIAb6+V5Rf0l2k1gFcTVJ8Zd6tWsYrrOzcxQXn2hzLtKZcxcM13HxiWo/5I4izZlfQlKyS+3DQkOuyrzOyn/WX0St6k6dfZafv5+vqoaFKPpinNXYlwroUbb4+nhr9NA+NuUZGZmKjYvXnoPHdP5ibF55TFy8Xps2U3sPHdOkiROcPisvNi7BZsWfq0npv0TmS4bHxScqNzfXZoVW/ntcJTRYAf6u/R5Lktnspnp1ahjO9XPlrMiizOnhUUlK+fs60MUxPCsZP38yMx1/9phMJk28Z5z+Pfm9vHuUk5urhUvXaOHSNQr091XLpg3VIqqBmjasp2aN6rm8zSsAAAAuI4EGAAAAlDO33zBE8xYtV0LS5Se2FotF0774Xu9NfryUI7t6KlUyF96oAO6VSv5PHX8Xk3Z/CfCz3RYvKTnFJoGWmJxi0+5qSXJxtZ2fr+2KveKUlO9nL0qS4+++foYEWnG+rldbgJ+vHho/1mG9xWLR+q279eaHXxkSrguWrFZwoL8euutGp+bJ/3pLrieFHPWzWCxKSklVoL8xSX6177E1V+5x/jPGiuJqjFGQnp3a6JlH7tIb//tSGfmSbQlJKVq1YbtWbdieF0vTRvXUp2t79e/RocirVgEAAK5FbOEIAAAAlDN+vj6688brDGXrt+7W1t0HHPRASfD2LNoqD3urQ1JT023KkpKKL9GTm2spvJEVd/OVJThdlZJmfD28r2BFjU++vqlptq91eWUymdSlXQvNePtZ1a1VzVD35dxFWr91t1Pj5H+9JfvvU2d4e3nZlNl7f3OPXTN8QA/N/uhVjRjQo8DXKis7Wzv2HtLbH3+jEeMf1+vTvrSbIAUAAIAtVqABAAAA5dCYYX01a/5iw0qaDz6foxlTny3FqK5taRkZReqXnm7bz8fHNungme8hefXwMPXr3qFIc5Y3vvnOmEqz85o5KzVfXx9v29e6vAsK9NeUSRN1y0OTlJGRmVf+6vtfaM70V23OCMsv/+st2X+fOiMt3TZ5Ze/9zT12XY3wMD0zcYIeu//Wy1+i2LVfO/cd1pETZ5STk2PTPjMrS3MXLtOaTTs07ZUnVLtGeClEDQAAUH6QQAMAAADKIU8PD917y/Wa/M5neWV7Dh7VinVb1LtLu1KMzPWzwyqKoq7qSEy23T7R3naQQQHGbel8vb0K3M6vIsn/eiRewWq8xHznveXf7q+iqFMzXPfePFLvz5iTV3buQoy+/fE33XXT8AL72nv/JRTxNc/fz2Qyyd/XdttS7nHReXt5qk/XdurT9fJnf3p6hnYfOKqtuw9o9cbtOnTslKH9+YuxevT5qZr94ctyL+btJgEAAMoztnAEAAAAyqmhfbspolZ1Q9mHM39QTk5ukcfMf3ZPZla2y2NcyYPv8uz4qbNF6nfs1J+Ga7PZrJCgAJt2VUKDDdenz0YrO9v1+1Me5T+36fjps0V6nyclp+hCzCXj2MEV90yocSMHqlqVyoayr+f9WmiyNzQkUCaTyVB29MTpIsWQv19IUIDc3GwfReS/xxdiLxXpsyQ3N9fmd7FycKDL45RnXl6eat+qie6/bZS++WCyvnrvBbVs0sDQ5tSf57Vo+bpSihAAAKB8IIEGAAAAlFNms5seuGO0oez46bNauGxNkcf08/U2XLu6qur4qbPKukaSOvnFxSfqz/MXXe635+BRw3XDiFryqFTJpl3rZo0M1+kZmdq669o4965Z4/qG6/SMTB06dtLlcXbtPyKLxXjeW/N8Y1cklSq5655bRhrKkpJT9c2PvxfYz8/H2+YMtV37jxQphp37DhuuHb3e+e/x5TkP22lZsEPHTtls/9i8caTL41QkjSPr2t2ycd2WXaUUEQAAQPlAAg0AAAAox3p3aadmjYwPnj/+5kdlZhZtG8WgQH/D9fHTrq2qWr9td5HmrSgWr9zgUvvklFStz/cQ214iQbr8EDwowHh/fvp9pWsBllMtohrYrIj6dYXrq2cWLltruPb09FDjyDpXFFtZN7hPF9UIDzOUzZq/uNDVXflXLK3ZtEPJKbbbjRbk0LFTOnLijKGsRb5x/9Kofh2bs9muxj2+POe1nUCTLm/7O6hXJ0PZ2eiYUooGAACgfCCBBgAAAJRzD44fY7iOvhin739ZWqSxGkbUNlxv3L7X6b5ZWdma/fOSIs1bUXz/y1KlpqU73f67+YuVkS/ZOah3F7ttTSaThg/obihbtmZzkVcGlSdBAX7q2LqpoeznxasVExfv9BhHT57RinVbDGV9urSr8GdAuZvNNmeepaSm6Zsffyuw38CenQ3XGZlZ+uqHX12a+5NvfzJcm93c1L97R4dx9u3W3lC2fO0Wl7ZGvRATpwWLVxnKOrRqquBA2y1Rr0U+3t6FNwIAAEAeEmgAAABAOde2RZQ6t21uKPtmXsEPxx1pHmVcqbF7/xHtOXDUQWuj9z6frbNF2MKwIrkYG6/3PpvlVNsjx09r5vcLDWUN6tVWiyjHq2Vuu2GofLy98q4tFoueeOm9Im0d+Ze4+ESbbQ3LoptGDDBcp6Sm6eX3Zjh1Flp6RqYmT/1M2dk5hvJxIwc46FGxDOnbVdXzrUKb/fMSJSQlO+zTrmWUGkTUMpR9NXeR9h507vPgtxXr9ce6rYayXl3aKrxKqMM++e9xdnaOJr/7mTIyMwudLzsnRy+/N0Mp+RLYFe0en42+WOTf1217jFu+hoc5vhcAAAAggQYAAABUCP+8c4xhi7v8D5Gd1b9HR7m7mw1lz731cYErfbKysjX14281a/7iIs1Z0fywaIXe/WyWsnNyHLbZf/i4HnzmTWVkGBMDD40fW+DYQQF+eviuGw1lsZcSdMfE57V8zWanY7RYLNpz4Kgmv/OZrrvjX8rJLTwJVdq6tGuhdi2iDGVrNu3QpDc/UkpqmsN+8QlJeuyFd7T30DFDef8eHRXVIKJYYi1r3M1mjR87zFCWkpqmbwtJtP/zTuPq1qzsbD086S1t3V3w2XuLlq/VC1M/MZR5enro3luvL7Bf48i66t/DuEJt9/4jevzFdxWfkOSwX0pqmia9/qHNmV5tWzRW1/YtC5yzvJk5Z6FG3/OkZs1frLj4RKf7zf55iVZt2G4o696x1dUODwAAoEKp2HtVAAAAANeIRvXraECPjvrdxTO48gsJCtCQPl31s9U2aKf+PK9x/3hGt40erC7tWyo8LETZ2TmKjonTph17NXfh8ryVZ80b11f0xThdiL10RXGUR+1aRGn/4eNKSUvX1z/8qg1bd2v00D5q17KJKgcHKjUtXSfOnNPilRv1y5LVNkmr6/p3t1lJaM/ooX109OQZff/LsryyhMRkPfnKB6pXp4YG9eqslk0aqHrVMPn7+SgnJ1dJKamKiYvXkeOntf/ICa3bslMXY53f/rAsMJlMeuHxe3XzP59RgtX5XUtWbdTOfYd1w9A+6tKuhaqGhUoWi85Gx2j1pu2a+8tyxScaky/VqlTWfx68o6R/hFI1rF83fT5rgc5d+Pvcq9k/L9G46wcpKMDPbp+u7VvqxuH9DVuzJian6IGnXlO/7h00qHdnNYyoLT8/H8UnJGnfoWOa//sqbdphu/Xro3ePU73aNQqN8z8P3qE9B44a4tywbY/G3Pcf3TCsj7p1aKXqVSvLzc1N0RfjtHbzTs1duFwXYuIM4wT6++rFx++zOTuvIjh9NlpvTf9GUz/5Vi2iGqhtiyg1rl9HdWpWU4C/r3y9vZSemaXoi7Hae/CYFi5bY7PVa+3qVW2SlQAAADAigQYAAABUEPffPkrL1m622abOVY9MuEkbtu42JMHiE5P0/ow5en/GHIf9qoeH6fWnH9KEx166ovnLq6pVQjXmun566pUPZLFYdOTEGb0+7Uun+nZo1VRP/ON2p+d67L5b5e3tpS/zbQF57OSf+t/MuS7FXZ5UqRyid198TI8+P1WXrFYkXYiJ0/9mznXqZ69etbLeffEx+fv5FmeoZY67u7vuvHGYXn3/i7yylLR0fTPvV5uVZtYm3n2TEpKS9duK9XllFotFS1Zt1JJVG52a++6bR2j00D5OtfX389V7kx/Tw5PeMiTR4hOT9Om38/Xpt/MLHSM40F9Tn39UVSqHODVneZWba9GOvYe0Y+8hl/oF+vvq5af+IS9Pj2KKDAAAoGJgC0cAAACggqhZrapGDux1xeME+Pvqw9eeUvWqlZ3uE9UgQh+/8V+FhQZf8fzlWZ+u7fTSE/fL04UH0/17dNRbz0106WG22eymh8aP1ZRJj9icbeUKNzeT2rVsIrdytEqnaaP6+uytSWrS0PXtF9u3aqLP3pqkurWqF0NkZd/w/t1tzr36fsFSxSc6PgvN3d1dLz5+n+699Xp5elRyab5Af1899697dN+to1zqV7dWdX3+9iS1a9nEpX6S1LRhPX3+9iQ1bVTf5b7lQaVKV/Y96KgGEfp0yjNqHFn36gQEAABQgbECDQAAAKhAJl+MgHwAAAO4SURBVIwbroXL1igtPeOKxqldI1xfv/+ivvh+oeYtWqHklFS77cLDQnXz9YM05rq+cjeb7ba51gzo2UlRDSI0/at5Wr52i7Kys23amEwmNWtUTxPGjbiiM5p6dm6jbh1a6feV67VgyRrt3n9YGZlZBfbx8fZS62aN1KFVE/Xt3kFVy+EqnVrVq2rmO89r6epNmvPzEu06cFQ5Ds6c86hUSa2bNdTN1w9Sl3YtSjjSssXd3V13jh2m16bNzCu7vOXoIj1YwPl7JpNJ99w8Utf1764vZi/QH+u3KfZSgsP2NcLDNKBnJ902enCRV/pVDgnSh68+qXVbdunbH3/T9j2HlJll/71tNpvVonF9jR3eX/26dyjSfOXFY/fdosG9O2vt5l3atueA9h06XujnvdnNTe1bNdGwft00oGenCrmtJQAAQHEwWSwWS2kHAQAAAKDsys7J0d4DR3XizDnFJybLYrEoJChAjerXUcN6tXkYW4CU1DTt2n9Ep/48r5TUNPl4eyksNFhNG9WzWQl0NWRmZWnfoeOKvhirhKRkJSWnysOjknx9vBUWEqy6taqpRniY3Nwq1mYkySmp2rX/iGLi4hWfkCSTyaSgQH9VCQ1WiyYN5O3lWdohVigWi0WHjp3SyTPnFZ+YqJTUdPn5+igkKECRdWupTs3wqz5nWnqGdu0/oouxl3QpIVG5uRYFB/qrckiQWkRFys/X56rPWR7k5OTq9Llonf4zWhdi4pSSmqas7Gx5e3vJ39dHdWtVU2TdWvwOAAAAFAEJNAAAAAAAAAAAAMBKxfraIQAAAAAAAAAAAHCFSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFZIoAEAAAAAAAAAAABWSKABAAAAAAAAAAAAVkigAQAAAAAAAAAAAFb+D9nwQyD1t+5RAAAAAElFTkSuQmCC
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sns</span><span class="o">.</span><span class="n">regplot</span><span class="p">(</span><span class="n">y</span><span class="o">=</span><span class="s2">&quot;PRICE&quot;</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="s2">&quot;DIS&quot;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">bos</span><span class="p">,</span> <span class="n">fit_reg</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
            <span class="n">scatter_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;alpha&#39;</span><span class="p">:</span><span class="mf">0.3</span><span class="p">,</span> <span class="s1">&#39;s&#39;</span><span class="p">:</span><span class="mi">60</span><span class="p">},</span>
            <span class="n">line_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;color&#39;</span><span class="p">:</span><span class="s1">&#39;C1&#39;</span><span class="p">})</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Distance from Employment Center&#39;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Median Home Value ($1,000s)&#39;</span><span class="p">)</span>
<span class="n">_</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Distance from Employment Centers vs. Median Home Value&#39;</span><span class="p">);</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Load and return the boston house-prices dataset (regression).</span>
<span class="kn">from</span> <span class="nn">sklearn.datasets</span> <span class="k">import</span> <span class="n">load_iris</span>

<span class="n">iris</span> <span class="o">=</span> <span class="n">load_iris</span><span class="p">()</span>
<span class="n">iris</span><span class="o">.</span><span class="n">keys</span><span class="p">()</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">iris</span><span class="o">.</span><span class="n">data</span><span class="p">)</span>
<span class="n">df</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">iris</span><span class="o">.</span><span class="n">feature_names</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;species&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">iris</span><span class="o">.</span><span class="n">target</span>

<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
<span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">()</span>
<span class="n">df</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>&lt;class &#39;pandas.core.frame.DataFrame&#39;&gt;
RangeIndex: 150 entries, 0 to 149
Data columns (total 5 columns):
sepal length (cm)    150 non-null float64
sepal width (cm)     150 non-null float64
petal length (cm)    150 non-null float64
petal width (cm)     150 non-null float64
species              150 non-null int64
dtypes: float64(4), int64(1)
memory usage: 5.9 KB
</pre>
</div>
</div>

<div class="output_area">

<div class="prompt output_prompt">Out[9]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>sepal length (cm)</th>
      <th>sepal width (cm)</th>
      <th>petal length (cm)</th>
      <th>petal width (cm)</th>
      <th>species</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>150.000000</td>
      <td>150.000000</td>
      <td>150.000000</td>
      <td>150.000000</td>
      <td>150.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>5.843333</td>
      <td>3.054000</td>
      <td>3.758667</td>
      <td>1.198667</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>std</th>
      <td>0.828066</td>
      <td>0.433594</td>
      <td>1.764420</td>
      <td>0.763161</td>
      <td>0.819232</td>
    </tr>
    <tr>
      <th>min</th>
      <td>4.300000</td>
      <td>2.000000</td>
      <td>1.000000</td>
      <td>0.100000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>5.100000</td>
      <td>2.800000</td>
      <td>1.600000</td>
      <td>0.300000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>5.800000</td>
      <td>3.000000</td>
      <td>4.350000</td>
      <td>1.300000</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>6.400000</td>
      <td>3.300000</td>
      <td>5.100000</td>
      <td>1.800000</td>
      <td>2.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>7.900000</td>
      <td>4.400000</td>
      <td>6.900000</td>
      <td>2.500000</td>
      <td>2.000000</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Load and return the digits dataset (classification).</span>
<span class="kn">from</span> <span class="nn">sklearn.datasets</span> <span class="k">import</span> <span class="n">load_digits</span>

<span class="n">digits</span> <span class="o">=</span> <span class="n">load_digits</span><span class="p">()</span>
<span class="n">digits</span><span class="o">.</span><span class="n">keys</span><span class="p">()</span>

<span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">digits</span><span class="o">.</span><span class="n">data</span><span class="p">)</span>
<span class="n">df</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">digits</span><span class="o">.</span><span class="n">images</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;digit&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">digits</span><span class="o">.</span><span class="n">target</span>

<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
<span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">()</span>
<span class="n">df</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_text output_error">
<pre>
<span class="ansi-red-fg">---------------------------------------------------------------------------</span>
<span class="ansi-red-fg">ValueError</span>                                Traceback (most recent call last)
<span class="ansi-green-fg">&lt;ipython-input-10-b11867e0a8d1&gt;</span> in <span class="ansi-cyan-fg">&lt;module&gt;</span><span class="ansi-blue-fg">()</span>
<span class="ansi-green-intense-fg ansi-bold">      6</span> 
<span class="ansi-green-intense-fg ansi-bold">      7</span> df <span class="ansi-blue-fg">=</span> pd<span class="ansi-blue-fg">.</span>DataFrame<span class="ansi-blue-fg">(</span>digits<span class="ansi-blue-fg">.</span>data<span class="ansi-blue-fg">)</span>
<span class="ansi-green-fg">----&gt; 8</span><span class="ansi-red-fg"> </span>df<span class="ansi-blue-fg">.</span>columns <span class="ansi-blue-fg">=</span> digits<span class="ansi-blue-fg">.</span>images
<span class="ansi-green-intense-fg ansi-bold">      9</span> df<span class="ansi-blue-fg">[</span><span class="ansi-blue-fg">&#39;digit&#39;</span><span class="ansi-blue-fg">]</span> <span class="ansi-blue-fg">=</span> digits<span class="ansi-blue-fg">.</span>target
<span class="ansi-green-intense-fg ansi-bold">     10</span> 

<span class="ansi-green-fg">~/anaconda3/lib/python3.6/site-packages/pandas/core/generic.py</span> in <span class="ansi-cyan-fg">__setattr__</span><span class="ansi-blue-fg">(self, name, value)</span>
<span class="ansi-green-intense-fg ansi-bold">   4383</span>         <span class="ansi-green-fg">try</span><span class="ansi-blue-fg">:</span>
<span class="ansi-green-intense-fg ansi-bold">   4384</span>             object<span class="ansi-blue-fg">.</span>__getattribute__<span class="ansi-blue-fg">(</span>self<span class="ansi-blue-fg">,</span> name<span class="ansi-blue-fg">)</span>
<span class="ansi-green-fg">-&gt; 4385</span><span class="ansi-red-fg">             </span><span class="ansi-green-fg">return</span> object<span class="ansi-blue-fg">.</span>__setattr__<span class="ansi-blue-fg">(</span>self<span class="ansi-blue-fg">,</span> name<span class="ansi-blue-fg">,</span> value<span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">   4386</span>         <span class="ansi-green-fg">except</span> AttributeError<span class="ansi-blue-fg">:</span>
<span class="ansi-green-intense-fg ansi-bold">   4387</span>             <span class="ansi-green-fg">pass</span>

<span class="ansi-green-fg">pandas/_libs/properties.pyx</span> in <span class="ansi-cyan-fg">pandas._libs.properties.AxisProperty.__set__</span><span class="ansi-blue-fg">()</span>

<span class="ansi-green-fg">~/anaconda3/lib/python3.6/site-packages/pandas/core/generic.py</span> in <span class="ansi-cyan-fg">_set_axis</span><span class="ansi-blue-fg">(self, axis, labels)</span>
<span class="ansi-green-intense-fg ansi-bold">    643</span> 
<span class="ansi-green-intense-fg ansi-bold">    644</span>     <span class="ansi-green-fg">def</span> _set_axis<span class="ansi-blue-fg">(</span>self<span class="ansi-blue-fg">,</span> axis<span class="ansi-blue-fg">,</span> labels<span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">:</span>
<span class="ansi-green-fg">--&gt; 645</span><span class="ansi-red-fg">         </span>self<span class="ansi-blue-fg">.</span>_data<span class="ansi-blue-fg">.</span>set_axis<span class="ansi-blue-fg">(</span>axis<span class="ansi-blue-fg">,</span> labels<span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">    646</span>         self<span class="ansi-blue-fg">.</span>_clear_item_cache<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">    647</span> 

<span class="ansi-green-fg">~/anaconda3/lib/python3.6/site-packages/pandas/core/internals.py</span> in <span class="ansi-cyan-fg">set_axis</span><span class="ansi-blue-fg">(self, axis, new_labels)</span>
<span class="ansi-green-intense-fg ansi-bold">   3321</span>             raise ValueError(
<span class="ansi-green-intense-fg ansi-bold">   3322</span>                 <span class="ansi-blue-fg">&#39;Length mismatch: Expected axis has {old} elements, new &#39;</span>
<span class="ansi-green-fg">-&gt; 3323</span><span class="ansi-red-fg">                 &#39;values have {new} elements&#39;.format(old=old_len, new=new_len))
</span><span class="ansi-green-intense-fg ansi-bold">   3324</span> 
<span class="ansi-green-intense-fg ansi-bold">   3325</span>         self<span class="ansi-blue-fg">.</span>axes<span class="ansi-blue-fg">[</span>axis<span class="ansi-blue-fg">]</span> <span class="ansi-blue-fg">=</span> new_labels

<span class="ansi-red-fg">ValueError</span>: Length mismatch: Expected axis has 64 elements, new values have 1797 elements</pre>
</div>
</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>