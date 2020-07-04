# Code Review Guide

## Things to do before you start reviewing the PR

* Make sure you are familiar with the packages the PR modifies. //熟悉修改的包

* Make sure you have enough continuous time to review the PR, use 300 LOC per hour to estimate.  //保证时间, 每小时300行

* Make sure you can follow the updates of the PR in the next few work days. 保持追踪

* Read the description of the PR, if it's not easy to understand, ask the coder to improve it. // 描述是易读的

* For a bug fix PR, if there is no test case, ask the coder to add tests.  修复 bug,必须要有测试用例

* For a performance PR, if no benchmark result is provided, ask the coder to add a benchmark result.  性能优化,必须要有性能对比


## Things to check during the review process

* Am I able to understand the purpose of each unit test? 理解每个单元测试的目的

* Do unit tests actually test that the code is performing the intended functionality?  测试功能是否到位  

* Do unit tests cover all the important code blocks and specially handled errors?  代码覆盖全

* Could procedure tests be rewritten to table driven tests? 表格驱动测试

* Is the code written following the style guide? 代码规范

* Is the same code duplicated more than twice? 重复代码

* Do comments exist and describe the intent of the code? 注释

* Are hacks, workarounds代替方法 and temporary fixes临时修复 commented 添加了注释? 

* Does this function do more than the name suggests? 功能超过 name 含义

* Can this function's behavior be inferred by its name? name含义准确

* Do tests exist and are they comprehensive?  有测试, 并且全面

* Do unit tests cover all the important code branches? 测试 cover 全面

* Could the test code be extracted into a table-driven test? 表格驱动测试


## Things to keep in mind when you are writing a review comment 写审核评论

* Be kind to the coder, not to the code. 别骂人,怼代码

* Ask questions rather than make statements. 问问题而不是陈述

* Treat people who know less than you with respect, deference 顺从, and patience. 对比自己无知的人 

* Remember to praise when the code quality exceeds your expectation. 鼓励表扬

* It isn't necessarily wrong if the coder's solution is different than yours. 不同不是错误

* Refer to the code style document when necessary. 参考代码规范


## Things to remember after you submitted the review comment

* Checkout Github notification regularly to keep track of the updates of the PR. 检查通知, 持续跟踪

* When the PR has been updated, start another round of review or give it a LGTM. Looks Good To Me
