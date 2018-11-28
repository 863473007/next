{"title":"Custom Navigation Arrows","meta":{"title":"Custom Navigation Arrows","description":"\n<p>You can pass custom navigation arrow components through the two attributes <code>prevArrow</code> and <code>nextArrow</code>.</p>\n","order":"7"},"codes":{"jsx":"import { Slider, Icon } from '@alifd/next';\n\nconst slides = [\n    { url: 'https://img.alicdn.com/tps/TB1bewbNVXXXXc5XXXXXXXXXXXX-1000-300.png', text: 'Tape Player Skin Design Competition' },\n    { url: 'https://img.alicdn.com/tps/TB1xuUcNVXXXXcRXXXXXXXXXXXX-1000-300.jpg', text: 'Mobile Phone Taobao Skin Call' },\n    { url: 'https://img.alicdn.com/tps/TB1ikP.NVXXXXaYXpXXXXXXXXXX-1000-300.jpg', text: 'Design Enabling Public Welfare' },\n    { url: 'https://img.alicdn.com/tps/TB1s1_JNVXXXXbhaXXXXXXXXXXX-1000-300.jpg', text: 'Amoy Doll Design Competition' },\n];\n\nconst arrowStyle = {\n    display: 'block',\n    background: 'red',\n    opacity: 1,\n    margin: '0 20px',\n};\n\nconst CustomNextArrow = (props) => {\n    return <div {...props} style={arrowStyle}><Icon type=\"arrow-double-right\" /></div>;\n};\n\nconst CustomPrevArrow = (props) => {\n    return <div {...props} style={arrowStyle}><Icon type=\"arrow-double-left\" /></div>;\n};\n\nReactDOM.render(\n    <Slider nextArrow={<CustomNextArrow />} prevArrow={<CustomPrevArrow />} lazyLoad>\n        {\n            slides.map((item, index) => <div key={index} className=\"slider-img-wrapper\"><img src={item.url} alt={item.text} /></div>)\n        }\n    </Slider>\n    , mountNode);\n","css":".slider-img-wrapper img {\n    width: 100%;\n}\n"},"body":"\n````jsx\nimport { Slider, Icon } from '@alifd/next';\n\nconst slides = [\n    { url: 'https://img.alicdn.com/tps/TB1bewbNVXXXXc5XXXXXXXXXXXX-1000-300.png', text: 'Tape Player Skin Design Competition' },\n    { url: 'https://img.alicdn.com/tps/TB1xuUcNVXXXXcRXXXXXXXXXXXX-1000-300.jpg', text: 'Mobile Phone Taobao Skin Call' },\n    { url: 'https://img.alicdn.com/tps/TB1ikP.NVXXXXaYXpXXXXXXXXXX-1000-300.jpg', text: 'Design Enabling Public Welfare' },\n    { url: 'https://img.alicdn.com/tps/TB1s1_JNVXXXXbhaXXXXXXXXXXX-1000-300.jpg', text: 'Amoy Doll Design Competition' },\n];\n\nconst arrowStyle = {\n    display: 'block',\n    background: 'red',\n    opacity: 1,\n    margin: '0 20px',\n};\n\nconst CustomNextArrow = (props) => {\n    return <div {...props} style={arrowStyle}><Icon type=\"arrow-double-right\" /></div>;\n};\n\nconst CustomPrevArrow = (props) => {\n    return <div {...props} style={arrowStyle}><Icon type=\"arrow-double-left\" /></div>;\n};\n\nReactDOM.render(\n    <Slider nextArrow={<CustomNextArrow />} prevArrow={<CustomPrevArrow />} lazyLoad>\n        {\n            slides.map((item, index) => <div key={index} className=\"slider-img-wrapper\"><img src={item.url} alt={item.text} /></div>)\n        }\n    </Slider>\n    , mountNode);\n````\n\n````css\n.slider-img-wrapper img {\n    width: 100%;\n}\n````","html":"<script>(function(){'use strict';\n\nvar _extends = Object.assign || function (target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i]; for (var key in source) { if (Object.prototype.hasOwnProperty.call(source, key)) { target[key] = source[key]; } } } return target; };\n\nvar _next = require('@alifd/next');\n\nvar slides = [{ url: 'https://img.alicdn.com/tps/TB1bewbNVXXXXc5XXXXXXXXXXXX-1000-300.png', text: 'Tape Player Skin Design Competition' }, { url: 'https://img.alicdn.com/tps/TB1xuUcNVXXXXcRXXXXXXXXXXXX-1000-300.jpg', text: 'Mobile Phone Taobao Skin Call' }, { url: 'https://img.alicdn.com/tps/TB1ikP.NVXXXXaYXpXXXXXXXXXX-1000-300.jpg', text: 'Design Enabling Public Welfare' }, { url: 'https://img.alicdn.com/tps/TB1s1_JNVXXXXbhaXXXXXXXXXXX-1000-300.jpg', text: 'Amoy Doll Design Competition' }];\n\nvar arrowStyle = {\n    display: 'block',\n    background: 'red',\n    opacity: 1,\n    margin: '0 20px'\n};\n\nvar CustomNextArrow = function CustomNextArrow(props) {\n    return React.createElement(\n        'div',\n        _extends({}, props, { style: arrowStyle }),\n        React.createElement(_next.Icon, { type: 'arrow-double-right' })\n    );\n};\n\nvar CustomPrevArrow = function CustomPrevArrow(props) {\n    return React.createElement(\n        'div',\n        _extends({}, props, { style: arrowStyle }),\n        React.createElement(_next.Icon, { type: 'arrow-double-left' })\n    );\n};\n\nReactDOM.render(React.createElement(\n    _next.Slider,\n    { nextArrow: React.createElement(CustomNextArrow, null), prevArrow: React.createElement(CustomPrevArrow, null), lazyLoad: true },\n    slides.map(function (item, index) {\n        return React.createElement(\n            'div',\n            { key: index, className: 'slider-img-wrapper' },\n            React.createElement('img', { src: item.url, alt: item.text })\n        );\n    })\n), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Slider<span class=\"token punctuation\">,</span> Icon <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> slides <span class=\"token operator\">=</span> <span class=\"token punctuation\">[</span>\n    <span class=\"token punctuation\">{</span> url<span class=\"token punctuation\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB1bewbNVXXXXc5XXXXXXXXXXXX-1000-300.png'</span><span class=\"token punctuation\">,</span> text<span class=\"token punctuation\">:</span> <span class=\"token string\">'Tape Player Skin Design Competition'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">,</span>\n    <span class=\"token punctuation\">{</span> url<span class=\"token punctuation\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB1xuUcNVXXXXcRXXXXXXXXXXXX-1000-300.jpg'</span><span class=\"token punctuation\">,</span> text<span class=\"token punctuation\">:</span> <span class=\"token string\">'Mobile Phone Taobao Skin Call'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">,</span>\n    <span class=\"token punctuation\">{</span> url<span class=\"token punctuation\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB1ikP.NVXXXXaYXpXXXXXXXXXX-1000-300.jpg'</span><span class=\"token punctuation\">,</span> text<span class=\"token punctuation\">:</span> <span class=\"token string\">'Design Enabling Public Welfare'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">,</span>\n    <span class=\"token punctuation\">{</span> url<span class=\"token punctuation\">:</span> <span class=\"token string\">'https://img.alicdn.com/tps/TB1s1_JNVXXXXbhaXXXXXXXXXXX-1000-300.jpg'</span><span class=\"token punctuation\">,</span> text<span class=\"token punctuation\">:</span> <span class=\"token string\">'Amoy Doll Design Competition'</span> <span class=\"token punctuation\">}</span><span class=\"token punctuation\">,</span>\n<span class=\"token punctuation\">]</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> arrowStyle <span class=\"token operator\">=</span> <span class=\"token punctuation\">{</span>\n    display<span class=\"token punctuation\">:</span> <span class=\"token string\">'block'</span><span class=\"token punctuation\">,</span>\n    background<span class=\"token punctuation\">:</span> <span class=\"token string\">'red'</span><span class=\"token punctuation\">,</span>\n    opacity<span class=\"token punctuation\">:</span> <span class=\"token number\">1</span><span class=\"token punctuation\">,</span>\n    margin<span class=\"token punctuation\">:</span> <span class=\"token string\">'0 20px'</span><span class=\"token punctuation\">,</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> <span class=\"token function-variable function\">CustomNextArrow</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span>props<span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n    <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token spread\"><span class=\"token punctuation\">{</span><span class=\"token punctuation\">...</span><span class=\"token attr-value\">props</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>arrowStyle<span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>Icon</span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation\">=</span><span class=\"token punctuation\">\"</span>arrow-double-right<span class=\"token punctuation\">\"</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> <span class=\"token function-variable function\">CustomPrevArrow</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span>props<span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n    <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token spread\"><span class=\"token punctuation\">{</span><span class=\"token punctuation\">...</span><span class=\"token attr-value\">props</span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>arrowStyle<span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>Icon</span> <span class=\"token attr-name\">type</span><span class=\"token attr-value\"><span class=\"token punctuation\">=</span><span class=\"token punctuation\">\"</span>arrow-double-left<span class=\"token punctuation\">\"</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span>\n    <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>Slider</span> <span class=\"token attr-name\">nextArrow</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>CustomNextArrow</span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">prevArrow</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>CustomPrevArrow</span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">lazyLoad</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token punctuation\">{</span>\n            slides<span class=\"token punctuation\">.</span><span class=\"token function\">map</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">(</span>item<span class=\"token punctuation\">,</span> index<span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token attr-name\">key</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>index<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">className</span><span class=\"token attr-value\"><span class=\"token punctuation\">=</span><span class=\"token punctuation\">\"</span>slider-img-wrapper<span class=\"token punctuation\">\"</span></span><span class=\"token punctuation\">></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>img</span> <span class=\"token attr-name\">src</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>item<span class=\"token punctuation\">.</span>url<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">alt</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span>item<span class=\"token punctuation\">.</span>text<span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">)</span>\n        <span class=\"token punctuation\">}</span><span class=\"token plain-text\">\n    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>Slider</span><span class=\"token punctuation\">></span></span>\n    <span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div><style type=\"text/css\">.slider-img-wrapper img {\n    width: 100%;\n}</style><div class=\"highlight\"><pre class=\"language-css\"><code class=\"language-css\"><span class=\"token selector\">.slider-img-wrapper img</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token property\">width</span><span class=\"token punctuation\">:</span> 100%<span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span></code></pre></div>"}