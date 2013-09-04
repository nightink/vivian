Vivian
======

Happy Birthday To Vivian


### base-data-render

#### 基础数据渲染组件---通用数据表格组件

#### 通用配置

```js
// schema 属性配置
[
    // 目前与数据处理模块商定，数据过滤完后默认添加_index属性，从1开始。
    {"name": "序号", "value": "{{_index}}", "width": 40, "fixed": true},
    // fixed表示是否固定列
    // click：表示有点击事件
    // tag：自定义标识，用户可能订阅默认事件，通过标识来判断
    // ob：触发事件的key（注意是冒号后面部分），若ob没有配置，使用默认事件key：base-data-render:click
    {"name": "名称", "value": "{{name}}", "width": 120, "fixed": true, "click": true, "ob": "observer.key"},
    {"name": "河流", "value": "{{szhl}}", "width": 100},
    // attr：添加到最近dom节点的属性，如：<td><span tip="时间:{{time}}">{{zkr}}</span></td>
    {"name": "容量", "value": "{{zkr}}", "width": 60, "over": true, attr: {"tip": "时间:{{time}}"},
    {"name": "水位", "value": "{{zcsw}}", "width": 60},
    {"name": "操作", "text": "基本信息", "width": 80, "click": true, "tag": "xq"}
]

/// data 扁平化数据
[
    {
        name: 福州,
        count: 10,
        data: [
            {
                name: 鼓楼,
                cout: 3,
                data: [
                    {
                        // 站点1
                    },
                    {
                        // 站点2
                    },
                    {
                        // 站点3
                    }
                ]
            },
            {
                // 站点4
            }
        ]
    }
    {
        // code.......
    }
]
```
-------------------------------------------------------------------------------
#### 成员

##### 属性

##### 方法

##### 事件

##### 公共事件
