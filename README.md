china-city-select
=================

简单可用的中国省份、城市、县区三级联动选择组件

![china-city-select](http://ww2.sinaimg.cn/mw690/831e9385jw1e60hh9sc2zj207q05kjrh.jpg)

原作者及项目地址：[http://blog.hpyer.cn/codes/js-auto-change-city-list](http://blog.hpyer.cn/codes/js-auto-change-city-list)

##使用说明

```javascript
var options = {
    country: 'country', //省级select ID
	state: 'state',     //市级select ID
	city: 'city',       //县区级select ID
	current: '',        //初始化时3个select的默认值，使用region code及 | 区分，如「 01|02|33 」，具体请查阅 xml 数据文件
	language: 'zh_cn',  
	path_to_xml: '',    //xml文件所在的地址
	read_only: false  
}

LocalList.mf_init(options);
```

##修改说明

原作者的代码会生成新的 3 个 select，不支持直接给已有的 select 绑定事件，因此拿来做了小小的改动支持上述特性。
