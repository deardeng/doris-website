---
{
    "title": "QUARTERS_ADD",
    "language": "zh-CN"
}
---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

### Description
#### Syntax

`DATE/DATETIME QUARTERS_ADD(DATE/DATETIME date, INT years)`

对给定日期加上指定数量的季度

参数 `date` 可以是 `DATETIME` 或者 `DATE` 类型，返回类型与参数 `date` 的类型一致。

### Example

```sql
mysql> select quarters_add("2020-01-31 02:02:02", 1);
+---------------------------------------------------------------+
| quarters_add(cast('2020-01-31 02:02:02' as DATETIMEV2(0)), 1) |
+---------------------------------------------------------------+
| 2020-04-30 02:02:02                                           |
+---------------------------------------------------------------+
1 row in set (0.10 sec)
```

### keywords
  QUARTERS, ADD, QUARTERS_ADD