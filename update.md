# plab v2 升级说明

## 0. 权限控制

考虑把 `DataV` `用户、菜单、权限` 复制过来用

## 1. 计划

### 1.1 新增 - 常量定义 - 部门所属

### 1.2 更新 - 常量定义 - 计划状态

- 对比

代码 | 名称 | 代码-v2 | 名称-v2
-----|------|------|------
1      | 未审核    | 1    | xxx
2      | 审核中    | 2    | 待审核
3      | 进行中    | 3    | 进行中
4      | 已驳回    | 4    | 已驳回
5      | 已完成    | 5    | 已完结
6      | 已延期    | 6    | 已延期
       |          | 7    | 已关闭
       |          | 8    | 已作废
       |          | 9    | 完结待审核

### 1.3 更新 - 计划

- 作废 `post_type`
- 新增 `部门所属 department_id`
- 新增 `附件id attachment_id`
- 新增 `驳回说明 reject_description`

## 2. 项目

### 2.1 新增 - 常量定义 - 项目业务线

### 2.2 更新 - 常量定义 - 项目状态

同计划状态

### 2.3 更新 - 项目

- 作废 `post_type`
- 新增 `项目业务线id business_type_id`
- 新增 `包含新模块 has_course_new_module`
- 新增 `新模块 course_new_modules`
- 新增 `质检验收人 qc_manager_id`
- 新增 `驳回说明 reject_description`
- 新增 `项目实际开始时间 actual_begin_date`
- 新增 `项目实际结束时间 actual_end_date`
- 新增 `项目总系数 project_rates`

### 2.4 新增 - 基础数据 - 部门学科

### 2.5 新增 - 项目 - 项目信息统计

### 2.6 新增 - 项目 - 计划侧栏导航

## 3. 任务

### 3.1 更新 - 任务 - 任务列表

- 新增 `实际开始 actual_begin_date`
- 新增 `实际结束 actual_end_date`
- 新增 `预估结果系数 estimate_result_weight`
- 新增 `实际结果系数 actual_result_weight`

### 3.2 更新 - 任务 - 任务完成 | 任务详情

- 新增 `差异说明 results.difference_desc`

## 4. 权限、权限点

### 4.1 新增 - 用户管理

### 4.2 新增 - 菜单管理

### 4.3 新增 - 权限组管理