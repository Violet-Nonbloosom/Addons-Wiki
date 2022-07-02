# 研究

在`/plugins/SlimeCustomizer/researches.yml`中，你可以配置研究。

!> 该功能为汉化版特有功能

每一项都代表一个研究。

```yaml
example_research:
  id: 10086
  name: "示例研究"
  cost: 34
  items:
    - EXAMPLE_ITEM
    - EXAMPLE_MACHINE
```

| 内容 | 描述 |
| -------- | -------- |
| `example_research` | 研究的key，每个研究的key不能相同。<br>**仅支持小写字母、数字、下划线!** |
| id | 研究的数字ID，最大为 2147483647。 |
| cost | 解锁研究所需要的经验等级。 |
| items | 研究所包含的物品列表。必须为粘液科技物品ID。 |

!> 目前粘液科技的研究系统仍依赖数字id进行研究的识别，本体和附属的研究都会使用该数字ID。因此，建议将数字ID设置为其他附属不太会用到的范围。