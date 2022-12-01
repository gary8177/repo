{
  "userStyles": {},
  "userPlugins": {
    "downloadVideo.outputs.aria2": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"video/download/aria2-output\"]=t():e[\"video/download/aria2-output\"]=t()}(globalThis,(()=>(()=>{var e={744:(e,t,n)=>{var o=n(355)((function(e){return e[1]}));o.push([e.id,\".rpc-config.download-video-config-section {\\n  display: flex;\\n  align-items: center;\\n  flex-direction: column;\\n  gap: 0;\\n  align-items: stretch;\\n}\\n.rpc-config.download-video-config-section > * {\\n  display: flex;\\n  align-items: center;\\n  gap: 0;\\n}\\n.rpc-config.download-video-config-section > *:not(:last-child) {\\n  margin-bottom: 12px;\\n}\\n.rpc-config.download-video-config-section .profile-item-name {\\n  margin-right: 8px;\\n}\\n.rpc-config.download-video-config-section .profile-other .profile-item-name {\\n  align-self: flex-start;\\n}\\n.rpc-config.download-video-config-section .profile-select .be-textbox,\\n.rpc-config.download-video-config-section .profile-select .be-dropdown {\\n  margin-right: 8px;\\n}\\n.rpc-config.download-video-config-section .profile-select .be-button {\\n  padding: 4px;\\n}\\n.rpc-config.download-video-config-section .profile-method {\\n  align-self: flex-start;\\n}\",\"\"]),e.exports=o},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var n=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(n,\"}\"):n})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,n,o){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var r={};if(o)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar s=this[i][0];null!=s&&(r[s]=!0)}for(var a=0;a<e.length;a++){var c=[].concat(e[a]);o&&r[c[0]]||(n&&(c[2]?c[2]=\"\".concat(n,\" and \").concat(c[2]):c[2]=n),t.push(c))}},t}},648:(e,t,n)=>{\"use strict\";var o,r=function(){return void 0===o&&(\n// @see http://browserhacks.com/#hack-e71d8692f65334173fee715c222cb805\n// @see https://github.com/webpack-contrib/style-loader/issues/177\no=Boolean(window&&document&&document.all&&!window.atob)),o},i=function(){var e={};return function(t){if(void 0===e[t]){var n=document.querySelector(t);if(window.HTMLIFrameElement&&n instanceof window.HTMLIFrameElement)try{n=n.contentDocument.head}catch(e){n=null}e[t]=n}return e[t]}}(),s=[];function a(e){for(var t=-1,n=0;n<s.length;n++)if(s[n].identifier===e){t=n;break}return t}function c(e,t){for(var n={},o=[],r=0;r<e.length;r++){var i=e[r],c=t.base?i[0]+t.base:i[0],l=n[c]||0,d=\"\".concat(c,\" \").concat(l);n[c]=l+1;var p=a(d),f={css:i[1],media:i[2],sourceMap:i[3]};-1!==p?(s[p].references++,s[p].updater(f)):s.push({identifier:d,updater:v(f,t),references:1}),o.push(d)}return o}function l(e){var t=document.createElement(\"style\"),o=e.attributes||{};if(void 0===o.nonce){var r=n.nc;r&&(o.nonce=r)}if(Object.keys(o).forEach((function(e){t.setAttribute(e,o[e])})),\"function\"==typeof e.insert)e.insert(t);else{var s=i(e.insert||\"head\");if(!s)throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");s.appendChild(t)}return t}var d,p=(d=[],function(e,t){return d[e]=t,d.filter(Boolean).join(\"\\n\")});function f(e,t,n,o){var r=n?\"\":o.media?\"@media \".concat(o.media,\" {\").concat(o.css,\"}\"):o.css;if(e.styleSheet)e.styleSheet.cssText=p(t,r);else{var i=document.createTextNode(r),s=e.childNodes;s[t]&&e.removeChild(s[t]),s.length?e.insertBefore(i,s[t]):e.appendChild(i)}}function u(e,t,n){var o=n.css,r=n.media,i=n.sourceMap;if(r?e.setAttribute(\"media\",r):e.removeAttribute(\"media\"),i&&\"undefined\"!=typeof btoa&&(o+=\"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))),\" */\")),e.styleSheet)e.styleSheet.cssText=o;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(o))}}var m=null,h=0;function v(e,t){var n,o,r;if(t.singleton){var i=h++;n=m||(m=l(t)),o=f.bind(null,n,i,!1),r=f.bind(null,n,i,!0)}else n=l(t),o=u.bind(null,n,t),r=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(n)};return o(e),function(t){if(t){if(t.css===e.css&&t.media===e.media&&t.sourceMap===e.sourceMap)return;o(e=t)}else r()}}e.exports=function(e,t){(t=t||{}).singleton||\"boolean\"==typeof t.singleton||(t.singleton=r());var n=c(e=e||[],t);return function(e){if(e=e||[],\"[object Array]\"===Object.prototype.toString.call(e)){for(var o=0;o<n.length;o++){var r=a(n[o]);s[r].references--}for(var i=c(e,t),l=0;l<n.length;l++){var d=a(n[l]);0===s[d].references&&(s[d].updater(),s.splice(d,1))}n=i}}}},273:(e,t,n)=>{\"use strict\";n.r(t),n.d(t,{default:()=>P});var o=function(){var e=this,t=e.$createElement,n=e._self._c||t;return n(\"div\",{staticClass:\"rpc-config download-video-config-section\"},[e.isRenaming?n(\"div\",{staticClass:\"profile-select\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"重命名 RPC 预设:\")]),e._v(\" \"),n(\"TextBox\",{ref:\"renameInput\",model:{value:e.profileRename,callback:function(t){e.profileRename=t},expression:\"profileRename\"}}),e._v(\" \"),n(\"VButton\",{key:\"check\",attrs:{type:\"transparent\",title:\"完成\"},on:{click:function(t){return e.endRename()}}},[n(\"VIcon\",{attrs:{icon:\"mdi-check\",size:16}})],1)],1):n(\"div\",{staticClass:\"profile-select\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"RPC 预设:\")]),e._v(\" \"),n(\"VDropdown\",{attrs:{items:e.rpcProfiles},scopedSlots:e._u([{key:\"item\",fn:function(t){var n=t.item;return[e._v(\"\\n        \"+e._s(n.name)+\"\\n      \")]}}]),model:{value:e.selectedRpcProfile,callback:function(t){e.selectedRpcProfile=t},expression:\"selectedRpcProfile\"}}),e._v(\" \"),n(\"VButton\",{key:\"edit\",attrs:{type:\"transparent\",title:\"重命名\"},on:{click:function(t){return e.startRename()}}},[n(\"VIcon\",{attrs:{icon:\"mdi-pencil-outline\",size:16}})],1),e._v(\" \"),n(\"VButton\",{key:\"new\",attrs:{type:\"transparent\",title:\"新建预设\"},on:{click:function(t){return e.newProfile()}}},[n(\"VIcon\",{attrs:{icon:\"mdi-plus\",size:16}})],1),e._v(\" \"),n(\"VButton\",{key:\"delete\",attrs:{disabled:e.rpcProfiles.length<2,type:\"transparent\",title:\"删除当前预设\"},on:{click:function(t){return e.deleteProfile()}}},[n(\"VIcon\",{attrs:{icon:\"mdi-trash-can-outline\",size:16}})],1)],1),e._v(\" \"),e.selectedRpcProfile?[n(\"div\",{staticClass:\"profile-secret-key\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"密钥:\")]),e._v(\" \"),n(\"TextBox\",{attrs:{\"change-on-blur\":\"\"},model:{value:e.selectedRpcProfile.secretKey,callback:function(t){e.$set(e.selectedRpcProfile,\"secretKey\",t)},expression:\"selectedRpcProfile.secretKey\"}})],1),e._v(\" \"),n(\"div\",{staticClass:\"profile-dir\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"路径:\")]),e._v(\" \"),n(\"TextBox\",{attrs:{\"change-on-blur\":\"\"},model:{value:e.selectedRpcProfile.dir,callback:function(t){e.$set(e.selectedRpcProfile,\"dir\",t)},expression:\"selectedRpcProfile.dir\"}})],1),e._v(\" \"),n(\"div\",{staticClass:\"profile-host\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"主机:\")]),e._v(\" \"),n(\"TextBox\",{attrs:{\"change-on-blur\":\"\"},model:{value:e.selectedRpcProfile.host,callback:function(t){e.$set(e.selectedRpcProfile,\"host\",t)},expression:\"selectedRpcProfile.host\"}})],1),e._v(\" \"),n(\"div\",{staticClass:\"profile-port\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"端口:\")]),e._v(\" \"),n(\"TextBox\",{attrs:{\"change-on-blur\":\"\"},model:{value:e.selectedRpcProfile.port,callback:function(t){e.$set(e.selectedRpcProfile,\"port\",t)},expression:\"selectedRpcProfile.port\"}})],1),e._v(\" \"),n(\"div\",{staticClass:\"profile-method\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"方法:\")]),e._v(\" \"),n(\"VDropdown\",{attrs:{items:[\"get\",\"post\"],\"key-mapper\":function(e){return e}},scopedSlots:e._u([{key:\"item\",fn:function(t){var n=t.item;return[e._v(\"\\n          \"+e._s(n)+\"\\n        \")]}}],null,!1,883355439),model:{value:e.selectedRpcProfile.method,callback:function(t){e.$set(e.selectedRpcProfile,\"method\",t)},expression:\"selectedRpcProfile.method\"}})],1),e._v(\" \"),n(\"div\",{staticClass:\"profile-other\"},[n(\"div\",{staticClass:\"profile-item-name\"},[e._v(\"其他配置:\")]),e._v(\" \"),n(\"TextArea\",{attrs:{placeholder:\"some-key=value\",\"change-on-blur\":\"\"},model:{value:e.selectedRpcProfile.other,callback:function(t){e.$set(e.selectedRpcProfile,\"other\",t)},expression:\"selectedRpcProfile.other\"}})],1)]:e._e()],2)};o._withStripped=!0;const r=coreApis.settings;var i=n(391);const s=coreApis.ui,a={name:\"未命名\",secretKey:\"\",dir:\"\",host:\"127.0.0.1\",port:\"6800\",method:\"get\",other:\"\"},{options:c}=(0,r.getComponentSettings)(\"downloadVideo\"),l={...{rpcProfiles:[a],selectedRpcProfileName:a.name},...c},d=l.rpcProfiles.find((e=>e.name===l.selectedRpcProfileName))??(l.rpcProfiles.length<1?(l.rpcProfiles.push(a),a):l.rpcProfiles[0]);console.log(l,d);const p=Vue.extend({components:{TextBox:s.TextBox,VButton:s.VButton,VIcon:s.VIcon,VDropdown:s.VDropdown,TextArea:s.TextArea},data:()=>({isRenaming:!1,profileRename:\"\",rpcProfiles:l.rpcProfiles,selectedRpcProfile:d}),methods:{saveSettings(){l.selectedRpcProfileName=this.selectedRpcProfile.name,l.rpcProfiles=this.rpcProfiles,Object.assign(c,l)},async startRename(){this.profileRename=this.selectedRpcProfile.name,this.isRenaming=!0,await this.$nextTick(),this.$refs.renameInput?.focus()},endRename(){const e=this.profileRename;e?l.rpcProfiles.some((t=>t.name!==this.selectedRpcProfile.name&&t.name===e))?i.Toast.error(\"名称不得与其他预设重复\",\"重命名 RPC 预设\",2e3):(this.selectedRpcProfile.name=this.profileRename,this.isRenaming=!1,this.saveSettings()):i.Toast.error(\"名称不得为空\",\"重命名 RPC 预设\",2e3)},newProfile(){const e={...this.selectedRpcProfile},t={num:1,toString(){return`未命名${this.num}`}};for(;l.rpcProfiles.some((e=>e.name===t.toString()));)t.num++;e.name=t.toString(),l.rpcProfiles.push(e),this.selectedRpcProfile=e},deleteProfile(){if(l.rpcProfiles.length<2)return;const e=l.rpcProfiles.findIndex((e=>e.name===this.selectedRpcProfile.name));-1!==e&&confirm(`确认删除 RPC 预设 \"${this.selectedRpcProfile.name}\" 吗?`)&&(l.rpcProfiles.splice(e,1),this.selectedRpcProfile=l.rpcProfiles[0])}}});var f=n(648),u=n.n(f),m=n(744),h=n.n(m),v={insert:\"head\",singleton:!1};u()(h(),v);h().locals;var g=function(e,t,n,o,r,i,s,a){var c,l=\"function\"==typeof e?e.options:e;if(t&&(l.render=t,l.staticRenderFns=n,l._compiled=!0),o&&(l.functional=!0),i&&(l._scopeId=\"data-v-\"+i),s?(c=function(e){(e=e||this.$vnode&&this.$vnode.ssrContext||this.parent&&this.parent.$vnode&&this.parent.$vnode.ssrContext)||\"undefined\"==typeof __VUE_SSR_CONTEXT__||(e=__VUE_SSR_CONTEXT__),r&&r.call(this,e),e&&e._registeredComponents&&e._registeredComponents.add(s)},l._ssrRegister=c):r&&(c=a?function(){r.call(this,(l.functional?this.parent:this).$root.$options.shadowRoot)}:r),c)if(l.functional){l._injectStyles=c;var d=l.render;l.render=function(e,t){return c.call(t),d(e,t)}}else{var p=l.beforeCreate;l.beforeCreate=p?[].concat(p,c):[c]}return{exports:e,options:l}}(p,o,[],!1,null,null,null);g.options.__file=\"registry/lib/plugins/video/download/aria2-output/RpcConfig.vue\";const P=g.exports},391:e=>{\"use strict\";e.exports=coreApis.toast}},t={};function n(o){var r=t[o];if(void 0!==r)return r.exports;var i=t[o]={id:o,exports:{}};return e[o](i,i.exports,n),i.exports}n.n=e=>{var t=e&&e.__esModule?()=>e.default:()=>e;return n.d(t,{a:t}),t},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var o={};return(()=>{\"use strict\";n.d(o,{plugin:()=>h});const e=coreApis.download,t=coreApis.utils.constants,r=coreApis.utils.title,i={name:\"aria2\",displayName:\"aria2 Input\",description:\"使用 aria2 命令行输入文件开始下载. (aria2c -i xxx.txt)\",runAction:async n=>{const{infos:o}=n,i=document.URL.replace(window.location.search,\"\"),s=`\\n# Generated by Bilibili Evolved Video Export\\n# https://github.com/the1812/Bilibili-Evolved/\\n${o.map((e=>e.titledFragments.map((e=>({url:e.url,params:{referer:i,userAgent:t.UserAgent,out:e.title}}))).flat().map((e=>{const t=Object.entries(e.params).map((e=>{let[t,n]=e;return`  ${lodash.kebabCase(t)}=${n}`})).join(\"\\n\");return`${e.url}\\n${t}`})))).flat().join(\"\\n\")}`.trim();await e.DownloadPackage.single(`${(0,r.getFriendlyTitle)()}.txt`,s)}},s=coreApis.ajax;var a=n(391);const c=coreApis.utils.log,l=e=>{const t=e.host.match(/^http[s]?:\\/\\//)?e.host:`http://${e.host}`;return{option:e,host:t,methodName:\"aria2.addUri\"}},d=async(e,t)=>{try{let n=await t();return\"string\"==typeof n&&(n=JSON.parse(n)),void 0!==n.error?1===n.error.code?{param:e,success:!1,message:\"请求遭到拒绝, 请检查您的密钥相关设置.\"}:{param:e,success:!1,message:`请求发生错误, code = ${n.error.code}, message = ${n.error.message}`}:{param:e,success:!0,message:n.result}}catch(t){return{param:e,success:!1,message:`无法连接到RPC主机, error = ${t.toString()}`}}},p=async(e,t)=>{const{option:n,host:o,methodName:r}=l(e);return d(t,(async()=>{const e=window.btoa(unescape(encodeURIComponent(JSON.stringify(t.params)))),i=`${o}:${n.port}/jsonrpc?method=${r}&id=${t.id}&params=${e}`;return console.log(`RPC request: ${i}`),i.startsWith(\"http:\")?(0,s.monkey)({method:\"GET\",url:i,responseType:\"json\"}):(0,s.getJson)(i)}))},f=async(e,t)=>{const{option:n,host:o,methodName:r}=l(e);return d(t,(async()=>{const e=`${o}:${n.port}/jsonrpc`,i={method:r,id:t.id,params:t.params};return e.startsWith(\"http:\")?(0,s.monkey)({method:\"POST\",url:e,responseType:\"json\",data:JSON.stringify(i)}):(0,s.postJson)(e,i)}))},u=e=>{if(!e)return{};const t=e.split(\"\\n\").map((e=>{const[t,...n]=e.trim().split(\"=\");return[t.trim(),n.join(\"=\").trim()]})).filter((e=>Boolean(e[1])));return Object.fromEntries(t)},m={name:\"aria2Rpc\",displayName:\"aria2 RPC\",description:\"使用 aria2 RPC 功能发送下载请求.\",runAction:async(e,n)=>{const{infos:o}=e,{selectedRpcProfile:r}=n,{secretKey:i,dir:s,other:l}=r,d=document.URL.replace(window.location.search,\"\"),m=o.map((e=>e.titledFragments.map((e=>{const n=[];i&&n.push(`token:${i}`),n.push([e.url]),n.push({referer:d,\"user-agent\":t.UserAgent,out:e.title,dir:s||void 0,...u(l)});return{params:n,id:encodeURIComponent(e.title)}})))).flat(),h=await(async(e,t)=>{const n=[];for(const o of t){let t;t=\"get\"===e.method?await p(e,o):await f(e,o),n.push(t)}return n})(r,m);if(console.table(h),1===h.length){const e=h[0];e.success?a.Toast.success(`成功发送了请求, GID = ${e.message}`,\"aria2 RPC\",5e3):(0,c.logError)(e.message)}else{const e=h.filter((e=>e.success)).length,t=h.length-e;a.Toast.info(`发送了 ${h.length} 个请求, 成功 ${e} 个, 失败 ${t} 个.`,\"aria2 RPC\",5e3)}},component:()=>Promise.resolve().then(n.bind(n,273)).then((e=>e.default))},h={name:\"downloadVideo.outputs.aria2\",displayName:\"下载视频 - aria2 输出支持\",description:\"为下载视频增加 aria2 文件导出和 RPC 输出支持.\",setup:e=>{let{addData:t}=e;t(\"downloadVideo.outputs\",(e=>{e.push(i),e.push(m)}))},commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"}})(),o=o.plugin})()));",
      "displayName": "下载视频 - aria2 输出支持",
      "name": "downloadVideo.outputs.aria2",
      "description": "为下载视频增加 aria2 文件导出和 RPC 输出支持.",
      "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
      "coreVersion": "2.5.2"
    }
  },
  "userComponents": {
    "hideRecommendedLive": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"style/hide/video/recommended-live\"]=t():e[\"style/hide/video/recommended-live\"]=t()}(globalThis,(()=>(()=>{var e,t,o={618:(e,t,o)=>{var n=o(355)((function(e){return e[1]}));n.push([e.id,\"#live_recommand_report,\\n#live_recommend_report {\\n  display: none !important;\\n}\",\"\"]),e.exports=n},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var o=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(o,\"}\"):o})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,o,n){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var r={};if(n)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[i][0];null!=a&&(r[a]=!0)}for(var c=0;c<e.length;c++){var d=[].concat(e[c]);n&&r[d[0]]||(o&&(d[2]?d[2]=\"\".concat(o,\" and \").concat(d[2]):d[2]=o),t.push(d))}},t}},97:(e,t,o)=>{var n=o(618);n&&n.__esModule&&(n=n.default),e.exports=\"string\"==typeof n?n:n.toString()}},n={};function r(e){var t=n[e];if(void 0!==t)return t.exports;var i=n[e]={id:e,exports:{}};return o[e](i,i.exports,r),i.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,r.t=function(o,n){if(1&n&&(o=this(o)),8&n)return o;if(\"object\"==typeof o&&o){if(4&n&&o.__esModule)return o;if(16&n&&\"function\"==typeof o.then)return o}var i=Object.create(null);r.r(i);var a={};e=e||[null,t({}),t([]),t(t)];for(var c=2&n&&o;\"object\"==typeof c&&!~e.indexOf(c);c=t(c))Object.getOwnPropertyNames(c).forEach((e=>a[e]=()=>o[e]));return a.default=()=>o,r.d(i,a),i},r.d=(e,t)=>{for(var o in t)r.o(t,o)&&!r.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},r.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),r.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";r.d(i,{component:()=>o});const e=coreApis.componentApis.define,t=coreApis.utils.urls,o=(0,e.defineComponentMetadata)({name:\"hideRecommendedLive\",entry:none,instantStyles:[{name:\"hideRecommendedLive\",style:()=>Promise.resolve().then(r.t.bind(r,97,23))}],displayName:\"隐藏直播推荐\",tags:[componentsTags.style,componentsTags.video],description:{\"zh-CN\":\"隐藏视频页面右侧下方的直播推荐.\"},urlInclude:t.videoUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "name": "hideRecommendedLive",
        "displayName": "隐藏直播推荐",
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          },
          {
            "name": "video",
            "displayName": "视频",
            "color": "#2196F3",
            "icon": "mdi-play-circle-outline",
            "order": 1
          }
        ],
        "description": {
          "zh-CN": "隐藏视频页面右侧下方的直播推荐."
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "collapseLiveSideBar": {
      "code": "!function(e,r){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=r():\"function\"==typeof define&&define.amd?define([],r):\"object\"==typeof exports?exports[\"live/side-bar\"]=r():e[\"live/side-bar\"]=r()}(globalThis,(()=>(()=>{var e,r,t={632:(e,r,t)=>{var n=t(355)((function(e){return e[1]}));n.push([e.id,'.side-bar-cntr {\\n  transition: 0.24s ease-out !important;\\n  overflow: visible !important;\\n  transform: translateZ(0) translateX(100%) !important;\\n}\\n.side-bar-cntr:hover {\\n  transform: translateZ(0) !important;\\n}\\n.side-bar-cntr::after {\\n  right: calc(100% + 4px);\\n  transform: translateY(-50%) rotate(45deg);\\n  width: 8px;\\n  height: 8px;\\n  border-radius: 2px;\\n  box-sizing: border-box;\\n  border: 4px solid #aaa;\\n  border-top-color: transparent;\\n  border-right-color: transparent;\\n}\\nbody.dark .side-bar-cntr::after {\\n  border: 4px solid #eee;\\n  border-top-color: transparent;\\n  border-right-color: transparent;\\n}\\n.side-bar-cntr::before {\\n  right: calc(100% - 8px);\\n  transform: translateY(-50%);\\n  width: 32px;\\n  height: 48px;\\n  border-radius: 8px 0 0 8px;\\n  background-color: #fff;\\n  border: 1px solid #e9eaec;\\n}\\nbody.dark .side-bar-cntr::before {\\n  background-color: #222;\\n  border-color: transparent;\\n}\\n.side-bar-cntr::before, .side-bar-cntr::after {\\n  content: \"\";\\n  transition: 0.24s ease-out;\\n  cursor: pointer;\\n  position: fixed;\\n  top: 50%;\\n}\\n.side-bar-cntr:hover::after, .side-bar-cntr:hover::before {\\n  opacity: 0;\\n}',\"\"]),e.exports=n},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var r=[];return r.toString=function(){return this.map((function(r){var t=e(r);return r[2]?\"@media \".concat(r[2],\" {\").concat(t,\"}\"):t})).join(\"\")},\n// eslint-disable-next-line func-names\nr.i=function(e,t,n){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var o={};if(n)for(var a=0;a<this.length;a++){\n// eslint-disable-next-line prefer-destructuring\nvar i=this[a][0];null!=i&&(o[i]=!0)}for(var s=0;s<e.length;s++){var c=[].concat(e[s]);n&&o[c[0]]||(t&&(c[2]?c[2]=\"\".concat(t,\" and \").concat(c[2]):c[2]=t),r.push(c))}},r}},693:(e,r,t)=>{var n=t(632);n&&n.__esModule&&(n=n.default),e.exports=\"string\"==typeof n?n:n.toString()}},n={};function o(e){var r=n[e];if(void 0!==r)return r.exports;var a=n[e]={id:e,exports:{}};return t[e](a,a.exports,o),a.exports}r=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,o.t=function(t,n){if(1&n&&(t=this(t)),8&n)return t;if(\"object\"==typeof t&&t){if(4&n&&t.__esModule)return t;if(16&n&&\"function\"==typeof t.then)return t}var a=Object.create(null);o.r(a);var i={};e=e||[null,r({}),r([]),r(r)];for(var s=2&n&&t;\"object\"==typeof s&&!~e.indexOf(s);s=r(s))Object.getOwnPropertyNames(s).forEach((e=>i[e]=()=>t[e]));return i.default=()=>t,o.d(a,i),a},o.d=(e,r)=>{for(var t in r)o.o(r,t)&&!o.o(e,t)&&Object.defineProperty(e,t,{enumerable:!0,get:r[t]})},o.o=(e,r)=>Object.prototype.hasOwnProperty.call(e,r),o.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var a={};return(()=>{\"use strict\";o.d(a,{component:()=>t});const e=coreApis.componentApis.define,r=coreApis.utils.urls,t=(0,e.defineComponentMetadata)({name:\"collapseLiveSideBar\",entry:none,instantStyles:[{name:\"collapseLiveSideBar\",style:()=>Promise.resolve().then(o.t.bind(o,693,23))}],displayName:\"自动收起直播侧栏\",description:'自动收起直播间右边偏下的侧栏. (上面有个 \"关注\" 的面板)',tags:[componentsTags.live,componentsTags.style],urlInclude:r.liveUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),a=a.component})()));",
      "metadata": {
        "name": "collapseLiveSideBar",
        "displayName": "自动收起直播侧栏",
        "description": "自动收起直播间右边偏下的侧栏. (上面有个 \"关注\" 的面板)",
        "tags": [
          {
            "name": "live",
            "displayName": "直播",
            "color": "#26A69A",
            "icon": "mdi-video-wireless-outline",
            "order": 4
          },
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "hideRelatedVideos": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"style/hide/video/related-videos\"]=t():e[\"style/hide/video/related-videos\"]=t()}(globalThis,(()=>(()=>{var e,t,n={625:(e,t,n)=>{var o=n(355)((function(e){return e[1]}));o.push([e.id,\"#recom_module,\\n#reco_list,\\n.bilibili-player-ending-panel-box-videos,\\n.r-con .rcmd-list {\\n  display: none !important;\\n}\\n\\n.bilibili-player-ending-panel-box-functions .bilibili-player-upinfo-spans {\\n  position: static !important;\\n}\\n\\n.bilibili-player-ending-panel-box {\\n  display: flex !important;\\n  justify-content: center !important;\\n  flex-direction: column !important;\\n}\",\"\"]),e.exports=o},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var n=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(n,\"}\"):n})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,n,o){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var r={};if(o)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[i][0];null!=a&&(r[a]=!0)}for(var s=0;s<e.length;s++){var l=[].concat(e[s]);o&&r[l[0]]||(n&&(l[2]?l[2]=\"\".concat(n,\" and \").concat(l[2]):l[2]=n),t.push(l))}},t}},196:(e,t,n)=>{var o=n(625);o&&o.__esModule&&(o=o.default),e.exports=\"string\"==typeof o?o:o.toString()}},o={};function r(e){var t=o[e];if(void 0!==t)return t.exports;var i=o[e]={id:e,exports:{}};return n[e](i,i.exports,r),i.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,r.t=function(n,o){if(1&o&&(n=this(n)),8&o)return n;if(\"object\"==typeof n&&n){if(4&o&&n.__esModule)return n;if(16&o&&\"function\"==typeof n.then)return n}var i=Object.create(null);r.r(i);var a={};e=e||[null,t({}),t([]),t(t)];for(var s=2&o&&n;\"object\"==typeof s&&!~e.indexOf(s);s=t(s))Object.getOwnPropertyNames(s).forEach((e=>a[e]=()=>n[e]));return a.default=()=>n,r.d(i,a),i},r.d=(e,t)=>{for(var n in t)r.o(t,n)&&!r.o(e,n)&&Object.defineProperty(e,n,{enumerable:!0,get:t[n]})},r.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),r.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";r.d(i,{component:()=>n});const e=coreApis.componentApis.define,t=coreApis.utils.urls,n=(0,e.defineComponentMetadata)({name:\"hideRelatedVideos\",displayName:\"隐藏视频推荐\",entry:none,instantStyles:[{name:\"hideRelatedVideos\",style:()=>Promise.resolve().then(r.t.bind(r,196,23))}],tags:[componentsTags.style,componentsTags.video],description:{\"zh-CN\":\"隐藏番剧和视频页面右侧的推荐视频列表. 注意: 如果你想关闭 b 站的自动连播 (自动播放下一个推荐视频) 功能, 需要先取消隐藏视频推荐才能看到开关.\"},urlInclude:t.videoAndBangumiUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "name": "hideRelatedVideos",
        "displayName": "隐藏视频推荐",
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          },
          {
            "name": "video",
            "displayName": "视频",
            "color": "#2196F3",
            "icon": "mdi-play-circle-outline",
            "order": 1
          }
        ],
        "description": {
          "zh-CN": "隐藏番剧和视频页面右侧的推荐视频列表. 注意: 如果你想关闭 b 站的自动连播 (自动播放下一个推荐视频) 功能, 需要先取消隐藏视频推荐才能看到开关."
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "hideVideoTopMask": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"style/hide/video/top-mask\"]=t():e[\"style/hide/video/top-mask\"]=t()}(globalThis,(()=>(()=>{var e,t,o={449:(e,t,o)=>{var r=o(355)((function(e){return e[1]}));r.push([e.id,\".bpx-player-top-wrap,\\n.bilibili-player-video-top {\\n  display: none !important;\\n}\",\"\"]),e.exports=r},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var o=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(o,\"}\"):o})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,o,r){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var n={};if(r)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[i][0];null!=a&&(n[a]=!0)}for(var p=0;p<e.length;p++){var s=[].concat(e[p]);r&&n[s[0]]||(o&&(s[2]?s[2]=\"\".concat(o,\" and \").concat(s[2]):s[2]=o),t.push(s))}},t}},51:(e,t,o)=>{var r=o(449);r&&r.__esModule&&(r=r.default),e.exports=\"string\"==typeof r?r:r.toString()}},r={};function n(e){var t=r[e];if(void 0!==t)return t.exports;var i=r[e]={id:e,exports:{}};return o[e](i,i.exports,n),i.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,n.t=function(o,r){if(1&r&&(o=this(o)),8&r)return o;if(\"object\"==typeof o&&o){if(4&r&&o.__esModule)return o;if(16&r&&\"function\"==typeof o.then)return o}var i=Object.create(null);n.r(i);var a={};e=e||[null,t({}),t([]),t(t)];for(var p=2&r&&o;\"object\"==typeof p&&!~e.indexOf(p);p=t(p))Object.getOwnPropertyNames(p).forEach((e=>a[e]=()=>o[e]));return a.default=()=>o,n.d(i,a),i},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";n.d(i,{component:()=>r});const e=coreApis.componentApis.define,t=coreApis.utils.urls,o=\"hideVideoTopMask\",r=(0,e.defineComponentMetadata)({name:o,displayName:\"隐藏视频标题层\",entry:none,instantStyles:[{name:o,style:()=>Promise.resolve().then(n.t.bind(n,51,23))}],tags:[componentsTags.style],description:{\"zh-CN\":\"隐藏视频里鼠标经过时出现在右上角的覆盖层.\"},urlInclude:t.playerUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "name": "hideVideoTopMask",
        "displayName": "隐藏视频标题层",
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "description": {
          "zh-CN": "隐藏视频里鼠标经过时出现在右上角的覆盖层."
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "disableSpecialDanmaku": {
      "code": "!function(t,e){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=e():\"function\"==typeof define&&define.amd?define([],e):\"object\"==typeof exports?exports[\"style/special-danmaku\"]=e():t[\"style/special-danmaku\"]=e()}(globalThis,(()=>(()=>{var t,e,n={667:(t,e,n)=>{var o=n(355)((function(t){return t[1]}));o.push([t.id,\"body.disable-highlight-danmaku-style .b-danmaku-high {\\n  display: block !important;\\n  padding: 0 !important;\\n  line-height: 1.125 !important;\\n}\\nbody.disable-highlight-danmaku-style .b-danmaku-high .b-danmaku-high-icon {\\n  display: none !important;\\n}\\nbody.disable-highlight-danmaku-style .b-danmaku-high .b-danmaku-high-text {\\n  margin: 0 !important;\\n  text-shadow: inherit;\\n}\\n\\nbody.disable-up-danmaku-style .b-danmaku-up {\\n  padding: 0 !important;\\n  line-height: 1.125 !important;\\n  background-color: transparent !important;\\n  border-radius: 0 !important;\\n}\\nbody.disable-up-danmaku-style .b-danmaku-up .b-danmaku-up-tip {\\n  display: none !important;\\n}\",\"\"]),t.exports=o},355:t=>{\"use strict\";\n// eslint-disable-next-line func-names\nt.exports=function(t){var e=[];return e.toString=function(){return this.map((function(e){var n=t(e);return e[2]?\"@media \".concat(e[2],\" {\").concat(n,\"}\"):n})).join(\"\")},\n// eslint-disable-next-line func-names\ne.i=function(t,n,o){\"string\"==typeof t&&(\n// eslint-disable-next-line no-param-reassign\nt=[[null,t,\"\"]]);var a={};if(o)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar r=this[i][0];null!=r&&(a[r]=!0)}for(var d=0;d<t.length;d++){var s=[].concat(t[d]);o&&a[s[0]]||(n&&(s[2]?s[2]=\"\".concat(n,\" and \").concat(s[2]):s[2]=n),e.push(s))}},e}},383:(t,e,n)=>{var o=n(667);o&&o.__esModule&&(o=o.default),t.exports=\"string\"==typeof o?o:o.toString()}},o={};function a(t){var e=o[t];if(void 0!==e)return e.exports;var i=o[t]={id:t,exports:{}};return n[t](i,i.exports,a),i.exports}e=Object.getPrototypeOf?t=>Object.getPrototypeOf(t):t=>t.__proto__,a.t=function(n,o){if(1&o&&(n=this(n)),8&o)return n;if(\"object\"==typeof n&&n){if(4&o&&n.__esModule)return n;if(16&o&&\"function\"==typeof n.then)return n}var i=Object.create(null);a.r(i);var r={};t=t||[null,e({}),e([]),e(e)];for(var d=2&o&&n;\"object\"==typeof d&&!~t.indexOf(d);d=e(d))Object.getOwnPropertyNames(d).forEach((t=>r[t]=()=>n[t]));return r.default=()=>n,a.d(i,r),i},a.d=(t,e)=>{for(var n in e)a.o(e,n)&&!a.o(t,n)&&Object.defineProperty(t,n,{enumerable:!0,get:e[n]})},a.o=(t,e)=>Object.prototype.hasOwnProperty.call(t,e),a.r=t=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(t,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(t,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";a.d(i,{component:()=>d});const t=coreApis.componentApis.define,e=coreApis.componentApis.styledComponent,n=coreApis.utils.urls,o=coreApis.settings,r=(0,t.defineOptionsMetadata)({highlight:{displayName:\"禁用高赞弹幕\",defaultValue:!0},up:{displayName:\"禁用UP主弹幕\",defaultValue:!0}}),d=(0,t.defineComponentMetadata)({displayName:\"禁用特殊弹幕样式\",tags:[componentsTags.style],...(0,e.toggleStyle)(\"disableSpecialDanmaku\",(()=>Promise.resolve().then(a.t.bind(a,383,23))),(t=>{let{metadata:e,settings:n}=t;Object.keys(n.options).forEach((t=>{(0,o.addComponentListener)(`${e.name}.${t}`,(e=>{document.body.classList.toggle(`disable-${t}-danmaku-style`,e)}),!0)}))})),urlInclude:n.playerUrls,description:{\"zh-CN\":\"移除高赞弹幕或 UP 主弹幕的特殊样式, 弹幕内容不会移除.\"},options:r,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "displayName": "禁用特殊弹幕样式",
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "name": "disableSpecialDanmaku",
        "description": {
          "zh-CN": "移除高赞弹幕或 UP 主弹幕的特殊样式, 弹幕内容不会移除."
        },
        "options": {
          "highlight": {
            "displayName": "禁用高赞弹幕",
            "defaultValue": true
          },
          "up": {
            "displayName": "禁用UP主弹幕",
            "defaultValue": true
          }
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {
          "highlight": true,
          "up": true
        }
      }
    },
    "removePlayerPopup": {
      "code": "!function(e,o){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=o():\"function\"==typeof define&&define.amd?define([],o):\"object\"==typeof exports?exports[\"video/player/remove-popup\"]=o():e[\"video/player/remove-popup\"]=o()}(globalThis,(()=>(()=>{var e,o,p={513:(e,o,p)=>{var r=p(355)((function(e){return e[1]}));r.push([e.id,\"body.remove-player-popup-combo-likes .bilibili-player-video-popup-three,\\nbody.remove-player-popup-combo-likes .bilibili-player-video-popup-three-animate,\\nbody.remove-player-popup-combo-likes .bilibili-player-video-popup-follow,\\nbody.remove-player-popup-combo-likes .bilibili-player-video-popup-there-cyc,\\nbody.remove-player-popup-combo-likes .bpx-player-popup-three,\\nbody.remove-player-popup-combo-likes .bpx-player-popup-animate,\\nbody.remove-player-popup-combo-likes .bpx-player-popup-follow,\\nbody.remove-player-popup-combo-likes .bpx-player-popup-cyc {\\n  display: none !important;\\n}\\nbody.remove-player-popup-related-videos .bilibili-player-video-link,\\nbody.remove-player-popup-related-videos .bilibili-player-link,\\nbody.remove-player-popup-related-videos .bpx-player-link {\\n  display: none !important;\\n}\\nbody.remove-player-popup-votes .bilibili-player-video-popup-vote,\\nbody.remove-player-popup-votes .bpx-player-popup-dm-close,\\nbody.remove-player-popup-votes .bpx-player-popup-dm-shrink,\\nbody.remove-player-popup-votes .bpx-player-popup-vote {\\n  display: none !important;\\n}\\nbody.remove-player-popup-rates .bilibili-player-score,\\nbody.remove-player-popup-rates .bpx-player-popup-dm-close,\\nbody.remove-player-popup-rates .bpx-player-score-summary-wrap,\\nbody.remove-player-popup-rates .bpx-player-score {\\n  display: none !important;\\n}\\nbody.remove-player-popup-reservations .bpx-player-reserve {\\n  display: none !important;\\n}\",\"\"]),e.exports=r},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var o=[];return o.toString=function(){return this.map((function(o){var p=e(o);return o[2]?\"@media \".concat(o[2],\" {\").concat(p,\"}\"):p})).join(\"\")},\n// eslint-disable-next-line func-names\no.i=function(e,p,r){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var t={};if(r)for(var a=0;a<this.length;a++){\n// eslint-disable-next-line prefer-destructuring\nvar n=this[a][0];null!=n&&(t[n]=!0)}for(var l=0;l<e.length;l++){var i=[].concat(e[l]);r&&t[i[0]]||(p&&(i[2]?i[2]=\"\".concat(p,\" and \").concat(i[2]):i[2]=p),o.push(i))}},o}},315:(e,o,p)=>{var r=p(513);r&&r.__esModule&&(r=r.default),e.exports=\"string\"==typeof r?r:r.toString()}},r={};function t(e){var o=r[e];if(void 0!==o)return o.exports;var a=r[e]={id:e,exports:{}};return p[e](a,a.exports,t),a.exports}o=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,t.t=function(p,r){if(1&r&&(p=this(p)),8&r)return p;if(\"object\"==typeof p&&p){if(4&r&&p.__esModule)return p;if(16&r&&\"function\"==typeof p.then)return p}var a=Object.create(null);t.r(a);var n={};e=e||[null,o({}),o([]),o(o)];for(var l=2&r&&p;\"object\"==typeof l&&!~e.indexOf(l);l=o(l))Object.getOwnPropertyNames(l).forEach((e=>n[e]=()=>p[e]));return n.default=()=>p,t.d(a,n),a},t.d=(e,o)=>{for(var p in o)t.o(o,p)&&!t.o(e,p)&&Object.defineProperty(e,p,{enumerable:!0,get:o[p]})},t.o=(e,o)=>Object.prototype.hasOwnProperty.call(e,o),t.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var a={};return(()=>{\"use strict\";t.d(a,{component:()=>n});const e=coreApis.componentApis.define,o=coreApis.settings,p=coreApis.utils.urls,r=\"removePlayerPopup\",n=(0,e.defineComponentMetadata)({name:r,entry:e=>{let{settings:p,metadata:r}=e;const{options:t}=p,{kebabCase:a}=lodash;Object.keys(t).forEach((e=>{(0,o.addComponentListener)(`${r.name}.${e}`,(o=>{document.body.classList.toggle(`${a(r.name)}-${a(e)}`,o)}),!0)}))},instantStyles:[{name:r,style:()=>Promise.resolve().then(t.t.bind(t,315,23))}],displayName:\"删除视频弹窗\",tags:[componentsTags.video,componentsTags.style],description:{\"zh-CN\":\"删除视频播放器中出现的各种弹窗, 类别可在选项中分别选择.\"},urlInclude:p.playerUrls,options:{votes:{defaultValue:!1,displayName:\"投票\"},relatedVideos:{defaultValue:!0,displayName:\"关联视频\"},comboLikes:{defaultValue:!0,displayName:\"关注/三连\"},rates:{defaultValue:!0,displayName:\"评分\"},reservations:{defaultValue:!0,displayName:\"预告\"}},commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),a=a.component})()));",
      "metadata": {
        "name": "removePlayerPopup",
        "displayName": "删除视频弹窗",
        "tags": [
          {
            "name": "video",
            "displayName": "视频",
            "color": "#2196F3",
            "icon": "mdi-play-circle-outline",
            "order": 1
          },
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "description": {
          "zh-CN": "删除视频播放器中出现的各种弹窗, 类别可在选项中分别选择."
        },
        "options": {
          "votes": {
            "defaultValue": false,
            "displayName": "投票"
          },
          "relatedVideos": {
            "defaultValue": true,
            "displayName": "关联视频"
          },
          "comboLikes": {
            "defaultValue": true,
            "displayName": "关注/三连"
          },
          "rates": {
            "defaultValue": true,
            "displayName": "评分"
          },
          "reservations": {
            "defaultValue": true,
            "displayName": "预告"
          }
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {
          "votes": false,
          "relatedVideos": true,
          "comboLikes": true,
          "rates": true,
          "reservations": true
        }
      }
    },
    "removePromotions": {
      "code": "!function(e,n){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=n():\"function\"==typeof define&&define.amd?define([],n):\"object\"==typeof exports?exports[\"utils/remove-promotions\"]=n():e[\"utils/remove-promotions\"]=n()}(globalThis,(()=>(()=>{var e,n,t={991:(e,n,t)=>{var o=t(355)((function(e){return e[1]}));o.push([e.id,\"#slide_ad,\\n.v-wrap .vcd,\\n.ad-report,\\n#home_popularize .l-con,\\n#home_popularize .adpos,\\n.gg-floor-module,\\n.home-app-download,\\n.bilibili-player-promote-wrap,\\n.bili-header-m .nav-menu .nav-con .nav-item .text-red,\\n.mobile-link-l,\\n.video-page-game-card,\\n.international-home .banner-card,\\n.bypb-window .operate-card,\\n.gg-window .operate-card,\\n#reportFirst2 .extension,\\n.video-page-special-card,\\n.mascot,\\n.rank-container .cm-module,\\nbody:not(.preserve-event-banner) .activity-m,\\nbody.remove-game-match-module .bili-wrapper > .home-match,\\nbody.remove-game-match-module #reportFirst3,\\n.home-content .ad-panel,\\n.recommend-list .rec-list > :not(.video-page-card),\\n.eva-extension-area,\\n.eva-banner,\\n.video-ad-creative-card,\\n.bili-dyn-home--member .bili-dyn-ads,\\n.video-page-special-card-small,\\n.video-page-game-card-small,\\n.video-page-operator-card-small,\\n[data-be-promotion-mark] {\\n  display: none !important;\\n}\\n\\n.recommend-list .rec-list > :not(.video-page-card) + .video-page-card {\\n  padding-top: 0 !important;\\n}\\n\\n#home_popularize {\\n  position: relative !important;\\n}\\n\\n.popularize-module .online,\\n.gg-window .online {\\n  position: absolute !important;\\n  top: 50% !important;\\n  right: 0.5% !important;\\n  transform: translateY(-100%) !important;\\n}\\n\\n.gg-window .online {\\n  right: 0 !important;\\n  padding: 0 16px !important;\\n}\\n\\n#reportFirst2 {\\n  position: relative;\\n  margin-bottom: 4px;\\n}\\n\\n.blocked-ads {\\n  width: 440px;\\n  height: 220px;\\n  display: flex;\\n  color: #888;\\n  background-color: rgba(136, 136, 136, 0.1333333333);\\n  font-size: 24pt;\\n  font-weight: bold;\\n  align-items: center;\\n  justify-content: space-evenly;\\n}\\n\\n.blocked-ads.new {\\n  width: 100%;\\n  height: 100%;\\n  background-color: #eee;\\n}\\n\\nbody.dark .blocked-ads.new {\\n  background-color: #333;\\n}\\n\\n.recommended-container .business-card {\\n  position: absolute !important;\\n  pointer-events: none !important;\\n  opacity: 0 !important;\\n}\",\"\"]),e.exports=o},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?\"@media \".concat(n[2],\" {\").concat(t,\"}\"):t})).join(\"\")},\n// eslint-disable-next-line func-names\nn.i=function(e,t,o){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var r={};if(o)for(var a=0;a<this.length;a++){\n// eslint-disable-next-line prefer-destructuring\nvar i=this[a][0];null!=i&&(r[i]=!0)}for(var s=0;s<e.length;s++){var l=[].concat(e[s]);o&&r[l[0]]||(t&&(l[2]?l[2]=\"\".concat(t,\" and \").concat(l[2]):l[2]=t),n.push(l))}},n}},53:(e,n,t)=>{var o=t(991);o&&o.__esModule&&(o=o.default),e.exports=\"string\"==typeof o?o:o.toString()},986:e=>{\"use strict\";e.exports=coreApis.settings},200:e=>{\"use strict\";e.exports=coreApis.spinQuery}},o={};function r(e){var n=o[e];if(void 0!==n)return n.exports;var a=o[e]={id:e,exports:{}};return t[e](a,a.exports,r),a.exports}n=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,r.t=function(t,o){if(1&o&&(t=this(t)),8&o)return t;if(\"object\"==typeof t&&t){if(4&o&&t.__esModule)return t;if(16&o&&\"function\"==typeof t.then)return t}var a=Object.create(null);r.r(a);var i={};e=e||[null,n({}),n([]),n(n)];for(var s=2&o&&t;\"object\"==typeof s&&!~e.indexOf(s);s=n(s))Object.getOwnPropertyNames(s).forEach((e=>i[e]=()=>t[e]));return i.default=()=>t,r.d(a,i),a},r.d=(e,n)=>{for(var t in n)r.o(n,t)&&!r.o(e,t)&&Object.defineProperty(e,t,{enumerable:!0,get:n[t]})},r.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),r.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var a={};return(()=>{\"use strict\";r.d(a,{component:()=>e});const e=(0,coreApis.componentApis.define.defineComponentMetadata)({name:\"removePromotions\",displayName:\"删除广告\",entry:async e=>{let{settings:n,metadata:t}=e;const{addComponentListener:o}=await Promise.resolve().then(r.t.bind(r,986,23));if(\"https://www.bilibili.com/\"===document.URL.replace(window.location.search,\"\")){const{selectAll:e,select:t}=await Promise.resolve().then(r.t.bind(r,200,23));t(\".eva-extension-area\").then((e=>{e&&(e.parentElement.style.margin=\"12px\")})),e(\".gg-pic\").then((e=>{0!==e.length&&e.forEach((e=>{const t=e.parentElement;t.style.display=\"none\";const o=[...t.parentElement.childNodes].indexOf(t)+1,r=t.parentElement.parentElement.querySelector(`.pic li:nth-child(${o})`);if(r){r.style.display=\"flex\";const e=r.querySelector(\"a:not(.more-text)\");e.insertAdjacentHTML(\"afterend\",`\\n            <div class=\"blocked-ads\">${n.options.showPlaceholder?\"🚫已屏蔽广告\":\"\"}</div>\\n          `),e.style.visibility=\"hidden\";[r.querySelector(\"a.more-text\"),r.querySelector(\"img\")].forEach((e=>e.style.display=\"none\"))}}))})),t(\".focus-carousel.home-slide\").then((e=>{e&&dqa(e,\".gg-icon,.bypb-icon\").map((e=>e.parentElement.parentElement)).forEach((e=>{e.style.display=\"none\",e.insertAdjacentHTML(\"afterend\",`\\n            <div class=\"blocked-ads new\">${n.options.showPlaceholder?\"🚫已屏蔽广告\":\"\"}</div>\\n          `)}))}))}o(`${t.name}.preserveEventBanner`,(e=>{document.body.classList.toggle(\"preserve-event-banner\",e)}),!0)},instantStyles:[{name:\"removePromotions\",style:()=>Promise.resolve().then(r.t.bind(r,53,23))}],tags:[componentsTags.utils],description:{\"zh-CN\":'\\n删除站内的各种广告. 包括首页的推广模块, 手机 app 推荐, 视频页面右侧的广告等. 注意: 首页推广模块删除后留下空白区域是正常现象, 如果觉得怪可以开启 `占位文本` 选项.\\n\\n- `占位文本`: 删除首页推广模块的广告后显示\"🚫已屏蔽广告\"来替代空白区域.\\n- `保留活动横幅`: 保留视频页面的活动横幅.\\n'.trim()},options:{showPlaceholder:{displayName:\"占位文本\",defaultValue:!0},preserveEventBanner:{displayName:\"保留活动横幅\",defaultValue:!1}},commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),a=a.component})()));",
      "metadata": {
        "name": "removePromotions",
        "displayName": "删除广告",
        "tags": [
          {
            "name": "utils",
            "displayName": "工具",
            "color": "#A36FFD",
            "icon": "mdi-rocket-launch-outline",
            "order": 5
          }
        ],
        "description": {
          "zh-CN": "删除站内的各种广告. 包括首页的推广模块, 手机 app 推荐, 视频页面右侧的广告等. 注意: 首页推广模块删除后留下空白区域是正常现象, 如果觉得怪可以开启 `占位文本` 选项.\n\n- `占位文本`: 删除首页推广模块的广告后显示\"🚫已屏蔽广告\"来替代空白区域.\n- `保留活动横幅`: 保留视频页面的活动横幅."
        },
        "options": {
          "showPlaceholder": {
            "displayName": "占位文本",
            "defaultValue": true
          },
          "preserveEventBanner": {
            "displayName": "保留活动横幅",
            "defaultValue": false
          }
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {
          "showPlaceholder": true,
          "preserveEventBanner": false
        }
      }
    },
    "simplifyComments": {
      "code": "!function(n,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"style/simplify/comments\"]=t():n[\"style/simplify/comments\"]=t()}(globalThis,(()=>(()=>{var n,t,e={354:(n,t,e)=>{var o=e(355)((function(n){return n[1]}));o.push([n.id,'@charset \"UTF-8\";\\n.bb-comment .comment-send-lite {\\n  position: sticky !important;\\n  bottom: 0 !important;\\n  background: linear-gradient(to top, #fff, rgba(255, 255, 255, 0)) !important;\\n  pointer-events: none;\\n  width: calc(100% + 12px) !important;\\n  margin: 0 0 0 -12px !important;\\n  padding-left: 97px !important;\\n}\\nbody.dark .bb-comment .comment-send-lite {\\n  background: linear-gradient(to top, #222, rgba(255, 255, 255, 0)) !important;\\n}\\n.bb-comment .comment-send-lite .comment-emoji-lite {\\n  background-color: #fff;\\n}\\n.bb-comment .comment-send-lite .comment-submit {\\n  height: 64px !important;\\n  padding: 4px 15px !important;\\n  position: relative !important;\\n  right: 0 !important;\\n  margin-left: 10px !important;\\n}\\n.bb-comment .comment-send-lite .textarea-container .baffle {\\n  line-height: 65px !important;\\n}\\n.bb-comment .comment-send-lite .textarea-container .baffle,\\n.bb-comment .comment-send-lite .textarea-container .ipt-txt {\\n  height: 65px !important;\\n  width: calc(100% - 80px) !important;\\n}\\n.bb-comment .comment-send-lite > * {\\n  pointer-events: initial;\\n}\\n.bb-comment .loading-state {\\n  font-size: 14px !important;\\n  height: 1.4em !important;\\n  line-height: 1.4 !important;\\n  margin: 12px 0 !important;\\n}\\n.bb-comment .loading-state + .bottom-page {\\n  margin: 0 !important;\\n}\\n.bb-comment .nameplate,\\n.bb-comment .comment-header .tabs-order li.on::after,\\n.bb-comment .true-love,\\n.bb-comment .medal,\\n.bb-comment .medal-level,\\n.bb-comment .reply-notice,\\n.bb-comment .sailing,\\n.bb-comment .perfect-reply {\\n  display: none !important;\\n}\\n.bb-comment .comment-send-lite .comment-emoji,\\n.bb-comment .comment-send .comment-emoji {\\n  box-shadow: none !important;\\n}\\n.bb-comment .comment-send-lite .comment-emoji span,\\n.bb-comment .comment-send .comment-emoji span {\\n  opacity: 0.4;\\n  color: black;\\n}\\n.bb-comment .comment-send-lite .comment-emoji .face,\\n.bb-comment .comment-send .comment-emoji .face {\\n  transition: all 0.2s ease-out;\\n  height: 16px !important;\\n  width: 16px !important;\\n  background-position: center !important;\\n  opacity: 0.4;\\n  display: inline-flex !important;\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-send-lite .comment-emoji .face,\\nbody.dark .bb-comment .comment-send .comment-emoji .face {\\n  color: #eee;\\n}\\n.bb-comment .comment-send-lite .comment-emoji .face::before,\\n.bb-comment .comment-send .comment-emoji .face::before {\\n  content: \"\\\\f01f5\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.bb-comment .comment-send-lite .comment-emoji .text,\\n.bb-comment .comment-send .comment-emoji .text {\\n  transition: all 0.2s ease-out;\\n}\\nbody.dark .bb-comment .comment-send-lite .comment-emoji .text,\\nbody.dark .bb-comment .comment-send .comment-emoji .text {\\n  filter: brightness(0) invert(1) !important;\\n}\\n.bb-comment .comment-send-lite .comment-emoji.open span,\\n.bb-comment .comment-send-lite .comment-emoji.open .face, .bb-comment .comment-send-lite .comment-emoji:hover span,\\n.bb-comment .comment-send-lite .comment-emoji:hover .face,\\n.bb-comment .comment-send .comment-emoji.open span,\\n.bb-comment .comment-send .comment-emoji.open .face,\\n.bb-comment .comment-send .comment-emoji:hover span,\\n.bb-comment .comment-send .comment-emoji:hover .face {\\n  opacity: 1;\\n}\\n.bb-comment .comment-list .list-item {\\n  position: relative;\\n}\\n.bb-comment .comment-list .list-item .info {\\n  margin-top: 0 !important;\\n  display: flex;\\n  align-items: center;\\n}\\n.bb-comment .comment-list .list-item .info .floor {\\n  opacity: 0.7;\\n  order: 1;\\n}\\n.bb-comment .comment-list .list-item .info .reply {\\n  order: 2;\\n}\\n.bb-comment .comment-list .list-item .info .reply-tags {\\n  order: 3;\\n  display: flex !important;\\n  margin: 0 !important;\\n}\\n.bb-comment .comment-list .list-item .info .reply-tags span {\\n  margin: 0 4px 0 0 !important;\\n  font-size: 12px !important;\\n  line-height: normal !important;\\n  display: flex !important;\\n  height: auto !important;\\n  padding: 2px 6px !important;\\n}\\n.bb-comment .comment-list .list-item .info .operation {\\n  order: 4;\\n  flex-grow: 1;\\n  display: flex !important;\\n  justify-content: flex-end;\\n  margin: 0 !important;\\n  padding: 3px !important;\\n}\\n.bb-comment .comment-list .list-item .info > * {\\n  display: flex;\\n  align-items: center;\\n  gap: 0;\\n}\\n.bb-comment .comment-list .list-item .info .like i,\\n.bb-comment .comment-list .list-item .info .hate i {\\n  transition: all 0.2s ease-out;\\n  height: 16px !important;\\n  width: 16px !important;\\n  background-position: center !important;\\n  opacity: 0.4;\\n  display: inline-flex !important;\\n}\\n.bb-comment .comment-list .list-item .info .like span,\\n.bb-comment .comment-list .list-item .info .hate span {\\n  opacity: 0.4;\\n  transition: all 0.2s ease-out;\\n  color: black;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .like span,\\nbody.dark .bb-comment .comment-list .list-item .info .hate span {\\n  color: #eee !important;\\n}\\n.bb-comment .comment-list .list-item .info .like.liked > *, .bb-comment .comment-list .list-item .info .like.hated > *, .bb-comment .comment-list .list-item .info .like:hover > *,\\n.bb-comment .comment-list .list-item .info .hate.liked > *,\\n.bb-comment .comment-list .list-item .info .hate.hated > *,\\n.bb-comment .comment-list .list-item .info .hate:hover > * {\\n  opacity: 1;\\n}\\n.bb-comment .comment-list .list-item .info .like i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .like i {\\n  color: #eee;\\n}\\n.bb-comment .comment-list .list-item .info .like i::before {\\n  content: \"\\\\f0514\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.bb-comment .comment-list .list-item .info .like.liked i, .bb-comment .comment-list .list-item .info .like.liked:hover i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .like.liked i, body.dark .bb-comment .comment-list .list-item .info .like.liked:hover i {\\n  color: #eee;\\n}\\n.bb-comment .comment-list .list-item .info .like.liked i::before, .bb-comment .comment-list .list-item .info .like.liked:hover i::before {\\n  content: \"\\\\f0513\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.bb-comment .comment-list .list-item .info .like.liked i, .bb-comment .comment-list .list-item .info .like.liked i + span, body.dark .bb-comment .comment-list .list-item .info .like.liked i, .bb-comment .comment-list .list-item .info .like.liked:hover i, .bb-comment .comment-list .list-item .info .like.liked:hover i + span, body.dark .bb-comment .comment-list .list-item .info .like.liked:hover i {\\n  color: var(--theme-color) !important;\\n}\\n.bb-comment .comment-list .list-item .info .hate i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .hate i {\\n  color: #eee;\\n}\\n.bb-comment .comment-list .list-item .info .hate i::before {\\n  content: \"\\\\f0512\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.bb-comment .comment-list .list-item .info .hate.hated i, .bb-comment .comment-list .list-item .info .hate.hated:hover i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .hate.hated i, body.dark .bb-comment .comment-list .list-item .info .hate.hated:hover i {\\n  color: #eee;\\n}\\n.bb-comment .comment-list .list-item .info .hate.hated i::before, .bb-comment .comment-list .list-item .info .hate.hated:hover i::before {\\n  content: \"\\\\f0511\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.bb-comment .comment-list .list-item .info .hate.hated i, .bb-comment .comment-list .list-item .info .hate.hated i + span, body.dark .bb-comment .comment-list .list-item .info .hate.hated i, .bb-comment .comment-list .list-item .info .hate.hated:hover i, .bb-comment .comment-list .list-item .info .hate.hated:hover i + span, body.dark .bb-comment .comment-list .list-item .info .hate.hated:hover i {\\n  color: var(--theme-color) !important;\\n}\\n.bb-comment .comment-list .list-item .info .operation:hover {\\n  background: transparent !important;\\n}\\n.bb-comment .comment-list .list-item .info .operation .spot {\\n  transition: all 0.2s ease-out;\\n  height: 16px !important;\\n  width: 16px !important;\\n  background-position: center !important;\\n  opacity: 0.4;\\n  display: inline-flex !important;\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .operation .spot {\\n  color: #eee;\\n}\\n.bb-comment .comment-list .list-item .info .operation .spot::before {\\n  content: \"\\\\f01d9\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\nbody.dark .bb-comment .comment-list .list-item .info .operation .spot {\\n  filter: brightness(0) invert(1) !important;\\n}\\n.bb-comment .comment-list .list-item .info .operation .spot:hover {\\n  opacity: 1;\\n}\\n.bb-comment .comment-list .list-item .text {\\n  white-space: pre-wrap;\\n}\\n.bb-comment .comment-list .list-item .user {\\n  margin-right: 120px;\\n}\\n.bb-comment .comment-list .list-item .user .level {\\n  visibility: hidden;\\n  width: 0;\\n  margin: 0;\\n}\\n.bb-comment .comment-list .list-item .user .text-con {\\n  white-space: pre-wrap;\\n  display: block;\\n  margin: 0 !important;\\n}\\n.bb-comment .comment-list .list-item .user-face .hot-follow,\\n.bb-comment .comment-list .list-item .con .vote-container {\\n  display: none !important;\\n}\\n.bb-comment .comment-list .list-item > .con .level-link {\\n  display: none !important;\\n}\\n.bb-comment .comment-list .list-item > .con > .reply-box {\\n  transform: translateX(0%);\\n}\\n.bb-comment .comment-list .list-item > .con > .info {\\n  margin-top: 4px;\\n}\\n.bb-comment .comment-list .list-item > .con > .info > .time-location,\\n.bb-comment .comment-list .list-item > .con > .info > .time {\\n  position: absolute;\\n  right: 8px;\\n  top: 24px;\\n  margin: 0 !important;\\n  line-height: normal;\\n  color: black;\\n}\\nbody.dark .bb-comment .comment-list .list-item > .con > .info > .time-location,\\nbody.dark .bb-comment .comment-list .list-item > .con > .info > .time,\\nbody.dark .bb-comment .comment-list .list-item > .con > .info > .floor {\\n  filter: brightness(0) invert(1) !important;\\n}\\n.bb-comment .comment-list .list-item > .con > .info > .plad {\\n  display: none !important;\\n}\\n.bb-comment .comment-list .reply-con {\\n  position: relative;\\n}\\n.bb-comment .comment-list .reply-con > .info > .time-location,\\n.bb-comment .comment-list .reply-con > .info > .time {\\n  position: absolute;\\n  right: 8px;\\n  top: 0px;\\n  margin: 0;\\n  opacity: 0.5;\\n  line-height: normal;\\n  color: black;\\n}\\nbody.dark .bb-comment .comment-list .reply-con > .info > .time-location,\\nbody.dark .bb-comment .comment-list .reply-con > .info > .time {\\n  filter: brightness(0) invert(1) !important;\\n}\\n.bb-comment .reply-item {\\n  position: relative;\\n}\\nbody.dark .bb-comment .reply-item > .info > .time {\\n  filter: brightness(0) invert(1) !important;\\n}\\n.bb-comment .reply-notice .notice-item {\\n  background-color: rgba(0, 0, 0, 0.0666666667) !important;\\n  border: none !important;\\n  display: flex !important;\\n  align-items: center;\\n  padding: 10px 14px !important;\\n}\\nbody.dark .bb-comment .reply-notice .notice-item {\\n  background-color: #333 !important;\\n}\\n.bb-comment .reply-notice .notice-item .icon-notice {\\n  order: 0;\\n  position: static !important;\\n  margin-right: 12px;\\n  background: url(\\'data:image/svg+xml;utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" version=\"1.1\" width=\"18\" height=\"18\" viewBox=\"0 0 24 24\"><path fill=\"black\" d=\"M20,11H4V8H20M20,15H13V13H20M20,19H13V17H20M11,19H4V13H11M20.33,4.67L18.67,3L17,4.67L15.33,3L13.67,4.67L12,3L10.33,4.67L8.67,3L7,4.67L5.33,3L3.67,4.67L2,3V19A2,2 0 0,0 4,21H20A2,2 0 0,0 22,19V3L20.33,4.67Z\" /></svg>\\') !important;\\n}\\n.bb-comment .reply-notice .notice-item a {\\n  order: 1;\\n  flex-grow: 1;\\n  color: black !important;\\n}\\nbody.dark .bb-comment .reply-notice .notice-item a {\\n  color: #eee !important;\\n}\\n.bb-comment .reply-notice .notice-item .icon-close-notice {\\n  order: 2;\\n  position: static !important;\\n  background: url(\\'data:image/svg+xml;utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" version=\"1.1\" width=\"18\" height=\"18\" viewBox=\"0 0 24 24\"><path fill=\"black\" d=\"M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z\" /></svg>\\') !important;\\n}\\n.bb-comment .reply-notice .notice-item .icon-close-notice,\\n.bb-comment .reply-notice .notice-item .icon-notice {\\n  height: 18px;\\n  width: 18px;\\n  background-position: center !important;\\n  opacity: 0.4;\\n}\\n.bb-comment .comment-send:not(.no-login) {\\n  position: relative !important;\\n}\\n.bb-comment .comment-send-lite:not(.no-login),\\n.bb-comment .comment-send:not(.no-login) {\\n  padding-top: 15px !important;\\n}\\n.bb-comment .comment-send-lite:not(.no-login) .dynamic-repost,\\n.bb-comment .comment-send:not(.no-login) .dynamic-repost {\\n  margin-left: 81px !important;\\n  margin-top: 4px;\\n}\\n.bb-comment .comment-send-lite:not(.no-login) .comment-emoji,\\n.bb-comment .comment-send:not(.no-login) .comment-emoji {\\n  position: absolute !important;\\n  right: 0;\\n  top: 51px;\\n  width: 68px !important;\\n  background: #fff;\\n  box-sizing: content-box !important;\\n}\\n.bb-comment .comment-send-lite:not(.no-login) .comment-submit,\\n.bb-comment .comment-send:not(.no-login) .comment-submit {\\n  height: 34px !important;\\n  font-size: 0;\\n}\\n.bb-comment .comment-send-lite:not(.no-login) .comment-submit body.dark,\\n.bb-comment .comment-send:not(.no-login) .comment-submit body.dark {\\n  color: var(--theme-color) !important;\\n}\\n.bb-comment .comment-send-lite:not(.no-login) .comment-submit::after,\\n.bb-comment .comment-send:not(.no-login) .comment-submit::after {\\n  content: \"发表\";\\n  color: #fff;\\n  position: absolute;\\n  top: 50%;\\n  left: 50%;\\n  transform: translate(-50%, -50%);\\n  font-size: 14px;\\n}\\nbody.dark .bb-comment .comment-send-lite:not(.no-login) .comment-submit::after,\\nbody.dark .bb-comment .comment-send:not(.no-login) .comment-submit::after {\\n  color: var(--foreground-color);\\n}\\n\\nbody.dark .panel-area .bb-comment .comment-send-lite {\\n  background: linear-gradient(to top, #444 30%, transparent) !important;\\n}\\n\\n.dynamic-list-item-wrap .info .plat {\\n  display: none !important;\\n}\\n.dynamic-list-item-wrap .reply-box .time-location,\\n.dynamic-list-item-wrap .reply-box .time {\\n  position: absolute;\\n  right: 8px;\\n  top: 0px;\\n  margin: 0;\\n  opacity: 0.5;\\n  line-height: normal;\\n  color: black;\\n  top: 10px;\\n}\\n.dynamic-list-item-wrap .reply-item > .info {\\n  display: flex;\\n  align-items: center;\\n}\\n.dynamic-list-item-wrap .reply-item > .info .floor {\\n  opacity: 0.7;\\n  order: 1;\\n}\\n.dynamic-list-item-wrap .reply-item > .info .reply {\\n  order: 2;\\n}\\n.dynamic-list-item-wrap .reply-item > .info .reply-tags {\\n  order: 3;\\n  display: flex !important;\\n  margin: 0 !important;\\n}\\n.dynamic-list-item-wrap .reply-item > .info .reply-tags span {\\n  margin: 0 4px 0 0 !important;\\n  font-size: 12px !important;\\n  line-height: normal !important;\\n  display: flex !important;\\n  height: auto !important;\\n  padding: 2px 6px !important;\\n}\\n.dynamic-list-item-wrap .reply-item > .info .operation {\\n  order: 4;\\n  flex-grow: 1;\\n  display: flex !important;\\n  justify-content: flex-end;\\n  margin: 0 !important;\\n  padding: 3px !important;\\n}\\n\\n.reply-item > .info > .time-location,\\n.reply-item > .info > .time {\\n  position: absolute;\\n  right: 8px;\\n  top: 24px;\\n  margin: 0 !important;\\n  line-height: normal;\\n  color: black;\\n  top: 12px;\\n  opacity: 1;\\n}\\nbody.dark .reply-item > .info > .time-location,\\nbody.dark .reply-item > .info > .time {\\n  filter: brightness(0) invert(1) !important;\\n}\\n\\n.reply-box .item-user > a {\\n  margin-right: 8px;\\n}\\n.reply-box .item-user .text {\\n  display: block;\\n}\\n\\n.comment-area .dynamic-level {\\n  display: none !important;\\n}\\n\\n.dynamic-like i,\\n.dynamic-hate i {\\n  transition: all 0.2s ease-out;\\n}\\n\\n.dynamic-like i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-like i {\\n  color: #eee;\\n}\\n.dynamic-like i::before {\\n  content: \"\\\\f0514\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-like:hover i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-like:hover i {\\n  color: #eee;\\n}\\n.dynamic-like:hover i::before {\\n  content: \"\\\\f0513\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-like:hover i, .dynamic-like:hover i + span, body.dark .dynamic-like:hover i {\\n  color: var(--theme-color) !important;\\n}\\n\\n.dynamic-liked:hover i,\\n.dynamic-liked i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-liked:hover i,\\nbody.dark .dynamic-liked i {\\n  color: #eee;\\n}\\n.dynamic-liked:hover i::before,\\n.dynamic-liked i::before {\\n  content: \"\\\\f0513\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-liked:hover i, .dynamic-liked:hover i + span, body.dark .dynamic-liked:hover i,\\n.dynamic-liked i,\\n.dynamic-liked i + span,\\nbody.dark .dynamic-liked i {\\n  color: var(--theme-color) !important;\\n}\\n\\n.dynamic-hate i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-hate i {\\n  color: #eee;\\n}\\n.dynamic-hate i::before {\\n  content: \"\\\\f0512\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-hate:hover i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-hate:hover i {\\n  color: #eee;\\n}\\n.dynamic-hate:hover i::before {\\n  content: \"\\\\f0511\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-hate:hover i, .dynamic-hate:hover i + span, body.dark .dynamic-hate:hover i {\\n  color: var(--theme-color) !important;\\n}\\n\\n.dynamic-hated:hover i,\\n.dynamic-hated i {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-hated:hover i,\\nbody.dark .dynamic-hated i {\\n  color: #eee;\\n}\\n.dynamic-hated:hover i::before,\\n.dynamic-hated i::before {\\n  content: \"\\\\f0511\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\n.dynamic-hated:hover i, .dynamic-hated:hover i + span, body.dark .dynamic-hated:hover i,\\n.dynamic-hated i,\\n.dynamic-hated i + span,\\nbody.dark .dynamic-hated i {\\n  color: var(--theme-color) !important;\\n}\\n\\n.dynamic-spot {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .dynamic-spot {\\n  color: #eee;\\n}\\n.dynamic-spot::before {\\n  content: \"\\\\f01d9\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\nbody.dark .dynamic-spot {\\n  filter: brightness(0) invert(1) !important;\\n}\\n\\n.textarea-container .comm-tool .comm-emoji .icon-face {\\n  background: none !important;\\n  color: #000;\\n}\\nbody.dark .textarea-container .comm-tool .comm-emoji .icon-face {\\n  color: #eee;\\n}\\n.textarea-container .comm-tool .comm-emoji .icon-face::before {\\n  content: \"\\\\f01f5\";\\n  display: inline-block;\\n  font: normal normal normal 24px/1 \"Material Design Icons\";\\n  font-size: 16px;\\n  line-height: 1;\\n  width: 16px;\\n  height: 16px;\\n}\\nbody.dark .textarea-container .comm-tool .comm-emoji .icon-face {\\n  filter: brightness(0) invert(1) !important;\\n}\\n\\n.dynamic-spot,\\n.textarea-container .comm-tool .comm-emoji .icon-face {\\n  height: 16px !important;\\n  width: 16px !important;\\n  background-position: center !important;\\n  opacity: 0.4;\\n  display: inline-flex !important;\\n}\\n\\n.comment-list .opera-list {\\n  right: 20px !important;\\n  top: -72px !important;\\n}\\n\\n.v-wrap #comment {\\n  z-index: 21 !important;\\n}\\n\\n.l-con .tag-channel-pane {\\n  z-index: 22 !important;\\n}',\"\"]),n.exports=o},355:n=>{\"use strict\";\n// eslint-disable-next-line func-names\nn.exports=function(n){var t=[];return t.toString=function(){return this.map((function(t){var e=n(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(e,\"}\"):e})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(n,e,o){\"string\"==typeof n&&(\n// eslint-disable-next-line no-param-reassign\nn=[[null,n,\"\"]]);var i={};if(o)for(var m=0;m<this.length;m++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[m][0];null!=a&&(i[a]=!0)}for(var r=0;r<n.length;r++){var c=[].concat(n[r]);o&&i[c[0]]||(e&&(c[2]?c[2]=\"\".concat(e,\" and \").concat(c[2]):c[2]=e),t.push(c))}},t}},32:(n,t,e)=>{var o=e(354);o&&o.__esModule&&(o=o.default),n.exports=\"string\"==typeof o?o:o.toString()},986:n=>{\"use strict\";n.exports=coreApis.settings}},o={};function i(n){var t=o[n];if(void 0!==t)return t.exports;var m=o[n]={id:n,exports:{}};return e[n](m,m.exports,i),m.exports}t=Object.getPrototypeOf?n=>Object.getPrototypeOf(n):n=>n.__proto__,i.t=function(e,o){if(1&o&&(e=this(e)),8&o)return e;if(\"object\"==typeof e&&e){if(4&o&&e.__esModule)return e;if(16&o&&\"function\"==typeof e.then)return e}var m=Object.create(null);i.r(m);var a={};n=n||[null,t({}),t([]),t(t)];for(var r=2&o&&e;\"object\"==typeof r&&!~n.indexOf(r);r=t(r))Object.getOwnPropertyNames(r).forEach((n=>a[n]=()=>e[n]));return a.default=()=>e,i.d(m,a),m},i.d=(n,t)=>{for(var e in t)i.o(t,e)&&!i.o(n,e)&&Object.defineProperty(n,e,{enumerable:!0,get:t[e]})},i.o=(n,t)=>Object.prototype.hasOwnProperty.call(n,t),i.r=n=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(n,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(n,\"__esModule\",{value:!0})};var m={};return(()=>{\"use strict\";i.d(m,{component:()=>t});const n=\"simplifyComments\",t=(0,coreApis.componentApis.define.defineComponentMetadata)({name:n,entry:async n=>{let{metadata:t}=n;const{addComponentListener:e}=await Promise.resolve().then(i.t.bind(i,986,23));e(t.name,(n=>{document.body.classList.toggle(\"simplify-comment\",n)}),!0)},instantStyles:[{name:n,style:()=>Promise.resolve().then(i.t.bind(i,32,23))}],displayName:\"简化评论区\",description:{\"zh-CN\":\"\\n- 删除热评头像下方的关注按钮\\n- 删除用户的等级标识\\n- 删除发送源信息(`来自安卓客户端` 这种)\\n- 删除用户名右边的勋章\\n- 删除评论区顶部的横幅\\n- 发送时间移动到右上角\\n- 位图图标全部换用矢量图标, 高分屏不会模糊\\n- 投票仅显示链接, 隐藏下面的大框.\\n\\n> 注: 关注和等级可以通过鼠标停留在头像上, 在弹出的资料卡小窗中查看.\".trim()},tags:[componentsTags.style],commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),m=m.component})()));",
      "metadata": {
        "name": "simplifyComments",
        "displayName": "简化评论区",
        "description": {
          "zh-CN": "- 删除热评头像下方的关注按钮\n- 删除用户的等级标识\n- 删除发送源信息(`来自安卓客户端` 这种)\n- 删除用户名右边的勋章\n- 删除评论区顶部的横幅\n- 发送时间移动到右上角\n- 位图图标全部换用矢量图标, 高分屏不会模糊\n- 投票仅显示链接, 隐藏下面的大框.\n\n> 注: 关注和等级可以通过鼠标停留在头像上, 在弹出的资料卡小窗中查看."
        },
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "removeLiveWatermark": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"live/remove-watermark\"]=t():e[\"live/remove-watermark\"]=t()}(globalThis,(()=>(()=>{var e,t,o={221:(e,t,o)=>{var r=o(355)((function(e){return e[1]}));r.push([e.id,\".live-player-ctnr .web-player-icon-roomStatus,\\n.bilibili-live-player-video-logo {\\n  display: none !important;\\n}\",\"\"]),e.exports=r},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var o=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(o,\"}\"):o})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,o,r){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var n={};if(r)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[i][0];null!=a&&(n[a]=!0)}for(var c=0;c<e.length;c++){var p=[].concat(e[c]);r&&n[p[0]]||(o&&(p[2]?p[2]=\"\".concat(o,\" and \").concat(p[2]):p[2]=o),t.push(p))}},t}},0:(e,t,o)=>{var r=o(221);r&&r.__esModule&&(r=r.default),e.exports=\"string\"==typeof r?r:r.toString()}},r={};function n(e){var t=r[e];if(void 0!==t)return t.exports;var i=r[e]={id:e,exports:{}};return o[e](i,i.exports,n),i.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,n.t=function(o,r){if(1&r&&(o=this(o)),8&r)return o;if(\"object\"==typeof o&&o){if(4&r&&o.__esModule)return o;if(16&r&&\"function\"==typeof o.then)return o}var i=Object.create(null);n.r(i);var a={};e=e||[null,t({}),t([]),t(t)];for(var c=2&r&&o;\"object\"==typeof c&&!~e.indexOf(c);c=t(c))Object.getOwnPropertyNames(c).forEach((e=>a[e]=()=>o[e]));return a.default=()=>o,n.d(i,a),i},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";n.d(i,{component:()=>r});const e=coreApis.componentApis.define,t=coreApis.componentApis.styledComponent,o=coreApis.utils.urls,r=(0,e.defineComponentMetadata)({...(0,t.toggleStyle)(\"removeLiveWatermark\",(()=>Promise.resolve().then(n.t.bind(n,0,23)))),displayName:\"删除直播水印\",tags:[componentsTags.live,componentsTags.style],description:{\"zh-CN\":\"删除观看直播时角落的水印.\"},urlInclude:o.liveUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "name": "removeLiveWatermark",
        "displayName": "删除直播水印",
        "tags": [
          {
            "name": "live",
            "displayName": "直播",
            "color": "#26A69A",
            "icon": "mdi-video-wireless-outline",
            "order": 4
          },
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "description": {
          "zh-CN": "删除观看直播时角落的水印."
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    },
    "simplifyHome": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"style/simplify/home\"]=t():e[\"style/simplify/home\"]=t()}(globalThis,(()=>(()=>{var e,t,i={720:(e,t,i)=>{var n=i(355)((function(e){return e[1]}));n.push([e.id,\"body.simplifyHome-switch-categories .z-top-container.has-menu {\\n  height: auto !important;\\n  min-height: unset !important;\\n}\\nbody.simplifyHome-switch-categories .bili-header-m > .bili-wrapper {\\n  visibility: hidden !important;\\n  height: 18px !important;\\n}\\nbody.simplifyHome-switch-categories .primary-menu-itnl {\\n  visibility: hidden !important;\\n  height: 24px !important;\\n  padding: 0 !important;\\n}\\nbody.simplifyHome-switch-categories .bili-header__channel {\\n  height: 12px !important;\\n}\\nbody.simplifyHome-switch-categories .bili-header__channel > * {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-categories.header-v3 .bili-wrapper {\\n  padding-top: 8px !important;\\n  border-top: none !important;\\n}\\nbody.simplifyHome-switch-trends .first-screen #reportFirst1 {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-trends .first-screen .space-between {\\n  margin-bottom: 0 !important;\\n}\\nbody.simplifyHome-switch-trends .bili-layout .bili-grid:first-child,\\nbody.simplifyHome-switch-trends .recommended-container,\\nbody.simplifyHome-switch-trends .rcmd-box-wrap {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-online .first-screen #reportFirst2 {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-ext-box .first-screen #reportFirst3 {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-special #bili_report_spe_rec {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-contact .bili-footer .b-footer-wrap,\\nbody.simplifyHome-switch-contact .international-footer {\\n  display: none !important;\\n}\\nbody.simplifyHome-switch-elevator .storey-box .elevator {\\n  display: none !important;\\n}\",\"\"]),e.exports=n},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var i=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(i,\"}\"):i})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,i,n){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var o={};if(n)for(var r=0;r<this.length;r++){\n// eslint-disable-next-line prefer-destructuring\nvar s=this[r][0];null!=s&&(o[s]=!0)}for(var a=0;a<e.length;a++){var l=[].concat(e[a]);n&&o[l[0]]||(i&&(l[2]?l[2]=\"\".concat(i,\" and \").concat(l[2]):l[2]=i),t.push(l))}},t}},946:(e,t,i)=>{var n=i(720);n&&n.__esModule&&(n=n.default),e.exports=\"string\"==typeof n?n:n.toString()}},n={};function o(e){var t=n[e];if(void 0!==t)return t.exports;var r=n[e]={id:e,exports:{}};return i[e](r,r.exports,o),r.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,o.t=function(i,n){if(1&n&&(i=this(i)),8&n)return i;if(\"object\"==typeof i&&i){if(4&n&&i.__esModule)return i;if(16&n&&\"function\"==typeof i.then)return i}var r=Object.create(null);o.r(r);var s={};e=e||[null,t({}),t([]),t(t)];for(var a=2&n&&i;\"object\"==typeof a&&!~e.indexOf(a);a=t(a))Object.getOwnPropertyNames(a).forEach((e=>s[e]=()=>i[e]));return s.default=()=>i,o.d(r,s),r},o.d=(e,t)=>{for(var i in t)o.o(t,i)&&!o.o(e,i)&&Object.defineProperty(e,i,{enumerable:!0,get:t[i]})},o.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),o.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var r={};return(()=>{\"use strict\";o.d(r,{component:()=>m});const e=coreApis.componentApis.switchOptions,t=coreApis.settings,i=coreApis.spinQuery,n=coreApis.style,s=coreApis.utils,a=coreApis.utils.log,l=coreApis.utils.urls,p={name:\"simplifyOptions\",dimAt:\"checked\",switchProps:{checkedIcon:\"mdi-eye-off-outline\",notCheckedIcon:\"mdi-eye-outline\"},switches:{categories:{defaultValue:!1,displayName:\"分区栏\"},trends:{defaultValue:!1,displayName:\"活动/热门视频\"},online:{defaultValue:!1,displayName:\"在线列表(旧)\"},\"ext-box\":{defaultValue:!1,displayName:\"电竞赛事(旧)\"},special:{defaultValue:!1,displayName:\"特别推荐(旧)\"},contact:{defaultValue:!1,displayName:\"联系方式\"},elevator:{defaultValue:!1,displayName:\"右侧分区导航(旧)\"}}},c=(0,a.useScopedConsole)(\"简化首页\"),d={name:\"simplifyHome\",displayName:\"简化首页\",description:\"隐藏原版首页不需要的元素 / 分区.\",instantStyles:[{name:\"simplifyHome\",style:()=>Promise.resolve().then(o.t.bind(o,946,23))}],urlInclude:l.mainSiteUrls,tags:[componentsTags.style],entry:async()=>{const e=(0,s.matchUrlPattern)(\"https://www.bilibili.com/\");if(!e)return;c.log(\"isHome\",e);const{options:o}=(0,t.getComponentSettings)(d.name),r=\"-1\"===(0,s.getCookieValue)(\"i-wanna-go-back\"),a=await(async()=>{if(!r){const t=await(0,i.sq)((()=>dqa(\".proxy-box > div\")),(t=>t.length>0||!e));return Object.fromEntries(t.map((e=>[e.id.replace(/^bili_/,\"\"),{displayName:e.querySelector(\"header .name\")?.textContent?.trim()??\"未知分区\",defaultValue:!1}])))}const t=[\"推广\"],n=await(0,i.sq)((()=>dqa(\".bili-grid .the-world\")),(t=>t.length>3||!e));c.log(n);const o=n?.filter((e=>!t.includes(e.id))).map((e=>{const t=(e=>{let t=e;for(;t.parentElement;){if(t.classList.contains(\"bili-grid\"))return t;t=t.parentElement}return null})(e),i=e.id;return t?(t.dataset.area=i,[i,{displayName:i,defaultValue:!1}]):null})).filter((e=>null!==e))??[];return Object.fromEntries(o)})(),l={};Object.entries(a).forEach((e=>{let[i,{displayName:n,defaultValue:r}]=e;const s={defaultValue:r,displayName:n},a=`switch-${i}`;void 0===o[a]&&(o[a]=r);const c=`switch-${i}`;(0,t.addComponentListener)(`${d.name}.${c}`,(e=>{document.body.classList.toggle(`${d.name}-${c}`,e)}),!0),p.switches[i]=s,l[i]=s})),o.simplifyOptions.switches=l;const m=Object.keys(a).map((e=>`\\n        body.simplifyHome-switch-${e} .bili-layout .bili-grid[data-area=\"${e}\"],\\n        body.simplifyHome-switch-${e} .storey-box .proxy-box #bili_${e} {\\n          display: none !important;\\n        }\\n      `.trim())).join(\"\\n\");(0,n.addStyle)(m,\"simplify-home-generated\")}},m=(0,e.createSwitchOptions)(p)(d)})(),r=r.component})()));",
      "metadata": {
        "name": "simplifyHome",
        "displayName": "简化首页",
        "description": "隐藏原版首页不需要的元素 / 分区.",
        "tags": [
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "options": {
          "switch-categories": {
            "defaultValue": false,
            "displayName": "分区栏",
            "hidden": true
          },
          "switch-trends": {
            "defaultValue": false,
            "displayName": "活动/热门视频",
            "hidden": true
          },
          "switch-online": {
            "defaultValue": false,
            "displayName": "在线列表(旧)",
            "hidden": true
          },
          "switch-ext-box": {
            "defaultValue": false,
            "displayName": "电竞赛事(旧)",
            "hidden": true
          },
          "switch-special": {
            "defaultValue": false,
            "displayName": "特别推荐(旧)",
            "hidden": true
          },
          "switch-contact": {
            "defaultValue": false,
            "displayName": "联系方式",
            "hidden": true
          },
          "switch-elevator": {
            "defaultValue": false,
            "displayName": "右侧分区导航(旧)",
            "hidden": true
          },
          "simplifyOptions": {
            "defaultValue": {
              "name": "simplifyOptions",
              "dimAt": "checked",
              "switchProps": {
                "checkedIcon": "mdi-eye-off-outline",
                "notCheckedIcon": "mdi-eye-outline"
              },
              "switches": {
                "categories": {
                  "defaultValue": false,
                  "displayName": "分区栏"
                },
                "trends": {
                  "defaultValue": false,
                  "displayName": "活动/热门视频"
                },
                "online": {
                  "defaultValue": false,
                  "displayName": "在线列表(旧)"
                },
                "ext-box": {
                  "defaultValue": false,
                  "displayName": "电竞赛事(旧)"
                },
                "special": {
                  "defaultValue": false,
                  "displayName": "特别推荐(旧)"
                },
                "contact": {
                  "defaultValue": false,
                  "displayName": "联系方式"
                },
                "elevator": {
                  "defaultValue": false,
                  "displayName": "右侧分区导航(旧)"
                }
              },
              "radio": false,
              "componentName": "simplifyHome",
              "optionDisplayName": "简化首页选项"
            },
            "displayName": "简化首页选项"
          }
        }
      },
      "settings": {
        "enabled": true,
        "options": {
          "switch-categories": false,
          "switch-trends": false,
          "switch-online": false,
          "switch-ext-box": false,
          "switch-special": false,
          "switch-contact": false,
          "switch-elevator": false,
          "simplifyOptions": {
            "name": "simplifyOptions",
            "dimAt": "checked",
            "switchProps": {
              "checkedIcon": "mdi-eye-off-outline",
              "notCheckedIcon": "mdi-eye-outline"
            },
            "switches": {
              "categories": {
                "defaultValue": false,
                "displayName": "分区栏"
              },
              "trends": {
                "defaultValue": false,
                "displayName": "活动/热门视频"
              },
              "online": {
                "defaultValue": false,
                "displayName": "在线列表(旧)"
              },
              "ext-box": {
                "defaultValue": false,
                "displayName": "电竞赛事(旧)"
              },
              "special": {
                "defaultValue": false,
                "displayName": "特别推荐(旧)"
              },
              "contact": {
                "defaultValue": false,
                "displayName": "联系方式"
              },
              "elevator": {
                "defaultValue": false,
                "displayName": "右侧分区导航(旧)"
              }
            },
            "radio": false,
            "componentName": "simplifyHome",
            "optionDisplayName": "简化首页选项"
          }
        }
      }
    },
    "simplifyLiveroom": {
      "code": "!function(i,e){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=e():\"function\"==typeof define&&define.amd?define([],e):\"object\"==typeof exports?exports[\"style/simplify/live\"]=e():i[\"style/simplify/live\"]=e()}(globalThis,(()=>(()=>{var i,e,t={838:(i,e,t)=>{\"use strict\";t.r(e),t.d(e,{setupSkinSimplify:()=>r});const n=coreApis.settings,o=coreApis.spinQuery,r=async()=>{(0,n.addComponentListener)(\"simplifyLiveroom.switch-skin\",(async i=>{const e=await(0,o.select)(\"#skin-css\");e&&(e.media=i?\"none\":\"all\")}),!0)}},946:(i,e,t)=>{var n=t(355)((function(i){return i[1]}));n.push([i.id,\".simplifyLiveroom-switch-vip .vip-icon, .simplifyLiveroom-switch-fansMedal .fans-medal-item-ctnr, .simplifyLiveroom-switch-title .title-label, .simplifyLiveroom-switch-userLevel .user-level-icon, .simplifyLiveroom-switch-guard .chat-history-panel .guard-icon, .simplifyLiveroom-switch-systemMessage .system-msg, .simplifyLiveroom-switch-systemMessage .announcement-wrapper, .simplifyLiveroom-switch-welcomeMessage .welcome-guard, .simplifyLiveroom-switch-welcomeMessage .welcome-msg, .simplifyLiveroom-switch-popup .chat-popups-section, .simplifyLiveroom-switch-popup #chat-draw-area-vm, .simplifyLiveroom-switch-giftMessage .chat-item.gift-item, .simplifyLiveroom-switch-giftMessage .chat-history-panel .penury-gift-msg, .simplifyLiveroom-switch-guardPurchase .chat-item.guard-buy, .simplifyLiveroom-switch-eventsBanner .z-section-blocks .left-container .flip-view, .simplifyLiveroom-switch-eventsBanner .activity-pushing-out, .simplifyLiveroom-switch-userEffect .live-room-app .aside-area .activity-welcome-section, .simplifyLiveroom-switch-kanban .live-haruna-ctnr, .simplifyLiveroom-switch-enterPrompt .chat-item.important-prompt-item, .simplifyLiveroom-switch-enterPrompt .chat-history-panel .brush-prompt, .simplifyLiveroom-switch-enterPrompt .chat-item.convention-msg, .simplifyLiveroom-switch-pk .chaos-pk, .simplifyLiveroom-switch-topRank .chat-item.top3-notice, .simplifyLiveroom-switch-topRank .chat-item .rank-icon {\\n  display: none !important;\\n}\\n\\n.simplifyLiveroom-switch-headerPanel .control-panel-ctnr .dialog-ctnr {\\n  z-index: 800 !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .player-ctnr .room-info-ctnr {\\n  display: inline-flex !important;\\n  flex: 1 0 auto;\\n  align-items: center !important;\\n  margin-left: 12px !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .head-info-section {\\n  height: 52px !important;\\n  box-sizing: content-box !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr {\\n  display: flex !important;\\n  padding: 10px 24px 10px 12px !important;\\n  height: auto !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .blive-avatar-icons,\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .face-pendants {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .blive-avatar-pendant {\\n  width: 48px !important;\\n  height: 48px !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .blive-avatar-face,\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .blive-avatar,\\n.simplifyLiveroom-switch-headerPanel .header-info-ctnr .avatar {\\n  height: 32px !important;\\n  width: 32px !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .room-cover {\\n  width: 32px !important;\\n  height: 32px !important;\\n  border-radius: 50% !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr {\\n  display: flex !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row {\\n  display: flex !important;\\n  align-items: center !important;\\n  flex: 1 0 auto !important;\\n  flex-direction: row-reverse !important;\\n  position: static !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .left-ctnr,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .normal-mode,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .left-ctnr,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .normal-mode {\\n  position: absolute !important;\\n  left: 50% !important;\\n  transform: translateX(-50%) !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .live-area,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .area-text,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .live-area,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .area-text {\\n  display: inline-flex !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .right-ctnr,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .upper-right-ctnr,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .right-ctnr,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .upper-right-ctnr {\\n  position: static !important;\\n  transform: none !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .live-title,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .room-title,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .live-title,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .room-title {\\n  display: flex !important;\\n  align-items: center !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .live-title .text,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .room-title .text,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .live-title .text,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .room-title .text {\\n  line-height: normal !important;\\n}\\n@media screen and (max-width: 1750px) {\\n  .simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .live-title .title-length-limit,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .room-title .title-length-limit,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .live-title .title-length-limit,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .room-title .title-length-limit {\\n    max-width: 250px !important;\\n  }\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .upper-row .info-section,\\n.simplifyLiveroom-switch-headerPanel .room-info-upper-row .info-section {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .lower-row,\\n.simplifyLiveroom-switch-headerPanel .room-info-down-row {\\n  margin: 0 !important;\\n  order: -1;\\n}\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .lower-row .right-ctnr,\\n.simplifyLiveroom-switch-headerPanel .rows-ctnr .lower-row .left-ctnr > :nth-child(n+3),\\n.simplifyLiveroom-switch-headerPanel .room-info-down-row .right-ctnr,\\n.simplifyLiveroom-switch-headerPanel .room-info-down-row .left-ctnr > :nth-child(n+3) {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .room-owner-username {\\n  max-width: 150px !important;\\n}\\n.simplifyLiveroom-switch-headerPanel .live-status,\\n.simplifyLiveroom-switch-headerPanel .live-status-label {\\n  display: none !important;\\n}\\n\\n.simplifyLiveroom-switch-giftMessage:not(.simplifyLiveroom-switch-enterPrompt) .chat-history-list.with-penury-gift:not(.with-brush-prompt) {\\n  height: 100% !important;\\n}\\n.simplifyLiveroom-switch-giftMessage:not(.simplifyLiveroom-switch-enterPrompt) .chat-history-list.with-penury-gift.with-brush-prompt {\\n  height: calc(100% - 32px) !important;\\n}\\n\\n.simplifyLiveroom-switch-enterPrompt:not(.simplifyLiveroom-switch-giftMessage) .chat-history-list.with-brush-prompt:not(.with-penury-gift) {\\n  height: 100% !important;\\n}\\n.simplifyLiveroom-switch-enterPrompt:not(.simplifyLiveroom-switch-giftMessage) .chat-history-list.with-brush-prompt.with-penury-gift {\\n  height: calc(100% - 32px) !important;\\n}\\n\\n.simplifyLiveroom-switch-enterPrompt.simplifyLiveroom-switch-giftMessage .chat-history-list {\\n  height: 100% !important;\\n}\\n\\n.simplifyLiveroom-switch-rankList .live-room-app .rank-list-section {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-rankList .live-room-app .chat-history-panel {\\n  height: calc(100% - 145px) !important;\\n}\\n.simplifyLiveroom-switch-rankList .live-room-app .chat-history-panel .chat-history-list::-webkit-scrollbar-track {\\n  background: transparent !important;\\n}\\n.simplifyLiveroom-switch-rankList .live-room-app .chat-history-panel,\\n.simplifyLiveroom-switch-rankList .live-room-app #pay-note-panel-vm .pay-note-panel,\\n.simplifyLiveroom-switch-rankList .live-room-app #pay-note-panel-vm .pay-note-panel .detail-info .mask {\\n  border-radius: 11px 11px 0 0 !important;\\n}\\n.simplifyLiveroom-switch-rankList.player-full-win .chat-history-panel,\\n.simplifyLiveroom-switch-rankList.player-full-win #pay-note-panel-vm .pay-note-panel,\\n.simplifyLiveroom-switch-rankList.player-full-win #pay-note-panel-vm .pay-note-panel .detail-info .mask {\\n  border-radius: 0 !important;\\n}\\n\\n.simplifyLiveroom-switch-giftPanel .gift-panel,\\n.simplifyLiveroom-switch-giftPanel .gift-panel-switch,\\n.simplifyLiveroom-switch-giftPanel .gift-section.guard-ent,\\n.simplifyLiveroom-switch-giftPanel .seeds-wrap > .dp-i-block > .item:not(.seeds),\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel .wish-icon,\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel .wish-tip {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .gift-control-section,\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel {\\n  height: 48px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry,\\n.simplifyLiveroom-switch-giftPanel .treasure-box {\\n  display: flex !important;\\n  align-items: center !important;\\n  padding: 10px 0 0 16px !important;\\n  max-height: 36px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box .draw-box-pic,\\n.simplifyLiveroom-switch-giftPanel .draw-box .anchor-lot-icon,\\n.simplifyLiveroom-switch-giftPanel .draw-box .box-icon,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .draw-box-pic,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .anchor-lot-icon,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .box-icon,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .draw-box-pic,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .anchor-lot-icon,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .box-icon {\\n  margin: 0 !important;\\n  width: 24px !important;\\n  height: 24px !important;\\n  background-position: 0 -2.5px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box .draw-box-pic.open,\\n.simplifyLiveroom-switch-giftPanel .draw-box .anchor-lot-icon.open,\\n.simplifyLiveroom-switch-giftPanel .draw-box .box-icon.open,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .draw-box-pic.open,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .anchor-lot-icon.open,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .box-icon.open,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .draw-box-pic.open,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .anchor-lot-icon.open,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .box-icon.open {\\n  background-position: 0 -1px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box .draw-box-pic,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .draw-box-pic,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .draw-box-pic {\\n  transform: scale(1.1);\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box #BLRHH_treasure_div_tip br,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry #BLRHH_treasure_div_tip br,\\n.simplifyLiveroom-switch-giftPanel .treasure-box #BLRHH_treasure_div_tip br {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box #BLRHH_treasure_div img,\\n.simplifyLiveroom-switch-giftPanel .draw-box #BLRHH_treasure_div canvas,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry #BLRHH_treasure_div img,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry #BLRHH_treasure_div canvas,\\n.simplifyLiveroom-switch-giftPanel .treasure-box #BLRHH_treasure_div img,\\n.simplifyLiveroom-switch-giftPanel .treasure-box #BLRHH_treasure_div canvas {\\n  max-height: 24px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box .draw-box-text,\\n.simplifyLiveroom-switch-giftPanel .draw-box .anchor-lot-text,\\n.simplifyLiveroom-switch-giftPanel .draw-box .count-down,\\n.simplifyLiveroom-switch-giftPanel .draw-box #BLRHH_treasure_div_tip,\\n.simplifyLiveroom-switch-giftPanel .draw-box #BLRHH_treasure_div_timer,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .draw-box-text,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .anchor-lot-text,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .count-down,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry #BLRHH_treasure_div_tip,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry #BLRHH_treasure_div_timer,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .draw-box-text,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .anchor-lot-text,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .count-down,\\n.simplifyLiveroom-switch-giftPanel .treasure-box #BLRHH_treasure_div_tip,\\n.simplifyLiveroom-switch-giftPanel .treasure-box #BLRHH_treasure_div_timer {\\n  margin-left: 12px !important;\\n  padding: 4px 8px !important;\\n  max-width: unset !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box .awarding-panel,\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry .awarding-panel,\\n.simplifyLiveroom-switch-giftPanel .treasure-box .awarding-panel {\\n  bottom: 42px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .draw-box {\\n  padding-top: 11px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .anchor-lottery-entry {\\n  padding-top: 12px !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel .right-part {\\n  height: 48px !important;\\n  display: flex !important;\\n  justify-content: flex-end !important;\\n  min-width: unset !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel .right-part > .dp-table-cell {\\n  display: flex !important;\\n  align-items: center !important;\\n}\\n.simplifyLiveroom-switch-giftPanel .gift-control-panel .right-part > .dp-table-cell .supporting-info {\\n  transform: translateY(-2px) !important;\\n}\\n\\n.simplifyLiveroom-switch-guard .guard-danmaku::before {\\n  border-image: none !important;\\n  background-color: transparent !important;\\n}\\n.simplifyLiveroom-switch-guard .guard-danmaku::before .guard-danmaku {\\n  margin: 0 !important;\\n  padding: 4px 5px !important;\\n}\\n.simplifyLiveroom-switch-guard .guard-danmaku::before .guard-danmaku::after {\\n  background-image: none !important;\\n}\\n.simplifyLiveroom-switch-guard .chat-history-panel [class*=guard-level-] {\\n  padding: 4px 5px !important;\\n  margin: 0 !important;\\n}\\n.simplifyLiveroom-switch-guard .chat-history-panel [class*=guard-level-]::after {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-guard .chat-history-panel .chat-colorful-bubble {\\n  margin: 0 !important;\\n  display: block !important;\\n  border-radius: 0 !important;\\n  background-color: transparent !important;\\n}\\n.simplifyLiveroom-switch-guard .fans-medal-item.medal-guard {\\n  margin-left: 0 !important;\\n}\\n\\n.simplifyLiveroom-switch-emoticons .control-panel-icon-row .emoticons-panel {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-emoticons .chat-history-list .chat-item .emoticon img {\\n  display: none !important;\\n}\\n.simplifyLiveroom-switch-emoticons .chat-history-list .chat-item .emoticon span {\\n  display: inline-flex !important;\\n}\\n.simplifyLiveroom-switch-emoticons .danmaku-item-container .bilibili-danmaku img {\\n  display: none !important;\\n}\",\"\"]),i.exports=n},355:i=>{\"use strict\";\n// eslint-disable-next-line func-names\ni.exports=function(i){var e=[];return e.toString=function(){return this.map((function(e){var t=i(e);return e[2]?\"@media \".concat(e[2],\" {\").concat(t,\"}\"):t})).join(\"\")},\n// eslint-disable-next-line func-names\ne.i=function(i,t,n){\"string\"==typeof i&&(\n// eslint-disable-next-line no-param-reassign\ni=[[null,i,\"\"]]);var o={};if(n)for(var r=0;r<this.length;r++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[r][0];null!=a&&(o[a]=!0)}for(var s=0;s<i.length;s++){var l=[].concat(i[s]);n&&o[l[0]]||(t&&(l[2]?l[2]=\"\".concat(t,\" and \").concat(l[2]):l[2]=t),e.push(l))}},e}},330:(i,e,t)=>{var n=t(946);n&&n.__esModule&&(n=n.default),i.exports=\"string\"==typeof n?n:n.toString()}},n={};function o(i){var e=n[i];if(void 0!==e)return e.exports;var r=n[i]={id:i,exports:{}};return t[i](r,r.exports,o),r.exports}e=Object.getPrototypeOf?i=>Object.getPrototypeOf(i):i=>i.__proto__,o.t=function(t,n){if(1&n&&(t=this(t)),8&n)return t;if(\"object\"==typeof t&&t){if(4&n&&t.__esModule)return t;if(16&n&&\"function\"==typeof t.then)return t}var r=Object.create(null);o.r(r);var a={};i=i||[null,e({}),e([]),e(e)];for(var s=2&n&&t;\"object\"==typeof s&&!~i.indexOf(s);s=e(s))Object.getOwnPropertyNames(s).forEach((i=>a[i]=()=>t[i]));return a.default=()=>t,o.d(r,a),r},o.d=(i,e)=>{for(var t in e)o.o(e,t)&&!o.o(i,t)&&Object.defineProperty(i,t,{enumerable:!0,get:e[t]})},o.o=(i,e)=>Object.prototype.hasOwnProperty.call(i,e),o.r=i=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(i,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(i,\"__esModule\",{value:!0})};var r={};return(()=>{\"use strict\";o.d(r,{component:()=>n});const i=coreApis.componentApis.switchOptions,e=coreApis.componentApis.styledComponent,t=coreApis.utils.urls,n=(0,i.createSwitchOptions)({name:\"simplifyOptions\",dimAt:\"checked\",switchProps:{checkedIcon:\"mdi-eye-off-outline\",notCheckedIcon:\"mdi-eye-outline\"},switches:{vip:{defaultValue:!0,displayName:\"老爷图标\"},enterPrompt:{defaultValue:!0,displayName:\"入场通知\"},fansMedal:{defaultValue:!0,displayName:\"粉丝勋章\"},title:{defaultValue:!0,displayName:\"活动头衔\"},guard:{defaultValue:!0,displayName:\"舰长图标\"},systemMessage:{defaultValue:!0,displayName:\"全区广播\"},welcomeMessage:{defaultValue:!0,displayName:\"欢迎信息\"},giftMessage:{defaultValue:!0,displayName:\"礼物弹幕\"},emoticons:{defaultValue:!0,displayName:\"表情特效\"},guardPurchase:{defaultValue:!0,displayName:\"上舰提示\"},giftPanel:{defaultValue:!0,displayName:\"付费礼物\"},headerPanel:{defaultValue:!1,displayName:\"标题栏活动\"},userEffect:{defaultValue:!0,displayName:\"入场特效\"},kanban:{defaultValue:!0,displayName:\"看板娘\"},eventsBanner:{defaultValue:!1,displayName:\"活动横幅\"},rankList:{defaultValue:!1,displayName:\"排行榜\"},popup:{defaultValue:!1,displayName:\"抽奖提示\"},pk:{defaultValue:!1,displayName:\"PK浮窗\"},topRank:{defaultValue:!1,displayName:\"高能榜提示\"},skin:{defaultValue:!1,displayName:\"房间皮肤\"}}})({name:\"simplifyLiveroom\",displayName:\"简化直播间\",entry:(0,e.styledComponentEntry)((()=>Promise.resolve().then(o.t.bind(o,330,23))),(async()=>{const{setupSkinSimplify:i}=await Promise.resolve().then(o.bind(o,838));i()})),description:{\"zh-CN\":\"隐藏直播间中各种不需要的内容.\"},tags:[componentsTags.live,componentsTags.style],urlInclude:t.liveUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),r=r.component})()));",
      "metadata": {
        "name": "simplifyLiveroom",
        "displayName": "简化直播间",
        "description": {
          "zh-CN": "隐藏直播间中各种不需要的内容."
        },
        "tags": [
          {
            "name": "live",
            "displayName": "直播",
            "color": "#26A69A",
            "icon": "mdi-video-wireless-outline",
            "order": 4
          },
          {
            "name": "style",
            "displayName": "样式",
            "color": "#8BC34A",
            "icon": "mdi-palette-outline",
            "order": 2
          }
        ],
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2",
        "options": {
          "switch-vip": {
            "defaultValue": true,
            "displayName": "老爷图标",
            "hidden": true
          },
          "switch-enterPrompt": {
            "defaultValue": true,
            "displayName": "入场通知",
            "hidden": true
          },
          "switch-fansMedal": {
            "defaultValue": true,
            "displayName": "粉丝勋章",
            "hidden": true
          },
          "switch-title": {
            "defaultValue": true,
            "displayName": "活动头衔",
            "hidden": true
          },
          "switch-guard": {
            "defaultValue": true,
            "displayName": "舰长图标",
            "hidden": true
          },
          "switch-systemMessage": {
            "defaultValue": true,
            "displayName": "全区广播",
            "hidden": true
          },
          "switch-welcomeMessage": {
            "defaultValue": true,
            "displayName": "欢迎信息",
            "hidden": true
          },
          "switch-giftMessage": {
            "defaultValue": true,
            "displayName": "礼物弹幕",
            "hidden": true
          },
          "switch-emoticons": {
            "defaultValue": true,
            "displayName": "表情特效",
            "hidden": true
          },
          "switch-guardPurchase": {
            "defaultValue": true,
            "displayName": "上舰提示",
            "hidden": true
          },
          "switch-giftPanel": {
            "defaultValue": true,
            "displayName": "付费礼物",
            "hidden": true
          },
          "switch-headerPanel": {
            "defaultValue": false,
            "displayName": "标题栏活动",
            "hidden": true
          },
          "switch-userEffect": {
            "defaultValue": true,
            "displayName": "入场特效",
            "hidden": true
          },
          "switch-kanban": {
            "defaultValue": true,
            "displayName": "看板娘",
            "hidden": true
          },
          "switch-eventsBanner": {
            "defaultValue": false,
            "displayName": "活动横幅",
            "hidden": true
          },
          "switch-rankList": {
            "defaultValue": false,
            "displayName": "排行榜",
            "hidden": true
          },
          "switch-popup": {
            "defaultValue": false,
            "displayName": "抽奖提示",
            "hidden": true
          },
          "switch-pk": {
            "defaultValue": false,
            "displayName": "PK浮窗",
            "hidden": true
          },
          "switch-topRank": {
            "defaultValue": false,
            "displayName": "高能榜提示",
            "hidden": true
          },
          "switch-skin": {
            "defaultValue": false,
            "displayName": "房间皮肤",
            "hidden": true
          },
          "simplifyOptions": {
            "defaultValue": {
              "name": "simplifyOptions",
              "dimAt": "checked",
              "switchProps": {
                "checkedIcon": "mdi-eye-off-outline",
                "notCheckedIcon": "mdi-eye-outline"
              },
              "switches": {
                "vip": {
                  "defaultValue": true,
                  "displayName": "老爷图标"
                },
                "enterPrompt": {
                  "defaultValue": true,
                  "displayName": "入场通知"
                },
                "fansMedal": {
                  "defaultValue": true,
                  "displayName": "粉丝勋章"
                },
                "title": {
                  "defaultValue": true,
                  "displayName": "活动头衔"
                },
                "guard": {
                  "defaultValue": true,
                  "displayName": "舰长图标"
                },
                "systemMessage": {
                  "defaultValue": true,
                  "displayName": "全区广播"
                },
                "welcomeMessage": {
                  "defaultValue": true,
                  "displayName": "欢迎信息"
                },
                "giftMessage": {
                  "defaultValue": true,
                  "displayName": "礼物弹幕"
                },
                "emoticons": {
                  "defaultValue": true,
                  "displayName": "表情特效"
                },
                "guardPurchase": {
                  "defaultValue": true,
                  "displayName": "上舰提示"
                },
                "giftPanel": {
                  "defaultValue": true,
                  "displayName": "付费礼物"
                },
                "headerPanel": {
                  "defaultValue": false,
                  "displayName": "标题栏活动"
                },
                "userEffect": {
                  "defaultValue": true,
                  "displayName": "入场特效"
                },
                "kanban": {
                  "defaultValue": true,
                  "displayName": "看板娘"
                },
                "eventsBanner": {
                  "defaultValue": false,
                  "displayName": "活动横幅"
                },
                "rankList": {
                  "defaultValue": false,
                  "displayName": "排行榜"
                },
                "popup": {
                  "defaultValue": false,
                  "displayName": "抽奖提示"
                },
                "pk": {
                  "defaultValue": false,
                  "displayName": "PK浮窗"
                },
                "topRank": {
                  "defaultValue": false,
                  "displayName": "高能榜提示"
                },
                "skin": {
                  "defaultValue": false,
                  "displayName": "房间皮肤"
                }
              },
              "radio": false,
              "componentName": "simplifyLiveroom",
              "optionDisplayName": "简化直播间选项"
            },
            "displayName": "简化直播间选项"
          }
        }
      },
      "settings": {
        "enabled": true,
        "options": {
          "switch-vip": true,
          "switch-enterPrompt": true,
          "switch-fansMedal": true,
          "switch-title": true,
          "switch-guard": true,
          "switch-systemMessage": true,
          "switch-welcomeMessage": true,
          "switch-giftMessage": true,
          "switch-emoticons": true,
          "switch-guardPurchase": true,
          "switch-giftPanel": true,
          "switch-headerPanel": false,
          "switch-userEffect": true,
          "switch-kanban": true,
          "switch-eventsBanner": false,
          "switch-rankList": false,
          "switch-popup": false,
          "switch-pk": false,
          "switch-topRank": false,
          "switch-skin": false,
          "simplifyOptions": {
            "name": "simplifyOptions",
            "dimAt": "checked",
            "switchProps": {
              "checkedIcon": "mdi-eye-off-outline",
              "notCheckedIcon": "mdi-eye-outline"
            },
            "switches": {
              "vip": {
                "defaultValue": true,
                "displayName": "老爷图标"
              },
              "enterPrompt": {
                "defaultValue": true,
                "displayName": "入场通知"
              },
              "fansMedal": {
                "defaultValue": true,
                "displayName": "粉丝勋章"
              },
              "title": {
                "defaultValue": true,
                "displayName": "活动头衔"
              },
              "guard": {
                "defaultValue": true,
                "displayName": "舰长图标"
              },
              "systemMessage": {
                "defaultValue": true,
                "displayName": "全区广播"
              },
              "welcomeMessage": {
                "defaultValue": true,
                "displayName": "欢迎信息"
              },
              "giftMessage": {
                "defaultValue": true,
                "displayName": "礼物弹幕"
              },
              "emoticons": {
                "defaultValue": true,
                "displayName": "表情特效"
              },
              "guardPurchase": {
                "defaultValue": true,
                "displayName": "上舰提示"
              },
              "giftPanel": {
                "defaultValue": true,
                "displayName": "付费礼物"
              },
              "headerPanel": {
                "defaultValue": false,
                "displayName": "标题栏活动"
              },
              "userEffect": {
                "defaultValue": true,
                "displayName": "入场特效"
              },
              "kanban": {
                "defaultValue": true,
                "displayName": "看板娘"
              },
              "eventsBanner": {
                "defaultValue": false,
                "displayName": "活动横幅"
              },
              "rankList": {
                "defaultValue": false,
                "displayName": "排行榜"
              },
              "popup": {
                "defaultValue": false,
                "displayName": "抽奖提示"
              },
              "pk": {
                "defaultValue": false,
                "displayName": "PK浮窗"
              },
              "topRank": {
                "defaultValue": false,
                "displayName": "高能榜提示"
              },
              "skin": {
                "defaultValue": false,
                "displayName": "房间皮肤"
              }
            },
            "radio": false,
            "componentName": "simplifyLiveroom",
            "optionDisplayName": "简化直播间选项"
          }
        }
      }
    },
    "skipChargeList": {
      "code": "!function(e,t){\"object\"==typeof exports&&\"object\"==typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define([],t):\"object\"==typeof exports?exports[\"video/player/skip-charge-list\"]=t():e[\"video/player/skip-charge-list\"]=t()}(globalThis,(()=>(()=>{var e,t,o={72:(e,t,o)=>{var r=o(355)((function(e){return e[1]}));r.push([e.id,\"body:not(.skip-charge-list-disable) .bilibili-player .bilibili-player-electric-panel,\\nbody:not(.skip-charge-list-disable) #bilibili-player .bpx-player-electric-panel {\\n  display: none !important;\\n}\",\"\"]),e.exports=r},355:e=>{\"use strict\";\n// eslint-disable-next-line func-names\ne.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var o=e(t);return t[2]?\"@media \".concat(t[2],\" {\").concat(o,\"}\"):o})).join(\"\")},\n// eslint-disable-next-line func-names\nt.i=function(e,o,r){\"string\"==typeof e&&(\n// eslint-disable-next-line no-param-reassign\ne=[[null,e,\"\"]]);var n={};if(r)for(var i=0;i<this.length;i++){\n// eslint-disable-next-line prefer-destructuring\nvar a=this[i][0];null!=a&&(n[a]=!0)}for(var s=0;s<e.length;s++){var c=[].concat(e[s]);r&&n[c[0]]||(o&&(c[2]?c[2]=\"\".concat(o,\" and \").concat(c[2]):c[2]=o),t.push(c))}},t}},147:(e,t,o)=>{var r=o(72);r&&r.__esModule&&(r=r.default),e.exports=\"string\"==typeof r?r:r.toString()},391:e=>{\"use strict\";e.exports=coreApis.observer},200:e=>{\"use strict\";e.exports=coreApis.spinQuery}},r={};function n(e){var t=r[e];if(void 0!==t)return t.exports;var i=r[e]={id:e,exports:{}};return o[e](i,i.exports,n),i.exports}t=Object.getPrototypeOf?e=>Object.getPrototypeOf(e):e=>e.__proto__,n.t=function(o,r){if(1&r&&(o=this(o)),8&r)return o;if(\"object\"==typeof o&&o){if(4&r&&o.__esModule)return o;if(16&r&&\"function\"==typeof o.then)return o}var i=Object.create(null);n.r(i);var a={};e=e||[null,t({}),t([]),t(t)];for(var s=2&r&&o;\"object\"==typeof s&&!~e.indexOf(s);s=t(s))Object.getOwnPropertyNames(s).forEach((e=>a[e]=()=>o[e]));return a.default=()=>o,n.d(i,a),i},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.r=e=>{\"undefined\"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:\"Module\"}),Object.defineProperty(e,\"__esModule\",{value:!0})};var i={};return(()=>{\"use strict\";n.d(i,{component:()=>s});const e=coreApis.componentApis.define,t=coreApis.componentApis.styledComponent,o=coreApis.utils.urls,r=\"skip-charge-list-disable\",a=(0,t.styledComponentEntry)((()=>Promise.resolve().then(n.t.bind(n,147,23))),(async()=>{const{videoChange:e}=await Promise.resolve().then(n.t.bind(n,391,23)),{select:t}=await Promise.resolve().then(n.t.bind(n,200,23));e((async()=>{(await t(\"video\"))?.addEventListener(\"ended\",(async()=>{if(document.body.classList.contains(r))return;(await t(\".bilibili-player-electric-panel-jump,.bpx-player-electric-jump\"))?.click()}))}))})),s=(0,e.defineComponentMetadata)({name:\"skipChargeList\",displayName:\"跳过充电鸣谢\",tags:[componentsTags.video],entry:a,description:{\"zh-CN\":\"自动跳过视频结尾的充电鸣谢. 注意: 不包括番剧承包鸣谢.\"},reload:()=>document.body.classList.remove(r),unload:()=>document.body.classList.add(r),urlInclude:o.playerUrls,commitHash:\"89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9\",coreVersion:\"2.5.2\"})})(),i=i.component})()));",
      "metadata": {
        "name": "skipChargeList",
        "displayName": "跳过充电鸣谢",
        "tags": [
          {
            "name": "video",
            "displayName": "视频",
            "color": "#2196F3",
            "icon": "mdi-play-circle-outline",
            "order": 1
          }
        ],
        "description": {
          "zh-CN": "自动跳过视频结尾的充电鸣谢. 注意: 不包括番剧承包鸣谢."
        },
        "commitHash": "89d37a1f2324e2617e2ad5d6de2a12e0a0736dc9",
        "coreVersion": "2.5.2"
      },
      "settings": {
        "enabled": true,
        "options": {}
      }
    }
  },
  "components": {
    "settingsPanel": {
      "enabled": true,
      "options": {
        "themeColor": "#00A0D8",
        "scriptLoadingMode": "延后",
        "styleLoadingMode": "同时",
        "textColor": "自动",
        "cdnRoot": "AltCdn",
        "dockSide": "左侧",
        "filenameFormat": "[title][ - ep]",
        "batchFilenameFormat": "[n - ][ep]",
        "downloadPackageEmitMode": "打包下载",
        "devMode": false
      }
    },
    "launchBar": {
      "enabled": true,
      "options": {}
    },
    "i18n": {
      "enabled": true,
      "options": {
        "language": "简体中文",
        "translator": "GoogleCN"
      }
    },
    "autoUpdate": {
      "enabled": true,
      "options": {
        "lastUpdateCheck": 1669531186960,
        "lastInstalledVersion": "2.5.2",
        "localPortOverride": "",
        "minimumDuration": 86400000,
        "urls": {
          "components": {
            "hideRecommendedLive": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/hide/video/recommended-live.js",
              "lastUpdateCheck": 1669531270581,
              "installTime": 1669531270581,
              "alwaysUpdate": false
            },
            "collapseLiveSideBar": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/live/side-bar.js",
              "lastUpdateCheck": 1669531270626,
              "installTime": 1669531270626,
              "alwaysUpdate": false
            },
            "hideRelatedVideos": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/hide/video/related-videos.js",
              "lastUpdateCheck": 1669531270680,
              "installTime": 1669531270680,
              "alwaysUpdate": false
            },
            "hideVideoTopMask": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/hide/video/top-mask.js",
              "lastUpdateCheck": 1669531270704,
              "installTime": 1669531270704,
              "alwaysUpdate": false
            },
            "disableSpecialDanmaku": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/special-danmaku.js",
              "lastUpdateCheck": 1669531270718,
              "installTime": 1669531270718,
              "alwaysUpdate": false
            },
            "removePlayerPopup": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/video/player/remove-popup.js",
              "lastUpdateCheck": 1669531270739,
              "installTime": 1669531270739,
              "alwaysUpdate": false
            },
            "removePromotions": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/utils/remove-promotions.js",
              "lastUpdateCheck": 1669531270755,
              "installTime": 1669531270755,
              "alwaysUpdate": false
            },
            "simplifyComments": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/simplify/comments.js",
              "lastUpdateCheck": 1669531270772,
              "installTime": 1669531270772,
              "alwaysUpdate": false
            },
            "removeLiveWatermark": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/live/remove-watermark.js",
              "lastUpdateCheck": 1669531270785,
              "installTime": 1669531270785,
              "alwaysUpdate": false
            },
            "simplifyHome": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/simplify/home.js",
              "lastUpdateCheck": 1669531270816,
              "installTime": 1669531270816,
              "alwaysUpdate": false
            },
            "simplifyLiveroom": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/style/simplify/live.js",
              "lastUpdateCheck": 1669531270881,
              "installTime": 1669531270882,
              "alwaysUpdate": false
            },
            "skipChargeList": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/components/video/player/skip-charge-list.js",
              "lastUpdateCheck": 1669533736676,
              "installTime": 1669533736676,
              "alwaysUpdate": false
            }
          },
          "plugins": {
            "downloadVideo.outputs.aria2": {
              "url": "https://fastly.jsdelivr.net/gh/the1812/Bilibili-Evolved@master/registry/dist/plugins/video/download/aria2-output.js",
              "lastUpdateCheck": 1669533719648,
              "installTime": 1669533719648,
              "alwaysUpdate": false
            }
          },
          "styles": {}
        },
        "maxUpdateCount": 4
      }
    },
    "notifyNewVersion": {
      "enabled": true,
      "options": {
        "lastUpdateCheck": 1669531188135,
        "minimumDuration": 86400000
      }
    }
  },
  "plugins": {
    "ajaxHook": true,
    "launchBar.actions.IDSearch": true
  }
}