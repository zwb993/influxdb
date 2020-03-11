# influxdb
### where语句
- 在WHERE子句中，如果是string类型的field value，一定要用单引号括起来，tag同理。
如果不适用引号括起来，或者使用的是双引号，将不会返回任何数据，有时甚至都不报错！！！例如：
```sql
select * from sensor_history where "kks"='4DCS.40CFB41GH0' limit 10
```
