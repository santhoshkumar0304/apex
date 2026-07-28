<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Apex Fashion — Curated Accessories</title>
<style>
  * { box-sizing: border-box; }
  body { margin: 0; }
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');
</style>
</head>
<body>
<div id="root"></div>
<script>
/**
 * @license React
 * react.production.min.js
 *
 * Copyright (c) Facebook, Inc. and its affiliates.
 *
 * This source code is licensed under the MIT license found in the
 * LICENSE file in the root directory of this source tree.
 */
(function(){'use strict';(function(c,x){"object"===typeof exports&&"undefined"!==typeof module?x(exports):"function"===typeof define&&define.amd?define(["exports"],x):(c=c||self,x(c.React={}))})(this,function(c){function x(a){if(null===a||"object"!==typeof a)return null;a=V&&a[V]||a["@@iterator"];return"function"===typeof a?a:null}function w(a,b,e){this.props=a;this.context=b;this.refs=W;this.updater=e||X}function Y(){}function K(a,b,e){this.props=a;this.context=b;this.refs=W;this.updater=e||X}function Z(a,b,
e){var m,d={},c=null,h=null;if(null!=b)for(m in void 0!==b.ref&&(h=b.ref),void 0!==b.key&&(c=""+b.key),b)aa.call(b,m)&&!ba.hasOwnProperty(m)&&(d[m]=b[m]);var l=arguments.length-2;if(1===l)d.children=e;else if(1<l){for(var f=Array(l),k=0;k<l;k++)f[k]=arguments[k+2];d.children=f}if(a&&a.defaultProps)for(m in l=a.defaultProps,l)void 0===d[m]&&(d[m]=l[m]);return{$$typeof:y,type:a,key:c,ref:h,props:d,_owner:L.current}}function oa(a,b){return{$$typeof:y,type:a.type,key:b,ref:a.ref,props:a.props,_owner:a._owner}}
function M(a){return"object"===typeof a&&null!==a&&a.$$typeof===y}function pa(a){var b={"=":"=0",":":"=2"};return"$"+a.replace(/[=:]/g,function(a){return b[a]})}function N(a,b){return"object"===typeof a&&null!==a&&null!=a.key?pa(""+a.key):b.toString(36)}function B(a,b,e,m,d){var c=typeof a;if("undefined"===c||"boolean"===c)a=null;var h=!1;if(null===a)h=!0;else switch(c){case "string":case "number":h=!0;break;case "object":switch(a.$$typeof){case y:case qa:h=!0}}if(h)return h=a,d=d(h),a=""===m?"."+
N(h,0):m,ca(d)?(e="",null!=a&&(e=a.replace(da,"$&/")+"/"),B(d,b,e,"",function(a){return a})):null!=d&&(M(d)&&(d=oa(d,e+(!d.key||h&&h.key===d.key?"":(""+d.key).replace(da,"$&/")+"/")+a)),b.push(d)),1;h=0;m=""===m?".":m+":";if(ca(a))for(var l=0;l<a.length;l++){c=a[l];var f=m+N(c,l);h+=B(c,b,e,f,d)}else if(f=x(a),"function"===typeof f)for(a=f.call(a),l=0;!(c=a.next()).done;)c=c.value,f=m+N(c,l++),h+=B(c,b,e,f,d);else if("object"===c)throw b=String(a),Error("Objects are not valid as a React child (found: "+
("[object Object]"===b?"object with keys {"+Object.keys(a).join(", ")+"}":b)+"). If you meant to render a collection of children, use an array instead.");return h}function C(a,b,e){if(null==a)return a;var c=[],d=0;B(a,c,"","",function(a){return b.call(e,a,d++)});return c}function ra(a){if(-1===a._status){var b=a._result;b=b();b.then(function(b){if(0===a._status||-1===a._status)a._status=1,a._result=b},function(b){if(0===a._status||-1===a._status)a._status=2,a._result=b});-1===a._status&&(a._status=
0,a._result=b)}if(1===a._status)return a._result.default;throw a._result;}function O(a,b){var e=a.length;a.push(b);a:for(;0<e;){var c=e-1>>>1,d=a[c];if(0<D(d,b))a[c]=b,a[e]=d,e=c;else break a}}function p(a){return 0===a.length?null:a[0]}function E(a){if(0===a.length)return null;var b=a[0],e=a.pop();if(e!==b){a[0]=e;a:for(var c=0,d=a.length,k=d>>>1;c<k;){var h=2*(c+1)-1,l=a[h],f=h+1,g=a[f];if(0>D(l,e))f<d&&0>D(g,l)?(a[c]=g,a[f]=e,c=f):(a[c]=l,a[h]=e,c=h);else if(f<d&&0>D(g,e))a[c]=g,a[f]=e,c=f;else break a}}return b}
function D(a,b){var c=a.sortIndex-b.sortIndex;return 0!==c?c:a.id-b.id}function P(a){for(var b=p(r);null!==b;){if(null===b.callback)E(r);else if(b.startTime<=a)E(r),b.sortIndex=b.expirationTime,O(q,b);else break;b=p(r)}}function Q(a){z=!1;P(a);if(!u)if(null!==p(q))u=!0,R(S);else{var b=p(r);null!==b&&T(Q,b.startTime-a)}}function S(a,b){u=!1;z&&(z=!1,ea(A),A=-1);F=!0;var c=k;try{P(b);for(n=p(q);null!==n&&(!(n.expirationTime>b)||a&&!fa());){var m=n.callback;if("function"===typeof m){n.callback=null;
k=n.priorityLevel;var d=m(n.expirationTime<=b);b=v();"function"===typeof d?n.callback=d:n===p(q)&&E(q);P(b)}else E(q);n=p(q)}if(null!==n)var g=!0;else{var h=p(r);null!==h&&T(Q,h.startTime-b);g=!1}return g}finally{n=null,k=c,F=!1}}function fa(){return v()-ha<ia?!1:!0}function R(a){G=a;H||(H=!0,I())}function T(a,b){A=ja(function(){a(v())},b)}function ka(a){throw Error("act(...) is not supported in production builds of React.");}var y=Symbol.for("react.element"),qa=Symbol.for("react.portal"),sa=Symbol.for("react.fragment"),
ta=Symbol.for("react.strict_mode"),ua=Symbol.for("react.profiler"),va=Symbol.for("react.provider"),wa=Symbol.for("react.context"),xa=Symbol.for("react.forward_ref"),ya=Symbol.for("react.suspense"),za=Symbol.for("react.memo"),Aa=Symbol.for("react.lazy"),V=Symbol.iterator,X={isMounted:function(a){return!1},enqueueForceUpdate:function(a,b,c){},enqueueReplaceState:function(a,b,c,m){},enqueueSetState:function(a,b,c,m){}},la=Object.assign,W={};w.prototype.isReactComponent={};w.prototype.setState=function(a,
b){if("object"!==typeof a&&"function"!==typeof a&&null!=a)throw Error("setState(...): takes an object of state variables to update or a function which returns an object of state variables.");this.updater.enqueueSetState(this,a,b,"setState")};w.prototype.forceUpdate=function(a){this.updater.enqueueForceUpdate(this,a,"forceUpdate")};Y.prototype=w.prototype;var t=K.prototype=new Y;t.constructor=K;la(t,w.prototype);t.isPureReactComponent=!0;var ca=Array.isArray,aa=Object.prototype.hasOwnProperty,L={current:null},
ba={key:!0,ref:!0,__self:!0,__source:!0},da=/\/+/g,g={current:null},J={transition:null};if("object"===typeof performance&&"function"===typeof performance.now){var Ba=performance;var v=function(){return Ba.now()}}else{var ma=Date,Ca=ma.now();v=function(){return ma.now()-Ca}}var q=[],r=[],Da=1,n=null,k=3,F=!1,u=!1,z=!1,ja="function"===typeof setTimeout?setTimeout:null,ea="function"===typeof clearTimeout?clearTimeout:null,na="undefined"!==typeof setImmediate?setImmediate:null;"undefined"!==typeof navigator&&
void 0!==navigator.scheduling&&void 0!==navigator.scheduling.isInputPending&&navigator.scheduling.isInputPending.bind(navigator.scheduling);var H=!1,G=null,A=-1,ia=5,ha=-1,U=function(){if(null!==G){var a=v();ha=a;var b=!0;try{b=G(!0,a)}finally{b?I():(H=!1,G=null)}}else H=!1};if("function"===typeof na)var I=function(){na(U)};else if("undefined"!==typeof MessageChannel){t=new MessageChannel;var Ea=t.port2;t.port1.onmessage=U;I=function(){Ea.postMessage(null)}}else I=function(){ja(U,0)};t={ReactCurrentDispatcher:g,
ReactCurrentOwner:L,ReactCurrentBatchConfig:J,Scheduler:{__proto__:null,unstable_ImmediatePriority:1,unstable_UserBlockingPriority:2,unstable_NormalPriority:3,unstable_IdlePriority:5,unstable_LowPriority:4,unstable_runWithPriority:function(a,b){switch(a){case 1:case 2:case 3:case 4:case 5:break;default:a=3}var c=k;k=a;try{return b()}finally{k=c}},unstable_next:function(a){switch(k){case 1:case 2:case 3:var b=3;break;default:b=k}var c=k;k=b;try{return a()}finally{k=c}},unstable_scheduleCallback:function(a,
b,c){var e=v();"object"===typeof c&&null!==c?(c=c.delay,c="number"===typeof c&&0<c?e+c:e):c=e;switch(a){case 1:var d=-1;break;case 2:d=250;break;case 5:d=1073741823;break;case 4:d=1E4;break;default:d=5E3}d=c+d;a={id:Da++,callback:b,priorityLevel:a,startTime:c,expirationTime:d,sortIndex:-1};c>e?(a.sortIndex=c,O(r,a),null===p(q)&&a===p(r)&&(z?(ea(A),A=-1):z=!0,T(Q,c-e))):(a.sortIndex=d,O(q,a),u||F||(u=!0,R(S)));return a},unstable_cancelCallback:function(a){a.callback=null},unstable_wrapCallback:function(a){var b=
k;return function(){var c=k;k=b;try{return a.apply(this,arguments)}finally{k=c}}},unstable_getCurrentPriorityLevel:function(){return k},unstable_shouldYield:fa,unstable_requestPaint:function(){},unstable_continueExecution:function(){u||F||(u=!0,R(S))},unstable_pauseExecution:function(){},unstable_getFirstCallbackNode:function(){return p(q)},get unstable_now(){return v},unstable_forceFrameRate:function(a){0>a||125<a?console.error("forceFrameRate takes a positive int between 0 and 125, forcing frame rates higher than 125 fps is not supported"):
ia=0<a?Math.floor(1E3/a):5},unstable_Profiling:null}};c.Children={map:C,forEach:function(a,b,c){C(a,function(){b.apply(this,arguments)},c)},count:function(a){var b=0;C(a,function(){b++});return b},toArray:function(a){return C(a,function(a){return a})||[]},only:function(a){if(!M(a))throw Error("React.Children.only expected to receive a single React element child.");return a}};c.Component=w;c.Fragment=sa;c.Profiler=ua;c.PureComponent=K;c.StrictMode=ta;c.Suspense=ya;c.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=
t;c.act=ka;c.cloneElement=function(a,b,c){if(null===a||void 0===a)throw Error("React.cloneElement(...): The argument must be a React element, but you passed "+a+".");var e=la({},a.props),d=a.key,k=a.ref,h=a._owner;if(null!=b){void 0!==b.ref&&(k=b.ref,h=L.current);void 0!==b.key&&(d=""+b.key);if(a.type&&a.type.defaultProps)var l=a.type.defaultProps;for(f in b)aa.call(b,f)&&!ba.hasOwnProperty(f)&&(e[f]=void 0===b[f]&&void 0!==l?l[f]:b[f])}var f=arguments.length-2;if(1===f)e.children=c;else if(1<f){l=
Array(f);for(var g=0;g<f;g++)l[g]=arguments[g+2];e.children=l}return{$$typeof:y,type:a.type,key:d,ref:k,props:e,_owner:h}};c.createContext=function(a){a={$$typeof:wa,_currentValue:a,_currentValue2:a,_threadCount:0,Provider:null,Consumer:null,_defaultValue:null,_globalName:null};a.Provider={$$typeof:va,_context:a};return a.Consumer=a};c.createElement=Z;c.createFactory=function(a){var b=Z.bind(null,a);b.type=a;return b};c.createRef=function(){return{current:null}};c.forwardRef=function(a){return{$$typeof:xa,
render:a}};c.isValidElement=M;c.lazy=function(a){return{$$typeof:Aa,_payload:{_status:-1,_result:a},_init:ra}};c.memo=function(a,b){return{$$typeof:za,type:a,compare:void 0===b?null:b}};c.startTransition=function(a,b){b=J.transition;J.transition={};try{a()}finally{J.transition=b}};c.unstable_act=ka;c.useCallback=function(a,b){return g.current.useCallback(a,b)};c.useContext=function(a){return g.current.useContext(a)};c.useDebugValue=function(a,b){};c.useDeferredValue=function(a){return g.current.useDeferredValue(a)};
c.useEffect=function(a,b){return g.current.useEffect(a,b)};c.useId=function(){return g.current.useId()};c.useImperativeHandle=function(a,b,c){return g.current.useImperativeHandle(a,b,c)};c.useInsertionEffect=function(a,b){return g.current.useInsertionEffect(a,b)};c.useLayoutEffect=function(a,b){return g.current.useLayoutEffect(a,b)};c.useMemo=function(a,b){return g.current.useMemo(a,b)};c.useReducer=function(a,b,c){return g.current.useReducer(a,b,c)};c.useRef=function(a){return g.current.useRef(a)};
c.useState=function(a){return g.current.useState(a)};c.useSyncExternalStore=function(a,b,c){return g.current.useSyncExternalStore(a,b,c)};c.useTransition=function(){return g.current.useTransition()};c.version="18.3.1"});
})();

</script>
<script>
/**
 * @license React
 * react-dom.production.min.js
 *
 * Copyright (c) Facebook, Inc. and its affiliates.
 *
 * This source code is licensed under the MIT license found in the
 * LICENSE file in the root directory of this source tree.
 */
(function(){/*
 Modernizr 3.0.0pre (Custom Build) | MIT
*/
'use strict';(function(Q,zb){"object"===typeof exports&&"undefined"!==typeof module?zb(exports,require("react")):"function"===typeof define&&define.amd?define(["exports","react"],zb):(Q=Q||self,zb(Q.ReactDOM={},Q.React))})(this,function(Q,zb){function m(a){for(var b="https://reactjs.org/docs/error-decoder.html?invariant="+a,c=1;c<arguments.length;c++)b+="&args[]="+encodeURIComponent(arguments[c]);return"Minified React error #"+a+"; visit "+b+" for the full message or use the non-minified dev environment for full errors and additional helpful warnings."}
function mb(a,b){Ab(a,b);Ab(a+"Capture",b)}function Ab(a,b){$b[a]=b;for(a=0;a<b.length;a++)cg.add(b[a])}function bj(a){if(Zd.call(dg,a))return!0;if(Zd.call(eg,a))return!1;if(cj.test(a))return dg[a]=!0;eg[a]=!0;return!1}function dj(a,b,c,d){if(null!==c&&0===c.type)return!1;switch(typeof b){case "function":case "symbol":return!0;case "boolean":if(d)return!1;if(null!==c)return!c.acceptsBooleans;a=a.toLowerCase().slice(0,5);return"data-"!==a&&"aria-"!==a;default:return!1}}function ej(a,b,c,d){if(null===
b||"undefined"===typeof b||dj(a,b,c,d))return!0;if(d)return!1;if(null!==c)switch(c.type){case 3:return!b;case 4:return!1===b;case 5:return isNaN(b);case 6:return isNaN(b)||1>b}return!1}function Y(a,b,c,d,e,f,g){this.acceptsBooleans=2===b||3===b||4===b;this.attributeName=d;this.attributeNamespace=e;this.mustUseProperty=c;this.propertyName=a;this.type=b;this.sanitizeURL=f;this.removeEmptyString=g}function $d(a,b,c,d){var e=R.hasOwnProperty(b)?R[b]:null;if(null!==e?0!==e.type:d||!(2<b.length)||"o"!==
b[0]&&"O"!==b[0]||"n"!==b[1]&&"N"!==b[1])ej(b,c,e,d)&&(c=null),d||null===e?bj(b)&&(null===c?a.removeAttribute(b):a.setAttribute(b,""+c)):e.mustUseProperty?a[e.propertyName]=null===c?3===e.type?!1:"":c:(b=e.attributeName,d=e.attributeNamespace,null===c?a.removeAttribute(b):(e=e.type,c=3===e||4===e&&!0===c?"":""+c,d?a.setAttributeNS(d,b,c):a.setAttribute(b,c)))}function ac(a){if(null===a||"object"!==typeof a)return null;a=fg&&a[fg]||a["@@iterator"];return"function"===typeof a?a:null}function bc(a,b,
c){if(void 0===ae)try{throw Error();}catch(d){ae=(b=d.stack.trim().match(/\n( *(at )?)/))&&b[1]||""}return"\n"+ae+a}function be(a,b){if(!a||ce)return"";ce=!0;var c=Error.prepareStackTrace;Error.prepareStackTrace=void 0;try{if(b)if(b=function(){throw Error();},Object.defineProperty(b.prototype,"props",{set:function(){throw Error();}}),"object"===typeof Reflect&&Reflect.construct){try{Reflect.construct(b,[])}catch(n){var d=n}Reflect.construct(a,[],b)}else{try{b.call()}catch(n){d=n}a.call(b.prototype)}else{try{throw Error();
}catch(n){d=n}a()}}catch(n){if(n&&d&&"string"===typeof n.stack){for(var e=n.stack.split("\n"),f=d.stack.split("\n"),g=e.length-1,h=f.length-1;1<=g&&0<=h&&e[g]!==f[h];)h--;for(;1<=g&&0<=h;g--,h--)if(e[g]!==f[h]){if(1!==g||1!==h){do if(g--,h--,0>h||e[g]!==f[h]){var k="\n"+e[g].replace(" at new "," at ");a.displayName&&k.includes("<anonymous>")&&(k=k.replace("<anonymous>",a.displayName));return k}while(1<=g&&0<=h)}break}}}finally{ce=!1,Error.prepareStackTrace=c}return(a=a?a.displayName||a.name:"")?bc(a):
""}function fj(a){switch(a.tag){case 5:return bc(a.type);case 16:return bc("Lazy");case 13:return bc("Suspense");case 19:return bc("SuspenseList");case 0:case 2:case 15:return a=be(a.type,!1),a;case 11:return a=be(a.type.render,!1),a;case 1:return a=be(a.type,!0),a;default:return""}}function de(a){if(null==a)return null;if("function"===typeof a)return a.displayName||a.name||null;if("string"===typeof a)return a;switch(a){case Bb:return"Fragment";case Cb:return"Portal";case ee:return"Profiler";case fe:return"StrictMode";
case ge:return"Suspense";case he:return"SuspenseList"}if("object"===typeof a)switch(a.$$typeof){case gg:return(a.displayName||"Context")+".Consumer";case hg:return(a._context.displayName||"Context")+".Provider";case ie:var b=a.render;a=a.displayName;a||(a=b.displayName||b.name||"",a=""!==a?"ForwardRef("+a+")":"ForwardRef");return a;case je:return b=a.displayName||null,null!==b?b:de(a.type)||"Memo";case Ta:b=a._payload;a=a._init;try{return de(a(b))}catch(c){}}return null}function gj(a){var b=a.type;
switch(a.tag){case 24:return"Cache";case 9:return(b.displayName||"Context")+".Consumer";case 10:return(b._context.displayName||"Context")+".Provider";case 18:return"DehydratedFragment";case 11:return a=b.render,a=a.displayName||a.name||"",b.displayName||(""!==a?"ForwardRef("+a+")":"ForwardRef");case 7:return"Fragment";case 5:return b;case 4:return"Portal";case 3:return"Root";case 6:return"Text";case 16:return de(b);case 8:return b===fe?"StrictMode":"Mode";case 22:return"Offscreen";case 12:return"Profiler";
case 21:return"Scope";case 13:return"Suspense";case 19:return"SuspenseList";case 25:return"TracingMarker";case 1:case 0:case 17:case 2:case 14:case 15:if("function"===typeof b)return b.displayName||b.name||null;if("string"===typeof b)return b}return null}function Ua(a){switch(typeof a){case "boolean":case "number":case "string":case "undefined":return a;case "object":return a;default:return""}}function ig(a){var b=a.type;return(a=a.nodeName)&&"input"===a.toLowerCase()&&("checkbox"===b||"radio"===
b)}function hj(a){var b=ig(a)?"checked":"value",c=Object.getOwnPropertyDescriptor(a.constructor.prototype,b),d=""+a[b];if(!a.hasOwnProperty(b)&&"undefined"!==typeof c&&"function"===typeof c.get&&"function"===typeof c.set){var e=c.get,f=c.set;Object.defineProperty(a,b,{configurable:!0,get:function(){return e.call(this)},set:function(a){d=""+a;f.call(this,a)}});Object.defineProperty(a,b,{enumerable:c.enumerable});return{getValue:function(){return d},setValue:function(a){d=""+a},stopTracking:function(){a._valueTracker=
null;delete a[b]}}}}function Pc(a){a._valueTracker||(a._valueTracker=hj(a))}function jg(a){if(!a)return!1;var b=a._valueTracker;if(!b)return!0;var c=b.getValue();var d="";a&&(d=ig(a)?a.checked?"true":"false":a.value);a=d;return a!==c?(b.setValue(a),!0):!1}function Qc(a){a=a||("undefined"!==typeof document?document:void 0);if("undefined"===typeof a)return null;try{return a.activeElement||a.body}catch(b){return a.body}}function ke(a,b){var c=b.checked;return E({},b,{defaultChecked:void 0,defaultValue:void 0,
value:void 0,checked:null!=c?c:a._wrapperState.initialChecked})}function kg(a,b){var c=null==b.defaultValue?"":b.defaultValue,d=null!=b.checked?b.checked:b.defaultChecked;c=Ua(null!=b.value?b.value:c);a._wrapperState={initialChecked:d,initialValue:c,controlled:"checkbox"===b.type||"radio"===b.type?null!=b.checked:null!=b.value}}function lg(a,b){b=b.checked;null!=b&&$d(a,"checked",b,!1)}function le(a,b){lg(a,b);var c=Ua(b.value),d=b.type;if(null!=c)if("number"===d){if(0===c&&""===a.value||a.value!=
c)a.value=""+c}else a.value!==""+c&&(a.value=""+c);else if("submit"===d||"reset"===d){a.removeAttribute("value");return}b.hasOwnProperty("value")?me(a,b.type,c):b.hasOwnProperty("defaultValue")&&me(a,b.type,Ua(b.defaultValue));null==b.checked&&null!=b.defaultChecked&&(a.defaultChecked=!!b.defaultChecked)}function mg(a,b,c){if(b.hasOwnProperty("value")||b.hasOwnProperty("defaultValue")){var d=b.type;if(!("submit"!==d&&"reset"!==d||void 0!==b.value&&null!==b.value))return;b=""+a._wrapperState.initialValue;
c||b===a.value||(a.value=b);a.defaultValue=b}c=a.name;""!==c&&(a.name="");a.defaultChecked=!!a._wrapperState.initialChecked;""!==c&&(a.name=c)}function me(a,b,c){if("number"!==b||Qc(a.ownerDocument)!==a)null==c?a.defaultValue=""+a._wrapperState.initialValue:a.defaultValue!==""+c&&(a.defaultValue=""+c)}function Db(a,b,c,d){a=a.options;if(b){b={};for(var e=0;e<c.length;e++)b["$"+c[e]]=!0;for(c=0;c<a.length;c++)e=b.hasOwnProperty("$"+a[c].value),a[c].selected!==e&&(a[c].selected=e),e&&d&&(a[c].defaultSelected=
!0)}else{c=""+Ua(c);b=null;for(e=0;e<a.length;e++){if(a[e].value===c){a[e].selected=!0;d&&(a[e].defaultSelected=!0);return}null!==b||a[e].disabled||(b=a[e])}null!==b&&(b.selected=!0)}}function ne(a,b){if(null!=b.dangerouslySetInnerHTML)throw Error(m(91));return E({},b,{value:void 0,defaultValue:void 0,children:""+a._wrapperState.initialValue})}function ng(a,b){var c=b.value;if(null==c){c=b.children;b=b.defaultValue;if(null!=c){if(null!=b)throw Error(m(92));if(cc(c)){if(1<c.length)throw Error(m(93));
c=c[0]}b=c}null==b&&(b="");c=b}a._wrapperState={initialValue:Ua(c)}}function og(a,b){var c=Ua(b.value),d=Ua(b.defaultValue);null!=c&&(c=""+c,c!==a.value&&(a.value=c),null==b.defaultValue&&a.defaultValue!==c&&(a.defaultValue=c));null!=d&&(a.defaultValue=""+d)}function pg(a,b){b=a.textContent;b===a._wrapperState.initialValue&&""!==b&&null!==b&&(a.value=b)}function qg(a){switch(a){case "svg":return"http://www.w3.org/2000/svg";case "math":return"http://www.w3.org/1998/Math/MathML";default:return"http://www.w3.org/1999/xhtml"}}
function oe(a,b){return null==a||"http://www.w3.org/1999/xhtml"===a?qg(b):"http://www.w3.org/2000/svg"===a&&"foreignObject"===b?"http://www.w3.org/1999/xhtml":a}function rg(a,b,c){return null==b||"boolean"===typeof b||""===b?"":c||"number"!==typeof b||0===b||dc.hasOwnProperty(a)&&dc[a]?(""+b).trim():b+"px"}function sg(a,b){a=a.style;for(var c in b)if(b.hasOwnProperty(c)){var d=0===c.indexOf("--"),e=rg(c,b[c],d);"float"===c&&(c="cssFloat");d?a.setProperty(c,e):a[c]=e}}function pe(a,b){if(b){if(ij[a]&&
(null!=b.children||null!=b.dangerouslySetInnerHTML))throw Error(m(137,a));if(null!=b.dangerouslySetInnerHTML){if(null!=b.children)throw Error(m(60));if("object"!==typeof b.dangerouslySetInnerHTML||!("__html"in b.dangerouslySetInnerHTML))throw Error(m(61));}if(null!=b.style&&"object"!==typeof b.style)throw Error(m(62));}}function qe(a,b){if(-1===a.indexOf("-"))return"string"===typeof b.is;switch(a){case "annotation-xml":case "color-profile":case "font-face":case "font-face-src":case "font-face-uri":case "font-face-format":case "font-face-name":case "missing-glyph":return!1;
default:return!0}}function re(a){a=a.target||a.srcElement||window;a.correspondingUseElement&&(a=a.correspondingUseElement);return 3===a.nodeType?a.parentNode:a}function tg(a){if(a=ec(a)){if("function"!==typeof se)throw Error(m(280));var b=a.stateNode;b&&(b=Rc(b),se(a.stateNode,a.type,b))}}function ug(a){Eb?Fb?Fb.push(a):Fb=[a]:Eb=a}function vg(){if(Eb){var a=Eb,b=Fb;Fb=Eb=null;tg(a);if(b)for(a=0;a<b.length;a++)tg(b[a])}}function wg(a,b,c){if(te)return a(b,c);te=!0;try{return xg(a,b,c)}finally{if(te=
!1,null!==Eb||null!==Fb)yg(),vg()}}function fc(a,b){var c=a.stateNode;if(null===c)return null;var d=Rc(c);if(null===d)return null;c=d[b];a:switch(b){case "onClick":case "onClickCapture":case "onDoubleClick":case "onDoubleClickCapture":case "onMouseDown":case "onMouseDownCapture":case "onMouseMove":case "onMouseMoveCapture":case "onMouseUp":case "onMouseUpCapture":case "onMouseEnter":(d=!d.disabled)||(a=a.type,d=!("button"===a||"input"===a||"select"===a||"textarea"===a));a=!d;break a;default:a=!1}if(a)return null;
if(c&&"function"!==typeof c)throw Error(m(231,b,typeof c));return c}function jj(a,b,c,d,e,f,g,h,k){gc=!1;Sc=null;kj.apply(lj,arguments)}function mj(a,b,c,d,e,f,g,h,k){jj.apply(this,arguments);if(gc){if(gc){var n=Sc;gc=!1;Sc=null}else throw Error(m(198));Tc||(Tc=!0,ue=n)}}function nb(a){var b=a,c=a;if(a.alternate)for(;b.return;)b=b.return;else{a=b;do b=a,0!==(b.flags&4098)&&(c=b.return),a=b.return;while(a)}return 3===b.tag?c:null}function zg(a){if(13===a.tag){var b=a.memoizedState;null===b&&(a=a.alternate,
null!==a&&(b=a.memoizedState));if(null!==b)return b.dehydrated}return null}function Ag(a){if(nb(a)!==a)throw Error(m(188));}function nj(a){var b=a.alternate;if(!b){b=nb(a);if(null===b)throw Error(m(188));return b!==a?null:a}for(var c=a,d=b;;){var e=c.return;if(null===e)break;var f=e.alternate;if(null===f){d=e.return;if(null!==d){c=d;continue}break}if(e.child===f.child){for(f=e.child;f;){if(f===c)return Ag(e),a;if(f===d)return Ag(e),b;f=f.sibling}throw Error(m(188));}if(c.return!==d.return)c=e,d=f;
else{for(var g=!1,h=e.child;h;){if(h===c){g=!0;c=e;d=f;break}if(h===d){g=!0;d=e;c=f;break}h=h.sibling}if(!g){for(h=f.child;h;){if(h===c){g=!0;c=f;d=e;break}if(h===d){g=!0;d=f;c=e;break}h=h.sibling}if(!g)throw Error(m(189));}}if(c.alternate!==d)throw Error(m(190));}if(3!==c.tag)throw Error(m(188));return c.stateNode.current===c?a:b}function Bg(a){a=nj(a);return null!==a?Cg(a):null}function Cg(a){if(5===a.tag||6===a.tag)return a;for(a=a.child;null!==a;){var b=Cg(a);if(null!==b)return b;a=a.sibling}return null}
function oj(a,b){if(Ca&&"function"===typeof Ca.onCommitFiberRoot)try{Ca.onCommitFiberRoot(Uc,a,void 0,128===(a.current.flags&128))}catch(c){}}function pj(a){a>>>=0;return 0===a?32:31-(qj(a)/rj|0)|0}function hc(a){switch(a&-a){case 1:return 1;case 2:return 2;case 4:return 4;case 8:return 8;case 16:return 16;case 32:return 32;case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:return a&
4194240;case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:return a&130023424;case 134217728:return 134217728;case 268435456:return 268435456;case 536870912:return 536870912;case 1073741824:return 1073741824;default:return a}}function Vc(a,b){var c=a.pendingLanes;if(0===c)return 0;var d=0,e=a.suspendedLanes,f=a.pingedLanes,g=c&268435455;if(0!==g){var h=g&~e;0!==h?d=hc(h):(f&=g,0!==f&&(d=hc(f)))}else g=c&~e,0!==g?d=hc(g):0!==f&&(d=hc(f));if(0===d)return 0;if(0!==b&&b!==d&&0===(b&e)&&
(e=d&-d,f=b&-b,e>=f||16===e&&0!==(f&4194240)))return b;0!==(d&4)&&(d|=c&16);b=a.entangledLanes;if(0!==b)for(a=a.entanglements,b&=d;0<b;)c=31-ta(b),e=1<<c,d|=a[c],b&=~e;return d}function sj(a,b){switch(a){case 1:case 2:case 4:return b+250;case 8:case 16:case 32:case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:return b+5E3;case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:return-1;
case 134217728:case 268435456:case 536870912:case 1073741824:return-1;default:return-1}}function tj(a,b){for(var c=a.suspendedLanes,d=a.pingedLanes,e=a.expirationTimes,f=a.pendingLanes;0<f;){var g=31-ta(f),h=1<<g,k=e[g];if(-1===k){if(0===(h&c)||0!==(h&d))e[g]=sj(h,b)}else k<=b&&(a.expiredLanes|=h);f&=~h}}function ve(a){a=a.pendingLanes&-1073741825;return 0!==a?a:a&1073741824?1073741824:0}function Dg(){var a=Wc;Wc<<=1;0===(Wc&4194240)&&(Wc=64);return a}function we(a){for(var b=[],c=0;31>c;c++)b.push(a);
return b}function ic(a,b,c){a.pendingLanes|=b;536870912!==b&&(a.suspendedLanes=0,a.pingedLanes=0);a=a.eventTimes;b=31-ta(b);a[b]=c}function uj(a,b){var c=a.pendingLanes&~b;a.pendingLanes=b;a.suspendedLanes=0;a.pingedLanes=0;a.expiredLanes&=b;a.mutableReadLanes&=b;a.entangledLanes&=b;b=a.entanglements;var d=a.eventTimes;for(a=a.expirationTimes;0<c;){var e=31-ta(c),f=1<<e;b[e]=0;d[e]=-1;a[e]=-1;c&=~f}}function xe(a,b){var c=a.entangledLanes|=b;for(a=a.entanglements;c;){var d=31-ta(c),e=1<<d;e&b|a[d]&
b&&(a[d]|=b);c&=~e}}function Eg(a){a&=-a;return 1<a?4<a?0!==(a&268435455)?16:536870912:4:1}function Fg(a,b){switch(a){case "focusin":case "focusout":Va=null;break;case "dragenter":case "dragleave":Wa=null;break;case "mouseover":case "mouseout":Xa=null;break;case "pointerover":case "pointerout":jc.delete(b.pointerId);break;case "gotpointercapture":case "lostpointercapture":kc.delete(b.pointerId)}}function lc(a,b,c,d,e,f){if(null===a||a.nativeEvent!==f)return a={blockedOn:b,domEventName:c,eventSystemFlags:d,
nativeEvent:f,targetContainers:[e]},null!==b&&(b=ec(b),null!==b&&Gg(b)),a;a.eventSystemFlags|=d;b=a.targetContainers;null!==e&&-1===b.indexOf(e)&&b.push(e);return a}function vj(a,b,c,d,e){switch(b){case "focusin":return Va=lc(Va,a,b,c,d,e),!0;case "dragenter":return Wa=lc(Wa,a,b,c,d,e),!0;case "mouseover":return Xa=lc(Xa,a,b,c,d,e),!0;case "pointerover":var f=e.pointerId;jc.set(f,lc(jc.get(f)||null,a,b,c,d,e));return!0;case "gotpointercapture":return f=e.pointerId,kc.set(f,lc(kc.get(f)||null,a,b,
c,d,e)),!0}return!1}function Hg(a){var b=ob(a.target);if(null!==b){var c=nb(b);if(null!==c)if(b=c.tag,13===b){if(b=zg(c),null!==b){a.blockedOn=b;wj(a.priority,function(){xj(c)});return}}else if(3===b&&c.stateNode.current.memoizedState.isDehydrated){a.blockedOn=3===c.tag?c.stateNode.containerInfo:null;return}}a.blockedOn=null}function Xc(a){if(null!==a.blockedOn)return!1;for(var b=a.targetContainers;0<b.length;){var c=ye(a.domEventName,a.eventSystemFlags,b[0],a.nativeEvent);if(null===c){c=a.nativeEvent;
var d=new c.constructor(c.type,c);ze=d;c.target.dispatchEvent(d);ze=null}else return b=ec(c),null!==b&&Gg(b),a.blockedOn=c,!1;b.shift()}return!0}function Ig(a,b,c){Xc(a)&&c.delete(b)}function yj(){Ae=!1;null!==Va&&Xc(Va)&&(Va=null);null!==Wa&&Xc(Wa)&&(Wa=null);null!==Xa&&Xc(Xa)&&(Xa=null);jc.forEach(Ig);kc.forEach(Ig)}function mc(a,b){a.blockedOn===b&&(a.blockedOn=null,Ae||(Ae=!0,Jg(Kg,yj)))}function nc(a){if(0<Yc.length){mc(Yc[0],a);for(var b=1;b<Yc.length;b++){var c=Yc[b];c.blockedOn===a&&(c.blockedOn=
null)}}null!==Va&&mc(Va,a);null!==Wa&&mc(Wa,a);null!==Xa&&mc(Xa,a);b=function(b){return mc(b,a)};jc.forEach(b);kc.forEach(b);for(b=0;b<Ya.length;b++)c=Ya[b],c.blockedOn===a&&(c.blockedOn=null);for(;0<Ya.length&&(b=Ya[0],null===b.blockedOn);)Hg(b),null===b.blockedOn&&Ya.shift()}function zj(a,b,c,d){var e=z,f=Gb.transition;Gb.transition=null;try{z=1,Be(a,b,c,d)}finally{z=e,Gb.transition=f}}function Aj(a,b,c,d){var e=z,f=Gb.transition;Gb.transition=null;try{z=4,Be(a,b,c,d)}finally{z=e,Gb.transition=
f}}function Be(a,b,c,d){if(Zc){var e=ye(a,b,c,d);if(null===e)Ce(a,b,d,$c,c),Fg(a,d);else if(vj(e,a,b,c,d))d.stopPropagation();else if(Fg(a,d),b&4&&-1<Bj.indexOf(a)){for(;null!==e;){var f=ec(e);null!==f&&Cj(f);f=ye(a,b,c,d);null===f&&Ce(a,b,d,$c,c);if(f===e)break;e=f}null!==e&&d.stopPropagation()}else Ce(a,b,d,null,c)}}function ye(a,b,c,d){$c=null;a=re(d);a=ob(a);if(null!==a)if(b=nb(a),null===b)a=null;else if(c=b.tag,13===c){a=zg(b);if(null!==a)return a;a=null}else if(3===c){if(b.stateNode.current.memoizedState.isDehydrated)return 3===
b.tag?b.stateNode.containerInfo:null;a=null}else b!==a&&(a=null);$c=a;return null}function Lg(a){switch(a){case "cancel":case "click":case "close":case "contextmenu":case "copy":case "cut":case "auxclick":case "dblclick":case "dragend":case "dragstart":case "drop":case "focusin":case "focusout":case "input":case "invalid":case "keydown":case "keypress":case "keyup":case "mousedown":case "mouseup":case "paste":case "pause":case "play":case "pointercancel":case "pointerdown":case "pointerup":case "ratechange":case "reset":case "resize":case "seeked":case "submit":case "touchcancel":case "touchend":case "touchstart":case "volumechange":case "change":case "selectionchange":case "textInput":case "compositionstart":case "compositionend":case "compositionupdate":case "beforeblur":case "afterblur":case "beforeinput":case "blur":case "fullscreenchange":case "focus":case "hashchange":case "popstate":case "select":case "selectstart":return 1;
case "drag":case "dragenter":case "dragexit":case "dragleave":case "dragover":case "mousemove":case "mouseout":case "mouseover":case "pointermove":case "pointerout":case "pointerover":case "scroll":case "toggle":case "touchmove":case "wheel":case "mouseenter":case "mouseleave":case "pointerenter":case "pointerleave":return 4;case "message":switch(Dj()){case De:return 1;case Mg:return 4;case ad:case Ej:return 16;case Ng:return 536870912;default:return 16}default:return 16}}function Og(){if(bd)return bd;
var a,b=Ee,c=b.length,d,e="value"in Za?Za.value:Za.textContent,f=e.length;for(a=0;a<c&&b[a]===e[a];a++);var g=c-a;for(d=1;d<=g&&b[c-d]===e[f-d];d++);return bd=e.slice(a,1<d?1-d:void 0)}function cd(a){var b=a.keyCode;"charCode"in a?(a=a.charCode,0===a&&13===b&&(a=13)):a=b;10===a&&(a=13);return 32<=a||13===a?a:0}function dd(){return!0}function Pg(){return!1}function ka(a){function b(b,d,e,f,g){this._reactName=b;this._targetInst=e;this.type=d;this.nativeEvent=f;this.target=g;this.currentTarget=null;
for(var c in a)a.hasOwnProperty(c)&&(b=a[c],this[c]=b?b(f):f[c]);this.isDefaultPrevented=(null!=f.defaultPrevented?f.defaultPrevented:!1===f.returnValue)?dd:Pg;this.isPropagationStopped=Pg;return this}E(b.prototype,{preventDefault:function(){this.defaultPrevented=!0;var a=this.nativeEvent;a&&(a.preventDefault?a.preventDefault():"unknown"!==typeof a.returnValue&&(a.returnValue=!1),this.isDefaultPrevented=dd)},stopPropagation:function(){var a=this.nativeEvent;a&&(a.stopPropagation?a.stopPropagation():
"unknown"!==typeof a.cancelBubble&&(a.cancelBubble=!0),this.isPropagationStopped=dd)},persist:function(){},isPersistent:dd});return b}function Fj(a){var b=this.nativeEvent;return b.getModifierState?b.getModifierState(a):(a=Gj[a])?!!b[a]:!1}function Fe(a){return Fj}function Qg(a,b){switch(a){case "keyup":return-1!==Hj.indexOf(b.keyCode);case "keydown":return 229!==b.keyCode;case "keypress":case "mousedown":case "focusout":return!0;default:return!1}}function Rg(a){a=a.detail;return"object"===typeof a&&
"data"in a?a.data:null}function Ij(a,b){switch(a){case "compositionend":return Rg(b);case "keypress":if(32!==b.which)return null;Sg=!0;return Tg;case "textInput":return a=b.data,a===Tg&&Sg?null:a;default:return null}}function Jj(a,b){if(Hb)return"compositionend"===a||!Ge&&Qg(a,b)?(a=Og(),bd=Ee=Za=null,Hb=!1,a):null;switch(a){case "paste":return null;case "keypress":if(!(b.ctrlKey||b.altKey||b.metaKey)||b.ctrlKey&&b.altKey){if(b.char&&1<b.char.length)return b.char;if(b.which)return String.fromCharCode(b.which)}return null;
case "compositionend":return Ug&&"ko"!==b.locale?null:b.data;default:return null}}function Vg(a){var b=a&&a.nodeName&&a.nodeName.toLowerCase();return"input"===b?!!Kj[a.type]:"textarea"===b?!0:!1}function Lj(a){if(!Ia)return!1;a="on"+a;var b=a in document;b||(b=document.createElement("div"),b.setAttribute(a,"return;"),b="function"===typeof b[a]);return b}function Wg(a,b,c,d){ug(d);b=ed(b,"onChange");0<b.length&&(c=new He("onChange","change",null,c,d),a.push({event:c,listeners:b}))}function Mj(a){Xg(a,
0)}function fd(a){var b=Ib(a);if(jg(b))return a}function Nj(a,b){if("change"===a)return b}function Yg(){oc&&(oc.detachEvent("onpropertychange",Zg),pc=oc=null)}function Zg(a){if("value"===a.propertyName&&fd(pc)){var b=[];Wg(b,pc,a,re(a));wg(Mj,b)}}function Oj(a,b,c){"focusin"===a?(Yg(),oc=b,pc=c,oc.attachEvent("onpropertychange",Zg)):"focusout"===a&&Yg()}function Pj(a,b){if("selectionchange"===a||"keyup"===a||"keydown"===a)return fd(pc)}function Qj(a,b){if("click"===a)return fd(b)}function Rj(a,b){if("input"===
a||"change"===a)return fd(b)}function Sj(a,b){return a===b&&(0!==a||1/a===1/b)||a!==a&&b!==b}function qc(a,b){if(ua(a,b))return!0;if("object"!==typeof a||null===a||"object"!==typeof b||null===b)return!1;var c=Object.keys(a),d=Object.keys(b);if(c.length!==d.length)return!1;for(d=0;d<c.length;d++){var e=c[d];if(!Zd.call(b,e)||!ua(a[e],b[e]))return!1}return!0}function $g(a){for(;a&&a.firstChild;)a=a.firstChild;return a}function ah(a,b){var c=$g(a);a=0;for(var d;c;){if(3===c.nodeType){d=a+c.textContent.length;
if(a<=b&&d>=b)return{node:c,offset:b-a};a=d}a:{for(;c;){if(c.nextSibling){c=c.nextSibling;break a}c=c.parentNode}c=void 0}c=$g(c)}}function bh(a,b){return a&&b?a===b?!0:a&&3===a.nodeType?!1:b&&3===b.nodeType?bh(a,b.parentNode):"contains"in a?a.contains(b):a.compareDocumentPosition?!!(a.compareDocumentPosition(b)&16):!1:!1}function ch(){for(var a=window,b=Qc();b instanceof a.HTMLIFrameElement;){try{var c="string"===typeof b.contentWindow.location.href}catch(d){c=!1}if(c)a=b.contentWindow;else break;
b=Qc(a.document)}return b}function Ie(a){var b=a&&a.nodeName&&a.nodeName.toLowerCase();return b&&("input"===b&&("text"===a.type||"search"===a.type||"tel"===a.type||"url"===a.type||"password"===a.type)||"textarea"===b||"true"===a.contentEditable)}function Tj(a){var b=ch(),c=a.focusedElem,d=a.selectionRange;if(b!==c&&c&&c.ownerDocument&&bh(c.ownerDocument.documentElement,c)){if(null!==d&&Ie(c))if(b=d.start,a=d.end,void 0===a&&(a=b),"selectionStart"in c)c.selectionStart=b,c.selectionEnd=Math.min(a,c.value.length);
else if(a=(b=c.ownerDocument||document)&&b.defaultView||window,a.getSelection){a=a.getSelection();var e=c.textContent.length,f=Math.min(d.start,e);d=void 0===d.end?f:Math.min(d.end,e);!a.extend&&f>d&&(e=d,d=f,f=e);e=ah(c,f);var g=ah(c,d);e&&g&&(1!==a.rangeCount||a.anchorNode!==e.node||a.anchorOffset!==e.offset||a.focusNode!==g.node||a.focusOffset!==g.offset)&&(b=b.createRange(),b.setStart(e.node,e.offset),a.removeAllRanges(),f>d?(a.addRange(b),a.extend(g.node,g.offset)):(b.setEnd(g.node,g.offset),
a.addRange(b)))}b=[];for(a=c;a=a.parentNode;)1===a.nodeType&&b.push({element:a,left:a.scrollLeft,top:a.scrollTop});"function"===typeof c.focus&&c.focus();for(c=0;c<b.length;c++)a=b[c],a.element.scrollLeft=a.left,a.element.scrollTop=a.top}}function dh(a,b,c){var d=c.window===c?c.document:9===c.nodeType?c:c.ownerDocument;Je||null==Jb||Jb!==Qc(d)||(d=Jb,"selectionStart"in d&&Ie(d)?d={start:d.selectionStart,end:d.selectionEnd}:(d=(d.ownerDocument&&d.ownerDocument.defaultView||window).getSelection(),d=
{anchorNode:d.anchorNode,anchorOffset:d.anchorOffset,focusNode:d.focusNode,focusOffset:d.focusOffset}),rc&&qc(rc,d)||(rc=d,d=ed(Ke,"onSelect"),0<d.length&&(b=new He("onSelect","select",null,b,c),a.push({event:b,listeners:d}),b.target=Jb)))}function gd(a,b){var c={};c[a.toLowerCase()]=b.toLowerCase();c["Webkit"+a]="webkit"+b;c["Moz"+a]="moz"+b;return c}function hd(a){if(Le[a])return Le[a];if(!Kb[a])return a;var b=Kb[a],c;for(c in b)if(b.hasOwnProperty(c)&&c in eh)return Le[a]=b[c];return a}function $a(a,
b){fh.set(a,b);mb(b,[a])}function gh(a,b,c){var d=a.type||"unknown-event";a.currentTarget=c;mj(d,b,void 0,a);a.currentTarget=null}function Xg(a,b){b=0!==(b&4);for(var c=0;c<a.length;c++){var d=a[c],e=d.event;d=d.listeners;a:{var f=void 0;if(b)for(var g=d.length-1;0<=g;g--){var h=d[g],k=h.instance,n=h.currentTarget;h=h.listener;if(k!==f&&e.isPropagationStopped())break a;gh(e,h,n);f=k}else for(g=0;g<d.length;g++){h=d[g];k=h.instance;n=h.currentTarget;h=h.listener;if(k!==f&&e.isPropagationStopped())break a;
gh(e,h,n);f=k}}}if(Tc)throw a=ue,Tc=!1,ue=null,a;}function B(a,b){var c=b[Me];void 0===c&&(c=b[Me]=new Set);var d=a+"__bubble";c.has(d)||(hh(b,a,2,!1),c.add(d))}function Ne(a,b,c){var d=0;b&&(d|=4);hh(c,a,d,b)}function sc(a){if(!a[id]){a[id]=!0;cg.forEach(function(b){"selectionchange"!==b&&(Uj.has(b)||Ne(b,!1,a),Ne(b,!0,a))});var b=9===a.nodeType?a:a.ownerDocument;null===b||b[id]||(b[id]=!0,Ne("selectionchange",!1,b))}}function hh(a,b,c,d,e){switch(Lg(b)){case 1:e=zj;break;case 4:e=Aj;break;default:e=
Be}c=e.bind(null,b,c,a);e=void 0;!Oe||"touchstart"!==b&&"touchmove"!==b&&"wheel"!==b||(e=!0);d?void 0!==e?a.addEventListener(b,c,{capture:!0,passive:e}):a.addEventListener(b,c,!0):void 0!==e?a.addEventListener(b,c,{passive:e}):a.addEventListener(b,c,!1)}function Ce(a,b,c,d,e){var f=d;if(0===(b&1)&&0===(b&2)&&null!==d)a:for(;;){if(null===d)return;var g=d.tag;if(3===g||4===g){var h=d.stateNode.containerInfo;if(h===e||8===h.nodeType&&h.parentNode===e)break;if(4===g)for(g=d.return;null!==g;){var k=g.tag;
if(3===k||4===k)if(k=g.stateNode.containerInfo,k===e||8===k.nodeType&&k.parentNode===e)return;g=g.return}for(;null!==h;){g=ob(h);if(null===g)return;k=g.tag;if(5===k||6===k){d=f=g;continue a}h=h.parentNode}}d=d.return}wg(function(){var d=f,e=re(c),g=[];a:{var h=fh.get(a);if(void 0!==h){var k=He,m=a;switch(a){case "keypress":if(0===cd(c))break a;case "keydown":case "keyup":k=Vj;break;case "focusin":m="focus";k=Pe;break;case "focusout":m="blur";k=Pe;break;case "beforeblur":case "afterblur":k=Pe;break;
case "click":if(2===c.button)break a;case "auxclick":case "dblclick":case "mousedown":case "mousemove":case "mouseup":case "mouseout":case "mouseover":case "contextmenu":k=ih;break;case "drag":case "dragend":case "dragenter":case "dragexit":case "dragleave":case "dragover":case "dragstart":case "drop":k=Wj;break;case "touchcancel":case "touchend":case "touchmove":case "touchstart":k=Xj;break;case jh:case kh:case lh:k=Yj;break;case mh:k=Zj;break;case "scroll":k=ak;break;case "wheel":k=bk;break;case "copy":case "cut":case "paste":k=
ck;break;case "gotpointercapture":case "lostpointercapture":case "pointercancel":case "pointerdown":case "pointermove":case "pointerout":case "pointerover":case "pointerup":k=nh}var l=0!==(b&4),p=!l&&"scroll"===a,w=l?null!==h?h+"Capture":null:h;l=[];for(var A=d,t;null!==A;){t=A;var M=t.stateNode;5===t.tag&&null!==M&&(t=M,null!==w&&(M=fc(A,w),null!=M&&l.push(tc(A,M,t))));if(p)break;A=A.return}0<l.length&&(h=new k(h,m,null,c,e),g.push({event:h,listeners:l}))}}if(0===(b&7)){a:{h="mouseover"===a||"pointerover"===
a;k="mouseout"===a||"pointerout"===a;if(h&&c!==ze&&(m=c.relatedTarget||c.fromElement)&&(ob(m)||m[Ja]))break a;if(k||h){h=e.window===e?e:(h=e.ownerDocument)?h.defaultView||h.parentWindow:window;if(k){if(m=c.relatedTarget||c.toElement,k=d,m=m?ob(m):null,null!==m&&(p=nb(m),m!==p||5!==m.tag&&6!==m.tag))m=null}else k=null,m=d;if(k!==m){l=ih;M="onMouseLeave";w="onMouseEnter";A="mouse";if("pointerout"===a||"pointerover"===a)l=nh,M="onPointerLeave",w="onPointerEnter",A="pointer";p=null==k?h:Ib(k);t=null==
m?h:Ib(m);h=new l(M,A+"leave",k,c,e);h.target=p;h.relatedTarget=t;M=null;ob(e)===d&&(l=new l(w,A+"enter",m,c,e),l.target=t,l.relatedTarget=p,M=l);p=M;if(k&&m)b:{l=k;w=m;A=0;for(t=l;t;t=Lb(t))A++;t=0;for(M=w;M;M=Lb(M))t++;for(;0<A-t;)l=Lb(l),A--;for(;0<t-A;)w=Lb(w),t--;for(;A--;){if(l===w||null!==w&&l===w.alternate)break b;l=Lb(l);w=Lb(w)}l=null}else l=null;null!==k&&oh(g,h,k,l,!1);null!==m&&null!==p&&oh(g,p,m,l,!0)}}}a:{h=d?Ib(d):window;k=h.nodeName&&h.nodeName.toLowerCase();if("select"===k||"input"===
k&&"file"===h.type)var ma=Nj;else if(Vg(h))if(ph)ma=Rj;else{ma=Pj;var va=Oj}else(k=h.nodeName)&&"input"===k.toLowerCase()&&("checkbox"===h.type||"radio"===h.type)&&(ma=Qj);if(ma&&(ma=ma(a,d))){Wg(g,ma,c,e);break a}va&&va(a,h,d);"focusout"===a&&(va=h._wrapperState)&&va.controlled&&"number"===h.type&&me(h,"number",h.value)}va=d?Ib(d):window;switch(a){case "focusin":if(Vg(va)||"true"===va.contentEditable)Jb=va,Ke=d,rc=null;break;case "focusout":rc=Ke=Jb=null;break;case "mousedown":Je=!0;break;case "contextmenu":case "mouseup":case "dragend":Je=
!1;dh(g,c,e);break;case "selectionchange":if(dk)break;case "keydown":case "keyup":dh(g,c,e)}var ab;if(Ge)b:{switch(a){case "compositionstart":var da="onCompositionStart";break b;case "compositionend":da="onCompositionEnd";break b;case "compositionupdate":da="onCompositionUpdate";break b}da=void 0}else Hb?Qg(a,c)&&(da="onCompositionEnd"):"keydown"===a&&229===c.keyCode&&(da="onCompositionStart");da&&(Ug&&"ko"!==c.locale&&(Hb||"onCompositionStart"!==da?"onCompositionEnd"===da&&Hb&&(ab=Og()):(Za=e,Ee=
"value"in Za?Za.value:Za.textContent,Hb=!0)),va=ed(d,da),0<va.length&&(da=new qh(da,a,null,c,e),g.push({event:da,listeners:va}),ab?da.data=ab:(ab=Rg(c),null!==ab&&(da.data=ab))));if(ab=ek?Ij(a,c):Jj(a,c))d=ed(d,"onBeforeInput"),0<d.length&&(e=new fk("onBeforeInput","beforeinput",null,c,e),g.push({event:e,listeners:d}),e.data=ab)}Xg(g,b)})}function tc(a,b,c){return{instance:a,listener:b,currentTarget:c}}function ed(a,b){for(var c=b+"Capture",d=[];null!==a;){var e=a,f=e.stateNode;5===e.tag&&null!==
f&&(e=f,f=fc(a,c),null!=f&&d.unshift(tc(a,f,e)),f=fc(a,b),null!=f&&d.push(tc(a,f,e)));a=a.return}return d}function Lb(a){if(null===a)return null;do a=a.return;while(a&&5!==a.tag);return a?a:null}function oh(a,b,c,d,e){for(var f=b._reactName,g=[];null!==c&&c!==d;){var h=c,k=h.alternate,n=h.stateNode;if(null!==k&&k===d)break;5===h.tag&&null!==n&&(h=n,e?(k=fc(c,f),null!=k&&g.unshift(tc(c,k,h))):e||(k=fc(c,f),null!=k&&g.push(tc(c,k,h))));c=c.return}0!==g.length&&a.push({event:b,listeners:g})}function rh(a){return("string"===
typeof a?a:""+a).replace(gk,"\n").replace(hk,"")}function jd(a,b,c,d){b=rh(b);if(rh(a)!==b&&c)throw Error(m(425));}function kd(){}function Qe(a,b){return"textarea"===a||"noscript"===a||"string"===typeof b.children||"number"===typeof b.children||"object"===typeof b.dangerouslySetInnerHTML&&null!==b.dangerouslySetInnerHTML&&null!=b.dangerouslySetInnerHTML.__html}function ik(a){setTimeout(function(){throw a;})}function Re(a,b){var c=b,d=0;do{var e=c.nextSibling;a.removeChild(c);if(e&&8===e.nodeType)if(c=
e.data,"/$"===c){if(0===d){a.removeChild(e);nc(b);return}d--}else"$"!==c&&"$?"!==c&&"$!"!==c||d++;c=e}while(c);nc(b)}function Ka(a){for(;null!=a;a=a.nextSibling){var b=a.nodeType;if(1===b||3===b)break;if(8===b){b=a.data;if("$"===b||"$!"===b||"$?"===b)break;if("/$"===b)return null}}return a}function sh(a){a=a.previousSibling;for(var b=0;a;){if(8===a.nodeType){var c=a.data;if("$"===c||"$!"===c||"$?"===c){if(0===b)return a;b--}else"/$"===c&&b++}a=a.previousSibling}return null}function ob(a){var b=a[Da];
if(b)return b;for(var c=a.parentNode;c;){if(b=c[Ja]||c[Da]){c=b.alternate;if(null!==b.child||null!==c&&null!==c.child)for(a=sh(a);null!==a;){if(c=a[Da])return c;a=sh(a)}return b}a=c;c=a.parentNode}return null}function ec(a){a=a[Da]||a[Ja];return!a||5!==a.tag&&6!==a.tag&&13!==a.tag&&3!==a.tag?null:a}function Ib(a){if(5===a.tag||6===a.tag)return a.stateNode;throw Error(m(33));}function Rc(a){return a[uc]||null}function bb(a){return{current:a}}function v(a,b){0>Mb||(a.current=Se[Mb],Se[Mb]=null,Mb--)}
function y(a,b,c){Mb++;Se[Mb]=a.current;a.current=b}function Nb(a,b){var c=a.type.contextTypes;if(!c)return cb;var d=a.stateNode;if(d&&d.__reactInternalMemoizedUnmaskedChildContext===b)return d.__reactInternalMemoizedMaskedChildContext;var e={},f;for(f in c)e[f]=b[f];d&&(a=a.stateNode,a.__reactInternalMemoizedUnmaskedChildContext=b,a.__reactInternalMemoizedMaskedChildContext=e);return e}function ea(a){a=a.childContextTypes;return null!==a&&void 0!==a}function th(a,b,c){if(J.current!==cb)throw Error(m(168));
y(J,b);y(S,c)}function uh(a,b,c){var d=a.stateNode;b=b.childContextTypes;if("function"!==typeof d.getChildContext)return c;d=d.getChildContext();for(var e in d)if(!(e in b))throw Error(m(108,gj(a)||"Unknown",e));return E({},c,d)}function ld(a){a=(a=a.stateNode)&&a.__reactInternalMemoizedMergedChildContext||cb;pb=J.current;y(J,a);y(S,S.current);return!0}function vh(a,b,c){var d=a.stateNode;if(!d)throw Error(m(169));c?(a=uh(a,b,pb),d.__reactInternalMemoizedMergedChildContext=a,v(S),v(J),y(J,a)):v(S);
y(S,c)}function wh(a){null===La?La=[a]:La.push(a)}function jk(a){md=!0;wh(a)}function db(){if(!Te&&null!==La){Te=!0;var a=0,b=z;try{var c=La;for(z=1;a<c.length;a++){var d=c[a];do d=d(!0);while(null!==d)}La=null;md=!1}catch(e){throw null!==La&&(La=La.slice(a+1)),xh(De,db),e;}finally{z=b,Te=!1}}return null}function qb(a,b){Ob[Pb++]=nd;Ob[Pb++]=od;od=a;nd=b}function yh(a,b,c){na[oa++]=Ma;na[oa++]=Na;na[oa++]=rb;rb=a;var d=Ma;a=Na;var e=32-ta(d)-1;d&=~(1<<e);c+=1;var f=32-ta(b)+e;if(30<f){var g=e-e%5;
f=(d&(1<<g)-1).toString(32);d>>=g;e-=g;Ma=1<<32-ta(b)+e|c<<e|d;Na=f+a}else Ma=1<<f|c<<e|d,Na=a}function Ue(a){null!==a.return&&(qb(a,1),yh(a,1,0))}function Ve(a){for(;a===od;)od=Ob[--Pb],Ob[Pb]=null,nd=Ob[--Pb],Ob[Pb]=null;for(;a===rb;)rb=na[--oa],na[oa]=null,Na=na[--oa],na[oa]=null,Ma=na[--oa],na[oa]=null}function zh(a,b){var c=pa(5,null,null,0);c.elementType="DELETED";c.stateNode=b;c.return=a;b=a.deletions;null===b?(a.deletions=[c],a.flags|=16):b.push(c)}function Ah(a,b){switch(a.tag){case 5:var c=
a.type;b=1!==b.nodeType||c.toLowerCase()!==b.nodeName.toLowerCase()?null:b;return null!==b?(a.stateNode=b,la=a,fa=Ka(b.firstChild),!0):!1;case 6:return b=""===a.pendingProps||3!==b.nodeType?null:b,null!==b?(a.stateNode=b,la=a,fa=null,!0):!1;case 13:return b=8!==b.nodeType?null:b,null!==b?(c=null!==rb?{id:Ma,overflow:Na}:null,a.memoizedState={dehydrated:b,treeContext:c,retryLane:1073741824},c=pa(18,null,null,0),c.stateNode=b,c.return=a,a.child=c,la=a,fa=null,!0):!1;default:return!1}}function We(a){return 0!==
(a.mode&1)&&0===(a.flags&128)}function Xe(a){if(D){var b=fa;if(b){var c=b;if(!Ah(a,b)){if(We(a))throw Error(m(418));b=Ka(c.nextSibling);var d=la;b&&Ah(a,b)?zh(d,c):(a.flags=a.flags&-4097|2,D=!1,la=a)}}else{if(We(a))throw Error(m(418));a.flags=a.flags&-4097|2;D=!1;la=a}}}function Bh(a){for(a=a.return;null!==a&&5!==a.tag&&3!==a.tag&&13!==a.tag;)a=a.return;la=a}function pd(a){if(a!==la)return!1;if(!D)return Bh(a),D=!0,!1;var b;(b=3!==a.tag)&&!(b=5!==a.tag)&&(b=a.type,b="head"!==b&&"body"!==b&&!Qe(a.type,
a.memoizedProps));if(b&&(b=fa)){if(We(a)){for(a=fa;a;)a=Ka(a.nextSibling);throw Error(m(418));}for(;b;)zh(a,b),b=Ka(b.nextSibling)}Bh(a);if(13===a.tag){a=a.memoizedState;a=null!==a?a.dehydrated:null;if(!a)throw Error(m(317));a:{a=a.nextSibling;for(b=0;a;){if(8===a.nodeType){var c=a.data;if("/$"===c){if(0===b){fa=Ka(a.nextSibling);break a}b--}else"$"!==c&&"$!"!==c&&"$?"!==c||b++}a=a.nextSibling}fa=null}}else fa=la?Ka(a.stateNode.nextSibling):null;return!0}function Qb(){fa=la=null;D=!1}function Ye(a){null===
wa?wa=[a]:wa.push(a)}function vc(a,b,c){a=c.ref;if(null!==a&&"function"!==typeof a&&"object"!==typeof a){if(c._owner){c=c._owner;if(c){if(1!==c.tag)throw Error(m(309));var d=c.stateNode}if(!d)throw Error(m(147,a));var e=d,f=""+a;if(null!==b&&null!==b.ref&&"function"===typeof b.ref&&b.ref._stringRef===f)return b.ref;b=function(a){var b=e.refs;null===a?delete b[f]:b[f]=a};b._stringRef=f;return b}if("string"!==typeof a)throw Error(m(284));if(!c._owner)throw Error(m(290,a));}return a}function qd(a,b){a=
Object.prototype.toString.call(b);throw Error(m(31,"[object Object]"===a?"object with keys {"+Object.keys(b).join(", ")+"}":a));}function Ch(a){var b=a._init;return b(a._payload)}function Dh(a){function b(b,c){if(a){var d=b.deletions;null===d?(b.deletions=[c],b.flags|=16):d.push(c)}}function c(c,d){if(!a)return null;for(;null!==d;)b(c,d),d=d.sibling;return null}function d(a,b){for(a=new Map;null!==b;)null!==b.key?a.set(b.key,b):a.set(b.index,b),b=b.sibling;return a}function e(a,b){a=eb(a,b);a.index=
0;a.sibling=null;return a}function f(b,c,d){b.index=d;if(!a)return b.flags|=1048576,c;d=b.alternate;if(null!==d)return d=d.index,d<c?(b.flags|=2,c):d;b.flags|=2;return c}function g(b){a&&null===b.alternate&&(b.flags|=2);return b}function h(a,b,c,d){if(null===b||6!==b.tag)return b=Ze(c,a.mode,d),b.return=a,b;b=e(b,c);b.return=a;return b}function k(a,b,c,d){var f=c.type;if(f===Bb)return l(a,b,c.props.children,d,c.key);if(null!==b&&(b.elementType===f||"object"===typeof f&&null!==f&&f.$$typeof===Ta&&
Ch(f)===b.type))return d=e(b,c.props),d.ref=vc(a,b,c),d.return=a,d;d=rd(c.type,c.key,c.props,null,a.mode,d);d.ref=vc(a,b,c);d.return=a;return d}function n(a,b,c,d){if(null===b||4!==b.tag||b.stateNode.containerInfo!==c.containerInfo||b.stateNode.implementation!==c.implementation)return b=$e(c,a.mode,d),b.return=a,b;b=e(b,c.children||[]);b.return=a;return b}function l(a,b,c,d,f){if(null===b||7!==b.tag)return b=sb(c,a.mode,d,f),b.return=a,b;b=e(b,c);b.return=a;return b}function u(a,b,c){if("string"===
typeof b&&""!==b||"number"===typeof b)return b=Ze(""+b,a.mode,c),b.return=a,b;if("object"===typeof b&&null!==b){switch(b.$$typeof){case sd:return c=rd(b.type,b.key,b.props,null,a.mode,c),c.ref=vc(a,null,b),c.return=a,c;case Cb:return b=$e(b,a.mode,c),b.return=a,b;case Ta:var d=b._init;return u(a,d(b._payload),c)}if(cc(b)||ac(b))return b=sb(b,a.mode,c,null),b.return=a,b;qd(a,b)}return null}function r(a,b,c,d){var e=null!==b?b.key:null;if("string"===typeof c&&""!==c||"number"===typeof c)return null!==
e?null:h(a,b,""+c,d);if("object"===typeof c&&null!==c){switch(c.$$typeof){case sd:return c.key===e?k(a,b,c,d):null;case Cb:return c.key===e?n(a,b,c,d):null;case Ta:return e=c._init,r(a,b,e(c._payload),d)}if(cc(c)||ac(c))return null!==e?null:l(a,b,c,d,null);qd(a,c)}return null}function p(a,b,c,d,e){if("string"===typeof d&&""!==d||"number"===typeof d)return a=a.get(c)||null,h(b,a,""+d,e);if("object"===typeof d&&null!==d){switch(d.$$typeof){case sd:return a=a.get(null===d.key?c:d.key)||null,k(b,a,d,
e);case Cb:return a=a.get(null===d.key?c:d.key)||null,n(b,a,d,e);case Ta:var f=d._init;return p(a,b,c,f(d._payload),e)}if(cc(d)||ac(d))return a=a.get(c)||null,l(b,a,d,e,null);qd(b,d)}return null}function x(e,g,h,k){for(var n=null,m=null,l=g,t=g=0,q=null;null!==l&&t<h.length;t++){l.index>t?(q=l,l=null):q=l.sibling;var A=r(e,l,h[t],k);if(null===A){null===l&&(l=q);break}a&&l&&null===A.alternate&&b(e,l);g=f(A,g,t);null===m?n=A:m.sibling=A;m=A;l=q}if(t===h.length)return c(e,l),D&&qb(e,t),n;if(null===l){for(;t<
h.length;t++)l=u(e,h[t],k),null!==l&&(g=f(l,g,t),null===m?n=l:m.sibling=l,m=l);D&&qb(e,t);return n}for(l=d(e,l);t<h.length;t++)q=p(l,e,t,h[t],k),null!==q&&(a&&null!==q.alternate&&l.delete(null===q.key?t:q.key),g=f(q,g,t),null===m?n=q:m.sibling=q,m=q);a&&l.forEach(function(a){return b(e,a)});D&&qb(e,t);return n}function I(e,g,h,k){var n=ac(h);if("function"!==typeof n)throw Error(m(150));h=n.call(h);if(null==h)throw Error(m(151));for(var l=n=null,q=g,t=g=0,A=null,w=h.next();null!==q&&!w.done;t++,w=
h.next()){q.index>t?(A=q,q=null):A=q.sibling;var x=r(e,q,w.value,k);if(null===x){null===q&&(q=A);break}a&&q&&null===x.alternate&&b(e,q);g=f(x,g,t);null===l?n=x:l.sibling=x;l=x;q=A}if(w.done)return c(e,q),D&&qb(e,t),n;if(null===q){for(;!w.done;t++,w=h.next())w=u(e,w.value,k),null!==w&&(g=f(w,g,t),null===l?n=w:l.sibling=w,l=w);D&&qb(e,t);return n}for(q=d(e,q);!w.done;t++,w=h.next())w=p(q,e,t,w.value,k),null!==w&&(a&&null!==w.alternate&&q.delete(null===w.key?t:w.key),g=f(w,g,t),null===l?n=w:l.sibling=
w,l=w);a&&q.forEach(function(a){return b(e,a)});D&&qb(e,t);return n}function v(a,d,f,h){"object"===typeof f&&null!==f&&f.type===Bb&&null===f.key&&(f=f.props.children);if("object"===typeof f&&null!==f){switch(f.$$typeof){case sd:a:{for(var k=f.key,n=d;null!==n;){if(n.key===k){k=f.type;if(k===Bb){if(7===n.tag){c(a,n.sibling);d=e(n,f.props.children);d.return=a;a=d;break a}}else if(n.elementType===k||"object"===typeof k&&null!==k&&k.$$typeof===Ta&&Ch(k)===n.type){c(a,n.sibling);d=e(n,f.props);d.ref=vc(a,
n,f);d.return=a;a=d;break a}c(a,n);break}else b(a,n);n=n.sibling}f.type===Bb?(d=sb(f.props.children,a.mode,h,f.key),d.return=a,a=d):(h=rd(f.type,f.key,f.props,null,a.mode,h),h.ref=vc(a,d,f),h.return=a,a=h)}return g(a);case Cb:a:{for(n=f.key;null!==d;){if(d.key===n)if(4===d.tag&&d.stateNode.containerInfo===f.containerInfo&&d.stateNode.implementation===f.implementation){c(a,d.sibling);d=e(d,f.children||[]);d.return=a;a=d;break a}else{c(a,d);break}else b(a,d);d=d.sibling}d=$e(f,a.mode,h);d.return=a;
a=d}return g(a);case Ta:return n=f._init,v(a,d,n(f._payload),h)}if(cc(f))return x(a,d,f,h);if(ac(f))return I(a,d,f,h);qd(a,f)}return"string"===typeof f&&""!==f||"number"===typeof f?(f=""+f,null!==d&&6===d.tag?(c(a,d.sibling),d=e(d,f),d.return=a,a=d):(c(a,d),d=Ze(f,a.mode,h),d.return=a,a=d),g(a)):c(a,d)}return v}function af(){bf=Rb=td=null}function cf(a,b){b=ud.current;v(ud);a._currentValue=b}function df(a,b,c){for(;null!==a;){var d=a.alternate;(a.childLanes&b)!==b?(a.childLanes|=b,null!==d&&(d.childLanes|=
b)):null!==d&&(d.childLanes&b)!==b&&(d.childLanes|=b);if(a===c)break;a=a.return}}function Sb(a,b){td=a;bf=Rb=null;a=a.dependencies;null!==a&&null!==a.firstContext&&(0!==(a.lanes&b)&&(ha=!0),a.firstContext=null)}function qa(a){var b=a._currentValue;if(bf!==a)if(a={context:a,memoizedValue:b,next:null},null===Rb){if(null===td)throw Error(m(308));Rb=a;td.dependencies={lanes:0,firstContext:a}}else Rb=Rb.next=a;return b}function ef(a){null===tb?tb=[a]:tb.push(a)}function Eh(a,b,c,d){var e=b.interleaved;
null===e?(c.next=c,ef(b)):(c.next=e.next,e.next=c);b.interleaved=c;return Oa(a,d)}function Oa(a,b){a.lanes|=b;var c=a.alternate;null!==c&&(c.lanes|=b);c=a;for(a=a.return;null!==a;)a.childLanes|=b,c=a.alternate,null!==c&&(c.childLanes|=b),c=a,a=a.return;return 3===c.tag?c.stateNode:null}function ff(a){a.updateQueue={baseState:a.memoizedState,firstBaseUpdate:null,lastBaseUpdate:null,shared:{pending:null,interleaved:null,lanes:0},effects:null}}function Fh(a,b){a=a.updateQueue;b.updateQueue===a&&(b.updateQueue=
{baseState:a.baseState,firstBaseUpdate:a.firstBaseUpdate,lastBaseUpdate:a.lastBaseUpdate,shared:a.shared,effects:a.effects})}function Pa(a,b){return{eventTime:a,lane:b,tag:0,payload:null,callback:null,next:null}}function fb(a,b,c){var d=a.updateQueue;if(null===d)return null;d=d.shared;if(0!==(p&2)){var e=d.pending;null===e?b.next=b:(b.next=e.next,e.next=b);d.pending=b;return kk(a,c)}e=d.interleaved;null===e?(b.next=b,ef(d)):(b.next=e.next,e.next=b);d.interleaved=b;return Oa(a,c)}function vd(a,b,c){b=
b.updateQueue;if(null!==b&&(b=b.shared,0!==(c&4194240))){var d=b.lanes;d&=a.pendingLanes;c|=d;b.lanes=c;xe(a,c)}}function Gh(a,b){var c=a.updateQueue,d=a.alternate;if(null!==d&&(d=d.updateQueue,c===d)){var e=null,f=null;c=c.firstBaseUpdate;if(null!==c){do{var g={eventTime:c.eventTime,lane:c.lane,tag:c.tag,payload:c.payload,callback:c.callback,next:null};null===f?e=f=g:f=f.next=g;c=c.next}while(null!==c);null===f?e=f=b:f=f.next=b}else e=f=b;c={baseState:d.baseState,firstBaseUpdate:e,lastBaseUpdate:f,
shared:d.shared,effects:d.effects};a.updateQueue=c;return}a=c.lastBaseUpdate;null===a?c.firstBaseUpdate=b:a.next=b;c.lastBaseUpdate=b}function wd(a,b,c,d){var e=a.updateQueue;gb=!1;var f=e.firstBaseUpdate,g=e.lastBaseUpdate,h=e.shared.pending;if(null!==h){e.shared.pending=null;var k=h,n=k.next;k.next=null;null===g?f=n:g.next=n;g=k;var l=a.alternate;null!==l&&(l=l.updateQueue,h=l.lastBaseUpdate,h!==g&&(null===h?l.firstBaseUpdate=n:h.next=n,l.lastBaseUpdate=k))}if(null!==f){var m=e.baseState;g=0;l=
n=k=null;h=f;do{var r=h.lane,p=h.eventTime;if((d&r)===r){null!==l&&(l=l.next={eventTime:p,lane:0,tag:h.tag,payload:h.payload,callback:h.callback,next:null});a:{var x=a,v=h;r=b;p=c;switch(v.tag){case 1:x=v.payload;if("function"===typeof x){m=x.call(p,m,r);break a}m=x;break a;case 3:x.flags=x.flags&-65537|128;case 0:x=v.payload;r="function"===typeof x?x.call(p,m,r):x;if(null===r||void 0===r)break a;m=E({},m,r);break a;case 2:gb=!0}}null!==h.callback&&0!==h.lane&&(a.flags|=64,r=e.effects,null===r?e.effects=
[h]:r.push(h))}else p={eventTime:p,lane:r,tag:h.tag,payload:h.payload,callback:h.callback,next:null},null===l?(n=l=p,k=m):l=l.next=p,g|=r;h=h.next;if(null===h)if(h=e.shared.pending,null===h)break;else r=h,h=r.next,r.next=null,e.lastBaseUpdate=r,e.shared.pending=null}while(1);null===l&&(k=m);e.baseState=k;e.firstBaseUpdate=n;e.lastBaseUpdate=l;b=e.shared.interleaved;if(null!==b){e=b;do g|=e.lane,e=e.next;while(e!==b)}else null===f&&(e.shared.lanes=0);ra|=g;a.lanes=g;a.memoizedState=m}}function Hh(a,
b,c){a=b.effects;b.effects=null;if(null!==a)for(b=0;b<a.length;b++){var d=a[b],e=d.callback;if(null!==e){d.callback=null;d=c;if("function"!==typeof e)throw Error(m(191,e));e.call(d)}}}function ub(a){if(a===wc)throw Error(m(174));return a}function gf(a,b){y(xc,b);y(yc,a);y(Ea,wc);a=b.nodeType;switch(a){case 9:case 11:b=(b=b.documentElement)?b.namespaceURI:oe(null,"");break;default:a=8===a?b.parentNode:b,b=a.namespaceURI||null,a=a.tagName,b=oe(b,a)}v(Ea);y(Ea,b)}function Tb(a){v(Ea);v(yc);v(xc)}function Ih(a){ub(xc.current);
var b=ub(Ea.current);var c=oe(b,a.type);b!==c&&(y(yc,a),y(Ea,c))}function hf(a){yc.current===a&&(v(Ea),v(yc))}function xd(a){for(var b=a;null!==b;){if(13===b.tag){var c=b.memoizedState;if(null!==c&&(c=c.dehydrated,null===c||"$?"===c.data||"$!"===c.data))return b}else if(19===b.tag&&void 0!==b.memoizedProps.revealOrder){if(0!==(b.flags&128))return b}else if(null!==b.child){b.child.return=b;b=b.child;continue}if(b===a)break;for(;null===b.sibling;){if(null===b.return||b.return===a)return null;b=b.return}b.sibling.return=
b.return;b=b.sibling}return null}function jf(){for(var a=0;a<kf.length;a++)kf[a]._workInProgressVersionPrimary=null;kf.length=0}function V(){throw Error(m(321));}function lf(a,b){if(null===b)return!1;for(var c=0;c<b.length&&c<a.length;c++)if(!ua(a[c],b[c]))return!1;return!0}function mf(a,b,c,d,e,f){vb=f;C=b;b.memoizedState=null;b.updateQueue=null;b.lanes=0;yd.current=null===a||null===a.memoizedState?lk:mk;a=c(d,e);if(zc){f=0;do{zc=!1;Ac=0;if(25<=f)throw Error(m(301));f+=1;N=K=null;b.updateQueue=null;
yd.current=nk;a=c(d,e)}while(zc)}yd.current=zd;b=null!==K&&null!==K.next;vb=0;N=K=C=null;Ad=!1;if(b)throw Error(m(300));return a}function nf(){var a=0!==Ac;Ac=0;return a}function Fa(){var a={memoizedState:null,baseState:null,baseQueue:null,queue:null,next:null};null===N?C.memoizedState=N=a:N=N.next=a;return N}function sa(){if(null===K){var a=C.alternate;a=null!==a?a.memoizedState:null}else a=K.next;var b=null===N?C.memoizedState:N.next;if(null!==b)N=b,K=a;else{if(null===a)throw Error(m(310));K=a;
a={memoizedState:K.memoizedState,baseState:K.baseState,baseQueue:K.baseQueue,queue:K.queue,next:null};null===N?C.memoizedState=N=a:N=N.next=a}return N}function Bc(a,b){return"function"===typeof b?b(a):b}function of(a,b,c){b=sa();c=b.queue;if(null===c)throw Error(m(311));c.lastRenderedReducer=a;var d=K,e=d.baseQueue,f=c.pending;if(null!==f){if(null!==e){var g=e.next;e.next=f.next;f.next=g}d.baseQueue=e=f;c.pending=null}if(null!==e){f=e.next;d=d.baseState;var h=g=null,k=null,n=f;do{var l=n.lane;if((vb&
l)===l)null!==k&&(k=k.next={lane:0,action:n.action,hasEagerState:n.hasEagerState,eagerState:n.eagerState,next:null}),d=n.hasEagerState?n.eagerState:a(d,n.action);else{var u={lane:l,action:n.action,hasEagerState:n.hasEagerState,eagerState:n.eagerState,next:null};null===k?(h=k=u,g=d):k=k.next=u;C.lanes|=l;ra|=l}n=n.next}while(null!==n&&n!==f);null===k?g=d:k.next=h;ua(d,b.memoizedState)||(ha=!0);b.memoizedState=d;b.baseState=g;b.baseQueue=k;c.lastRenderedState=d}a=c.interleaved;if(null!==a){e=a;do f=
e.lane,C.lanes|=f,ra|=f,e=e.next;while(e!==a)}else null===e&&(c.lanes=0);return[b.memoizedState,c.dispatch]}function pf(a,b,c){b=sa();c=b.queue;if(null===c)throw Error(m(311));c.lastRenderedReducer=a;var d=c.dispatch,e=c.pending,f=b.memoizedState;if(null!==e){c.pending=null;var g=e=e.next;do f=a(f,g.action),g=g.next;while(g!==e);ua(f,b.memoizedState)||(ha=!0);b.memoizedState=f;null===b.baseQueue&&(b.baseState=f);c.lastRenderedState=f}return[f,d]}function Jh(a,b,c){}function Kh(a,b,c){c=C;var d=sa(),
e=b(),f=!ua(d.memoizedState,e);f&&(d.memoizedState=e,ha=!0);d=d.queue;qf(Lh.bind(null,c,d,a),[a]);if(d.getSnapshot!==b||f||null!==N&&N.memoizedState.tag&1){c.flags|=2048;Cc(9,Mh.bind(null,c,d,e,b),void 0,null);if(null===O)throw Error(m(349));0!==(vb&30)||Nh(c,b,e)}return e}function Nh(a,b,c){a.flags|=16384;a={getSnapshot:b,value:c};b=C.updateQueue;null===b?(b={lastEffect:null,stores:null},C.updateQueue=b,b.stores=[a]):(c=b.stores,null===c?b.stores=[a]:c.push(a))}function Mh(a,b,c,d){b.value=c;b.getSnapshot=
d;Oh(b)&&Ph(a)}function Lh(a,b,c){return c(function(){Oh(b)&&Ph(a)})}function Oh(a){var b=a.getSnapshot;a=a.value;try{var c=b();return!ua(a,c)}catch(d){return!0}}function Ph(a){var b=Oa(a,1);null!==b&&xa(b,a,1,-1)}function Qh(a){var b=Fa();"function"===typeof a&&(a=a());b.memoizedState=b.baseState=a;a={pending:null,interleaved:null,lanes:0,dispatch:null,lastRenderedReducer:Bc,lastRenderedState:a};b.queue=a;a=a.dispatch=ok.bind(null,C,a);return[b.memoizedState,a]}function Cc(a,b,c,d){a={tag:a,create:b,
destroy:c,deps:d,next:null};b=C.updateQueue;null===b?(b={lastEffect:null,stores:null},C.updateQueue=b,b.lastEffect=a.next=a):(c=b.lastEffect,null===c?b.lastEffect=a.next=a:(d=c.next,c.next=a,a.next=d,b.lastEffect=a));return a}function Rh(a){return sa().memoizedState}function Bd(a,b,c,d){var e=Fa();C.flags|=a;e.memoizedState=Cc(1|b,c,void 0,void 0===d?null:d)}function Cd(a,b,c,d){var e=sa();d=void 0===d?null:d;var f=void 0;if(null!==K){var g=K.memoizedState;f=g.destroy;if(null!==d&&lf(d,g.deps)){e.memoizedState=
Cc(b,c,f,d);return}}C.flags|=a;e.memoizedState=Cc(1|b,c,f,d)}function Sh(a,b){return Bd(8390656,8,a,b)}function qf(a,b){return Cd(2048,8,a,b)}function Th(a,b){return Cd(4,2,a,b)}function Uh(a,b){return Cd(4,4,a,b)}function Vh(a,b){if("function"===typeof b)return a=a(),b(a),function(){b(null)};if(null!==b&&void 0!==b)return a=a(),b.current=a,function(){b.current=null}}function Wh(a,b,c){c=null!==c&&void 0!==c?c.concat([a]):null;return Cd(4,4,Vh.bind(null,b,a),c)}function rf(a,b){}function Xh(a,b){var c=
sa();b=void 0===b?null:b;var d=c.memoizedState;if(null!==d&&null!==b&&lf(b,d[1]))return d[0];c.memoizedState=[a,b];return a}function Yh(a,b){var c=sa();b=void 0===b?null:b;var d=c.memoizedState;if(null!==d&&null!==b&&lf(b,d[1]))return d[0];a=a();c.memoizedState=[a,b];return a}function Zh(a,b,c){if(0===(vb&21))return a.baseState&&(a.baseState=!1,ha=!0),a.memoizedState=c;ua(c,b)||(c=Dg(),C.lanes|=c,ra|=c,a.baseState=!0);return b}function pk(a,b,c){c=z;z=0!==c&&4>c?c:4;a(!0);var d=sf.transition;sf.transition=
{};try{a(!1),b()}finally{z=c,sf.transition=d}}function $h(){return sa().memoizedState}function qk(a,b,c){var d=hb(a);c={lane:d,action:c,hasEagerState:!1,eagerState:null,next:null};if(ai(a))bi(b,c);else if(c=Eh(a,b,c,d),null!==c){var e=Z();xa(c,a,d,e);ci(c,b,d)}}function ok(a,b,c){var d=hb(a),e={lane:d,action:c,hasEagerState:!1,eagerState:null,next:null};if(ai(a))bi(b,e);else{var f=a.alternate;if(0===a.lanes&&(null===f||0===f.lanes)&&(f=b.lastRenderedReducer,null!==f))try{var g=b.lastRenderedState,
h=f(g,c);e.hasEagerState=!0;e.eagerState=h;if(ua(h,g)){var k=b.interleaved;null===k?(e.next=e,ef(b)):(e.next=k.next,k.next=e);b.interleaved=e;return}}catch(n){}finally{}c=Eh(a,b,e,d);null!==c&&(e=Z(),xa(c,a,d,e),ci(c,b,d))}}function ai(a){var b=a.alternate;return a===C||null!==b&&b===C}function bi(a,b){zc=Ad=!0;var c=a.pending;null===c?b.next=b:(b.next=c.next,c.next=b);a.pending=b}function ci(a,b,c){if(0!==(c&4194240)){var d=b.lanes;d&=a.pendingLanes;c|=d;b.lanes=c;xe(a,c)}}function ya(a,b){if(a&&
a.defaultProps){b=E({},b);a=a.defaultProps;for(var c in a)void 0===b[c]&&(b[c]=a[c]);return b}return b}function tf(a,b,c,d){b=a.memoizedState;c=c(d,b);c=null===c||void 0===c?b:E({},b,c);a.memoizedState=c;0===a.lanes&&(a.updateQueue.baseState=c)}function di(a,b,c,d,e,f,g){a=a.stateNode;return"function"===typeof a.shouldComponentUpdate?a.shouldComponentUpdate(d,f,g):b.prototype&&b.prototype.isPureReactComponent?!qc(c,d)||!qc(e,f):!0}function ei(a,b,c){var d=!1,e=cb;var f=b.contextType;"object"===typeof f&&
null!==f?f=qa(f):(e=ea(b)?pb:J.current,d=b.contextTypes,f=(d=null!==d&&void 0!==d)?Nb(a,e):cb);b=new b(c,f);a.memoizedState=null!==b.state&&void 0!==b.state?b.state:null;b.updater=Dd;a.stateNode=b;b._reactInternals=a;d&&(a=a.stateNode,a.__reactInternalMemoizedUnmaskedChildContext=e,a.__reactInternalMemoizedMaskedChildContext=f);return b}function fi(a,b,c,d){a=b.state;"function"===typeof b.componentWillReceiveProps&&b.componentWillReceiveProps(c,d);"function"===typeof b.UNSAFE_componentWillReceiveProps&&
b.UNSAFE_componentWillReceiveProps(c,d);b.state!==a&&Dd.enqueueReplaceState(b,b.state,null)}function uf(a,b,c,d){var e=a.stateNode;e.props=c;e.state=a.memoizedState;e.refs={};ff(a);var f=b.contextType;"object"===typeof f&&null!==f?e.context=qa(f):(f=ea(b)?pb:J.current,e.context=Nb(a,f));e.state=a.memoizedState;f=b.getDerivedStateFromProps;"function"===typeof f&&(tf(a,b,f,c),e.state=a.memoizedState);"function"===typeof b.getDerivedStateFromProps||"function"===typeof e.getSnapshotBeforeUpdate||"function"!==
typeof e.UNSAFE_componentWillMount&&"function"!==typeof e.componentWillMount||(b=e.state,"function"===typeof e.componentWillMount&&e.componentWillMount(),"function"===typeof e.UNSAFE_componentWillMount&&e.UNSAFE_componentWillMount(),b!==e.state&&Dd.enqueueReplaceState(e,e.state,null),wd(a,c,e,d),e.state=a.memoizedState);"function"===typeof e.componentDidMount&&(a.flags|=4194308)}function Ub(a,b){try{var c="",d=b;do c+=fj(d),d=d.return;while(d);var e=c}catch(f){e="\nError generating stack: "+f.message+
"\n"+f.stack}return{value:a,source:b,stack:e,digest:null}}function vf(a,b,c){return{value:a,source:null,stack:null!=c?c:null,digest:null!=b?b:null}}function wf(a,b){try{console.error(b.value)}catch(c){setTimeout(function(){throw c;})}}function gi(a,b,c){c=Pa(-1,c);c.tag=3;c.payload={element:null};var d=b.value;c.callback=function(){Ed||(Ed=!0,xf=d);wf(a,b)};return c}function hi(a,b,c){c=Pa(-1,c);c.tag=3;var d=a.type.getDerivedStateFromError;if("function"===typeof d){var e=b.value;c.payload=function(){return d(e)};
c.callback=function(){wf(a,b)}}var f=a.stateNode;null!==f&&"function"===typeof f.componentDidCatch&&(c.callback=function(){wf(a,b);"function"!==typeof d&&(null===ib?ib=new Set([this]):ib.add(this));var c=b.stack;this.componentDidCatch(b.value,{componentStack:null!==c?c:""})});return c}function ii(a,b,c){var d=a.pingCache;if(null===d){d=a.pingCache=new rk;var e=new Set;d.set(b,e)}else e=d.get(b),void 0===e&&(e=new Set,d.set(b,e));e.has(c)||(e.add(c),a=sk.bind(null,a,b,c),b.then(a,a))}function ji(a){do{var b;
if(b=13===a.tag)b=a.memoizedState,b=null!==b?null!==b.dehydrated?!0:!1:!0;if(b)return a;a=a.return}while(null!==a);return null}function ki(a,b,c,d,e){if(0===(a.mode&1))return a===b?a.flags|=65536:(a.flags|=128,c.flags|=131072,c.flags&=-52805,1===c.tag&&(null===c.alternate?c.tag=17:(b=Pa(-1,1),b.tag=2,fb(c,b,1))),c.lanes|=1),a;a.flags|=65536;a.lanes=e;return a}function aa(a,b,c,d){b.child=null===a?li(b,null,c,d):Vb(b,a.child,c,d)}function mi(a,b,c,d,e){c=c.render;var f=b.ref;Sb(b,e);d=mf(a,b,c,d,f,
e);c=nf();if(null!==a&&!ha)return b.updateQueue=a.updateQueue,b.flags&=-2053,a.lanes&=~e,Qa(a,b,e);D&&c&&Ue(b);b.flags|=1;aa(a,b,d,e);return b.child}function ni(a,b,c,d,e){if(null===a){var f=c.type;if("function"===typeof f&&!yf(f)&&void 0===f.defaultProps&&null===c.compare&&void 0===c.defaultProps)return b.tag=15,b.type=f,oi(a,b,f,d,e);a=rd(c.type,null,d,b,b.mode,e);a.ref=b.ref;a.return=b;return b.child=a}f=a.child;if(0===(a.lanes&e)){var g=f.memoizedProps;c=c.compare;c=null!==c?c:qc;if(c(g,d)&&a.ref===
b.ref)return Qa(a,b,e)}b.flags|=1;a=eb(f,d);a.ref=b.ref;a.return=b;return b.child=a}function oi(a,b,c,d,e){if(null!==a){var f=a.memoizedProps;if(qc(f,d)&&a.ref===b.ref)if(ha=!1,b.pendingProps=d=f,0!==(a.lanes&e))0!==(a.flags&131072)&&(ha=!0);else return b.lanes=a.lanes,Qa(a,b,e)}return zf(a,b,c,d,e)}function pi(a,b,c){var d=b.pendingProps,e=d.children,f=null!==a?a.memoizedState:null;if("hidden"===d.mode)if(0===(b.mode&1))b.memoizedState={baseLanes:0,cachePool:null,transitions:null},y(Ga,ba),ba|=c;
else{if(0===(c&1073741824))return a=null!==f?f.baseLanes|c:c,b.lanes=b.childLanes=1073741824,b.memoizedState={baseLanes:a,cachePool:null,transitions:null},b.updateQueue=null,y(Ga,ba),ba|=a,null;b.memoizedState={baseLanes:0,cachePool:null,transitions:null};d=null!==f?f.baseLanes:c;y(Ga,ba);ba|=d}else null!==f?(d=f.baseLanes|c,b.memoizedState=null):d=c,y(Ga,ba),ba|=d;aa(a,b,e,c);return b.child}function qi(a,b){var c=b.ref;if(null===a&&null!==c||null!==a&&a.ref!==c)b.flags|=512,b.flags|=2097152}function zf(a,
b,c,d,e){var f=ea(c)?pb:J.current;f=Nb(b,f);Sb(b,e);c=mf(a,b,c,d,f,e);d=nf();if(null!==a&&!ha)return b.updateQueue=a.updateQueue,b.flags&=-2053,a.lanes&=~e,Qa(a,b,e);D&&d&&Ue(b);b.flags|=1;aa(a,b,c,e);return b.child}function ri(a,b,c,d,e){if(ea(c)){var f=!0;ld(b)}else f=!1;Sb(b,e);if(null===b.stateNode)Fd(a,b),ei(b,c,d),uf(b,c,d,e),d=!0;else if(null===a){var g=b.stateNode,h=b.memoizedProps;g.props=h;var k=g.context,n=c.contextType;"object"===typeof n&&null!==n?n=qa(n):(n=ea(c)?pb:J.current,n=Nb(b,
n));var l=c.getDerivedStateFromProps,m="function"===typeof l||"function"===typeof g.getSnapshotBeforeUpdate;m||"function"!==typeof g.UNSAFE_componentWillReceiveProps&&"function"!==typeof g.componentWillReceiveProps||(h!==d||k!==n)&&fi(b,g,d,n);gb=!1;var r=b.memoizedState;g.state=r;wd(b,d,g,e);k=b.memoizedState;h!==d||r!==k||S.current||gb?("function"===typeof l&&(tf(b,c,l,d),k=b.memoizedState),(h=gb||di(b,c,h,d,r,k,n))?(m||"function"!==typeof g.UNSAFE_componentWillMount&&"function"!==typeof g.componentWillMount||
("function"===typeof g.componentWillMount&&g.componentWillMount(),"function"===typeof g.UNSAFE_componentWillMount&&g.UNSAFE_componentWillMount()),"function"===typeof g.componentDidMount&&(b.flags|=4194308)):("function"===typeof g.componentDidMount&&(b.flags|=4194308),b.memoizedProps=d,b.memoizedState=k),g.props=d,g.state=k,g.context=n,d=h):("function"===typeof g.componentDidMount&&(b.flags|=4194308),d=!1)}else{g=b.stateNode;Fh(a,b);h=b.memoizedProps;n=b.type===b.elementType?h:ya(b.type,h);g.props=
n;m=b.pendingProps;r=g.context;k=c.contextType;"object"===typeof k&&null!==k?k=qa(k):(k=ea(c)?pb:J.current,k=Nb(b,k));var p=c.getDerivedStateFromProps;(l="function"===typeof p||"function"===typeof g.getSnapshotBeforeUpdate)||"function"!==typeof g.UNSAFE_componentWillReceiveProps&&"function"!==typeof g.componentWillReceiveProps||(h!==m||r!==k)&&fi(b,g,d,k);gb=!1;r=b.memoizedState;g.state=r;wd(b,d,g,e);var x=b.memoizedState;h!==m||r!==x||S.current||gb?("function"===typeof p&&(tf(b,c,p,d),x=b.memoizedState),
(n=gb||di(b,c,n,d,r,x,k)||!1)?(l||"function"!==typeof g.UNSAFE_componentWillUpdate&&"function"!==typeof g.componentWillUpdate||("function"===typeof g.componentWillUpdate&&g.componentWillUpdate(d,x,k),"function"===typeof g.UNSAFE_componentWillUpdate&&g.UNSAFE_componentWillUpdate(d,x,k)),"function"===typeof g.componentDidUpdate&&(b.flags|=4),"function"===typeof g.getSnapshotBeforeUpdate&&(b.flags|=1024)):("function"!==typeof g.componentDidUpdate||h===a.memoizedProps&&r===a.memoizedState||(b.flags|=
4),"function"!==typeof g.getSnapshotBeforeUpdate||h===a.memoizedProps&&r===a.memoizedState||(b.flags|=1024),b.memoizedProps=d,b.memoizedState=x),g.props=d,g.state=x,g.context=k,d=n):("function"!==typeof g.componentDidUpdate||h===a.memoizedProps&&r===a.memoizedState||(b.flags|=4),"function"!==typeof g.getSnapshotBeforeUpdate||h===a.memoizedProps&&r===a.memoizedState||(b.flags|=1024),d=!1)}return Af(a,b,c,d,f,e)}function Af(a,b,c,d,e,f){qi(a,b);var g=0!==(b.flags&128);if(!d&&!g)return e&&vh(b,c,!1),
Qa(a,b,f);d=b.stateNode;tk.current=b;var h=g&&"function"!==typeof c.getDerivedStateFromError?null:d.render();b.flags|=1;null!==a&&g?(b.child=Vb(b,a.child,null,f),b.child=Vb(b,null,h,f)):aa(a,b,h,f);b.memoizedState=d.state;e&&vh(b,c,!0);return b.child}function si(a){var b=a.stateNode;b.pendingContext?th(a,b.pendingContext,b.pendingContext!==b.context):b.context&&th(a,b.context,!1);gf(a,b.containerInfo)}function ti(a,b,c,d,e){Qb();Ye(e);b.flags|=256;aa(a,b,c,d);return b.child}function Bf(a){return{baseLanes:a,
cachePool:null,transitions:null}}function ui(a,b,c){var d=b.pendingProps,e=F.current,f=!1,g=0!==(b.flags&128),h;(h=g)||(h=null!==a&&null===a.memoizedState?!1:0!==(e&2));if(h)f=!0,b.flags&=-129;else if(null===a||null!==a.memoizedState)e|=1;y(F,e&1);if(null===a){Xe(b);a=b.memoizedState;if(null!==a&&(a=a.dehydrated,null!==a))return 0===(b.mode&1)?b.lanes=1:"$!"===a.data?b.lanes=8:b.lanes=1073741824,null;g=d.children;a=d.fallback;return f?(d=b.mode,f=b.child,g={mode:"hidden",children:g},0===(d&1)&&null!==
f?(f.childLanes=0,f.pendingProps=g):f=Gd(g,d,0,null),a=sb(a,d,c,null),f.return=b,a.return=b,f.sibling=a,b.child=f,b.child.memoizedState=Bf(c),b.memoizedState=Cf,a):Df(b,g)}e=a.memoizedState;if(null!==e&&(h=e.dehydrated,null!==h))return uk(a,b,g,d,h,e,c);if(f){f=d.fallback;g=b.mode;e=a.child;h=e.sibling;var k={mode:"hidden",children:d.children};0===(g&1)&&b.child!==e?(d=b.child,d.childLanes=0,d.pendingProps=k,b.deletions=null):(d=eb(e,k),d.subtreeFlags=e.subtreeFlags&14680064);null!==h?f=eb(h,f):(f=
sb(f,g,c,null),f.flags|=2);f.return=b;d.return=b;d.sibling=f;b.child=d;d=f;f=b.child;g=a.child.memoizedState;g=null===g?Bf(c):{baseLanes:g.baseLanes|c,cachePool:null,transitions:g.transitions};f.memoizedState=g;f.childLanes=a.childLanes&~c;b.memoizedState=Cf;return d}f=a.child;a=f.sibling;d=eb(f,{mode:"visible",children:d.children});0===(b.mode&1)&&(d.lanes=c);d.return=b;d.sibling=null;null!==a&&(c=b.deletions,null===c?(b.deletions=[a],b.flags|=16):c.push(a));b.child=d;b.memoizedState=null;return d}
function Df(a,b,c){b=Gd({mode:"visible",children:b},a.mode,0,null);b.return=a;return a.child=b}function Hd(a,b,c,d){null!==d&&Ye(d);Vb(b,a.child,null,c);a=Df(b,b.pendingProps.children);a.flags|=2;b.memoizedState=null;return a}function uk(a,b,c,d,e,f,g){if(c){if(b.flags&256)return b.flags&=-257,d=vf(Error(m(422))),Hd(a,b,g,d);if(null!==b.memoizedState)return b.child=a.child,b.flags|=128,null;f=d.fallback;e=b.mode;d=Gd({mode:"visible",children:d.children},e,0,null);f=sb(f,e,g,null);f.flags|=2;d.return=
b;f.return=b;d.sibling=f;b.child=d;0!==(b.mode&1)&&Vb(b,a.child,null,g);b.child.memoizedState=Bf(g);b.memoizedState=Cf;return f}if(0===(b.mode&1))return Hd(a,b,g,null);if("$!"===e.data){d=e.nextSibling&&e.nextSibling.dataset;if(d)var h=d.dgst;d=h;f=Error(m(419));d=vf(f,d,void 0);return Hd(a,b,g,d)}h=0!==(g&a.childLanes);if(ha||h){d=O;if(null!==d){switch(g&-g){case 4:e=2;break;case 16:e=8;break;case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:e=
32;break;case 536870912:e=268435456;break;default:e=0}e=0!==(e&(d.suspendedLanes|g))?0:e;0!==e&&e!==f.retryLane&&(f.retryLane=e,Oa(a,e),xa(d,a,e,-1))}Ef();d=vf(Error(m(421)));return Hd(a,b,g,d)}if("$?"===e.data)return b.flags|=128,b.child=a.child,b=vk.bind(null,a),e._reactRetry=b,null;a=f.treeContext;fa=Ka(e.nextSibling);la=b;D=!0;wa=null;null!==a&&(na[oa++]=Ma,na[oa++]=Na,na[oa++]=rb,Ma=a.id,Na=a.overflow,rb=b);b=Df(b,d.children);b.flags|=4096;return b}function vi(a,b,c){a.lanes|=b;var d=a.alternate;
null!==d&&(d.lanes|=b);df(a.return,b,c)}function Ff(a,b,c,d,e){var f=a.memoizedState;null===f?a.memoizedState={isBackwards:b,rendering:null,renderingStartTime:0,last:d,tail:c,tailMode:e}:(f.isBackwards=b,f.rendering=null,f.renderingStartTime=0,f.last=d,f.tail=c,f.tailMode=e)}function wi(a,b,c){var d=b.pendingProps,e=d.revealOrder,f=d.tail;aa(a,b,d.children,c);d=F.current;if(0!==(d&2))d=d&1|2,b.flags|=128;else{if(null!==a&&0!==(a.flags&128))a:for(a=b.child;null!==a;){if(13===a.tag)null!==a.memoizedState&&
vi(a,c,b);else if(19===a.tag)vi(a,c,b);else if(null!==a.child){a.child.return=a;a=a.child;continue}if(a===b)break a;for(;null===a.sibling;){if(null===a.return||a.return===b)break a;a=a.return}a.sibling.return=a.return;a=a.sibling}d&=1}y(F,d);if(0===(b.mode&1))b.memoizedState=null;else switch(e){case "forwards":c=b.child;for(e=null;null!==c;)a=c.alternate,null!==a&&null===xd(a)&&(e=c),c=c.sibling;c=e;null===c?(e=b.child,b.child=null):(e=c.sibling,c.sibling=null);Ff(b,!1,e,c,f);break;case "backwards":c=
null;e=b.child;for(b.child=null;null!==e;){a=e.alternate;if(null!==a&&null===xd(a)){b.child=e;break}a=e.sibling;e.sibling=c;c=e;e=a}Ff(b,!0,c,null,f);break;case "together":Ff(b,!1,null,null,void 0);break;default:b.memoizedState=null}return b.child}function Fd(a,b){0===(b.mode&1)&&null!==a&&(a.alternate=null,b.alternate=null,b.flags|=2)}function Qa(a,b,c){null!==a&&(b.dependencies=a.dependencies);ra|=b.lanes;if(0===(c&b.childLanes))return null;if(null!==a&&b.child!==a.child)throw Error(m(153));if(null!==
b.child){a=b.child;c=eb(a,a.pendingProps);b.child=c;for(c.return=b;null!==a.sibling;)a=a.sibling,c=c.sibling=eb(a,a.pendingProps),c.return=b;c.sibling=null}return b.child}function wk(a,b,c){switch(b.tag){case 3:si(b);Qb();break;case 5:Ih(b);break;case 1:ea(b.type)&&ld(b);break;case 4:gf(b,b.stateNode.containerInfo);break;case 10:var d=b.type._context,e=b.memoizedProps.value;y(ud,d._currentValue);d._currentValue=e;break;case 13:d=b.memoizedState;if(null!==d){if(null!==d.dehydrated)return y(F,F.current&
1),b.flags|=128,null;if(0!==(c&b.child.childLanes))return ui(a,b,c);y(F,F.current&1);a=Qa(a,b,c);return null!==a?a.sibling:null}y(F,F.current&1);break;case 19:d=0!==(c&b.childLanes);if(0!==(a.flags&128)){if(d)return wi(a,b,c);b.flags|=128}e=b.memoizedState;null!==e&&(e.rendering=null,e.tail=null,e.lastEffect=null);y(F,F.current);if(d)break;else return null;case 22:case 23:return b.lanes=0,pi(a,b,c)}return Qa(a,b,c)}function Dc(a,b){if(!D)switch(a.tailMode){case "hidden":b=a.tail;for(var c=null;null!==
b;)null!==b.alternate&&(c=b),b=b.sibling;null===c?a.tail=null:c.sibling=null;break;case "collapsed":c=a.tail;for(var d=null;null!==c;)null!==c.alternate&&(d=c),c=c.sibling;null===d?b||null===a.tail?a.tail=null:a.tail.sibling=null:d.sibling=null}}function W(a){var b=null!==a.alternate&&a.alternate.child===a.child,c=0,d=0;if(b)for(var e=a.child;null!==e;)c|=e.lanes|e.childLanes,d|=e.subtreeFlags&14680064,d|=e.flags&14680064,e.return=a,e=e.sibling;else for(e=a.child;null!==e;)c|=e.lanes|e.childLanes,
d|=e.subtreeFlags,d|=e.flags,e.return=a,e=e.sibling;a.subtreeFlags|=d;a.childLanes=c;return b}function xk(a,b,c){var d=b.pendingProps;Ve(b);switch(b.tag){case 2:case 16:case 15:case 0:case 11:case 7:case 8:case 12:case 9:case 14:return W(b),null;case 1:return ea(b.type)&&(v(S),v(J)),W(b),null;case 3:d=b.stateNode;Tb();v(S);v(J);jf();d.pendingContext&&(d.context=d.pendingContext,d.pendingContext=null);if(null===a||null===a.child)pd(b)?b.flags|=4:null===a||a.memoizedState.isDehydrated&&0===(b.flags&
256)||(b.flags|=1024,null!==wa&&(Gf(wa),wa=null));xi(a,b);W(b);return null;case 5:hf(b);var e=ub(xc.current);c=b.type;if(null!==a&&null!=b.stateNode)yk(a,b,c,d,e),a.ref!==b.ref&&(b.flags|=512,b.flags|=2097152);else{if(!d){if(null===b.stateNode)throw Error(m(166));W(b);return null}a=ub(Ea.current);if(pd(b)){d=b.stateNode;c=b.type;var f=b.memoizedProps;d[Da]=b;d[uc]=f;a=0!==(b.mode&1);switch(c){case "dialog":B("cancel",d);B("close",d);break;case "iframe":case "object":case "embed":B("load",d);break;
case "video":case "audio":for(e=0;e<Ec.length;e++)B(Ec[e],d);break;case "source":B("error",d);break;case "img":case "image":case "link":B("error",d);B("load",d);break;case "details":B("toggle",d);break;case "input":kg(d,f);B("invalid",d);break;case "select":d._wrapperState={wasMultiple:!!f.multiple};B("invalid",d);break;case "textarea":ng(d,f),B("invalid",d)}pe(c,f);e=null;for(var g in f)if(f.hasOwnProperty(g)){var h=f[g];"children"===g?"string"===typeof h?d.textContent!==h&&(!0!==f.suppressHydrationWarning&&
jd(d.textContent,h,a),e=["children",h]):"number"===typeof h&&d.textContent!==""+h&&(!0!==f.suppressHydrationWarning&&jd(d.textContent,h,a),e=["children",""+h]):$b.hasOwnProperty(g)&&null!=h&&"onScroll"===g&&B("scroll",d)}switch(c){case "input":Pc(d);mg(d,f,!0);break;case "textarea":Pc(d);pg(d);break;case "select":case "option":break;default:"function"===typeof f.onClick&&(d.onclick=kd)}d=e;b.updateQueue=d;null!==d&&(b.flags|=4)}else{g=9===e.nodeType?e:e.ownerDocument;"http://www.w3.org/1999/xhtml"===
a&&(a=qg(c));"http://www.w3.org/1999/xhtml"===a?"script"===c?(a=g.createElement("div"),a.innerHTML="<script>\x3c/script>",a=a.removeChild(a.firstChild)):"string"===typeof d.is?a=g.createElement(c,{is:d.is}):(a=g.createElement(c),"select"===c&&(g=a,d.multiple?g.multiple=!0:d.size&&(g.size=d.size))):a=g.createElementNS(a,c);a[Da]=b;a[uc]=d;zk(a,b,!1,!1);b.stateNode=a;a:{g=qe(c,d);switch(c){case "dialog":B("cancel",a);B("close",a);e=d;break;case "iframe":case "object":case "embed":B("load",a);e=d;break;
case "video":case "audio":for(e=0;e<Ec.length;e++)B(Ec[e],a);e=d;break;case "source":B("error",a);e=d;break;case "img":case "image":case "link":B("error",a);B("load",a);e=d;break;case "details":B("toggle",a);e=d;break;case "input":kg(a,d);e=ke(a,d);B("invalid",a);break;case "option":e=d;break;case "select":a._wrapperState={wasMultiple:!!d.multiple};e=E({},d,{value:void 0});B("invalid",a);break;case "textarea":ng(a,d);e=ne(a,d);B("invalid",a);break;default:e=d}pe(c,e);h=e;for(f in h)if(h.hasOwnProperty(f)){var k=
h[f];"style"===f?sg(a,k):"dangerouslySetInnerHTML"===f?(k=k?k.__html:void 0,null!=k&&yi(a,k)):"children"===f?"string"===typeof k?("textarea"!==c||""!==k)&&Fc(a,k):"number"===typeof k&&Fc(a,""+k):"suppressContentEditableWarning"!==f&&"suppressHydrationWarning"!==f&&"autoFocus"!==f&&($b.hasOwnProperty(f)?null!=k&&"onScroll"===f&&B("scroll",a):null!=k&&$d(a,f,k,g))}switch(c){case "input":Pc(a);mg(a,d,!1);break;case "textarea":Pc(a);pg(a);break;case "option":null!=d.value&&a.setAttribute("value",""+Ua(d.value));
break;case "select":a.multiple=!!d.multiple;f=d.value;null!=f?Db(a,!!d.multiple,f,!1):null!=d.defaultValue&&Db(a,!!d.multiple,d.defaultValue,!0);break;default:"function"===typeof e.onClick&&(a.onclick=kd)}switch(c){case "button":case "input":case "select":case "textarea":d=!!d.autoFocus;break a;case "img":d=!0;break a;default:d=!1}}d&&(b.flags|=4)}null!==b.ref&&(b.flags|=512,b.flags|=2097152)}W(b);return null;case 6:if(a&&null!=b.stateNode)Ak(a,b,a.memoizedProps,d);else{if("string"!==typeof d&&null===
b.stateNode)throw Error(m(166));c=ub(xc.current);ub(Ea.current);if(pd(b)){d=b.stateNode;c=b.memoizedProps;d[Da]=b;if(f=d.nodeValue!==c)if(a=la,null!==a)switch(a.tag){case 3:jd(d.nodeValue,c,0!==(a.mode&1));break;case 5:!0!==a.memoizedProps.suppressHydrationWarning&&jd(d.nodeValue,c,0!==(a.mode&1))}f&&(b.flags|=4)}else d=(9===c.nodeType?c:c.ownerDocument).createTextNode(d),d[Da]=b,b.stateNode=d}W(b);return null;case 13:v(F);d=b.memoizedState;if(null===a||null!==a.memoizedState&&null!==a.memoizedState.dehydrated){if(D&&
null!==fa&&0!==(b.mode&1)&&0===(b.flags&128)){for(f=fa;f;)f=Ka(f.nextSibling);Qb();b.flags|=98560;f=!1}else if(f=pd(b),null!==d&&null!==d.dehydrated){if(null===a){if(!f)throw Error(m(318));f=b.memoizedState;f=null!==f?f.dehydrated:null;if(!f)throw Error(m(317));f[Da]=b}else Qb(),0===(b.flags&128)&&(b.memoizedState=null),b.flags|=4;W(b);f=!1}else null!==wa&&(Gf(wa),wa=null),f=!0;if(!f)return b.flags&65536?b:null}if(0!==(b.flags&128))return b.lanes=c,b;d=null!==d;d!==(null!==a&&null!==a.memoizedState)&&
d&&(b.child.flags|=8192,0!==(b.mode&1)&&(null===a||0!==(F.current&1)?0===L&&(L=3):Ef()));null!==b.updateQueue&&(b.flags|=4);W(b);return null;case 4:return Tb(),xi(a,b),null===a&&sc(b.stateNode.containerInfo),W(b),null;case 10:return cf(b.type._context),W(b),null;case 17:return ea(b.type)&&(v(S),v(J)),W(b),null;case 19:v(F);f=b.memoizedState;if(null===f)return W(b),null;d=0!==(b.flags&128);g=f.rendering;if(null===g)if(d)Dc(f,!1);else{if(0!==L||null!==a&&0!==(a.flags&128))for(a=b.child;null!==a;){g=
xd(a);if(null!==g){b.flags|=128;Dc(f,!1);d=g.updateQueue;null!==d&&(b.updateQueue=d,b.flags|=4);b.subtreeFlags=0;d=c;for(c=b.child;null!==c;)f=c,a=d,f.flags&=14680066,g=f.alternate,null===g?(f.childLanes=0,f.lanes=a,f.child=null,f.subtreeFlags=0,f.memoizedProps=null,f.memoizedState=null,f.updateQueue=null,f.dependencies=null,f.stateNode=null):(f.childLanes=g.childLanes,f.lanes=g.lanes,f.child=g.child,f.subtreeFlags=0,f.deletions=null,f.memoizedProps=g.memoizedProps,f.memoizedState=g.memoizedState,
f.updateQueue=g.updateQueue,f.type=g.type,a=g.dependencies,f.dependencies=null===a?null:{lanes:a.lanes,firstContext:a.firstContext}),c=c.sibling;y(F,F.current&1|2);return b.child}a=a.sibling}null!==f.tail&&P()>Hf&&(b.flags|=128,d=!0,Dc(f,!1),b.lanes=4194304)}else{if(!d)if(a=xd(g),null!==a){if(b.flags|=128,d=!0,c=a.updateQueue,null!==c&&(b.updateQueue=c,b.flags|=4),Dc(f,!0),null===f.tail&&"hidden"===f.tailMode&&!g.alternate&&!D)return W(b),null}else 2*P()-f.renderingStartTime>Hf&&1073741824!==c&&(b.flags|=
128,d=!0,Dc(f,!1),b.lanes=4194304);f.isBackwards?(g.sibling=b.child,b.child=g):(c=f.last,null!==c?c.sibling=g:b.child=g,f.last=g)}if(null!==f.tail)return b=f.tail,f.rendering=b,f.tail=b.sibling,f.renderingStartTime=P(),b.sibling=null,c=F.current,y(F,d?c&1|2:c&1),b;W(b);return null;case 22:case 23:return ba=Ga.current,v(Ga),d=null!==b.memoizedState,null!==a&&null!==a.memoizedState!==d&&(b.flags|=8192),d&&0!==(b.mode&1)?0!==(ba&1073741824)&&(W(b),b.subtreeFlags&6&&(b.flags|=8192)):W(b),null;case 24:return null;
case 25:return null}throw Error(m(156,b.tag));}function Bk(a,b,c){Ve(b);switch(b.tag){case 1:return ea(b.type)&&(v(S),v(J)),a=b.flags,a&65536?(b.flags=a&-65537|128,b):null;case 3:return Tb(),v(S),v(J),jf(),a=b.flags,0!==(a&65536)&&0===(a&128)?(b.flags=a&-65537|128,b):null;case 5:return hf(b),null;case 13:v(F);a=b.memoizedState;if(null!==a&&null!==a.dehydrated){if(null===b.alternate)throw Error(m(340));Qb()}a=b.flags;return a&65536?(b.flags=a&-65537|128,b):null;case 19:return v(F),null;case 4:return Tb(),
null;case 10:return cf(b.type._context),null;case 22:case 23:return ba=Ga.current,v(Ga),null;case 24:return null;default:return null}}function Wb(a,b){var c=a.ref;if(null!==c)if("function"===typeof c)try{c(null)}catch(d){G(a,b,d)}else c.current=null}function If(a,b,c){try{c()}catch(d){G(a,b,d)}}function Ck(a,b){Jf=Zc;a=ch();if(Ie(a)){if("selectionStart"in a)var c={start:a.selectionStart,end:a.selectionEnd};else a:{c=(c=a.ownerDocument)&&c.defaultView||window;var d=c.getSelection&&c.getSelection();
if(d&&0!==d.rangeCount){c=d.anchorNode;var e=d.anchorOffset,f=d.focusNode;d=d.focusOffset;try{c.nodeType,f.nodeType}catch(M){c=null;break a}var g=0,h=-1,k=-1,n=0,q=0,u=a,r=null;b:for(;;){for(var p;;){u!==c||0!==e&&3!==u.nodeType||(h=g+e);u!==f||0!==d&&3!==u.nodeType||(k=g+d);3===u.nodeType&&(g+=u.nodeValue.length);if(null===(p=u.firstChild))break;r=u;u=p}for(;;){if(u===a)break b;r===c&&++n===e&&(h=g);r===f&&++q===d&&(k=g);if(null!==(p=u.nextSibling))break;u=r;r=u.parentNode}u=p}c=-1===h||-1===k?null:
{start:h,end:k}}else c=null}c=c||{start:0,end:0}}else c=null;Kf={focusedElem:a,selectionRange:c};Zc=!1;for(l=b;null!==l;)if(b=l,a=b.child,0!==(b.subtreeFlags&1028)&&null!==a)a.return=b,l=a;else for(;null!==l;){b=l;try{var x=b.alternate;if(0!==(b.flags&1024))switch(b.tag){case 0:case 11:case 15:break;case 1:if(null!==x){var v=x.memoizedProps,z=x.memoizedState,w=b.stateNode,A=w.getSnapshotBeforeUpdate(b.elementType===b.type?v:ya(b.type,v),z);w.__reactInternalSnapshotBeforeUpdate=A}break;case 3:var t=
b.stateNode.containerInfo;1===t.nodeType?t.textContent="":9===t.nodeType&&t.documentElement&&t.removeChild(t.documentElement);break;case 5:case 6:case 4:case 17:break;default:throw Error(m(163));}}catch(M){G(b,b.return,M)}a=b.sibling;if(null!==a){a.return=b.return;l=a;break}l=b.return}x=zi;zi=!1;return x}function Gc(a,b,c){var d=b.updateQueue;d=null!==d?d.lastEffect:null;if(null!==d){var e=d=d.next;do{if((e.tag&a)===a){var f=e.destroy;e.destroy=void 0;void 0!==f&&If(b,c,f)}e=e.next}while(e!==d)}}
function Id(a,b){b=b.updateQueue;b=null!==b?b.lastEffect:null;if(null!==b){var c=b=b.next;do{if((c.tag&a)===a){var d=c.create;c.destroy=d()}c=c.next}while(c!==b)}}function Lf(a){var b=a.ref;if(null!==b){var c=a.stateNode;switch(a.tag){case 5:a=c;break;default:a=c}"function"===typeof b?b(a):b.current=a}}function Ai(a){var b=a.alternate;null!==b&&(a.alternate=null,Ai(b));a.child=null;a.deletions=null;a.sibling=null;5===a.tag&&(b=a.stateNode,null!==b&&(delete b[Da],delete b[uc],delete b[Me],delete b[Dk],
delete b[Ek]));a.stateNode=null;a.return=null;a.dependencies=null;a.memoizedProps=null;a.memoizedState=null;a.pendingProps=null;a.stateNode=null;a.updateQueue=null}function Bi(a){return 5===a.tag||3===a.tag||4===a.tag}function Ci(a){a:for(;;){for(;null===a.sibling;){if(null===a.return||Bi(a.return))return null;a=a.return}a.sibling.return=a.return;for(a=a.sibling;5!==a.tag&&6!==a.tag&&18!==a.tag;){if(a.flags&2)continue a;if(null===a.child||4===a.tag)continue a;else a.child.return=a,a=a.child}if(!(a.flags&
2))return a.stateNode}}function Mf(a,b,c){var d=a.tag;if(5===d||6===d)a=a.stateNode,b?8===c.nodeType?c.parentNode.insertBefore(a,b):c.insertBefore(a,b):(8===c.nodeType?(b=c.parentNode,b.insertBefore(a,c)):(b=c,b.appendChild(a)),c=c._reactRootContainer,null!==c&&void 0!==c||null!==b.onclick||(b.onclick=kd));else if(4!==d&&(a=a.child,null!==a))for(Mf(a,b,c),a=a.sibling;null!==a;)Mf(a,b,c),a=a.sibling}function Nf(a,b,c){var d=a.tag;if(5===d||6===d)a=a.stateNode,b?c.insertBefore(a,b):c.appendChild(a);
else if(4!==d&&(a=a.child,null!==a))for(Nf(a,b,c),a=a.sibling;null!==a;)Nf(a,b,c),a=a.sibling}function jb(a,b,c){for(c=c.child;null!==c;)Di(a,b,c),c=c.sibling}function Di(a,b,c){if(Ca&&"function"===typeof Ca.onCommitFiberUnmount)try{Ca.onCommitFiberUnmount(Uc,c)}catch(h){}switch(c.tag){case 5:X||Wb(c,b);case 6:var d=T,e=za;T=null;jb(a,b,c);T=d;za=e;null!==T&&(za?(a=T,c=c.stateNode,8===a.nodeType?a.parentNode.removeChild(c):a.removeChild(c)):T.removeChild(c.stateNode));break;case 18:null!==T&&(za?
(a=T,c=c.stateNode,8===a.nodeType?Re(a.parentNode,c):1===a.nodeType&&Re(a,c),nc(a)):Re(T,c.stateNode));break;case 4:d=T;e=za;T=c.stateNode.containerInfo;za=!0;jb(a,b,c);T=d;za=e;break;case 0:case 11:case 14:case 15:if(!X&&(d=c.updateQueue,null!==d&&(d=d.lastEffect,null!==d))){e=d=d.next;do{var f=e,g=f.destroy;f=f.tag;void 0!==g&&(0!==(f&2)?If(c,b,g):0!==(f&4)&&If(c,b,g));e=e.next}while(e!==d)}jb(a,b,c);break;case 1:if(!X&&(Wb(c,b),d=c.stateNode,"function"===typeof d.componentWillUnmount))try{d.props=
c.memoizedProps,d.state=c.memoizedState,d.componentWillUnmount()}catch(h){G(c,b,h)}jb(a,b,c);break;case 21:jb(a,b,c);break;case 22:c.mode&1?(X=(d=X)||null!==c.memoizedState,jb(a,b,c),X=d):jb(a,b,c);break;default:jb(a,b,c)}}function Ei(a){var b=a.updateQueue;if(null!==b){a.updateQueue=null;var c=a.stateNode;null===c&&(c=a.stateNode=new Fk);b.forEach(function(b){var d=Gk.bind(null,a,b);c.has(b)||(c.add(b),b.then(d,d))})}}function Aa(a,b,c){c=b.deletions;if(null!==c)for(var d=0;d<c.length;d++){var e=
c[d];try{var f=a,g=b,h=g;a:for(;null!==h;){switch(h.tag){case 5:T=h.stateNode;za=!1;break a;case 3:T=h.stateNode.containerInfo;za=!0;break a;case 4:T=h.stateNode.containerInfo;za=!0;break a}h=h.return}if(null===T)throw Error(m(160));Di(f,g,e);T=null;za=!1;var k=e.alternate;null!==k&&(k.return=null);e.return=null}catch(n){G(e,b,n)}}if(b.subtreeFlags&12854)for(b=b.child;null!==b;)Fi(b,a),b=b.sibling}function Fi(a,b,c){var d=a.alternate;c=a.flags;switch(a.tag){case 0:case 11:case 14:case 15:Aa(b,a);
Ha(a);if(c&4){try{Gc(3,a,a.return),Id(3,a)}catch(I){G(a,a.return,I)}try{Gc(5,a,a.return)}catch(I){G(a,a.return,I)}}break;case 1:Aa(b,a);Ha(a);c&512&&null!==d&&Wb(d,d.return);break;case 5:Aa(b,a);Ha(a);c&512&&null!==d&&Wb(d,d.return);if(a.flags&32){var e=a.stateNode;try{Fc(e,"")}catch(I){G(a,a.return,I)}}if(c&4&&(e=a.stateNode,null!=e)){var f=a.memoizedProps,g=null!==d?d.memoizedProps:f,h=a.type,k=a.updateQueue;a.updateQueue=null;if(null!==k)try{"input"===h&&"radio"===f.type&&null!=f.name&&lg(e,f);
qe(h,g);var n=qe(h,f);for(g=0;g<k.length;g+=2){var q=k[g],u=k[g+1];"style"===q?sg(e,u):"dangerouslySetInnerHTML"===q?yi(e,u):"children"===q?Fc(e,u):$d(e,q,u,n)}switch(h){case "input":le(e,f);break;case "textarea":og(e,f);break;case "select":var r=e._wrapperState.wasMultiple;e._wrapperState.wasMultiple=!!f.multiple;var p=f.value;null!=p?Db(e,!!f.multiple,p,!1):r!==!!f.multiple&&(null!=f.defaultValue?Db(e,!!f.multiple,f.defaultValue,!0):Db(e,!!f.multiple,f.multiple?[]:"",!1))}e[uc]=f}catch(I){G(a,a.return,
I)}}break;case 6:Aa(b,a);Ha(a);if(c&4){if(null===a.stateNode)throw Error(m(162));e=a.stateNode;f=a.memoizedProps;try{e.nodeValue=f}catch(I){G(a,a.return,I)}}break;case 3:Aa(b,a);Ha(a);if(c&4&&null!==d&&d.memoizedState.isDehydrated)try{nc(b.containerInfo)}catch(I){G(a,a.return,I)}break;case 4:Aa(b,a);Ha(a);break;case 13:Aa(b,a);Ha(a);e=a.child;e.flags&8192&&(f=null!==e.memoizedState,e.stateNode.isHidden=f,!f||null!==e.alternate&&null!==e.alternate.memoizedState||(Of=P()));c&4&&Ei(a);break;case 22:q=
null!==d&&null!==d.memoizedState;a.mode&1?(X=(n=X)||q,Aa(b,a),X=n):Aa(b,a);Ha(a);if(c&8192){n=null!==a.memoizedState;if((a.stateNode.isHidden=n)&&!q&&0!==(a.mode&1))for(l=a,q=a.child;null!==q;){for(u=l=q;null!==l;){r=l;p=r.child;switch(r.tag){case 0:case 11:case 14:case 15:Gc(4,r,r.return);break;case 1:Wb(r,r.return);var x=r.stateNode;if("function"===typeof x.componentWillUnmount){c=r;b=r.return;try{d=c,x.props=d.memoizedProps,x.state=d.memoizedState,x.componentWillUnmount()}catch(I){G(c,b,I)}}break;
case 5:Wb(r,r.return);break;case 22:if(null!==r.memoizedState){Gi(u);continue}}null!==p?(p.return=r,l=p):Gi(u)}q=q.sibling}a:for(q=null,u=a;;){if(5===u.tag){if(null===q){q=u;try{e=u.stateNode,n?(f=e.style,"function"===typeof f.setProperty?f.setProperty("display","none","important"):f.display="none"):(h=u.stateNode,k=u.memoizedProps.style,g=void 0!==k&&null!==k&&k.hasOwnProperty("display")?k.display:null,h.style.display=rg("display",g))}catch(I){G(a,a.return,I)}}}else if(6===u.tag){if(null===q)try{u.stateNode.nodeValue=
n?"":u.memoizedProps}catch(I){G(a,a.return,I)}}else if((22!==u.tag&&23!==u.tag||null===u.memoizedState||u===a)&&null!==u.child){u.child.return=u;u=u.child;continue}if(u===a)break a;for(;null===u.sibling;){if(null===u.return||u.return===a)break a;q===u&&(q=null);u=u.return}q===u&&(q=null);u.sibling.return=u.return;u=u.sibling}}break;case 19:Aa(b,a);Ha(a);c&4&&Ei(a);break;case 21:break;default:Aa(b,a),Ha(a)}}function Ha(a){var b=a.flags;if(b&2){try{a:{for(var c=a.return;null!==c;){if(Bi(c)){var d=c;
break a}c=c.return}throw Error(m(160));}switch(d.tag){case 5:var e=d.stateNode;d.flags&32&&(Fc(e,""),d.flags&=-33);var f=Ci(a);Nf(a,f,e);break;case 3:case 4:var g=d.stateNode.containerInfo,h=Ci(a);Mf(a,h,g);break;default:throw Error(m(161));}}catch(k){G(a,a.return,k)}a.flags&=-3}b&4096&&(a.flags&=-4097)}function Hk(a,b,c){l=a;Hi(a,b,c)}function Hi(a,b,c){for(var d=0!==(a.mode&1);null!==l;){var e=l,f=e.child;if(22===e.tag&&d){var g=null!==e.memoizedState||Jd;if(!g){var h=e.alternate,k=null!==h&&null!==
h.memoizedState||X;h=Jd;var n=X;Jd=g;if((X=k)&&!n)for(l=e;null!==l;)g=l,k=g.child,22===g.tag&&null!==g.memoizedState?Ii(e):null!==k?(k.return=g,l=k):Ii(e);for(;null!==f;)l=f,Hi(f,b,c),f=f.sibling;l=e;Jd=h;X=n}Ji(a,b,c)}else 0!==(e.subtreeFlags&8772)&&null!==f?(f.return=e,l=f):Ji(a,b,c)}}function Ji(a,b,c){for(;null!==l;){b=l;if(0!==(b.flags&8772)){c=b.alternate;try{if(0!==(b.flags&8772))switch(b.tag){case 0:case 11:case 15:X||Id(5,b);break;case 1:var d=b.stateNode;if(b.flags&4&&!X)if(null===c)d.componentDidMount();
else{var e=b.elementType===b.type?c.memoizedProps:ya(b.type,c.memoizedProps);d.componentDidUpdate(e,c.memoizedState,d.__reactInternalSnapshotBeforeUpdate)}var f=b.updateQueue;null!==f&&Hh(b,f,d);break;case 3:var g=b.updateQueue;if(null!==g){c=null;if(null!==b.child)switch(b.child.tag){case 5:c=b.child.stateNode;break;case 1:c=b.child.stateNode}Hh(b,g,c)}break;case 5:var h=b.stateNode;if(null===c&&b.flags&4){c=h;var k=b.memoizedProps;switch(b.type){case "button":case "input":case "select":case "textarea":k.autoFocus&&
c.focus();break;case "img":k.src&&(c.src=k.src)}}break;case 6:break;case 4:break;case 12:break;case 13:if(null===b.memoizedState){var n=b.alternate;if(null!==n){var q=n.memoizedState;if(null!==q){var p=q.dehydrated;null!==p&&nc(p)}}}break;case 19:case 17:case 21:case 22:case 23:case 25:break;default:throw Error(m(163));}X||b.flags&512&&Lf(b)}catch(r){G(b,b.return,r)}}if(b===a){l=null;break}c=b.sibling;if(null!==c){c.return=b.return;l=c;break}l=b.return}}function Gi(a){for(;null!==l;){var b=l;if(b===
a){l=null;break}var c=b.sibling;if(null!==c){c.return=b.return;l=c;break}l=b.return}}function Ii(a){for(;null!==l;){var b=l;try{switch(b.tag){case 0:case 11:case 15:var c=b.return;try{Id(4,b)}catch(k){G(b,c,k)}break;case 1:var d=b.stateNode;if("function"===typeof d.componentDidMount){var e=b.return;try{d.componentDidMount()}catch(k){G(b,e,k)}}var f=b.return;try{Lf(b)}catch(k){G(b,f,k)}break;case 5:var g=b.return;try{Lf(b)}catch(k){G(b,g,k)}}}catch(k){G(b,b.return,k)}if(b===a){l=null;break}var h=b.sibling;
if(null!==h){h.return=b.return;l=h;break}l=b.return}}function Hc(){Hf=P()+500}function Z(){return 0!==(p&6)?P():-1!==Kd?Kd:Kd=P()}function hb(a){if(0===(a.mode&1))return 1;if(0!==(p&2)&&0!==U)return U&-U;if(null!==Ik.transition)return 0===Ld&&(Ld=Dg()),Ld;a=z;if(0!==a)return a;a=window.event;a=void 0===a?16:Lg(a.type);return a}function xa(a,b,c,d){if(50<Ic)throw Ic=0,Pf=null,Error(m(185));ic(a,c,d);if(0===(p&2)||a!==O)a===O&&(0===(p&2)&&(Md|=c),4===L&&kb(a,U)),ia(a,d),1===c&&0===p&&0===(b.mode&1)&&
(Hc(),md&&db())}function ia(a,b){var c=a.callbackNode;tj(a,b);var d=Vc(a,a===O?U:0);if(0===d)null!==c&&Ki(c),a.callbackNode=null,a.callbackPriority=0;else if(b=d&-d,a.callbackPriority!==b){null!=c&&Ki(c);if(1===b)0===a.tag?jk(Li.bind(null,a)):wh(Li.bind(null,a)),Jk(function(){0===(p&6)&&db()}),c=null;else{switch(Eg(d)){case 1:c=De;break;case 4:c=Mg;break;case 16:c=ad;break;case 536870912:c=Ng;break;default:c=ad}c=Mi(c,Ni.bind(null,a))}a.callbackPriority=b;a.callbackNode=c}}function Ni(a,b){Kd=-1;
Ld=0;if(0!==(p&6))throw Error(m(327));var c=a.callbackNode;if(Xb()&&a.callbackNode!==c)return null;var d=Vc(a,a===O?U:0);if(0===d)return null;if(0!==(d&30)||0!==(d&a.expiredLanes)||b)b=Nd(a,d);else{b=d;var e=p;p|=2;var f=Oi();if(O!==a||U!==b)Ra=null,Hc(),wb(a,b);do try{Kk();break}catch(h){Pi(a,h)}while(1);af();Od.current=f;p=e;null!==H?b=0:(O=null,U=0,b=L)}if(0!==b){2===b&&(e=ve(a),0!==e&&(d=e,b=Qf(a,e)));if(1===b)throw c=Jc,wb(a,0),kb(a,d),ia(a,P()),c;if(6===b)kb(a,d);else{e=a.current.alternate;
if(0===(d&30)&&!Lk(e)&&(b=Nd(a,d),2===b&&(f=ve(a),0!==f&&(d=f,b=Qf(a,f))),1===b))throw c=Jc,wb(a,0),kb(a,d),ia(a,P()),c;a.finishedWork=e;a.finishedLanes=d;switch(b){case 0:case 1:throw Error(m(345));case 2:xb(a,ja,Ra);break;case 3:kb(a,d);if((d&130023424)===d&&(b=Of+500-P(),10<b)){if(0!==Vc(a,0))break;e=a.suspendedLanes;if((e&d)!==d){Z();a.pingedLanes|=a.suspendedLanes&e;break}a.timeoutHandle=Rf(xb.bind(null,a,ja,Ra),b);break}xb(a,ja,Ra);break;case 4:kb(a,d);if((d&4194240)===d)break;b=a.eventTimes;
for(e=-1;0<d;){var g=31-ta(d);f=1<<g;g=b[g];g>e&&(e=g);d&=~f}d=e;d=P()-d;d=(120>d?120:480>d?480:1080>d?1080:1920>d?1920:3E3>d?3E3:4320>d?4320:1960*Mk(d/1960))-d;if(10<d){a.timeoutHandle=Rf(xb.bind(null,a,ja,Ra),d);break}xb(a,ja,Ra);break;case 5:xb(a,ja,Ra);break;default:throw Error(m(329));}}}ia(a,P());return a.callbackNode===c?Ni.bind(null,a):null}function Qf(a,b){var c=Kc;a.current.memoizedState.isDehydrated&&(wb(a,b).flags|=256);a=Nd(a,b);2!==a&&(b=ja,ja=c,null!==b&&Gf(b));return a}function Gf(a){null===
ja?ja=a:ja.push.apply(ja,a)}function Lk(a){for(var b=a;;){if(b.flags&16384){var c=b.updateQueue;if(null!==c&&(c=c.stores,null!==c))for(var d=0;d<c.length;d++){var e=c[d],f=e.getSnapshot;e=e.value;try{if(!ua(f(),e))return!1}catch(g){return!1}}}c=b.child;if(b.subtreeFlags&16384&&null!==c)c.return=b,b=c;else{if(b===a)break;for(;null===b.sibling;){if(null===b.return||b.return===a)return!0;b=b.return}b.sibling.return=b.return;b=b.sibling}}return!0}function kb(a,b){b&=~Sf;b&=~Md;a.suspendedLanes|=b;a.pingedLanes&=
~b;for(a=a.expirationTimes;0<b;){var c=31-ta(b),d=1<<c;a[c]=-1;b&=~d}}function Li(a){if(0!==(p&6))throw Error(m(327));Xb();var b=Vc(a,0);if(0===(b&1))return ia(a,P()),null;var c=Nd(a,b);if(0!==a.tag&&2===c){var d=ve(a);0!==d&&(b=d,c=Qf(a,d))}if(1===c)throw c=Jc,wb(a,0),kb(a,b),ia(a,P()),c;if(6===c)throw Error(m(345));a.finishedWork=a.current.alternate;a.finishedLanes=b;xb(a,ja,Ra);ia(a,P());return null}function Tf(a,b){var c=p;p|=1;try{return a(b)}finally{p=c,0===p&&(Hc(),md&&db())}}function yb(a){null!==
lb&&0===lb.tag&&0===(p&6)&&Xb();var b=p;p|=1;var c=ca.transition,d=z;try{if(ca.transition=null,z=1,a)return a()}finally{z=d,ca.transition=c,p=b,0===(p&6)&&db()}}function wb(a,b){a.finishedWork=null;a.finishedLanes=0;var c=a.timeoutHandle;-1!==c&&(a.timeoutHandle=-1,Nk(c));if(null!==H)for(c=H.return;null!==c;){var d=c;Ve(d);switch(d.tag){case 1:d=d.type.childContextTypes;null!==d&&void 0!==d&&(v(S),v(J));break;case 3:Tb();v(S);v(J);jf();break;case 5:hf(d);break;case 4:Tb();break;case 13:v(F);break;
case 19:v(F);break;case 10:cf(d.type._context);break;case 22:case 23:ba=Ga.current,v(Ga)}c=c.return}O=a;H=a=eb(a.current,null);U=ba=b;L=0;Jc=null;Sf=Md=ra=0;ja=Kc=null;if(null!==tb){for(b=0;b<tb.length;b++)if(c=tb[b],d=c.interleaved,null!==d){c.interleaved=null;var e=d.next,f=c.pending;if(null!==f){var g=f.next;f.next=e;d.next=g}c.pending=d}tb=null}return a}function Pi(a,b){do{var c=H;try{af();yd.current=zd;if(Ad){for(var d=C.memoizedState;null!==d;){var e=d.queue;null!==e&&(e.pending=null);d=d.next}Ad=
!1}vb=0;N=K=C=null;zc=!1;Ac=0;Uf.current=null;if(null===c||null===c.return){L=1;Jc=b;H=null;break}a:{var f=a,g=c.return,h=c,k=b;b=U;h.flags|=32768;if(null!==k&&"object"===typeof k&&"function"===typeof k.then){var n=k,l=h,p=l.tag;if(0===(l.mode&1)&&(0===p||11===p||15===p)){var r=l.alternate;r?(l.updateQueue=r.updateQueue,l.memoizedState=r.memoizedState,l.lanes=r.lanes):(l.updateQueue=null,l.memoizedState=null)}var v=ji(g);if(null!==v){v.flags&=-257;ki(v,g,h,f,b);v.mode&1&&ii(f,n,b);b=v;k=n;var x=b.updateQueue;
if(null===x){var z=new Set;z.add(k);b.updateQueue=z}else x.add(k);break a}else{if(0===(b&1)){ii(f,n,b);Ef();break a}k=Error(m(426))}}else if(D&&h.mode&1){var y=ji(g);if(null!==y){0===(y.flags&65536)&&(y.flags|=256);ki(y,g,h,f,b);Ye(Ub(k,h));break a}}f=k=Ub(k,h);4!==L&&(L=2);null===Kc?Kc=[f]:Kc.push(f);f=g;do{switch(f.tag){case 3:f.flags|=65536;b&=-b;f.lanes|=b;var w=gi(f,k,b);Gh(f,w);break a;case 1:h=k;var A=f.type,t=f.stateNode;if(0===(f.flags&128)&&("function"===typeof A.getDerivedStateFromError||
null!==t&&"function"===typeof t.componentDidCatch&&(null===ib||!ib.has(t)))){f.flags|=65536;b&=-b;f.lanes|=b;var B=hi(f,h,b);Gh(f,B);break a}}f=f.return}while(null!==f)}Qi(c)}catch(ma){b=ma;H===c&&null!==c&&(H=c=c.return);continue}break}while(1)}function Oi(){var a=Od.current;Od.current=zd;return null===a?zd:a}function Ef(){if(0===L||3===L||2===L)L=4;null===O||0===(ra&268435455)&&0===(Md&268435455)||kb(O,U)}function Nd(a,b){var c=p;p|=2;var d=Oi();if(O!==a||U!==b)Ra=null,wb(a,b);do try{Ok();break}catch(e){Pi(a,
e)}while(1);af();p=c;Od.current=d;if(null!==H)throw Error(m(261));O=null;U=0;return L}function Ok(){for(;null!==H;)Ri(H)}function Kk(){for(;null!==H&&!Pk();)Ri(H)}function Ri(a){var b=Qk(a.alternate,a,ba);a.memoizedProps=a.pendingProps;null===b?Qi(a):H=b;Uf.current=null}function Qi(a){var b=a;do{var c=b.alternate;a=b.return;if(0===(b.flags&32768)){if(c=xk(c,b,ba),null!==c){H=c;return}}else{c=Bk(c,b);if(null!==c){c.flags&=32767;H=c;return}if(null!==a)a.flags|=32768,a.subtreeFlags=0,a.deletions=null;
else{L=6;H=null;return}}b=b.sibling;if(null!==b){H=b;return}H=b=a}while(null!==b);0===L&&(L=5)}function xb(a,b,c){var d=z,e=ca.transition;try{ca.transition=null,z=1,Rk(a,b,c,d)}finally{ca.transition=e,z=d}return null}function Rk(a,b,c,d){do Xb();while(null!==lb);if(0!==(p&6))throw Error(m(327));c=a.finishedWork;var e=a.finishedLanes;if(null===c)return null;a.finishedWork=null;a.finishedLanes=0;if(c===a.current)throw Error(m(177));a.callbackNode=null;a.callbackPriority=0;var f=c.lanes|c.childLanes;
uj(a,f);a===O&&(H=O=null,U=0);0===(c.subtreeFlags&2064)&&0===(c.flags&2064)||Pd||(Pd=!0,Mi(ad,function(){Xb();return null}));f=0!==(c.flags&15990);if(0!==(c.subtreeFlags&15990)||f){f=ca.transition;ca.transition=null;var g=z;z=1;var h=p;p|=4;Uf.current=null;Ck(a,c);Fi(c,a);Tj(Kf);Zc=!!Jf;Kf=Jf=null;a.current=c;Hk(c,a,e);Sk();p=h;z=g;ca.transition=f}else a.current=c;Pd&&(Pd=!1,lb=a,Qd=e);f=a.pendingLanes;0===f&&(ib=null);oj(c.stateNode,d);ia(a,P());if(null!==b)for(d=a.onRecoverableError,c=0;c<b.length;c++)e=
b[c],d(e.value,{componentStack:e.stack,digest:e.digest});if(Ed)throw Ed=!1,a=xf,xf=null,a;0!==(Qd&1)&&0!==a.tag&&Xb();f=a.pendingLanes;0!==(f&1)?a===Pf?Ic++:(Ic=0,Pf=a):Ic=0;db();return null}function Xb(){if(null!==lb){var a=Eg(Qd),b=ca.transition,c=z;try{ca.transition=null;z=16>a?16:a;if(null===lb)var d=!1;else{a=lb;lb=null;Qd=0;if(0!==(p&6))throw Error(m(331));var e=p;p|=4;for(l=a.current;null!==l;){var f=l,g=f.child;if(0!==(l.flags&16)){var h=f.deletions;if(null!==h){for(var k=0;k<h.length;k++){var n=
h[k];for(l=n;null!==l;){var q=l;switch(q.tag){case 0:case 11:case 15:Gc(8,q,f)}var u=q.child;if(null!==u)u.return=q,l=u;else for(;null!==l;){q=l;var r=q.sibling,v=q.return;Ai(q);if(q===n){l=null;break}if(null!==r){r.return=v;l=r;break}l=v}}}var x=f.alternate;if(null!==x){var y=x.child;if(null!==y){x.child=null;do{var C=y.sibling;y.sibling=null;y=C}while(null!==y)}}l=f}}if(0!==(f.subtreeFlags&2064)&&null!==g)g.return=f,l=g;else b:for(;null!==l;){f=l;if(0!==(f.flags&2048))switch(f.tag){case 0:case 11:case 15:Gc(9,
f,f.return)}var w=f.sibling;if(null!==w){w.return=f.return;l=w;break b}l=f.return}}var A=a.current;for(l=A;null!==l;){g=l;var t=g.child;if(0!==(g.subtreeFlags&2064)&&null!==t)t.return=g,l=t;else b:for(g=A;null!==l;){h=l;if(0!==(h.flags&2048))try{switch(h.tag){case 0:case 11:case 15:Id(9,h)}}catch(ma){G(h,h.return,ma)}if(h===g){l=null;break b}var B=h.sibling;if(null!==B){B.return=h.return;l=B;break b}l=h.return}}p=e;db();if(Ca&&"function"===typeof Ca.onPostCommitFiberRoot)try{Ca.onPostCommitFiberRoot(Uc,
a)}catch(ma){}d=!0}return d}finally{z=c,ca.transition=b}}return!1}function Si(a,b,c){b=Ub(c,b);b=gi(a,b,1);a=fb(a,b,1);b=Z();null!==a&&(ic(a,1,b),ia(a,b))}function G(a,b,c){if(3===a.tag)Si(a,a,c);else for(;null!==b;){if(3===b.tag){Si(b,a,c);break}else if(1===b.tag){var d=b.stateNode;if("function"===typeof b.type.getDerivedStateFromError||"function"===typeof d.componentDidCatch&&(null===ib||!ib.has(d))){a=Ub(c,a);a=hi(b,a,1);b=fb(b,a,1);a=Z();null!==b&&(ic(b,1,a),ia(b,a));break}}b=b.return}}function sk(a,
b,c){var d=a.pingCache;null!==d&&d.delete(b);b=Z();a.pingedLanes|=a.suspendedLanes&c;O===a&&(U&c)===c&&(4===L||3===L&&(U&130023424)===U&&500>P()-Of?wb(a,0):Sf|=c);ia(a,b)}function Ti(a,b){0===b&&(0===(a.mode&1)?b=1:(b=Rd,Rd<<=1,0===(Rd&130023424)&&(Rd=4194304)));var c=Z();a=Oa(a,b);null!==a&&(ic(a,b,c),ia(a,c))}function vk(a){var b=a.memoizedState,c=0;null!==b&&(c=b.retryLane);Ti(a,c)}function Gk(a,b){var c=0;switch(a.tag){case 13:var d=a.stateNode;var e=a.memoizedState;null!==e&&(c=e.retryLane);
break;case 19:d=a.stateNode;break;default:throw Error(m(314));}null!==d&&d.delete(b);Ti(a,c)}function Mi(a,b){return xh(a,b)}function Tk(a,b,c,d){this.tag=a;this.key=c;this.sibling=this.child=this.return=this.stateNode=this.type=this.elementType=null;this.index=0;this.ref=null;this.pendingProps=b;this.dependencies=this.memoizedState=this.updateQueue=this.memoizedProps=null;this.mode=d;this.subtreeFlags=this.flags=0;this.deletions=null;this.childLanes=this.lanes=0;this.alternate=null}function yf(a){a=
a.prototype;return!(!a||!a.isReactComponent)}function Uk(a){if("function"===typeof a)return yf(a)?1:0;if(void 0!==a&&null!==a){a=a.$$typeof;if(a===ie)return 11;if(a===je)return 14}return 2}function eb(a,b){var c=a.alternate;null===c?(c=pa(a.tag,b,a.key,a.mode),c.elementType=a.elementType,c.type=a.type,c.stateNode=a.stateNode,c.alternate=a,a.alternate=c):(c.pendingProps=b,c.type=a.type,c.flags=0,c.subtreeFlags=0,c.deletions=null);c.flags=a.flags&14680064;c.childLanes=a.childLanes;c.lanes=a.lanes;c.child=
a.child;c.memoizedProps=a.memoizedProps;c.memoizedState=a.memoizedState;c.updateQueue=a.updateQueue;b=a.dependencies;c.dependencies=null===b?null:{lanes:b.lanes,firstContext:b.firstContext};c.sibling=a.sibling;c.index=a.index;c.ref=a.ref;return c}function rd(a,b,c,d,e,f){var g=2;d=a;if("function"===typeof a)yf(a)&&(g=1);else if("string"===typeof a)g=5;else a:switch(a){case Bb:return sb(c.children,e,f,b);case fe:g=8;e|=8;break;case ee:return a=pa(12,c,b,e|2),a.elementType=ee,a.lanes=f,a;case ge:return a=
pa(13,c,b,e),a.elementType=ge,a.lanes=f,a;case he:return a=pa(19,c,b,e),a.elementType=he,a.lanes=f,a;case Ui:return Gd(c,e,f,b);default:if("object"===typeof a&&null!==a)switch(a.$$typeof){case hg:g=10;break a;case gg:g=9;break a;case ie:g=11;break a;case je:g=14;break a;case Ta:g=16;d=null;break a}throw Error(m(130,null==a?a:typeof a,""));}b=pa(g,c,b,e);b.elementType=a;b.type=d;b.lanes=f;return b}function sb(a,b,c,d){a=pa(7,a,d,b);a.lanes=c;return a}function Gd(a,b,c,d){a=pa(22,a,d,b);a.elementType=
Ui;a.lanes=c;a.stateNode={isHidden:!1};return a}function Ze(a,b,c){a=pa(6,a,null,b);a.lanes=c;return a}function $e(a,b,c){b=pa(4,null!==a.children?a.children:[],a.key,b);b.lanes=c;b.stateNode={containerInfo:a.containerInfo,pendingChildren:null,implementation:a.implementation};return b}function Vk(a,b,c,d,e){this.tag=b;this.containerInfo=a;this.finishedWork=this.pingCache=this.current=this.pendingChildren=null;this.timeoutHandle=-1;this.callbackNode=this.pendingContext=this.context=null;this.callbackPriority=
0;this.eventTimes=we(0);this.expirationTimes=we(-1);this.entangledLanes=this.finishedLanes=this.mutableReadLanes=this.expiredLanes=this.pingedLanes=this.suspendedLanes=this.pendingLanes=0;this.entanglements=we(0);this.identifierPrefix=d;this.onRecoverableError=e;this.mutableSourceEagerHydrationData=null}function Vf(a,b,c,d,e,f,g,h,k,l){a=new Vk(a,b,c,h,k);1===b?(b=1,!0===f&&(b|=8)):b=0;f=pa(3,null,null,b);a.current=f;f.stateNode=a;f.memoizedState={element:d,isDehydrated:c,cache:null,transitions:null,
pendingSuspenseBoundaries:null};ff(f);return a}function Wk(a,b,c){var d=3<arguments.length&&void 0!==arguments[3]?arguments[3]:null;return{$$typeof:Cb,key:null==d?null:""+d,children:a,containerInfo:b,implementation:c}}function Vi(a){if(!a)return cb;a=a._reactInternals;a:{if(nb(a)!==a||1!==a.tag)throw Error(m(170));var b=a;do{switch(b.tag){case 3:b=b.stateNode.context;break a;case 1:if(ea(b.type)){b=b.stateNode.__reactInternalMemoizedMergedChildContext;break a}}b=b.return}while(null!==b);throw Error(m(171));
}if(1===a.tag){var c=a.type;if(ea(c))return uh(a,c,b)}return b}function Wi(a,b,c,d,e,f,g,h,k,l){a=Vf(c,d,!0,a,e,f,g,h,k);a.context=Vi(null);c=a.current;d=Z();e=hb(c);f=Pa(d,e);f.callback=void 0!==b&&null!==b?b:null;fb(c,f,e);a.current.lanes=e;ic(a,e,d);ia(a,d);return a}function Sd(a,b,c,d){var e=b.current,f=Z(),g=hb(e);c=Vi(c);null===b.context?b.context=c:b.pendingContext=c;b=Pa(f,g);b.payload={element:a};d=void 0===d?null:d;null!==d&&(b.callback=d);a=fb(e,b,g);null!==a&&(xa(a,e,g,f),vd(a,e,g));return g}
function Td(a){a=a.current;if(!a.child)return null;switch(a.child.tag){case 5:return a.child.stateNode;default:return a.child.stateNode}}function Xi(a,b){a=a.memoizedState;if(null!==a&&null!==a.dehydrated){var c=a.retryLane;a.retryLane=0!==c&&c<b?c:b}}function Wf(a,b){Xi(a,b);(a=a.alternate)&&Xi(a,b)}function Xk(a){a=Bg(a);return null===a?null:a.stateNode}function Yk(a){return null}function Xf(a){this._internalRoot=a}function Ud(a){this._internalRoot=a}function Yf(a){return!(!a||1!==a.nodeType&&9!==
a.nodeType&&11!==a.nodeType)}function Vd(a){return!(!a||1!==a.nodeType&&9!==a.nodeType&&11!==a.nodeType&&(8!==a.nodeType||" react-mount-point-unstable "!==a.nodeValue))}function Yi(){}function Zk(a,b,c,d,e){if(e){if("function"===typeof d){var f=d;d=function(){var a=Td(g);f.call(a)}}var g=Wi(b,d,a,0,null,!1,!1,"",Yi);a._reactRootContainer=g;a[Ja]=g.current;sc(8===a.nodeType?a.parentNode:a);yb();return g}for(;e=a.lastChild;)a.removeChild(e);if("function"===typeof d){var h=d;d=function(){var a=Td(k);
h.call(a)}}var k=Vf(a,0,!1,null,null,!1,!1,"",Yi);a._reactRootContainer=k;a[Ja]=k.current;sc(8===a.nodeType?a.parentNode:a);yb(function(){Sd(b,k,c,d)});return k}function Wd(a,b,c,d,e){var f=c._reactRootContainer;if(f){var g=f;if("function"===typeof e){var h=e;e=function(){var a=Td(g);h.call(a)}}Sd(b,g,a,e)}else g=Zk(c,b,a,e,d);return Td(g)}var cg=new Set,$b={},Ia=!("undefined"===typeof window||"undefined"===typeof window.document||"undefined"===typeof window.document.createElement),Zd=Object.prototype.hasOwnProperty,
cj=/^[:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD][:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD\-.0-9\u00B7\u0300-\u036F\u203F-\u2040]*$/,eg={},dg={},R={};"children dangerouslySetInnerHTML defaultValue defaultChecked innerHTML suppressContentEditableWarning suppressHydrationWarning style".split(" ").forEach(function(a){R[a]=
new Y(a,0,!1,a,null,!1,!1)});[["acceptCharset","accept-charset"],["className","class"],["htmlFor","for"],["httpEquiv","http-equiv"]].forEach(function(a){var b=a[0];R[b]=new Y(b,1,!1,a[1],null,!1,!1)});["contentEditable","draggable","spellCheck","value"].forEach(function(a){R[a]=new Y(a,2,!1,a.toLowerCase(),null,!1,!1)});["autoReverse","externalResourcesRequired","focusable","preserveAlpha"].forEach(function(a){R[a]=new Y(a,2,!1,a,null,!1,!1)});"allowFullScreen async autoFocus autoPlay controls default defer disabled disablePictureInPicture disableRemotePlayback formNoValidate hidden loop noModule noValidate open playsInline readOnly required reversed scoped seamless itemScope".split(" ").forEach(function(a){R[a]=
new Y(a,3,!1,a.toLowerCase(),null,!1,!1)});["checked","multiple","muted","selected"].forEach(function(a){R[a]=new Y(a,3,!0,a,null,!1,!1)});["capture","download"].forEach(function(a){R[a]=new Y(a,4,!1,a,null,!1,!1)});["cols","rows","size","span"].forEach(function(a){R[a]=new Y(a,6,!1,a,null,!1,!1)});["rowSpan","start"].forEach(function(a){R[a]=new Y(a,5,!1,a.toLowerCase(),null,!1,!1)});var Zf=/[\-:]([a-z])/g,$f=function(a){return a[1].toUpperCase()};"accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height".split(" ").forEach(function(a){var b=
a.replace(Zf,$f);R[b]=new Y(b,1,!1,a,null,!1,!1)});"xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type".split(" ").forEach(function(a){var b=a.replace(Zf,$f);R[b]=new Y(b,1,!1,a,"http://www.w3.org/1999/xlink",!1,!1)});["xml:base","xml:lang","xml:space"].forEach(function(a){var b=a.replace(Zf,$f);R[b]=new Y(b,1,!1,a,"http://www.w3.org/XML/1998/namespace",!1,!1)});["tabIndex","crossOrigin"].forEach(function(a){R[a]=new Y(a,1,!1,a.toLowerCase(),null,!1,!1)});R.xlinkHref=new Y("xlinkHref",
1,!1,"xlink:href","http://www.w3.org/1999/xlink",!0,!1);["src","href","action","formAction"].forEach(function(a){R[a]=new Y(a,1,!1,a.toLowerCase(),null,!0,!0)});var Sa=zb.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED,sd=Symbol.for("react.element"),Cb=Symbol.for("react.portal"),Bb=Symbol.for("react.fragment"),fe=Symbol.for("react.strict_mode"),ee=Symbol.for("react.profiler"),hg=Symbol.for("react.provider"),gg=Symbol.for("react.context"),ie=Symbol.for("react.forward_ref"),ge=Symbol.for("react.suspense"),
he=Symbol.for("react.suspense_list"),je=Symbol.for("react.memo"),Ta=Symbol.for("react.lazy");Symbol.for("react.scope");Symbol.for("react.debug_trace_mode");var Ui=Symbol.for("react.offscreen");Symbol.for("react.legacy_hidden");Symbol.for("react.cache");Symbol.for("react.tracing_marker");var fg=Symbol.iterator,E=Object.assign,ae,ce=!1,cc=Array.isArray,Xd,yi=function(a){return"undefined"!==typeof MSApp&&MSApp.execUnsafeLocalFunction?function(b,c,d,e){MSApp.execUnsafeLocalFunction(function(){return a(b,
c,d,e)})}:a}(function(a,b){if("http://www.w3.org/2000/svg"!==a.namespaceURI||"innerHTML"in a)a.innerHTML=b;else{Xd=Xd||document.createElement("div");Xd.innerHTML="<svg>"+b.valueOf().toString()+"</svg>";for(b=Xd.firstChild;a.firstChild;)a.removeChild(a.firstChild);for(;b.firstChild;)a.appendChild(b.firstChild)}}),Fc=function(a,b){if(b){var c=a.firstChild;if(c&&c===a.lastChild&&3===c.nodeType){c.nodeValue=b;return}}a.textContent=b},dc={animationIterationCount:!0,aspectRatio:!0,borderImageOutset:!0,
borderImageSlice:!0,borderImageWidth:!0,boxFlex:!0,boxFlexGroup:!0,boxOrdinalGroup:!0,columnCount:!0,columns:!0,flex:!0,flexGrow:!0,flexPositive:!0,flexShrink:!0,flexNegative:!0,flexOrder:!0,gridArea:!0,gridRow:!0,gridRowEnd:!0,gridRowSpan:!0,gridRowStart:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnSpan:!0,gridColumnStart:!0,fontWeight:!0,lineClamp:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,tabSize:!0,widows:!0,zIndex:!0,zoom:!0,fillOpacity:!0,floodOpacity:!0,stopOpacity:!0,strokeDasharray:!0,
strokeDashoffset:!0,strokeMiterlimit:!0,strokeOpacity:!0,strokeWidth:!0},$k=["Webkit","ms","Moz","O"];Object.keys(dc).forEach(function(a){$k.forEach(function(b){b=b+a.charAt(0).toUpperCase()+a.substring(1);dc[b]=dc[a]})});var ij=E({menuitem:!0},{area:!0,base:!0,br:!0,col:!0,embed:!0,hr:!0,img:!0,input:!0,keygen:!0,link:!0,meta:!0,param:!0,source:!0,track:!0,wbr:!0}),ze=null,se=null,Eb=null,Fb=null,xg=function(a,b){return a(b)},yg=function(){},te=!1,Oe=!1;if(Ia)try{var Lc={};Object.defineProperty(Lc,
"passive",{get:function(){Oe=!0}});window.addEventListener("test",Lc,Lc);window.removeEventListener("test",Lc,Lc)}catch(a){Oe=!1}var kj=function(a,b,c,d,e,f,g,h,k){var l=Array.prototype.slice.call(arguments,3);try{b.apply(c,l)}catch(q){this.onError(q)}},gc=!1,Sc=null,Tc=!1,ue=null,lj={onError:function(a){gc=!0;Sc=a}},Ba=zb.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.Scheduler,Jg=Ba.unstable_scheduleCallback,Kg=Ba.unstable_NormalPriority,xh=Jg,Ki=Ba.unstable_cancelCallback,Pk=Ba.unstable_shouldYield,
Sk=Ba.unstable_requestPaint,P=Ba.unstable_now,Dj=Ba.unstable_getCurrentPriorityLevel,De=Ba.unstable_ImmediatePriority,Mg=Ba.unstable_UserBlockingPriority,ad=Kg,Ej=Ba.unstable_LowPriority,Ng=Ba.unstable_IdlePriority,Uc=null,Ca=null,ta=Math.clz32?Math.clz32:pj,qj=Math.log,rj=Math.LN2,Wc=64,Rd=4194304,z=0,Ae=!1,Yc=[],Va=null,Wa=null,Xa=null,jc=new Map,kc=new Map,Ya=[],Bj="mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" "),
Gb=Sa.ReactCurrentBatchConfig,Zc=!0,$c=null,Za=null,Ee=null,bd=null,Yb={eventPhase:0,bubbles:0,cancelable:0,timeStamp:function(a){return a.timeStamp||Date.now()},defaultPrevented:0,isTrusted:0},He=ka(Yb),Mc=E({},Yb,{view:0,detail:0}),ak=ka(Mc),ag,bg,Nc,Yd=E({},Mc,{screenX:0,screenY:0,clientX:0,clientY:0,pageX:0,pageY:0,ctrlKey:0,shiftKey:0,altKey:0,metaKey:0,getModifierState:Fe,button:0,buttons:0,relatedTarget:function(a){return void 0===a.relatedTarget?a.fromElement===a.srcElement?a.toElement:a.fromElement:
a.relatedTarget},movementX:function(a){if("movementX"in a)return a.movementX;a!==Nc&&(Nc&&"mousemove"===a.type?(ag=a.screenX-Nc.screenX,bg=a.screenY-Nc.screenY):bg=ag=0,Nc=a);return ag},movementY:function(a){return"movementY"in a?a.movementY:bg}}),ih=ka(Yd),al=E({},Yd,{dataTransfer:0}),Wj=ka(al),bl=E({},Mc,{relatedTarget:0}),Pe=ka(bl),cl=E({},Yb,{animationName:0,elapsedTime:0,pseudoElement:0}),Yj=ka(cl),dl=E({},Yb,{clipboardData:function(a){return"clipboardData"in a?a.clipboardData:window.clipboardData}}),
ck=ka(dl),el=E({},Yb,{data:0}),qh=ka(el),fk=qh,fl={Esc:"Escape",Spacebar:" ",Left:"ArrowLeft",Up:"ArrowUp",Right:"ArrowRight",Down:"ArrowDown",Del:"Delete",Win:"OS",Menu:"ContextMenu",Apps:"ContextMenu",Scroll:"ScrollLock",MozPrintableKey:"Unidentified"},gl={8:"Backspace",9:"Tab",12:"Clear",13:"Enter",16:"Shift",17:"Control",18:"Alt",19:"Pause",20:"CapsLock",27:"Escape",32:" ",33:"PageUp",34:"PageDown",35:"End",36:"Home",37:"ArrowLeft",38:"ArrowUp",39:"ArrowRight",40:"ArrowDown",45:"Insert",46:"Delete",
112:"F1",113:"F2",114:"F3",115:"F4",116:"F5",117:"F6",118:"F7",119:"F8",120:"F9",121:"F10",122:"F11",123:"F12",144:"NumLock",145:"ScrollLock",224:"Meta"},Gj={Alt:"altKey",Control:"ctrlKey",Meta:"metaKey",Shift:"shiftKey"},hl=E({},Mc,{key:function(a){if(a.key){var b=fl[a.key]||a.key;if("Unidentified"!==b)return b}return"keypress"===a.type?(a=cd(a),13===a?"Enter":String.fromCharCode(a)):"keydown"===a.type||"keyup"===a.type?gl[a.keyCode]||"Unidentified":""},code:0,location:0,ctrlKey:0,shiftKey:0,altKey:0,
metaKey:0,repeat:0,locale:0,getModifierState:Fe,charCode:function(a){return"keypress"===a.type?cd(a):0},keyCode:function(a){return"keydown"===a.type||"keyup"===a.type?a.keyCode:0},which:function(a){return"keypress"===a.type?cd(a):"keydown"===a.type||"keyup"===a.type?a.keyCode:0}}),Vj=ka(hl),il=E({},Yd,{pointerId:0,width:0,height:0,pressure:0,tangentialPressure:0,tiltX:0,tiltY:0,twist:0,pointerType:0,isPrimary:0}),nh=ka(il),jl=E({},Mc,{touches:0,targetTouches:0,changedTouches:0,altKey:0,metaKey:0,
ctrlKey:0,shiftKey:0,getModifierState:Fe}),Xj=ka(jl),kl=E({},Yb,{propertyName:0,elapsedTime:0,pseudoElement:0}),Zj=ka(kl),ll=E({},Yd,{deltaX:function(a){return"deltaX"in a?a.deltaX:"wheelDeltaX"in a?-a.wheelDeltaX:0},deltaY:function(a){return"deltaY"in a?a.deltaY:"wheelDeltaY"in a?-a.wheelDeltaY:"wheelDelta"in a?-a.wheelDelta:0},deltaZ:0,deltaMode:0}),bk=ka(ll),Hj=[9,13,27,32],Ge=Ia&&"CompositionEvent"in window,Oc=null;Ia&&"documentMode"in document&&(Oc=document.documentMode);var ek=Ia&&"TextEvent"in
window&&!Oc,Ug=Ia&&(!Ge||Oc&&8<Oc&&11>=Oc),Tg=String.fromCharCode(32),Sg=!1,Hb=!1,Kj={color:!0,date:!0,datetime:!0,"datetime-local":!0,email:!0,month:!0,number:!0,password:!0,range:!0,search:!0,tel:!0,text:!0,time:!0,url:!0,week:!0},oc=null,pc=null,ph=!1;Ia&&(ph=Lj("input")&&(!document.documentMode||9<document.documentMode));var ua="function"===typeof Object.is?Object.is:Sj,dk=Ia&&"documentMode"in document&&11>=document.documentMode,Jb=null,Ke=null,rc=null,Je=!1,Kb={animationend:gd("Animation","AnimationEnd"),
animationiteration:gd("Animation","AnimationIteration"),animationstart:gd("Animation","AnimationStart"),transitionend:gd("Transition","TransitionEnd")},Le={},eh={};Ia&&(eh=document.createElement("div").style,"AnimationEvent"in window||(delete Kb.animationend.animation,delete Kb.animationiteration.animation,delete Kb.animationstart.animation),"TransitionEvent"in window||delete Kb.transitionend.transition);var jh=hd("animationend"),kh=hd("animationiteration"),lh=hd("animationstart"),mh=hd("transitionend"),
fh=new Map,Zi="abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
(function(){for(var a=0;a<Zi.length;a++){var b=Zi[a],c=b.toLowerCase();b=b[0].toUpperCase()+b.slice(1);$a(c,"on"+b)}$a(jh,"onAnimationEnd");$a(kh,"onAnimationIteration");$a(lh,"onAnimationStart");$a("dblclick","onDoubleClick");$a("focusin","onFocus");$a("focusout","onBlur");$a(mh,"onTransitionEnd")})();Ab("onMouseEnter",["mouseout","mouseover"]);Ab("onMouseLeave",["mouseout","mouseover"]);Ab("onPointerEnter",["pointerout","pointerover"]);Ab("onPointerLeave",["pointerout","pointerover"]);mb("onChange",
"change click focusin focusout input keydown keyup selectionchange".split(" "));mb("onSelect","focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" "));mb("onBeforeInput",["compositionend","keypress","textInput","paste"]);mb("onCompositionEnd","compositionend focusout keydown keypress keyup mousedown".split(" "));mb("onCompositionStart","compositionstart focusout keydown keypress keyup mousedown".split(" "));mb("onCompositionUpdate","compositionupdate focusout keydown keypress keyup mousedown".split(" "));
var Ec="abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange resize seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),Uj=new Set("cancel close invalid load scroll toggle".split(" ").concat(Ec)),id="_reactListening"+Math.random().toString(36).slice(2),gk=/\r\n?/g,hk=/\u0000|\uFFFD/g,Jf=null,Kf=null,Rf="function"===typeof setTimeout?setTimeout:void 0,Nk="function"===typeof clearTimeout?
clearTimeout:void 0,$i="function"===typeof Promise?Promise:void 0,Jk="function"===typeof queueMicrotask?queueMicrotask:"undefined"!==typeof $i?function(a){return $i.resolve(null).then(a).catch(ik)}:Rf,Zb=Math.random().toString(36).slice(2),Da="__reactFiber$"+Zb,uc="__reactProps$"+Zb,Ja="__reactContainer$"+Zb,Me="__reactEvents$"+Zb,Dk="__reactListeners$"+Zb,Ek="__reactHandles$"+Zb,Se=[],Mb=-1,cb={},J=bb(cb),S=bb(!1),pb=cb,La=null,md=!1,Te=!1,Ob=[],Pb=0,od=null,nd=0,na=[],oa=0,rb=null,Ma=1,Na="",la=
null,fa=null,D=!1,wa=null,Ik=Sa.ReactCurrentBatchConfig,Vb=Dh(!0),li=Dh(!1),ud=bb(null),td=null,Rb=null,bf=null,tb=null,kk=Oa,gb=!1,wc={},Ea=bb(wc),yc=bb(wc),xc=bb(wc),F=bb(0),kf=[],yd=Sa.ReactCurrentDispatcher,sf=Sa.ReactCurrentBatchConfig,vb=0,C=null,K=null,N=null,Ad=!1,zc=!1,Ac=0,ml=0,zd={readContext:qa,useCallback:V,useContext:V,useEffect:V,useImperativeHandle:V,useInsertionEffect:V,useLayoutEffect:V,useMemo:V,useReducer:V,useRef:V,useState:V,useDebugValue:V,useDeferredValue:V,useTransition:V,
useMutableSource:V,useSyncExternalStore:V,useId:V,unstable_isNewReconciler:!1},lk={readContext:qa,useCallback:function(a,b){Fa().memoizedState=[a,void 0===b?null:b];return a},useContext:qa,useEffect:Sh,useImperativeHandle:function(a,b,c){c=null!==c&&void 0!==c?c.concat([a]):null;return Bd(4194308,4,Vh.bind(null,b,a),c)},useLayoutEffect:function(a,b){return Bd(4194308,4,a,b)},useInsertionEffect:function(a,b){return Bd(4,2,a,b)},useMemo:function(a,b){var c=Fa();b=void 0===b?null:b;a=a();c.memoizedState=
[a,b];return a},useReducer:function(a,b,c){var d=Fa();b=void 0!==c?c(b):b;d.memoizedState=d.baseState=b;a={pending:null,interleaved:null,lanes:0,dispatch:null,lastRenderedReducer:a,lastRenderedState:b};d.queue=a;a=a.dispatch=qk.bind(null,C,a);return[d.memoizedState,a]},useRef:function(a){var b=Fa();a={current:a};return b.memoizedState=a},useState:Qh,useDebugValue:rf,useDeferredValue:function(a){return Fa().memoizedState=a},useTransition:function(){var a=Qh(!1),b=a[0];a=pk.bind(null,a[1]);Fa().memoizedState=
a;return[b,a]},useMutableSource:function(a,b,c){},useSyncExternalStore:function(a,b,c){var d=C,e=Fa();if(D){if(void 0===c)throw Error(m(407));c=c()}else{c=b();if(null===O)throw Error(m(349));0!==(vb&30)||Nh(d,b,c)}e.memoizedState=c;var f={value:c,getSnapshot:b};e.queue=f;Sh(Lh.bind(null,d,f,a),[a]);d.flags|=2048;Cc(9,Mh.bind(null,d,f,c,b),void 0,null);return c},useId:function(){var a=Fa(),b=O.identifierPrefix;if(D){var c=Na;var d=Ma;c=(d&~(1<<32-ta(d)-1)).toString(32)+c;b=":"+b+"R"+c;c=Ac++;0<c&&
(b+="H"+c.toString(32));b+=":"}else c=ml++,b=":"+b+"r"+c.toString(32)+":";return a.memoizedState=b},unstable_isNewReconciler:!1},mk={readContext:qa,useCallback:Xh,useContext:qa,useEffect:qf,useImperativeHandle:Wh,useInsertionEffect:Th,useLayoutEffect:Uh,useMemo:Yh,useReducer:of,useRef:Rh,useState:function(a){return of(Bc)},useDebugValue:rf,useDeferredValue:function(a){var b=sa();return Zh(b,K.memoizedState,a)},useTransition:function(){var a=of(Bc)[0],b=sa().memoizedState;return[a,b]},useMutableSource:Jh,
useSyncExternalStore:Kh,useId:$h,unstable_isNewReconciler:!1},nk={readContext:qa,useCallback:Xh,useContext:qa,useEffect:qf,useImperativeHandle:Wh,useInsertionEffect:Th,useLayoutEffect:Uh,useMemo:Yh,useReducer:pf,useRef:Rh,useState:function(a){return pf(Bc)},useDebugValue:rf,useDeferredValue:function(a){var b=sa();return null===K?b.memoizedState=a:Zh(b,K.memoizedState,a)},useTransition:function(){var a=pf(Bc)[0],b=sa().memoizedState;return[a,b]},useMutableSource:Jh,useSyncExternalStore:Kh,useId:$h,
unstable_isNewReconciler:!1},Dd={isMounted:function(a){return(a=a._reactInternals)?nb(a)===a:!1},enqueueSetState:function(a,b,c){a=a._reactInternals;var d=Z(),e=hb(a),f=Pa(d,e);f.payload=b;void 0!==c&&null!==c&&(f.callback=c);b=fb(a,f,e);null!==b&&(xa(b,a,e,d),vd(b,a,e))},enqueueReplaceState:function(a,b,c){a=a._reactInternals;var d=Z(),e=hb(a),f=Pa(d,e);f.tag=1;f.payload=b;void 0!==c&&null!==c&&(f.callback=c);b=fb(a,f,e);null!==b&&(xa(b,a,e,d),vd(b,a,e))},enqueueForceUpdate:function(a,b){a=a._reactInternals;
var c=Z(),d=hb(a),e=Pa(c,d);e.tag=2;void 0!==b&&null!==b&&(e.callback=b);b=fb(a,e,d);null!==b&&(xa(b,a,d,c),vd(b,a,d))}},rk="function"===typeof WeakMap?WeakMap:Map,tk=Sa.ReactCurrentOwner,ha=!1,Cf={dehydrated:null,treeContext:null,retryLane:0};var zk=function(a,b,c,d){for(c=b.child;null!==c;){if(5===c.tag||6===c.tag)a.appendChild(c.stateNode);else if(4!==c.tag&&null!==c.child){c.child.return=c;c=c.child;continue}if(c===b)break;for(;null===c.sibling;){if(null===c.return||c.return===b)return;c=c.return}c.sibling.return=
c.return;c=c.sibling}};var xi=function(a,b){};var yk=function(a,b,c,d,e){var f=a.memoizedProps;if(f!==d){a=b.stateNode;ub(Ea.current);e=null;switch(c){case "input":f=ke(a,f);d=ke(a,d);e=[];break;case "select":f=E({},f,{value:void 0});d=E({},d,{value:void 0});e=[];break;case "textarea":f=ne(a,f);d=ne(a,d);e=[];break;default:"function"!==typeof f.onClick&&"function"===typeof d.onClick&&(a.onclick=kd)}pe(c,d);var g;c=null;for(l in f)if(!d.hasOwnProperty(l)&&f.hasOwnProperty(l)&&null!=f[l])if("style"===
l){var h=f[l];for(g in h)h.hasOwnProperty(g)&&(c||(c={}),c[g]="")}else"dangerouslySetInnerHTML"!==l&&"children"!==l&&"suppressContentEditableWarning"!==l&&"suppressHydrationWarning"!==l&&"autoFocus"!==l&&($b.hasOwnProperty(l)?e||(e=[]):(e=e||[]).push(l,null));for(l in d){var k=d[l];h=null!=f?f[l]:void 0;if(d.hasOwnProperty(l)&&k!==h&&(null!=k||null!=h))if("style"===l)if(h){for(g in h)!h.hasOwnProperty(g)||k&&k.hasOwnProperty(g)||(c||(c={}),c[g]="");for(g in k)k.hasOwnProperty(g)&&h[g]!==k[g]&&(c||
(c={}),c[g]=k[g])}else c||(e||(e=[]),e.push(l,c)),c=k;else"dangerouslySetInnerHTML"===l?(k=k?k.__html:void 0,h=h?h.__html:void 0,null!=k&&h!==k&&(e=e||[]).push(l,k)):"children"===l?"string"!==typeof k&&"number"!==typeof k||(e=e||[]).push(l,""+k):"suppressContentEditableWarning"!==l&&"suppressHydrationWarning"!==l&&($b.hasOwnProperty(l)?(null!=k&&"onScroll"===l&&B("scroll",a),e||h===k||(e=[])):(e=e||[]).push(l,k))}c&&(e=e||[]).push("style",c);var l=e;if(b.updateQueue=l)b.flags|=4}};var Ak=function(a,
b,c,d){c!==d&&(b.flags|=4)};var Jd=!1,X=!1,Fk="function"===typeof WeakSet?WeakSet:Set,l=null,zi=!1,T=null,za=!1,Mk=Math.ceil,Od=Sa.ReactCurrentDispatcher,Uf=Sa.ReactCurrentOwner,ca=Sa.ReactCurrentBatchConfig,p=0,O=null,H=null,U=0,ba=0,Ga=bb(0),L=0,Jc=null,ra=0,Md=0,Sf=0,Kc=null,ja=null,Of=0,Hf=Infinity,Ra=null,Ed=!1,xf=null,ib=null,Pd=!1,lb=null,Qd=0,Ic=0,Pf=null,Kd=-1,Ld=0;var Qk=function(a,b,c){if(null!==a)if(a.memoizedProps!==b.pendingProps||S.current)ha=!0;else{if(0===(a.lanes&c)&&0===(b.flags&
128))return ha=!1,wk(a,b,c);ha=0!==(a.flags&131072)?!0:!1}else ha=!1,D&&0!==(b.flags&1048576)&&yh(b,nd,b.index);b.lanes=0;switch(b.tag){case 2:var d=b.type;Fd(a,b);a=b.pendingProps;var e=Nb(b,J.current);Sb(b,c);e=mf(null,b,d,a,e,c);var f=nf();b.flags|=1;"object"===typeof e&&null!==e&&"function"===typeof e.render&&void 0===e.$$typeof?(b.tag=1,b.memoizedState=null,b.updateQueue=null,ea(d)?(f=!0,ld(b)):f=!1,b.memoizedState=null!==e.state&&void 0!==e.state?e.state:null,ff(b),e.updater=Dd,b.stateNode=
e,e._reactInternals=b,uf(b,d,a,c),b=Af(null,b,d,!0,f,c)):(b.tag=0,D&&f&&Ue(b),aa(null,b,e,c),b=b.child);return b;case 16:d=b.elementType;a:{Fd(a,b);a=b.pendingProps;e=d._init;d=e(d._payload);b.type=d;e=b.tag=Uk(d);a=ya(d,a);switch(e){case 0:b=zf(null,b,d,a,c);break a;case 1:b=ri(null,b,d,a,c);break a;case 11:b=mi(null,b,d,a,c);break a;case 14:b=ni(null,b,d,ya(d.type,a),c);break a}throw Error(m(306,d,""));}return b;case 0:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ya(d,e),zf(a,b,d,e,c);
case 1:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ya(d,e),ri(a,b,d,e,c);case 3:a:{si(b);if(null===a)throw Error(m(387));d=b.pendingProps;f=b.memoizedState;e=f.element;Fh(a,b);wd(b,d,null,c);var g=b.memoizedState;d=g.element;if(f.isDehydrated)if(f={element:d,isDehydrated:!1,cache:g.cache,pendingSuspenseBoundaries:g.pendingSuspenseBoundaries,transitions:g.transitions},b.updateQueue.baseState=f,b.memoizedState=f,b.flags&256){e=Ub(Error(m(423)),b);b=ti(a,b,d,c,e);break a}else if(d!==e){e=
Ub(Error(m(424)),b);b=ti(a,b,d,c,e);break a}else for(fa=Ka(b.stateNode.containerInfo.firstChild),la=b,D=!0,wa=null,c=li(b,null,d,c),b.child=c;c;)c.flags=c.flags&-3|4096,c=c.sibling;else{Qb();if(d===e){b=Qa(a,b,c);break a}aa(a,b,d,c)}b=b.child}return b;case 5:return Ih(b),null===a&&Xe(b),d=b.type,e=b.pendingProps,f=null!==a?a.memoizedProps:null,g=e.children,Qe(d,e)?g=null:null!==f&&Qe(d,f)&&(b.flags|=32),qi(a,b),aa(a,b,g,c),b.child;case 6:return null===a&&Xe(b),null;case 13:return ui(a,b,c);case 4:return gf(b,
b.stateNode.containerInfo),d=b.pendingProps,null===a?b.child=Vb(b,null,d,c):aa(a,b,d,c),b.child;case 11:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ya(d,e),mi(a,b,d,e,c);case 7:return aa(a,b,b.pendingProps,c),b.child;case 8:return aa(a,b,b.pendingProps.children,c),b.child;case 12:return aa(a,b,b.pendingProps.children,c),b.child;case 10:a:{d=b.type._context;e=b.pendingProps;f=b.memoizedProps;g=e.value;y(ud,d._currentValue);d._currentValue=g;if(null!==f)if(ua(f.value,g)){if(f.children===
e.children&&!S.current){b=Qa(a,b,c);break a}}else for(f=b.child,null!==f&&(f.return=b);null!==f;){var h=f.dependencies;if(null!==h){g=f.child;for(var k=h.firstContext;null!==k;){if(k.context===d){if(1===f.tag){k=Pa(-1,c&-c);k.tag=2;var l=f.updateQueue;if(null!==l){l=l.shared;var p=l.pending;null===p?k.next=k:(k.next=p.next,p.next=k);l.pending=k}}f.lanes|=c;k=f.alternate;null!==k&&(k.lanes|=c);df(f.return,c,b);h.lanes|=c;break}k=k.next}}else if(10===f.tag)g=f.type===b.type?null:f.child;else if(18===
f.tag){g=f.return;if(null===g)throw Error(m(341));g.lanes|=c;h=g.alternate;null!==h&&(h.lanes|=c);df(g,c,b);g=f.sibling}else g=f.child;if(null!==g)g.return=f;else for(g=f;null!==g;){if(g===b){g=null;break}f=g.sibling;if(null!==f){f.return=g.return;g=f;break}g=g.return}f=g}aa(a,b,e.children,c);b=b.child}return b;case 9:return e=b.type,d=b.pendingProps.children,Sb(b,c),e=qa(e),d=d(e),b.flags|=1,aa(a,b,d,c),b.child;case 14:return d=b.type,e=ya(d,b.pendingProps),e=ya(d.type,e),ni(a,b,d,e,c);case 15:return oi(a,
b,b.type,b.pendingProps,c);case 17:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ya(d,e),Fd(a,b),b.tag=1,ea(d)?(a=!0,ld(b)):a=!1,Sb(b,c),ei(b,d,e),uf(b,d,e,c),Af(null,b,d,!0,a,c);case 19:return wi(a,b,c);case 22:return pi(a,b,c)}throw Error(m(156,b.tag));};var pa=function(a,b,c,d){return new Tk(a,b,c,d)},aj="function"===typeof reportError?reportError:function(a){console.error(a)};Ud.prototype.render=Xf.prototype.render=function(a){var b=this._internalRoot;if(null===b)throw Error(m(409));
Sd(a,b,null,null)};Ud.prototype.unmount=Xf.prototype.unmount=function(){var a=this._internalRoot;if(null!==a){this._internalRoot=null;var b=a.containerInfo;yb(function(){Sd(null,a,null,null)});b[Ja]=null}};Ud.prototype.unstable_scheduleHydration=function(a){if(a){var b=nl();a={blockedOn:null,target:a,priority:b};for(var c=0;c<Ya.length&&0!==b&&b<Ya[c].priority;c++);Ya.splice(c,0,a);0===c&&Hg(a)}};var Cj=function(a){switch(a.tag){case 3:var b=a.stateNode;if(b.current.memoizedState.isDehydrated){var c=
hc(b.pendingLanes);0!==c&&(xe(b,c|1),ia(b,P()),0===(p&6)&&(Hc(),db()))}break;case 13:yb(function(){var b=Oa(a,1);if(null!==b){var c=Z();xa(b,a,1,c)}}),Wf(a,1)}};var Gg=function(a){if(13===a.tag){var b=Oa(a,134217728);if(null!==b){var c=Z();xa(b,a,134217728,c)}Wf(a,134217728)}};var xj=function(a){if(13===a.tag){var b=hb(a),c=Oa(a,b);if(null!==c){var d=Z();xa(c,a,b,d)}Wf(a,b)}};var nl=function(){return z};var wj=function(a,b){var c=z;try{return z=a,b()}finally{z=c}};se=function(a,b,c){switch(b){case "input":le(a,
c);b=c.name;if("radio"===c.type&&null!=b){for(c=a;c.parentNode;)c=c.parentNode;c=c.querySelectorAll("input[name="+JSON.stringify(""+b)+'][type="radio"]');for(b=0;b<c.length;b++){var d=c[b];if(d!==a&&d.form===a.form){var e=Rc(d);if(!e)throw Error(m(90));jg(d);le(d,e)}}}break;case "textarea":og(a,c);break;case "select":b=c.value,null!=b&&Db(a,!!c.multiple,b,!1)}};(function(a,b,c){xg=a;yg=c})(Tf,function(a,b,c,d,e){var f=z,g=ca.transition;try{return ca.transition=null,z=1,a(b,c,d,e)}finally{z=f,ca.transition=
g,0===p&&Hc()}},yb);var ol={usingClientEntryPoint:!1,Events:[ec,Ib,Rc,ug,vg,Tf]};(function(a){a={bundleType:a.bundleType,version:a.version,rendererPackageName:a.rendererPackageName,rendererConfig:a.rendererConfig,overrideHookState:null,overrideHookStateDeletePath:null,overrideHookStateRenamePath:null,overrideProps:null,overridePropsDeletePath:null,overridePropsRenamePath:null,setErrorHandler:null,setSuspenseHandler:null,scheduleUpdate:null,currentDispatcherRef:Sa.ReactCurrentDispatcher,findHostInstanceByFiber:Xk,
findFiberByHostInstance:a.findFiberByHostInstance||Yk,findHostInstancesForRefresh:null,scheduleRefresh:null,scheduleRoot:null,setRefreshHandler:null,getCurrentFiber:null,reconcilerVersion:"18.3.1"};if("undefined"===typeof __REACT_DEVTOOLS_GLOBAL_HOOK__)a=!1;else{var b=__REACT_DEVTOOLS_GLOBAL_HOOK__;if(b.isDisabled||!b.supportsFiber)a=!0;else{try{Uc=b.inject(a),Ca=b}catch(c){}a=b.checkDCE?!0:!1}}return a})({findFiberByHostInstance:ob,bundleType:0,version:"18.3.1-next-f1338f8080-20240426",
rendererPackageName:"react-dom"});Q.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=ol;Q.createPortal=function(a,b){var c=2<arguments.length&&void 0!==arguments[2]?arguments[2]:null;if(!Yf(b))throw Error(m(200));return Wk(a,b,null,c)};Q.createRoot=function(a,b){if(!Yf(a))throw Error(m(299));var c=!1,d="",e=aj;null!==b&&void 0!==b&&(!0===b.unstable_strictMode&&(c=!0),void 0!==b.identifierPrefix&&(d=b.identifierPrefix),void 0!==b.onRecoverableError&&(e=b.onRecoverableError));b=Vf(a,1,!1,null,null,
c,!1,d,e);a[Ja]=b.current;sc(8===a.nodeType?a.parentNode:a);return new Xf(b)};Q.findDOMNode=function(a){if(null==a)return null;if(1===a.nodeType)return a;var b=a._reactInternals;if(void 0===b){if("function"===typeof a.render)throw Error(m(188));a=Object.keys(a).join(",");throw Error(m(268,a));}a=Bg(b);a=null===a?null:a.stateNode;return a};Q.flushSync=function(a){return yb(a)};Q.hydrate=function(a,b,c){if(!Vd(b))throw Error(m(200));return Wd(null,a,b,!0,c)};Q.hydrateRoot=function(a,b,c){if(!Yf(a))throw Error(m(405));
var d=null!=c&&c.hydratedSources||null,e=!1,f="",g=aj;null!==c&&void 0!==c&&(!0===c.unstable_strictMode&&(e=!0),void 0!==c.identifierPrefix&&(f=c.identifierPrefix),void 0!==c.onRecoverableError&&(g=c.onRecoverableError));b=Wi(b,null,a,1,null!=c?c:null,e,!1,f,g);a[Ja]=b.current;sc(a);if(d)for(a=0;a<d.length;a++)c=d[a],e=c._getVersion,e=e(c._source),null==b.mutableSourceEagerHydrationData?b.mutableSourceEagerHydrationData=[c,e]:b.mutableSourceEagerHydrationData.push(c,e);return new Ud(b)};Q.render=
function(a,b,c){if(!Vd(b))throw Error(m(200));return Wd(null,a,b,!1,c)};Q.unmountComponentAtNode=function(a){if(!Vd(a))throw Error(m(40));return a._reactRootContainer?(yb(function(){Wd(null,null,a,!1,function(){a._reactRootContainer=null;a[Ja]=null})}),!0):!1};Q.unstable_batchedUpdates=Tf;Q.unstable_renderSubtreeIntoContainer=function(a,b,c,d){if(!Vd(c))throw Error(m(200));if(null==a||void 0===a._reactInternals)throw Error(m(38));return Wd(a,b,c,!1,d)};Q.version="18.3.1-next-f1338f8080-20240426"});
})();

</script>
<script>
const {
  useState,
  useEffect,
  useMemo
} = React;
function Icon({
  children,
  size = 16,
  color = "currentColor",
  style,
  ...rest
}) {
  return /*#__PURE__*/React.createElement("svg", {
    width: size,
    height: size,
    viewBox: "0 0 24 24",
    fill: "none",
    stroke: color,
    strokeWidth: "1.6",
    strokeLinecap: "round",
    strokeLinejoin: "round",
    style: style,
    ...rest
  }, children);
}
const Watch = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("circle", {
  cx: "12",
  cy: "12",
  r: "7"
}), /*#__PURE__*/React.createElement("path", {
  d: "M12 9v3l2 1.5"
}), /*#__PURE__*/React.createElement("path", {
  d: "M9.5 3h5M9.5 21h5"
}));
const Gem = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M6 9l6-6 6 6-6 12z"
}), /*#__PURE__*/React.createElement("path", {
  d: "M6 9h12M9 9l3 12 3-12"
}));
const Link2 = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("rect", {
  x: "3",
  y: "8",
  width: "8",
  height: "8",
  rx: "4"
}), /*#__PURE__*/React.createElement("rect", {
  x: "13",
  y: "8",
  width: "8",
  height: "8",
  rx: "4"
}));
const Circle = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("circle", {
  cx: "12",
  cy: "12",
  r: "8"
}));
const ShoppingCart = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("circle", {
  cx: "9",
  cy: "20",
  r: "1"
}), /*#__PURE__*/React.createElement("circle", {
  cx: "18",
  cy: "20",
  r: "1"
}), /*#__PURE__*/React.createElement("path", {
  d: "M3 4h2l2.4 12.4a2 2 0 0 0 2 1.6h7.2a2 2 0 0 0 2-1.6L21 8H6"
}));
const ShoppingBag = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M6 8h12l-1 12H7z"
}), /*#__PURE__*/React.createElement("path", {
  d: "M9 8V6a3 3 0 0 1 6 0v2"
}));
const Plus = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M12 5v14M5 12h14"
}));
const Minus = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M5 12h14"
}));
const Trash2 = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M3 6h18M8 6V4h8v2M6 6l1 14h10l1-14"
}));
const X = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M18 6 6 18M6 6l12 12"
}));
const MapPin = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M12 21s7-6.5 7-11a7 7 0 1 0-14 0c0 4.5 7 11 7 11z"
}), /*#__PURE__*/React.createElement("circle", {
  cx: "12",
  cy: "10",
  r: "2.5"
}));
const Phone = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M5 4h4l1.5 4-2 1.5a12 12 0 0 0 6 6l1.5-2 4 1.5v4a2 2 0 0 1-2 2A16 16 0 0 1 3 6a2 2 0 0 1 2-2z"
}));
const Mail = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("rect", {
  x: "3",
  y: "5",
  width: "18",
  height: "14",
  rx: "2"
}), /*#__PURE__*/React.createElement("path", {
  d: "m3 7 9 6 9-6"
}));
const QrCode = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("rect", {
  x: "3",
  y: "3",
  width: "7",
  height: "7"
}), /*#__PURE__*/React.createElement("rect", {
  x: "14",
  y: "3",
  width: "7",
  height: "7"
}), /*#__PURE__*/React.createElement("rect", {
  x: "3",
  y: "14",
  width: "7",
  height: "7"
}), /*#__PURE__*/React.createElement("path", {
  d: "M14 14h3v3h-3zM19 14h2v2h-2zM14 19h2v2h-2zM19 19h2v2h-2z"
}));
const Printer = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M6 9V3h12v6"
}), /*#__PURE__*/React.createElement("rect", {
  x: "4",
  y: "9",
  width: "16",
  height: "8",
  rx: "1"
}), /*#__PURE__*/React.createElement("path", {
  d: "M6 17v4h12v-4"
}));
const ArrowLeft = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M19 12H5M11 6l-6 6 6 6"
}));
const ArrowRight = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M5 12h14M13 6l6 6-6 6"
}));
const Check = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M20 6 9 17l-5-5"
}));
const Search = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("circle", {
  cx: "11",
  cy: "11",
  r: "7"
}), /*#__PURE__*/React.createElement("path", {
  d: "m21 21-4.3-4.3"
}));
const User = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("circle", {
  cx: "12",
  cy: "8",
  r: "4"
}), /*#__PURE__*/React.createElement("path", {
  d: "M4 21c0-4 4-6 8-6s8 2 8 6"
}));
const Edit2 = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M12 20h9"
}), /*#__PURE__*/React.createElement("path", {
  d: "M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4z"
}));
const Star = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M12 3l2.7 5.7 6.3.9-4.5 4.4 1 6.2L12 17l-5.5 3.2 1-6.2L3 9.6l6.3-.9z"
}));
const Lock = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("rect", {
  x: "5",
  y: "11",
  width: "14",
  height: "9",
  rx: "2"
}), /*#__PURE__*/React.createElement("path", {
  d: "M8 11V7a4 4 0 0 1 8 0v4"
}));
const LogOut = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M9 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h4"
}), /*#__PURE__*/React.createElement("path", {
  d: "M16 17l5-5-5-5M21 12H9"
}));
const ImageIcon = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("rect", {
  x: "3",
  y: "3",
  width: "18",
  height: "18",
  rx: "2"
}), /*#__PURE__*/React.createElement("circle", {
  cx: "8.5",
  cy: "8.5",
  r: "1.5"
}), /*#__PURE__*/React.createElement("path", {
  d: "m21 15-5-5L5 21"
}));
const Tag = p => /*#__PURE__*/React.createElement(Icon, p, /*#__PURE__*/React.createElement("path", {
  d: "M12 2H2v10l9.29 9.29a1 1 0 0 0 1.41 0l8.59-8.59a1 1 0 0 0 0-1.41L12 2Z"
}), /*#__PURE__*/React.createElement("circle", {
  cx: "7",
  cy: "7",
  r: "1.3"
}));

/* ---------------------------------------------------------
   APEX FASHION — Curated Accessories
   Palette: near-black stage, taupe-gold accent (from the AF mark),
   warm cream type. Playfair Display for the voice of the brand,
   Inter for interface text, JetBrains Mono for prices & ledger data.
--------------------------------------------------------- */

const CATS = [{
  id: "watches",
  label: "Watches",
  icon: Watch
}, {
  id: "rings",
  label: "Rings",
  icon: Gem
}, {
  id: "chains",
  label: "Chains",
  icon: Link2
}, {
  id: "bracelets",
  label: "Bracelets",
  icon: Circle
}];
const SEED_PRODUCTS = [{
  id: "p1",
  name: "Meridian Chronograph",
  category: "watches",
  price: 8999,
  stock: 12,
  desc: "Brushed steel case, sapphire crystal, quiet-tick movement."
}, {
  id: "p2",
  name: "Noir Automatic",
  category: "watches",
  price: 12499,
  stock: 6,
  desc: "Full black PVD finish with an exhibition case back."
}, {
  id: "p3",
  name: "Solstice Band",
  category: "rings",
  price: 2199,
  stock: 20,
  desc: "Hammered gold-tone band, comfort-fit interior."
}, {
  id: "p4",
  name: "Ember Signet",
  category: "rings",
  price: 2899,
  stock: 14,
  desc: "Signet profile with a hand-set garnet stone."
}, {
  id: "p5",
  name: "Cuban Link Noir",
  category: "chains",
  price: 3499,
  stock: 18,
  desc: "Matte black Cuban links, 20-inch length."
}, {
  id: "p6",
  name: "Vertex Chain",
  category: "chains",
  price: 4299,
  stock: 9,
  desc: "Fine box-chain in warm gold tone, 22-inch length."
}, {
  id: "p7",
  name: "Anchor Cuff",
  category: "bracelets",
  price: 2799,
  stock: 15,
  desc: "Structured cuff bracelet, adjustable clasp."
}, {
  id: "p8",
  name: "Linea Bracelet",
  category: "bracelets",
  price: 1999,
  stock: 22,
  desc: "Slim beaded bracelet, layers well with others."
}];
const INR = n => "₹" + Number(n).toLocaleString("en-IN");
const catIcon = id => (CATS.find(c => c.id === id) || CATS[0]).icon;
const catLabel = id => (CATS.find(c => c.id === id) || CATS[0]).label;
const uid = p => p + Math.random().toString(36).slice(2, 9);

// Orders are sent to the owner's WhatsApp — no backend/server needed.
const OWNER_WHATSAPP = "916383489833"; // +91 6383489833
const OWNER_PIN = "apex2026"; // simple owner gate — change this to your own PIN
const UPI_ID = "6383489833-3@ybl"; // UPI VPA payments are sent to
const UPI_PAYEE_NAME = "Apex Fashion";
function buildUpiLink(app, amount, note) {
  const amt = Number(amount || 0).toFixed(2);
  const params = `pa=${encodeURIComponent(UPI_ID)}&pn=${encodeURIComponent(UPI_PAYEE_NAME)}&am=${amt}&cu=INR&tn=${encodeURIComponent(note || "Apex Fashion order")}`;
  if (app === "gpay") return `tez://upi/pay?${params}`;
  if (app === "phonepe") return `phonepe://pay?${params}`;
  if (app === "paytm") return `paytmmp://pay?${params}`;
  return `upi://pay?${params}`;
}

function buildWhatsAppMessage(customer, items, total, invoiceNo) {
  const lines = [`*New Order — Apex Fashion*`, `Invoice: ${invoiceNo}`, ``, `*Customer Details*`, `Name: ${customer.name}`, `Phone: ${customer.phone}`, customer.email ? `Email: ${customer.email}` : null, `Address: ${customer.address}, ${customer.city}, ${customer.state} ${customer.pincode}`, ``, `*Order Items*`, ...items.map(c => `• ${c.product.name} (${catLabel(c.product.category)}) x${c.qty} — ${INR(c.product.price * c.qty)}`), ``, `*Total: ${INR(total)}*`, `Payment: Paid via UPI QR (screenshot attached separately)`].filter(Boolean);
  return lines.join("\n");
}
const PAYMENT_QR_IMAGE = "data:image/jpeg;base64,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hTzzygBDzyhBSDTxDRDjyAhQDwgATiSDDDTxQjywTwABTDTijTzzywAAAARhwzBTxTyiyQABTzxDyhyRzyxzABzxwhQSABSzhTzzxRTzzzijxzzyiAwDxQBRzTRzygxABzDAACDzyhRyhCywRTzzxQAgBSigQggSDyiwgzRzyhzyDyTxRRSihzzzzwgCTzzQQTzzxQCgBSihTyyTjTSSDxxzTzDQAiDxgziRTxzziSQCTCAizzzzxQCABSihTDBDBTzAwTjDCjDBgATyxwwgyjADDxzxjzCSjzzzxRzzzyyjzzzxSwThBwiRzRgDjzzzzTzyzDzzzTwCwjzjBTzzxDDDDDCTzzzzzgSzDyBTjBzjzzzzzzzyizDDDTxhzzzzxjzzjDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz/xAAC/9oADAMBAAIAAwAAABDzTzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzDxSwQwwwwggAAAABxyxTzzzwTyhjyABTwwxDzzxBQAQwwwxADwCgxzzzBQACDTTDQAxTDTASBQghCTAijCDhwwhxTjDTzCSADwChBTzhxQTQiTygRSzyARxSRwDxxwTzyDThSThxSgDzyRgADwChRTzxRSTiSziDyTwDRSjwhyDiwxRwwyBxTyiDSgDzxSgADwChBTzhRTBAxRSQSjBBBCDyTyzzzQDCyCSgjBRzygDzxygADwCgwAACBQAziTSDTgwhBTjCgBBSQDyiwRCBTBjjSgQABBwADwSjzzzyxgCzgAyjSjTBRRxBjgBDQAAASDhxAABjwTzzzzyQDxTwgAAQwgBSgCwwiQSgCDxDzxjjDCzhTBDBzDDDCAQwAADwDxTzxATyRhTyQgTzzjTTzxSiwzxjAzzxgQxwwwyzRSyxwhSADxTzwizziQCBSiywzRDRhCyxxgAAAwADxSyQhThhRiRQSgxgDxBARTzijCTiCjxiiBRwjTwCgCgTijhAACCTDwRCzwDDTQhADwCjwSzwSzxjhCBzxiTxAADjDSQhSyghjDzwShwhRzDgAASADwCCTRwQAjTxgDTQThzxRDSzgxzzywhxzDRQwwgQizSCAwCADxTzxQhBxggwhBzhyzzxQw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";
function LogoBadge({
  size = 96,
  stamp = false
}) {
  return /*#__PURE__*/React.createElement("svg", {
    viewBox: "0 0 200 200",
    width: size,
    height: size
  }, /*#__PURE__*/React.createElement("defs", null, /*#__PURE__*/React.createElement("path", {
    id: `topArc-${size}-${stamp}`,
    d: "M 28,108 A 74,74 0 1,1 172,108",
    fill: "none"
  }), /*#__PURE__*/React.createElement("path", {
    id: `botArc-${size}-${stamp}`,
    d: "M 42,150 A 74,74 0 0,0 158,150",
    fill: "none"
  })), /*#__PURE__*/React.createElement("circle", {
    cx: "100",
    cy: "100",
    r: "96",
    fill: "#0b0b0c",
    stroke: "#a8927c",
    strokeWidth: stamp ? 2 : 1
  }), /*#__PURE__*/React.createElement("circle", {
    cx: "100",
    cy: "100",
    r: "90",
    fill: "none",
    stroke: "#3a352e",
    strokeWidth: "0.75"
  }), /*#__PURE__*/React.createElement("text", {
    fill: "#ede7df",
    fontSize: "10.5",
    letterSpacing: "3",
    fontFamily: "Inter, sans-serif"
  }, /*#__PURE__*/React.createElement("textPath", {
    href: `#topArc-${size}-${stamp}`,
    startOffset: "50%",
    textAnchor: "middle"
  }, stamp ? "PAYMENT CONFIRMED" : "CURATED ACCESSORIES")), /*#__PURE__*/React.createElement("text", {
    x: "100",
    y: "128",
    textAnchor: "middle",
    fontFamily: "Playfair Display, serif",
    fontWeight: "700",
    fontSize: "70",
    fill: "#a8927c"
  }, "AF"), /*#__PURE__*/React.createElement("text", {
    x: "100",
    y: "150",
    textAnchor: "middle",
    fontFamily: "Playfair Display, serif",
    fontSize: "13",
    letterSpacing: "2",
    fill: "#ede7df"
  }, "APEX FASHION"), /*#__PURE__*/React.createElement("text", {
    fill: "#ede7df",
    fontSize: "10",
    letterSpacing: "3",
    fontFamily: "Inter, sans-serif"
  }, /*#__PURE__*/React.createElement("textPath", {
    href: `#botArc-${size}-${stamp}`,
    startOffset: "50%",
    textAnchor: "middle"
  }, stamp ? "· THANK YOU ·" : "· EST 2026 ·")));
}
function ApexFashion() {
  const [products, setProducts] = useState(SEED_PRODUCTS);
  const [cart, setCart] = useState([]); // [{id, qty}]
  const [view, setView] = useState("shop"); // shop | product | cart | address | payment | invoice | admin
  const [activeCat, setActiveCat] = useState("all");
  const [query, setQuery] = useState("");
  const [selectedId, setSelectedId] = useState(null);
  const [buyNowOnly, setBuyNowOnly] = useState(false); // when true, checkout uses only selected item
  const [customer, setCustomer] = useState({
    name: "",
    phone: "",
    email: "",
    address: "",
    city: "",
    state: "",
    pincode: ""
  });
  const [formError, setFormError] = useState("");
  const [invoice, setInvoice] = useState(null);
  const [pendingInvoiceNo, setPendingInvoiceNo] = useState("");
  const [editingProduct, setEditingProduct] = useState(null); // product being edited in admin
  const [showForm, setShowForm] = useState(false);
  const [toast, setToast] = useState("");
  const [isOwner, setIsOwner] = useState(false);
  const [pinInput, setPinInput] = useState("");
  const [pinError, setPinError] = useState("");
  const [awaitingPaymentReturn, setAwaitingPaymentReturn] = useState(false);
  const [showReturnBanner, setShowReturnBanner] = useState(false);
  const [catVersion, setCatVersion] = useState(0);
  const [addingCategory, setAddingCategory] = useState(false);
  const [newCategoryName, setNewCategoryName] = useState("");
  const [categoryError, setCategoryError] = useState("");

  useEffect(() => {
    try {
      const raw = localStorage.getItem("apex-custom-categories");
      if (raw) {
        const saved = JSON.parse(raw);
        saved.forEach(c => {
          if (!CATS.find(x => x.id === c.id)) CATS.push({
            id: c.id,
            label: c.label,
            icon: Tag
          });
        });
        setCatVersion(v => v + 1);
      }
    } catch (e) {/* no saved categories yet */}
  }, []);
  function addCategory(rawName) {
    const label = (rawName || "").trim();
    if (!label) {
      setCategoryError("Enter a category name");
      return null;
    }
    let id = label.toLowerCase().replace(/[^a-z0-9]+/g, "-").replace(/(^-|-$)/g, "");
    if (!id) id = uid("cat");
    const existing = CATS.find(c => c.id === id || c.label.toLowerCase() === label.toLowerCase());
    if (existing) {
      setCategoryError("");
      setAddingCategory(false);
      setNewCategoryName("");
      return existing.id;
    }
    CATS.push({
      id,
      label,
      icon: Tag
    });
    try {
      const custom = CATS.filter(c => c.icon === Tag).map(c => ({
        id: c.id,
        label: c.label
      }));
      localStorage.setItem("apex-custom-categories", JSON.stringify(custom));
    } catch (e) {}
    setCatVersion(v => v + 1);
    setCategoryError("");
    setAddingCategory(false);
    setNewCategoryName("");
    return id;
  }

  useEffect(() => {
    function handleVisibility() {
      if (document.visibilityState === "visible" && awaitingPaymentReturn) {
        setShowReturnBanner(true);
        setAwaitingPaymentReturn(false);
      }
    }
    document.addEventListener("visibilitychange", handleVisibility);
    window.addEventListener("focus", handleVisibility);
    return () => {
      document.removeEventListener("visibilitychange", handleVisibility);
      window.removeEventListener("focus", handleVisibility);
    };
  }, [awaitingPaymentReturn]);
  function openUpiApp(app) {
    const link = buildUpiLink(app, checkoutTotal, `Apex Fashion order ${pendingInvoiceNo || ""}`.trim());
    setAwaitingPaymentReturn(true);
    setShowReturnBanner(false);
    window.location.href = link;
  }

  // persistence (best-effort)
  useEffect(() => {
    (async () => {
      try {
        const raw = localStorage.getItem("apex-products");
        if (raw) setProducts(JSON.parse(raw));
      } catch (e) {/* no saved products yet */}
    })();
  }, []);
  useEffect(() => {
    (async () => {
      try {
        localStorage.setItem("apex-products", JSON.stringify(products));
      } catch (e) {}
    })();
  }, [products]);
  useEffect(() => {
    if (!toast) return;
    const t = setTimeout(() => setToast(""), 1800);
    return () => clearTimeout(t);
  }, [toast]);
  useEffect(() => {
    window.scrollTo({
      top: 0,
      behavior: "smooth"
    });
  }, [view]);
  const cartItems = useMemo(() => cart.map(c => ({
    ...c,
    product: products.find(p => p.id === c.id)
  })).filter(c => c.product), [cart, products]);
  const cartCount = cartItems.reduce((s, c) => s + c.qty, 0);
  const cartTotal = cartItems.reduce((s, c) => s + c.qty * c.product.price, 0);
  const checkoutItems = useMemo(() => {
    if (buyNowOnly && selectedId) {
      const p = products.find(x => x.id === selectedId);
      return p ? [{
        id: p.id,
        qty: 1,
        product: p
      }] : [];
    }
    return cartItems;
  }, [buyNowOnly, selectedId, products, cartItems]);
  const checkoutTotal = checkoutItems.reduce((s, c) => s + c.qty * c.product.price, 0);
  const whatsappLink = useMemo(() => `https://wa.me/${OWNER_WHATSAPP}?text=${encodeURIComponent(buildWhatsAppMessage(customer, checkoutItems, checkoutTotal, pendingInvoiceNo))}`, [customer, checkoutItems, checkoutTotal, pendingInvoiceNo]);
  const filtered = products.filter(p => {
    const matchCat = activeCat === "all" || p.category === activeCat;
    const matchQ = p.name.toLowerCase().includes(query.toLowerCase());
    return matchCat && matchQ;
  });
  function addToCart(id, qty = 1) {
    setCart(c => {
      const existing = c.find(x => x.id === id);
      if (existing) return c.map(x => x.id === id ? {
        ...x,
        qty: x.qty + qty
      } : x);
      return [...c, {
        id,
        qty
      }];
    });
    setToast("Added to cart");
  }
  function setQty(id, qty) {
    setCart(c => c.map(x => x.id === id ? {
      ...x,
      qty: Math.max(1, qty)
    } : x));
  }
  function removeFromCart(id) {
    setCart(c => c.filter(x => x.id !== id));
  }
  function clearCart() {
    setCart([]);
    setToast("Cart cleared");
  }
  function buyNow(id) {
    setSelectedId(id);
    setBuyNowOnly(true);
    setView("address");
  }
  function goCheckoutFromCart() {
    setBuyNowOnly(false);
    setView("address");
  }
  function submitAddress(e) {
    e.preventDefault();
    const {
      name,
      phone,
      address,
      city,
      pincode
    } = customer;
    if (!name || !phone || !address || !city || !pincode) {
      setFormError("Please fill in name, phone, address, city and pincode.");
      return;
    }
    if (!/^\d{10}$/.test(phone.trim())) {
      setFormError("Enter a valid 10-digit phone number.");
      return;
    }
    setFormError("");
    setPendingInvoiceNo("AF-" + Date.now().toString().slice(-8));
    setView("payment");
  }
  function confirmPayment() {
    const inv = {
      number: pendingInvoiceNo,
      date: new Date(),
      customer: {
        ...customer
      },
      items: checkoutItems.map(c => ({
        name: c.product.name,
        category: c.product.category,
        price: c.product.price,
        qty: c.qty
      })),
      total: checkoutTotal,
      method: "UPI — QR Payment",
      status: "Paid"
    };
    setInvoice(inv);
    if (buyNowOnly) {
      setBuyNowOnly(false);
      setSelectedId(null);
    } else {
      setCart([]);
    }
    setView("invoice");
  }
  function backToShop() {
    setView("shop");
    setInvoice(null);
    setCustomer({
      name: "",
      phone: "",
      email: "",
      address: "",
      city: "",
      state: "",
      pincode: ""
    });
  }
  function openManage() {
    setView("admin");
  }
  function submitPin(e) {
    e.preventDefault();
    if (pinInput === OWNER_PIN) {
      setIsOwner(true);
      setPinError("");
      setPinInput("");
    } else {
      setPinError("Incorrect PIN.");
    }
  }
  function ownerLogout() {
    setIsOwner(false);
    setView("shop");
  }

  // ---- Admin CRUD ----
  function openNewProduct() {
    setEditingProduct({
      id: "",
      name: "",
      category: "watches",
      price: "",
      stock: "",
      desc: "",
      image: "",
      images: []
    });
    setShowForm(true);
  }
  function openEditProduct(p) {
    setEditingProduct({
      ...p,
      images: p.images && p.images.length ? p.images : p.image ? [p.image] : []
    });
    setShowForm(true);
  }
  function handleImageUpload(files) {
    const fileList = Array.from(files || []);
    if (!fileList.length) return;
    fileList.forEach(file => {
      const reader = new FileReader();
      reader.onload = () => {
        setEditingProduct(p => ({
          ...p,
          images: [...(p.images || []), reader.result]
        }));
      };
      reader.readAsDataURL(file);
    });
  }
  function removeEditingImage(idx) {
    setEditingProduct(p => ({
      ...p,
      images: (p.images || []).filter((_, i) => i !== idx)
    }));
  }
  function saveProduct(e) {
    e.preventDefault();
    const p = editingProduct;
    if (!p.name || !p.price || !p.stock) return;
    const images = p.images || [];
    const payload = {
      ...p,
      images,
      image: images[0] || "",
      price: Number(p.price),
      stock: Number(p.stock)
    };
    if (p.id) {
      setProducts(list => list.map(x => x.id === p.id ? payload : x));
      setToast("Product updated");
    } else {
      setProducts(list => [...list, {
        ...payload,
        id: uid("p")
      }]);
      setToast("Product added");
    }
    setShowForm(false);
    setEditingProduct(null);
  }
  function deleteProduct(id) {
    setProducts(list => list.filter(p => p.id !== id));
    setCart(c => c.filter(x => x.id !== id));
    setToast("Product deleted");
  }
  const selectedProduct = products.find(p => p.id === selectedId);
  return /*#__PURE__*/React.createElement("div", {
    style: {
      "--bg": "#0b0b0c",
      "--surface": "#161615",
      "--surface2": "#1e1e1c",
      "--gold": "#a8927c",
      "--gold-light": "#c9b9a4",
      "--cream": "#ede7df",
      "--muted": "#938d85",
      "--line": "#2a2a27",
      backgroundColor: "var(--bg)",
      color: "var(--cream)",
      minHeight: "100vh",
      fontFamily: "Inter, sans-serif"
    }
  }, /*#__PURE__*/React.createElement("style", null, `
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');
        html { scroll-behavior: smooth; }
        .af-serif { font-family: 'Playfair Display', serif; }
        .af-mono { font-family: 'JetBrains Mono', monospace; }

        /* buttons + cards */
        .af-btn { transition: transform .18s cubic-bezier(.2,.8,.2,1), box-shadow .18s ease, background-color .18s ease, border-color .18s ease, opacity .18s ease; }
        .af-btn:hover { transform: translateY(-1px); }
        .af-btn:active { transform: translateY(0) scale(0.97); }
        .af-card { transition: border-color .25s ease, transform .25s cubic-bezier(.2,.8,.2,1), box-shadow .25s ease; }
        .af-card:hover { border-color: var(--gold); transform: translateY(-5px); box-shadow: 0 14px 30px -12px rgba(168,146,124,0.35); }
        .af-card:hover .af-card-icon { transform: scale(1.08); }
        .af-card-icon, .af-card-img { transition: transform .4s cubic-bezier(.2,.8,.2,1); }
        .af-tab { transition: all .2s cubic-bezier(.2,.8,.2,1); }
        .af-tab:hover { border-color: var(--gold-light) !important; }
        .af-tab.active { transform: scale(1.03); }

        /* view transitions */
        .view-enter { animation: viewIn .38s cubic-bezier(.16,.8,.3,1) both; }
        @keyframes viewIn {
          from { opacity: 0; transform: translateY(10px); }
          to { opacity: 1; transform: translateY(0); }
        }

        /* product grid stagger */
        .card-enter { opacity: 0; animation: cardIn .5s cubic-bezier(.16,.8,.3,1) both; }
        @keyframes cardIn {
          from { opacity: 0; transform: translateY(14px) scale(.98); }
          to { opacity: 1; transform: translateY(0) scale(1); }
        }

        /* hero badge */
        .badge-in { animation: badgeIn .7s cubic-bezier(.16,.8,.3,1) both; }
        @keyframes badgeIn {
          from { opacity: 0; transform: scale(.85) rotate(-8deg); }
          to { opacity: 1; transform: scale(1) rotate(0deg); }
        }
        .hero-text-in { animation: heroTextIn .6s .15s cubic-bezier(.16,.8,.3,1) both; }
        @keyframes heroTextIn {
          from { opacity: 0; transform: translateY(12px); }
          to { opacity: 1; transform: translateY(0); }
        }

        /* invoice stamp */
        .stamp-in { animation: stampIn .6s .1s cubic-bezier(.34,1.4,.64,1) both; }
        @keyframes stampIn {
          from { opacity: 0; transform: scale(1.6) rotate(-18deg); }
          to { opacity: 1; transform: scale(1) rotate(0deg); }
        }

        /* toast */
        .toast-in { animation: toastIn .35s cubic-bezier(.16,.8,.3,1) both; }
        @keyframes toastIn {
          from { opacity: 0; transform: translate(-50%, -14px); }
          to { opacity: 1; transform: translate(-50%, 0); }
        }

        /* cart badge bump */
        .bump { animation: bump .35s cubic-bezier(.34,1.6,.64,1) both; }
        @keyframes bump {
          0% { transform: scale(1); }
          40% { transform: scale(1.35); }
          100% { transform: scale(1); }
        }

        /* qty +/- press */
        .qty-btn { transition: transform .12s ease, color .15s ease; }
        .qty-btn:active { transform: scale(0.82); }
        .qty-btn:hover { color: var(--gold-light); }

        /* step dot fill */
        .step-dot { transition: all .3s cubic-bezier(.2,.8,.2,1); }

        ::-webkit-scrollbar { width: 8px; height: 8px; }
        ::-webkit-scrollbar-thumb { background: #2f2b26; border-radius: 4px; }
        input:focus, select:focus, textarea:focus { outline: 2px solid var(--gold); outline-offset: 1px; }
        a:focus-visible, button:focus-visible { outline: 2px solid var(--gold); outline-offset: 2px; }
        @media print {
          .no-print { display: none !important; }
          body { background: white; }
        }

        /* ===== Responsive layout rules ===== */
        .af-grid { grid-template-columns: repeat(auto-fill, minmax(230px, 1fr)) !important; }
        .af-pd-gallery-thumb { cursor: pointer; }

        @media (max-width: 900px) {
          .af-pd-grid { grid-template-columns: 1fr !important; gap: 24px !important; }
          .af-pd-image { height: 300px !important; }
        }

        @media (max-width: 720px) {
          .af-grid { grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)) !important; gap: 12px !important; }
          .af-hero-title { font-size: 26px !important; }
          .af-hero-desc { font-size: 13.5px !important; max-width: 92% !important; }
          .af-hero { padding: 36px 0 26px !important; }
          main { padding: 0 14px 60px !important; }
          .af-header-inner { padding: 10px 14px !important; }
          .af-brand-label { display: none; }
          .af-nav { gap: 8px !important; }
          .af-nav .af-owner-label { display: none; }
          .af-toolbar { flex-direction: column !important; align-items: stretch !important; }
          .af-tabs { overflow-x: auto !important; flex-wrap: nowrap !important; padding-bottom: 4px !important; -webkit-overflow-scrolling: touch; }
          .af-tabs::-webkit-scrollbar { height: 4px; }
          .af-tabs button { flex-shrink: 0; }
          .af-search { width: 100% !important; }
          .af-search-input { width: 100% !important; }
          .af-form-row { flex-direction: column !important; gap: 14px !important; }
          .af-cart-row { flex-wrap: wrap !important; }
          .af-cart-row .af-cart-name-block { min-width: 130px; }
          .af-cart-actions { flex-direction: column !important; align-items: stretch !important; gap: 14px !important; }
          .af-cart-actions > div { justify-content: space-between !important; width: 100% !important; }
          .af-pd-title { font-size: 24px !important; }
          .af-pd-actions { flex-direction: column !important; }
          .af-admin-header { flex-direction: column !important; align-items: stretch !important; gap: 12px !important; }
          .af-admin-header > div { justify-content: flex-start !important; }
          .af-admin-table-wrap { overflow-x: auto !important; }
          .af-admin-table-wrap table { min-width: 560px; }
          .af-modal-card { width: 94vw !important; padding: 20px !important; }
          .af-pd-gallery { grid-template-columns: repeat(auto-fill, minmax(54px, 1fr)) !important; }
          .af-upi-grid { gap: 6px !important; }
        }

        @media (max-width: 420px) {
          .af-grid { grid-template-columns: repeat(2, 1fr) !important; }
          .af-hero-title { font-size: 22px !important; }
        }
        @media (prefers-reduced-motion: reduce) {
          *, *::before, *::after { animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration: 0.001ms !important; }
        }
      `), toast && /*#__PURE__*/React.createElement("div", {
    className: "no-print toast-in",
    style: {
      position: "fixed",
      top: 16,
      left: "50%",
      zIndex: 100,
      background: "var(--gold)",
      color: "#0b0b0c",
      padding: "8px 18px",
      borderRadius: 999,
      fontSize: 13,
      fontWeight: 600
    }
  }, toast), /*#__PURE__*/React.createElement("header", {
    className: "no-print",
    style: {
      position: "sticky",
      top: 0,
      zIndex: 40,
      backdropFilter: "blur(8px)",
      backgroundColor: "rgba(11,11,12,0.85)",
      borderBottom: "1px solid var(--line)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    className: "af-header-inner",
    style: {
      maxWidth: 1100,
      margin: "0 auto",
      display: "flex",
      alignItems: "center",
      justifyContent: "space-between",
      padding: "12px 20px"
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: backToShop,
    className: "af-btn",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 10,
      background: "none",
      border: "none",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      width: 34,
      height: 34,
      borderRadius: "50%",
      background: "var(--bg)",
      border: "1px solid var(--gold)",
      display: "flex",
      alignItems: "center",
      justifyContent: "center"
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "af-serif",
    style: {
      color: "var(--gold)",
      fontWeight: 700,
      fontSize: 14
    }
  }, "AF")), /*#__PURE__*/React.createElement("span", {
    className: "af-serif af-brand-label",
    style: {
      fontSize: 18,
      letterSpacing: 1,
      color: "var(--cream)"
    }
  }, "APEX FASHION")), /*#__PURE__*/React.createElement("nav", {
    className: "af-nav",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 18
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => setView("shop"),
    className: "af-btn",
    style: {
      background: "none",
      border: "none",
      color: view === "shop" ? "var(--gold)" : "var(--muted)",
      fontSize: 14,
      cursor: "pointer"
    }
  }, "Shop"), /*#__PURE__*/React.createElement("button", {
    onClick: openManage,
    title: "Owner access only",
    className: "af-btn",
    style: {
      background: "none",
      border: "none",
      color: view === "admin" ? "var(--gold)" : "var(--muted)",
      fontSize: 13,
      cursor: "pointer",
      display: "flex",
      alignItems: "center",
      gap: 5,
      opacity: 0.7
    }
  }, /*#__PURE__*/React.createElement(Lock, {
    size: 13
  }), /*#__PURE__*/React.createElement("span", {
    className: "af-owner-label"
  }, " Owner")), /*#__PURE__*/React.createElement("button", {
    onClick: () => setView("cart"),
    className: "af-btn",
    style: {
      position: "relative",
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 10,
      padding: "8px 12px",
      cursor: "pointer",
      color: "var(--cream)",
      display: "flex",
      alignItems: "center",
      gap: 6
    }
  }, /*#__PURE__*/React.createElement(ShoppingCart, {
    size: 16
  }), /*#__PURE__*/React.createElement("span", {
    key: cartCount,
    style: {
      fontSize: 13
    },
    className: "af-mono bump"
  }, cartCount))))), /*#__PURE__*/React.createElement("main", {
    key: view,
    className: "view-enter",
    style: {
      maxWidth: 1100,
      margin: "0 auto",
      padding: "0 20px 80px"
    }
  }, view === "shop" && /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("section", {
    className: "af-hero",
    style: {
      display: "flex",
      flexDirection: "column",
      alignItems: "center",
      textAlign: "center",
      padding: "56px 0 36px",
      borderBottom: "1px solid var(--line)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    className: "badge-in"
  }, /*#__PURE__*/React.createElement(LogoBadge, {
    size: 128
  })), /*#__PURE__*/React.createElement("h1", {
    className: "af-serif hero-text-in af-hero-title",
    style: {
      fontSize: 34,
      marginTop: 22,
      marginBottom: 8,
      color: "var(--cream)"
    }
  }, "Curated Accessories, Quietly Made"), /*#__PURE__*/React.createElement("p", {
    className: "hero-text-in af-hero-desc",
    style: {
      color: "var(--muted)",
      maxWidth: 480,
      fontSize: 15,
      lineHeight: 1.6
    }
  }, "Watches, rings, chains and bracelets — chosen for restraint over noise. Add a piece to the cart, or skip straight to checkout.")), /*#__PURE__*/React.createElement("div", {
    className: "af-toolbar",
    style: {
      display: "flex",
      flexWrap: "wrap",
      gap: 10,
      alignItems: "center",
      justifyContent: "space-between",
      padding: "22px 0"
    }
  }, /*#__PURE__*/React.createElement("div", {
    className: "af-tabs",
    style: {
      display: "flex",
      gap: 8,
      flexWrap: "wrap"
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => setActiveCat("all"),
    className: `af-btn af-tab ${activeCat === "all" ? "active" : ""}`,
    style: {
      padding: "7px 14px",
      borderRadius: 999,
      border: `1px solid ${activeCat === "all" ? "var(--gold)" : "var(--line)"}`,
      background: activeCat === "all" ? "var(--surface2)" : "transparent",
      color: activeCat === "all" ? "var(--gold-light)" : "var(--muted)",
      fontSize: 13,
      cursor: "pointer"
    }
  }, "All"), CATS.map(c => {
    const Icon = c.icon;
    const active = activeCat === c.id;
    return /*#__PURE__*/React.createElement("button", {
      key: c.id,
      onClick: () => setActiveCat(c.id),
      className: `af-btn af-tab ${active ? "active" : ""}`,
      style: {
        padding: "7px 14px",
        borderRadius: 999,
        border: `1px solid ${active ? "var(--gold)" : "var(--line)"}`,
        background: active ? "var(--surface2)" : "transparent",
        color: active ? "var(--gold-light)" : "var(--muted)",
        fontSize: 13,
        cursor: "pointer",
        display: "flex",
        alignItems: "center",
        gap: 6
      }
    }, /*#__PURE__*/React.createElement(Icon, {
      size: 14
    }), " ", c.label);
  })), /*#__PURE__*/React.createElement("div", {
    className: "af-search",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 8,
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 10,
      padding: "8px 12px"
    }
  }, /*#__PURE__*/React.createElement(Search, {
    size: 15,
    color: "var(--muted)"
  }), /*#__PURE__*/React.createElement("input", {
    value: query,
    onChange: e => setQuery(e.target.value),
    placeholder: "Search products",
    className: "af-search-input",
    style: {
      background: "transparent",
      border: "none",
      color: "var(--cream)",
      fontSize: 13,
      width: 160
    }
  }))), /*#__PURE__*/React.createElement("div", {
    className: "af-grid",
    style: {
      display: "grid",
      gridTemplateColumns: "repeat(auto-fill, minmax(230px, 1fr))",
      gap: 18
    }
  }, filtered.map((p, i) => {
    const Icon = catIcon(p.category);
    return /*#__PURE__*/React.createElement("div", {
      key: p.id,
      className: "af-card card-enter",
      style: {
        border: "1px solid var(--line)",
        borderRadius: 14,
        background: "var(--surface)",
        overflow: "hidden",
        display: "flex",
        flexDirection: "column",
        animationDelay: `${Math.min(i, 10) * 45}ms`
      }
    }, /*#__PURE__*/React.createElement("div", {
      style: {
        height: 150,
        background: "linear-gradient(160deg, #1c1a17, #0b0b0c)",
        display: "flex",
        alignItems: "center",
        justifyContent: "center",
        cursor: "pointer",
        overflow: "hidden"
      },
      onClick: () => {
        setSelectedId(p.id);
        setView("product");
      }
    }, p.image ? /*#__PURE__*/React.createElement("img", {
      src: p.image,
      alt: p.name,
      className: "af-card-img",
      style: {
        width: "100%",
        height: "100%",
        objectFit: "cover"
      }
    }) : /*#__PURE__*/React.createElement(Icon, {
      size: 46,
      color: "var(--gold)",
      strokeWidth: 1.2,
      className: "af-card-icon"
    })), /*#__PURE__*/React.createElement("div", {
      style: {
        padding: 16,
        display: "flex",
        flexDirection: "column",
        gap: 8,
        flex: 1
      }
    }, /*#__PURE__*/React.createElement("span", {
      style: {
        fontSize: 11,
        letterSpacing: 1,
        color: "var(--muted)",
        textTransform: "uppercase"
      }
    }, catLabel(p.category)), /*#__PURE__*/React.createElement("h3", {
      className: "af-serif",
      onClick: () => {
        setSelectedId(p.id);
        setView("product");
      },
      style: {
        fontSize: 17,
        cursor: "pointer",
        color: "var(--cream)"
      }
    }, p.name), /*#__PURE__*/React.createElement("div", {
      className: "af-mono",
      style: {
        color: "var(--gold-light)",
        fontSize: 15,
        marginTop: "auto"
      }
    }, INR(p.price)), /*#__PURE__*/React.createElement("div", {
      style: {
        display: "flex",
        gap: 8,
        marginTop: 6
      }
    }, /*#__PURE__*/React.createElement("button", {
      onClick: () => addToCart(p.id),
      className: "af-btn",
      style: {
        flex: 1,
        padding: "8px 0",
        borderRadius: 8,
        border: "1px solid var(--gold)",
        background: "transparent",
        color: "var(--gold-light)",
        fontSize: 12.5,
        cursor: "pointer"
      }
    }, "Add to Cart"), /*#__PURE__*/React.createElement("button", {
      onClick: () => buyNow(p.id),
      className: "af-btn",
      style: {
        flex: 1,
        padding: "8px 0",
        borderRadius: 8,
        border: "none",
        background: "var(--gold)",
        color: "#0b0b0c",
        fontSize: 12.5,
        fontWeight: 600,
        cursor: "pointer"
      }
    }, "Buy Now"))));
  }), filtered.length === 0 && /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      gridColumn: "1/-1",
      textAlign: "center",
      padding: "40px 0"
    }
  }, "Nothing matches that search yet — try another term or category."))), view === "product" && selectedProduct && /*#__PURE__*/React.createElement(ProductDetail, {
    product: selectedProduct,
    onBack: () => setView("shop"),
    onAdd: addToCart,
    onBuyNow: buyNow
  }), view === "cart" && /*#__PURE__*/React.createElement("div", {
    style: {
      padding: "40px 0"
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => setView("shop"),
    className: "af-btn",
    style: {
      background: "none",
      border: "none",
      color: "var(--muted)",
      display: "flex",
      alignItems: "center",
      gap: 6,
      marginBottom: 20,
      cursor: "pointer",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement(ArrowLeft, {
    size: 15
  }), " Continue shopping"), /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 26,
      marginBottom: 20
    }
  }, "Your Cart"), cartItems.length === 0 ? /*#__PURE__*/React.createElement("div", {
    style: {
      textAlign: "center",
      padding: "60px 0",
      color: "var(--muted)"
    }
  }, /*#__PURE__*/React.createElement(ShoppingBag, {
    size: 36,
    style: {
      marginBottom: 10
    }
  }), /*#__PURE__*/React.createElement("p", null, "Your cart is empty. Add a piece to begin.")) : /*#__PURE__*/React.createElement(React.Fragment, null, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      gap: 12
    }
  }, cartItems.map(({
    product,
    qty
  }) => {
    const Icon = catIcon(product.category);
    return /*#__PURE__*/React.createElement("div", {
      key: product.id,
      className: "af-cart-row",
      style: {
        display: "flex",
        alignItems: "center",
        gap: 14,
        border: "1px solid var(--line)",
        background: "var(--surface)",
        borderRadius: 12,
        padding: 14
      }
    }, /*#__PURE__*/React.createElement("div", {
      style: {
        width: 52,
        height: 52,
        borderRadius: 8,
        background: "var(--surface2)",
        display: "flex",
        alignItems: "center",
        justifyContent: "center",
        flexShrink: 0,
        overflow: "hidden"
      }
    }, product.image ? /*#__PURE__*/React.createElement("img", {
      src: product.image,
      alt: product.name,
      style: {
        width: "100%",
        height: "100%",
        objectFit: "cover"
      }
    }) : /*#__PURE__*/React.createElement(Icon, {
      size: 22,
      color: "var(--gold)"
    })), /*#__PURE__*/React.createElement("div", {
      className: "af-cart-name-block",
      style: {
        flex: 1
      }
    }, /*#__PURE__*/React.createElement("div", {
      className: "af-serif",
      style: {
        fontSize: 15
      }
    }, product.name), /*#__PURE__*/React.createElement("div", {
      className: "af-mono",
      style: {
        fontSize: 13,
        color: "var(--gold-light)"
      }
    }, INR(product.price))), /*#__PURE__*/React.createElement("div", {
      style: {
        display: "flex",
        alignItems: "center",
        gap: 8,
        border: "1px solid var(--line)",
        borderRadius: 8,
        padding: "4px 8px"
      }
    }, /*#__PURE__*/React.createElement("button", {
      onClick: () => setQty(product.id, qty - 1),
      className: "qty-btn",
      style: {
        background: "none",
        border: "none",
        color: "var(--cream)",
        cursor: "pointer"
      }
    }, /*#__PURE__*/React.createElement(Minus, {
      size: 14
    })), /*#__PURE__*/React.createElement("span", {
      className: "af-mono",
      style: {
        fontSize: 13,
        minWidth: 18,
        textAlign: "center"
      }
    }, qty), /*#__PURE__*/React.createElement("button", {
      onClick: () => setQty(product.id, qty + 1),
      className: "qty-btn",
      style: {
        background: "none",
        border: "none",
        color: "var(--cream)",
        cursor: "pointer"
      }
    }, /*#__PURE__*/React.createElement(Plus, {
      size: 14
    }))), /*#__PURE__*/React.createElement("div", {
      className: "af-mono",
      style: {
        width: 90,
        textAlign: "right",
        fontSize: 14
      }
    }, INR(qty * product.price)), /*#__PURE__*/React.createElement("button", {
      onClick: () => removeFromCart(product.id),
      style: {
        background: "none",
        border: "none",
        color: "var(--muted)",
        cursor: "pointer"
      }
    }, /*#__PURE__*/React.createElement(Trash2, {
      size: 16
    })));
  })), /*#__PURE__*/React.createElement("div", {
    className: "af-cart-actions",
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginTop: 28,
      borderTop: "1px solid var(--line)",
      paddingTop: 20
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: clearCart,
    className: "af-btn",
    style: {
      background: "none",
      border: "1px solid var(--line)",
      color: "var(--muted)",
      padding: "10px 16px",
      borderRadius: 8,
      cursor: "pointer",
      fontSize: 13
    }
  }, "Clear Cart"), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      alignItems: "center",
      gap: 18
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "af-mono",
    style: {
      fontSize: 18,
      color: "var(--gold-light)"
    }
  }, "Total: ", INR(cartTotal)), /*#__PURE__*/React.createElement("button", {
    onClick: goCheckoutFromCart,
    className: "af-btn",
    style: {
      background: "var(--gold)",
      border: "none",
      color: "#0b0b0c",
      padding: "12px 22px",
      borderRadius: 8,
      fontWeight: 600,
      cursor: "pointer",
      display: "flex",
      alignItems: "center",
      gap: 6
    }
  }, "Checkout ", /*#__PURE__*/React.createElement(ArrowRight, {
    size: 15
  })))))), view === "address" && /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: 560,
      margin: "0 auto",
      padding: "40px 0"
    }
  }, /*#__PURE__*/React.createElement(Steps, {
    current: 1
  }), /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 24,
      margin: "20px 0 6px"
    }
  }, "Delivery & Contact Details"), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 13,
      marginBottom: 22
    }
  }, "We'll use this to ship your order and reach you if anything comes up."), /*#__PURE__*/React.createElement("form", {
    onSubmit: submitAddress,
    style: {
      display: "flex",
      flexDirection: "column",
      gap: 14
    }
  }, /*#__PURE__*/React.createElement(Field, {
    icon: User,
    label: "Full name",
    value: customer.name,
    onChange: v => setCustomer({
      ...customer,
      name: v
    }),
    placeholder: "e.g. Santhosh Kumar"
  }), /*#__PURE__*/React.createElement("div", {
    className: "af-form-row",
    style: {
      display: "flex",
      gap: 12
    }
  }, /*#__PURE__*/React.createElement(Field, {
    icon: Phone,
    label: "Phone number",
    value: customer.phone,
    onChange: v => setCustomer({
      ...customer,
      phone: v
    }),
    placeholder: "10-digit mobile"
  }), /*#__PURE__*/React.createElement(Field, {
    icon: Mail,
    label: "Email (optional)",
    value: customer.email,
    onChange: v => setCustomer({
      ...customer,
      email: v
    }),
    placeholder: "you@example.com"
  })), /*#__PURE__*/React.createElement(Field, {
    icon: MapPin,
    label: "Address",
    value: customer.address,
    onChange: v => setCustomer({
      ...customer,
      address: v
    }),
    placeholder: "House / street / area"
  }), /*#__PURE__*/React.createElement("div", {
    className: "af-form-row",
    style: {
      display: "flex",
      gap: 12
    }
  }, /*#__PURE__*/React.createElement(Field, {
    label: "City",
    value: customer.city,
    onChange: v => setCustomer({
      ...customer,
      city: v
    }),
    placeholder: "City"
  }), /*#__PURE__*/React.createElement(Field, {
    label: "State",
    value: customer.state,
    onChange: v => setCustomer({
      ...customer,
      state: v
    }),
    placeholder: "State"
  }), /*#__PURE__*/React.createElement(Field, {
    label: "Pincode",
    value: customer.pincode,
    onChange: v => setCustomer({
      ...customer,
      pincode: v
    }),
    placeholder: "600001"
  })), formError && /*#__PURE__*/React.createElement("p", {
    style: {
      color: "#e2897a",
      fontSize: 13
    }
  }, formError), /*#__PURE__*/React.createElement("div", {
    style: {
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 10,
      padding: 14,
      display: "flex",
      justifyContent: "space-between",
      fontSize: 14
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      color: "var(--muted)"
    }
  }, "Order total (", checkoutItems.reduce((s, c) => s + c.qty, 0), " item", checkoutItems.reduce((s, c) => s + c.qty, 0) !== 1 ? "s" : "", ")"), /*#__PURE__*/React.createElement("span", {
    className: "af-mono",
    style: {
      color: "var(--gold-light)"
    }
  }, INR(checkoutTotal))), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 10
    }
  }, /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => setView(buyNowOnly ? "shop" : "cart"),
    className: "af-btn",
    style: {
      flex: 1,
      padding: 12,
      borderRadius: 8,
      border: "1px solid var(--line)",
      background: "transparent",
      color: "var(--muted)",
      cursor: "pointer"
    }
  }, "Back"), /*#__PURE__*/React.createElement("button", {
    type: "submit",
    className: "af-btn",
    style: {
      flex: 2,
      padding: 12,
      borderRadius: 8,
      border: "none",
      background: "var(--gold)",
      color: "#0b0b0c",
      fontWeight: 600,
      cursor: "pointer"
    }
  }, "Continue to Payment")))), view === "payment" && /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: 460,
      margin: "0 auto",
      padding: "40px 0",
      textAlign: "center"
    }
  }, /*#__PURE__*/React.createElement(Steps, {
    current: 2
  }), /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 24,
      margin: "20px 0 6px"
    }
  }, "Scan & Pay"), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 13,
      marginBottom: 22
    }
  }, "Pay via any UPI app, then confirm below."), /*#__PURE__*/React.createElement("div", {
    style: {
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 16,
      padding: 26,
      display: "inline-flex",
      flexDirection: "column",
      alignItems: "center",
      gap: 16
    }
  }, /*#__PURE__*/React.createElement("img", {
    src: PAYMENT_QR_IMAGE,
    alt: "Scan to pay",
    style: {
      width: 176,
      height: 176,
      borderRadius: 8,
      objectFit: "contain",
      background: "#fff"
    }
  }), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      alignItems: "center",
      gap: 6,
      color: "var(--muted)",
      fontSize: 12
    }
  }, /*#__PURE__*/React.createElement(QrCode, {
    size: 14
  }), " Scan with any UPI app"), /*#__PURE__*/React.createElement("div", {
    className: "af-mono",
    style: {
      fontSize: 24,
      color: "var(--gold-light)"
    }
  }, INR(checkoutTotal))), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 11.5,
      margin: "18px 0 8px",
      letterSpacing: 0.5,
      textTransform: "uppercase"
    }
  }, "Or pay directly with your app"), /*#__PURE__*/React.createElement("div", {
    className: "af-upi-grid",
    style: {
      display: "grid",
      gridTemplateColumns: "repeat(4, 1fr)",
      gap: 8
    }
  }, [{
    key: "gpay",
    label: "Google Pay",
    color: "#4285F4"
  }, {
    key: "phonepe",
    label: "PhonePe",
    color: "#5F259F"
  }, {
    key: "paytm",
    label: "Paytm",
    color: "#00BAF2"
  }, {
    key: "other",
    label: "Other UPI",
    color: "var(--gold)"
  }].map(app => /*#__PURE__*/React.createElement("button", {
    key: app.key,
    onClick: () => openUpiApp(app.key),
    className: "af-btn",
    style: {
      display: "flex",
      flexDirection: "column",
      alignItems: "center",
      gap: 6,
      padding: "10px 4px",
      borderRadius: 10,
      border: "1px solid var(--line)",
      background: "var(--surface)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      width: 30,
      height: 30,
      borderRadius: "50%",
      background: app.color,
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      color: "#fff",
      fontSize: 12,
      fontWeight: 700
    }
  }, app.label[0]), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 10.5,
      color: "var(--muted)"
    }
  }, app.label)))), showReturnBanner && /*#__PURE__*/React.createElement("div", {
    style: {
      marginTop: 18,
      padding: "10px 14px",
      borderRadius: 10,
      border: "1px solid var(--gold)",
      background: "rgba(212,175,109,0.08)",
      color: "var(--gold-light)",
      fontSize: 12.5,
      textAlign: "left"
    }
  }, "Welcome back! If your payment went through, confirm your order below."), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 11.5,
      marginTop: 14,
      lineHeight: 1.5
    }
  }, "After paying, tap the button below — it opens WhatsApp with your order details already filled in for ", "+91 " + OWNER_WHATSAPP.slice(2), ". Just hit send (and attach your payment screenshot) to confirm the order."), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 10,
      marginTop: 24
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => setView("address"),
    className: "af-btn",
    style: {
      flex: 1,
      padding: 12,
      borderRadius: 8,
      border: "1px solid var(--line)",
      background: "transparent",
      color: "var(--muted)",
      cursor: "pointer"
    }
  }, "Back"), /*#__PURE__*/React.createElement("a", {
    href: whatsappLink,
    target: "_blank",
    rel: "noopener noreferrer",
    onClick: confirmPayment,
    className: "af-btn",
    style: {
      flex: 2,
      padding: 12,
      borderRadius: 8,
      border: "none",
      background: "var(--gold)",
      color: "#0b0b0c",
      fontWeight: 600,
      cursor: "pointer",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      gap: 6,
      textDecoration: "none"
    }
  }, /*#__PURE__*/React.createElement(Check, {
    size: 16
  }), " I've Paid — Send Order on WhatsApp"))), view === "invoice" && invoice && /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: 640,
      margin: "0 auto",
      padding: "40px 0"
    }
  }, /*#__PURE__*/React.createElement("div", {
    className: "no-print",
    style: {
      display: "flex",
      justifyContent: "flex-end",
      gap: 10,
      marginBottom: 16
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => window.print(),
    className: "af-btn",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 6,
      padding: "9px 14px",
      borderRadius: 8,
      border: "1px solid var(--line)",
      background: "var(--surface)",
      color: "var(--cream)",
      cursor: "pointer",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement(Printer, {
    size: 14
  }), " Print / Save PDF"), /*#__PURE__*/React.createElement("button", {
    onClick: backToShop,
    className: "af-btn",
    style: {
      padding: "9px 14px",
      borderRadius: 8,
      border: "none",
      background: "var(--gold)",
      color: "#0b0b0c",
      cursor: "pointer",
      fontSize: 13,
      fontWeight: 600
    }
  }, "Back to Shop")), /*#__PURE__*/React.createElement("div", {
    style: {
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 16,
      padding: 32
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "flex-start",
      borderBottom: "1px solid var(--line)",
      paddingBottom: 20,
      marginBottom: 20
    }
  }, /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 22
    }
  }, "APEX FASHION"), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 12
    }
  }, "Curated Accessories · Est. 2026")), /*#__PURE__*/React.createElement("div", {
    className: "stamp-in"
  }, /*#__PURE__*/React.createElement(LogoBadge, {
    size: 72,
    stamp: true
  }))), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      flexWrap: "wrap",
      gap: 20,
      marginBottom: 22
    }
  }, /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    style: {
      color: "var(--muted)",
      fontSize: 11,
      textTransform: "uppercase",
      letterSpacing: 1
    }
  }, "Invoice No."), /*#__PURE__*/React.createElement("div", {
    className: "af-mono",
    style: {
      fontSize: 14
    }
  }, invoice.number)), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    style: {
      color: "var(--muted)",
      fontSize: 11,
      textTransform: "uppercase",
      letterSpacing: 1
    }
  }, "Booking Date"), /*#__PURE__*/React.createElement("div", {
    className: "af-mono",
    style: {
      fontSize: 14
    }
  }, invoice.date.toLocaleString("en-IN"))), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    style: {
      color: "var(--muted)",
      fontSize: 11,
      textTransform: "uppercase",
      letterSpacing: 1
    }
  }, "Payment Status"), /*#__PURE__*/React.createElement("div", {
    className: "af-mono",
    style: {
      fontSize: 14,
      color: "#8fbf8a"
    }
  }, invoice.status))), /*#__PURE__*/React.createElement("div", {
    style: {
      marginBottom: 22
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      color: "var(--muted)",
      fontSize: 11,
      textTransform: "uppercase",
      letterSpacing: 1,
      marginBottom: 4
    }
  }, "Billed To"), /*#__PURE__*/React.createElement("div", {
    style: {
      fontSize: 14
    }
  }, invoice.customer.name, " · ", invoice.customer.phone), /*#__PURE__*/React.createElement("div", {
    style: {
      fontSize: 13,
      color: "var(--muted)"
    }
  }, invoice.customer.address, ", ", invoice.customer.city, ", ", invoice.customer.state, " ", invoice.customer.pincode)), /*#__PURE__*/React.createElement("table", {
    style: {
      width: "100%",
      borderCollapse: "collapse",
      fontSize: 13,
      marginBottom: 20
    }
  }, /*#__PURE__*/React.createElement("thead", null, /*#__PURE__*/React.createElement("tr", {
    style: {
      borderBottom: "1px solid var(--line)",
      color: "var(--muted)",
      textAlign: "left"
    }
  }, /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "8px 0"
    }
  }, "Product"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "8px 0"
    }
  }, "Category"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "8px 0",
      textAlign: "center"
    }
  }, "Qty"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "8px 0",
      textAlign: "right"
    }
  }, "Price"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "8px 0",
      textAlign: "right"
    }
  }, "Subtotal"))), /*#__PURE__*/React.createElement("tbody", null, invoice.items.map((it, i) => /*#__PURE__*/React.createElement("tr", {
    key: i,
    style: {
      borderBottom: "1px solid var(--line)"
    }
  }, /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "8px 0"
    },
    className: "af-serif"
  }, it.name), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "8px 0",
      color: "var(--muted)"
    }
  }, catLabel(it.category)), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "8px 0",
      textAlign: "center"
    },
    className: "af-mono"
  }, it.qty), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "8px 0",
      textAlign: "right"
    },
    className: "af-mono"
  }, INR(it.price)), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "8px 0",
      textAlign: "right"
    },
    className: "af-mono"
  }, INR(it.price * it.qty)))))), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      marginBottom: 6,
      fontSize: 13,
      color: "var(--muted)"
    }
  }, /*#__PURE__*/React.createElement("span", null, "Payment Method"), /*#__PURE__*/React.createElement("span", {
    className: "af-mono"
  }, invoice.method)), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      paddingTop: 12,
      borderTop: "1px solid var(--line)",
      fontSize: 18
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "af-serif"
  }, "Total Paid"), /*#__PURE__*/React.createElement("span", {
    className: "af-mono",
    style: {
      color: "var(--gold-light)"
    }
  }, INR(invoice.total))))), view === "admin" && !isOwner && /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: 360,
      margin: "0 auto",
      padding: "60px 0",
      textAlign: "center"
    }
  }, /*#__PURE__*/React.createElement(Lock, {
    size: 28,
    color: "var(--gold)",
    style: {
      marginBottom: 14
    }
  }), /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 22,
      marginBottom: 6
    }
  }, "Owner Access"), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 13,
      marginBottom: 20
    }
  }, "Enter the owner PIN to manage products. Customers can't edit the catalog."), /*#__PURE__*/React.createElement("form", {
    onSubmit: submitPin,
    style: {
      display: "flex",
      flexDirection: "column",
      gap: 12
    }
  }, /*#__PURE__*/React.createElement("input", {
    type: "password",
    value: pinInput,
    onChange: e => setPinInput(e.target.value),
    placeholder: "Owner PIN",
    style: {
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "10px 12px",
      color: "var(--cream)",
      fontSize: 14,
      textAlign: "center"
    }
  }), pinError && /*#__PURE__*/React.createElement("p", {
    style: {
      color: "#e2897a",
      fontSize: 13
    }
  }, pinError), /*#__PURE__*/React.createElement("button", {
    type: "submit",
    className: "af-btn",
    style: {
      background: "var(--gold)",
      border: "none",
      color: "#0b0b0c",
      padding: 11,
      borderRadius: 8,
      fontWeight: 600,
      cursor: "pointer"
    }
  }, "Unlock"), /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => setView("shop"),
    style: {
      background: "none",
      border: "none",
      color: "var(--muted)",
      fontSize: 13,
      cursor: "pointer"
    }
  }, "Back to shop"))), view === "admin" && isOwner && /*#__PURE__*/React.createElement("div", {
    style: {
      padding: "40px 0"
    }
  }, /*#__PURE__*/React.createElement("div", {
    className: "af-admin-header",
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginBottom: 20
    }
  }, /*#__PURE__*/React.createElement("h2", {
    className: "af-serif",
    style: {
      fontSize: 24
    }
  }, "Manage Products"), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 10
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: openNewProduct,
    className: "af-btn",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 6,
      background: "var(--gold)",
      border: "none",
      color: "#0b0b0c",
      padding: "9px 16px",
      borderRadius: 8,
      fontWeight: 600,
      cursor: "pointer",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement(Plus, {
    size: 15
  }), " Add Product"), /*#__PURE__*/React.createElement("button", {
    onClick: ownerLogout,
    className: "af-btn",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 6,
      background: "transparent",
      border: "1px solid var(--line)",
      color: "var(--muted)",
      padding: "9px 14px",
      borderRadius: 8,
      cursor: "pointer",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement(LogOut, {
    size: 14
  }), " Log out"))), /*#__PURE__*/React.createElement("div", {
    className: "af-admin-table-wrap",
    style: {
      border: "1px solid var(--line)",
      borderRadius: 12,
      overflow: "auto"
    }
  }, /*#__PURE__*/React.createElement("table", {
    style: {
      width: "100%",
      borderCollapse: "collapse",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement("thead", null, /*#__PURE__*/React.createElement("tr", {
    style: {
      background: "var(--surface2)",
      textAlign: "left",
      color: "var(--muted)"
    }
  }, /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }, "Image"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }, "Name"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }, "Category"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }, "Price"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }, "Stock"), /*#__PURE__*/React.createElement("th", {
    style: {
      padding: "10px 14px"
    }
  }))), /*#__PURE__*/React.createElement("tbody", null, products.map(p => /*#__PURE__*/React.createElement("tr", {
    key: p.id,
    style: {
      borderTop: "1px solid var(--line)",
      background: "var(--surface)"
    }
  }, /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      width: 40,
      height: 40,
      borderRadius: 6,
      background: "var(--surface2)",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      overflow: "hidden"
    }
  }, p.image ? /*#__PURE__*/React.createElement("img", {
    src: p.image,
    alt: p.name,
    style: {
      width: "100%",
      height: "100%",
      objectFit: "cover"
    }
  }) : React.createElement(catIcon(p.category), {
    size: 18,
    color: "var(--gold)"
  }))), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px"
    },
    className: "af-serif"
  }, p.name), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px",
      color: "var(--muted)"
    }
  }, catLabel(p.category)), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px"
    },
    className: "af-mono"
  }, INR(p.price)), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px"
    },
    className: "af-mono"
  }, p.stock), /*#__PURE__*/React.createElement("td", {
    style: {
      padding: "10px 14px",
      display: "flex",
      gap: 10,
      justifyContent: "flex-end"
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => openEditProduct(p),
    style: {
      background: "none",
      border: "none",
      color: "var(--gold-light)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement(Edit2, {
    size: 15
  })), /*#__PURE__*/React.createElement("button", {
    onClick: () => deleteProduct(p.id),
    style: {
      background: "none",
      border: "none",
      color: "var(--muted)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement(Trash2, {
    size: 15
  }))))), products.length === 0 && /*#__PURE__*/React.createElement("tr", null, /*#__PURE__*/React.createElement("td", {
    colSpan: 5,
    style: {
      padding: 24,
      textAlign: "center",
      color: "var(--muted)"
    }
  }, "No products yet — add your first one."))))))), showForm && editingProduct && /*#__PURE__*/React.createElement("div", {
    style: {
      position: "fixed",
      inset: 0,
      background: "rgba(0,0,0,0.6)",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      zIndex: 60,
      padding: 20
    }
  }, /*#__PURE__*/React.createElement("form", {
    onSubmit: saveProduct,
    className: "af-modal-card",
    style: {
      background: "var(--surface)",
      border: "1px solid var(--line)",
      borderRadius: 14,
      padding: 24,
      width: 380,
      maxHeight: "90vh",
      overflowY: "auto",
      display: "flex",
      flexDirection: "column",
      gap: 12
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginBottom: 4
    }
  }, /*#__PURE__*/React.createElement("h3", {
    className: "af-serif",
    style: {
      fontSize: 18
    }
  }, editingProduct.id ? "Edit Product" : "New Product"), /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => {
      setShowForm(false);
      setEditingProduct(null);
    },
    style: {
      background: "none",
      border: "none",
      color: "var(--muted)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement(X, {
    size: 18
  }))), /*#__PURE__*/React.createElement(Field, {
    label: "Name",
    value: editingProduct.name,
    onChange: v => setEditingProduct({
      ...editingProduct,
      name: v
    }),
    placeholder: "Product name"
  }), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("label", {
    style: {
      fontSize: 12,
      color: "var(--muted)"
    }
  }, "Category"), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 8,
      marginTop: 4
    }
  }, /*#__PURE__*/React.createElement("select", {
    value: editingProduct.category,
    onChange: e => setEditingProduct({
      ...editingProduct,
      category: e.target.value
    }),
    style: {
      flex: 1,
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "9px 10px",
      color: "var(--cream)",
      fontSize: 13
    }
  }, CATS.map(c => /*#__PURE__*/React.createElement("option", {
    key: c.id,
    value: c.id
  }, c.label))), /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => {
      setAddingCategory(a => !a);
      setCategoryError("");
    },
    className: "af-btn",
    style: {
      display: "flex",
      alignItems: "center",
      gap: 4,
      padding: "0 12px",
      borderRadius: 8,
      border: "1px solid var(--line)",
      background: "transparent",
      color: "var(--gold-light)",
      fontSize: 12.5,
      cursor: "pointer",
      whiteSpace: "nowrap"
    }
  }, /*#__PURE__*/React.createElement(Plus, {
    size: 13
  }), " New")), addingCategory && /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 8,
      marginTop: 8
    }
  }, /*#__PURE__*/React.createElement("input", {
    autoFocus: true,
    value: newCategoryName,
    onChange: e => {
      setNewCategoryName(e.target.value);
      setCategoryError("");
    },
    onKeyDown: e => {
      if (e.key === "Enter") {
        e.preventDefault();
        const id = addCategory(newCategoryName);
        if (id) setEditingProduct(p => ({
          ...p,
          category: id
        }));
      }
    },
    placeholder: "New category name",
    style: {
      flex: 1,
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "9px 10px",
      color: "var(--cream)",
      fontSize: 13
    }
  }), /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => {
      const id = addCategory(newCategoryName);
      if (id) setEditingProduct(p => ({
        ...p,
        category: id
      }));
    },
    className: "af-btn",
    style: {
      padding: "0 14px",
      borderRadius: 8,
      border: "none",
      background: "var(--gold)",
      color: "#0b0b0c",
      fontSize: 12.5,
      fontWeight: 600,
      cursor: "pointer"
    }
  }, "Add")), categoryError && /*#__PURE__*/React.createElement("p", {
    style: {
      color: "#e07a6b",
      fontSize: 11.5,
      marginTop: 6
    }
  }, categoryError)), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 10
    }
  }, /*#__PURE__*/React.createElement(Field, {
    label: "Price (₹)",
    value: editingProduct.price,
    onChange: v => setEditingProduct({
      ...editingProduct,
      price: v
    }),
    placeholder: "0"
  }), /*#__PURE__*/React.createElement(Field, {
    label: "Stock",
    value: editingProduct.stock,
    onChange: v => setEditingProduct({
      ...editingProduct,
      stock: v
    }),
    placeholder: "0"
  })), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("label", {
    style: {
      fontSize: 12,
      color: "var(--muted)"
    }
  }, "Description"), /*#__PURE__*/React.createElement("textarea", {
    value: editingProduct.desc,
    onChange: e => setEditingProduct({
      ...editingProduct,
      desc: e.target.value
    }),
    rows: 3,
    style: {
      width: "100%",
      marginTop: 4,
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "9px 10px",
      color: "var(--cream)",
      fontSize: 13,
      resize: "none"
    }
  })), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("label", {
    style: {
      fontSize: 12,
      color: "var(--muted)"
    }
  }, "Product Photos"), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "grid",
      gridTemplateColumns: "repeat(auto-fill, minmax(56px, 1fr))",
      gap: 8,
      marginTop: 4
    }
  }, (editingProduct.images || []).map((img, idx) => /*#__PURE__*/React.createElement("div", {
    key: idx,
    style: {
      position: "relative",
      width: "100%",
      paddingTop: "100%",
      borderRadius: 8,
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      overflow: "hidden"
    }
  }, /*#__PURE__*/React.createElement("img", {
    src: img,
    alt: `Photo ${idx + 1}`,
    style: {
      position: "absolute",
      inset: 0,
      width: "100%",
      height: "100%",
      objectFit: "cover"
    }
  }), /*#__PURE__*/React.createElement("button", {
    type: "button",
    onClick: () => removeEditingImage(idx),
    style: {
      position: "absolute",
      top: 2,
      right: 2,
      width: 18,
      height: 18,
      borderRadius: "50%",
      background: "rgba(11,11,12,0.75)",
      border: "none",
      color: "var(--cream)",
      cursor: "pointer",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      padding: 0
    }
  }, /*#__PURE__*/React.createElement(X, {
    size: 11
  })))), /*#__PURE__*/React.createElement("label", {
    style: {
      width: "100%",
      paddingTop: "100%",
      position: "relative",
      borderRadius: 8,
      border: "1px dashed var(--line)",
      color: "var(--gold-light)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      position: "absolute",
      inset: 0,
      display: "flex",
      alignItems: "center",
      justifyContent: "center"
    }
  }, /*#__PURE__*/React.createElement(ImageIcon, {
    size: 18,
    color: "var(--muted)"
  })), /*#__PURE__*/React.createElement("input", {
    type: "file",
    accept: "image/*",
    multiple: true,
    onChange: e => {
      handleImageUpload(e.target.files);
      e.target.value = "";
    },
    style: {
      display: "none"
    }
  }))), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 11,
      color: "var(--muted)",
      marginTop: 6
    }
  }, "Add one or more photos. The first photo is used as the cover image in the shop.")), /*#__PURE__*/React.createElement("button", {
    type: "submit",
    className: "af-btn",
    style: {
      marginTop: 6,
      background: "var(--gold)",
      border: "none",
      color: "#0b0b0c",
      padding: 11,
      borderRadius: 8,
      fontWeight: 600,
      cursor: "pointer"
    }
  }, editingProduct.id ? "Save Changes" : "Add Product"))), /*#__PURE__*/React.createElement("footer", {
    className: "no-print",
    style: {
      textAlign: "center",
      padding: "30px 20px",
      borderTop: "1px solid var(--line)",
      color: "var(--muted)",
      fontSize: 12
    }
  }, "© 2026 Apex Fashion · Curated Accessories"));
}
function ProductDetail({
  product,
  onBack,
  onAdd,
  onBuyNow
}) {
  const [qty, setQty] = useState(1);
  const Icon = catIcon(product.category);
  const images = (product.images && product.images.length ? product.images : product.image ? [product.image] : []);
  const [activeImg, setActiveImg] = useState(0);
  useEffect(() => {
    setActiveImg(0);
  }, [product.id]);
  return /*#__PURE__*/React.createElement("div", {
    className: "af-pd",
    style: {
      padding: "40px 0"
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: onBack,
    className: "af-btn",
    style: {
      background: "none",
      border: "none",
      color: "var(--muted)",
      display: "flex",
      alignItems: "center",
      gap: 6,
      marginBottom: 24,
      cursor: "pointer",
      fontSize: 13
    }
  }, /*#__PURE__*/React.createElement(ArrowLeft, {
    size: 15
  }), " Back to shop"), /*#__PURE__*/React.createElement("div", {
    className: "af-pd-grid",
    style: {
      display: "grid",
      gridTemplateColumns: "1fr 1fr",
      gap: 40
    }
  }, /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    className: "af-pd-image",
    style: {
      height: 420,
      borderRadius: 16,
      background: "linear-gradient(160deg, #1c1a17, #0b0b0c)",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      border: "1px solid var(--line)",
      overflow: "hidden"
    }
  }, images.length ? /*#__PURE__*/React.createElement("img", {
    src: images[activeImg] || images[0],
    alt: product.name,
    style: {
      width: "100%",
      height: "100%",
      objectFit: "cover"
    }
  }) : /*#__PURE__*/React.createElement(Icon, {
    size: 90,
    color: "var(--gold)",
    strokeWidth: 1.1
  })), images.length > 1 && /*#__PURE__*/React.createElement("div", {
    className: "af-pd-gallery",
    style: {
      display: "grid",
      gridTemplateColumns: "repeat(auto-fill, minmax(64px, 1fr))",
      gap: 8,
      marginTop: 10
    }
  }, images.map((img, idx) => /*#__PURE__*/React.createElement("button", {
    key: idx,
    onClick: () => setActiveImg(idx),
    className: "af-pd-gallery-thumb",
    style: {
      height: 64,
      borderRadius: 8,
      overflow: "hidden",
      padding: 0,
      background: "var(--surface2)",
      border: `2px solid ${idx === activeImg ? "var(--gold)" : "var(--line)"}`,
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement("img", {
    src: img,
    alt: `${product.name} ${idx + 1}`,
    style: {
      width: "100%",
      height: "100%",
      objectFit: "cover"
    }
  }))))), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 11,
      letterSpacing: 1.5,
      color: "var(--muted)",
      textTransform: "uppercase"
    }
  }, catLabel(product.category)), /*#__PURE__*/React.createElement("h1", {
    className: "af-serif af-pd-title",
    style: {
      fontSize: 30,
      margin: "8px 0"
    }
  }, product.name), /*#__PURE__*/React.createElement("div", {
    className: "af-mono",
    style: {
      fontSize: 22,
      color: "var(--gold-light)",
      marginBottom: 14
    }
  }, INR(product.price)), /*#__PURE__*/React.createElement("p", {
    style: {
      color: "var(--muted)",
      fontSize: 14,
      lineHeight: 1.6,
      marginBottom: 20
    }
  }, product.desc), /*#__PURE__*/React.createElement("div", {
    style: {
      fontSize: 12,
      color: product.stock > 0 ? "#8fbf8a" : "#e2897a",
      display: "flex",
      alignItems: "center",
      gap: 5,
      marginBottom: 20
    }
  }, /*#__PURE__*/React.createElement(Star, {
    size: 12
  }), " ", product.stock > 0 ? `${product.stock} in stock` : "Out of stock"), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      alignItems: "center",
      gap: 8,
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "6px 10px",
      width: "fit-content",
      marginBottom: 20
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => setQty(Math.max(1, qty - 1)),
    className: "qty-btn",
    style: {
      background: "none",
      border: "none",
      color: "var(--cream)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement(Minus, {
    size: 15
  })), /*#__PURE__*/React.createElement("span", {
    className: "af-mono",
    style: {
      minWidth: 22,
      textAlign: "center"
    }
  }, qty), /*#__PURE__*/React.createElement("button", {
    onClick: () => setQty(qty + 1),
    className: "qty-btn",
    style: {
      background: "none",
      border: "none",
      color: "var(--cream)",
      cursor: "pointer"
    }
  }, /*#__PURE__*/React.createElement(Plus, {
    size: 15
  }))), /*#__PURE__*/React.createElement("div", {
    className: "af-pd-actions",
    style: {
      display: "flex",
      gap: 12
    }
  }, /*#__PURE__*/React.createElement("button", {
    onClick: () => onAdd(product.id, qty),
    className: "af-btn",
    style: {
      flex: 1,
      padding: 13,
      borderRadius: 8,
      border: "1px solid var(--gold)",
      background: "transparent",
      color: "var(--gold-light)",
      cursor: "pointer",
      fontWeight: 500
    }
  }, "Add to Cart"), /*#__PURE__*/React.createElement("button", {
    onClick: () => onBuyNow(product.id),
    className: "af-btn",
    style: {
      flex: 1,
      padding: 13,
      borderRadius: 8,
      border: "none",
      background: "var(--gold)",
      color: "#0b0b0c",
      fontWeight: 600,
      cursor: "pointer"
    }
  }, "Buy Now")))));
}
function Field({
  icon: Icon,
  label,
  value,
  onChange,
  placeholder
}) {
  return /*#__PURE__*/React.createElement("div", {
    style: {
      flex: 1
    }
  }, /*#__PURE__*/React.createElement("label", {
    style: {
      fontSize: 12,
      color: "var(--muted)"
    }
  }, label), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      alignItems: "center",
      gap: 8,
      background: "var(--surface2)",
      border: "1px solid var(--line)",
      borderRadius: 8,
      padding: "9px 10px",
      marginTop: 4
    }
  }, Icon && /*#__PURE__*/React.createElement(Icon, {
    size: 14,
    color: "var(--muted)"
  }), /*#__PURE__*/React.createElement("input", {
    value: value,
    onChange: e => onChange(e.target.value),
    placeholder: placeholder,
    style: {
      background: "transparent",
      border: "none",
      color: "var(--cream)",
      fontSize: 13,
      width: "100%"
    }
  })));
}
function Steps({
  current
}) {
  const steps = ["Cart", "Address", "Payment", "Invoice"];
  return /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: 8,
      justifyContent: "center"
    }
  }, steps.map((s, i) => /*#__PURE__*/React.createElement("div", {
    key: s,
    style: {
      display: "flex",
      alignItems: "center",
      gap: 8
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      width: 24,
      height: 24,
      borderRadius: "50%",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      fontSize: 11,
      border: `1px solid ${i <= current ? "var(--gold)" : "var(--line)"}`,
      color: i <= current ? "var(--gold-light)" : "var(--muted)",
      background: i <= current ? "var(--surface2)" : "transparent"
    },
    className: "af-mono step-dot"
  }, i + 1), i < steps.length - 1 && /*#__PURE__*/React.createElement("div", {
    style: {
      width: 20,
      height: 1,
      background: "var(--line)"
    }
  }))));
}
ReactDOM.createRoot(document.getElementById("root")).render(React.createElement(ApexFashion));
</script>
</body>
</html>
