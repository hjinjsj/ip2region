# nodejs 客户端

## 实现情况：

现已实现同步和异步查询，具体使用方法可以参考 `nodejs\tests\constructorTest.spec.js` 和`nodejs\tests\createTest.spec.js`。

## 如何贡献？

你可以任意修改代码，但必须确保通过全部的单元测试。要保证通过全部的单元测试，请在 Nodejs 控制台下切换到 nodejs 目录：

1）在此之前，请先运行 `npm i` 确保你已经安装了各类初始化第三方工具。
2）然后运行 `npm run coverage` 确保你的代码可以通过全部测试（必要时可以添加测试），同时保证代码覆盖率都是绿色（80%以上）。

```bash
D:\Projects\ip2region\binding\nodejs>npm run coverage

> ip2region@0.0.1 coverage D:\Projects\ip2region\binding\nodejs
> npm run test && jest --coverage


> ip2region@0.0.1 test D:\Projects\ip2region\binding\nodejs
> jest

 PASS  tests\constructorTest.spec.js
 PASS  tests\createTest.spec.js
 PASS  tests\exceptionTest.spec.js

Snapshot Summary
 › 168 snapshots written in 2 test suites.

Test Suites: 3 passed, 3 total
Tests:       14 passed, 14 total
Snapshots:   168 added, 168 total
Time:        1.645s
Ran all test suites.
 PASS  tests\constructorTest.spec.js
 PASS  tests\createTest.spec.js
 PASS  tests\exceptionTest.spec.js
----------------------|----------|----------|----------|----------|-------------------|
File                  |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
----------------------|----------|----------|----------|----------|-------------------|
All files             |    92.34 |    80.77 |       96 |    93.83 |                   |
 nodejs               |    91.95 |    80.26 |    95.65 |    93.51 |                   |
  ip2region.js        |    91.95 |    80.26 |    95.65 |    93.51 |... 09,410,460,484 |
 nodejs/tests/utils   |      100 |      100 |      100 |      100 |                   |
  asyncFor.js         |      100 |      100 |      100 |      100 |                   |
  fetchMainVersion.js |      100 |      100 |      100 |      100 |                   |
  testData.js         |      100 |      100 |      100 |      100 |                   |
----------------------|----------|----------|----------|----------|-------------------|

Test Suites: 3 passed, 3 total
Tests:       14 passed, 14 total
Snapshots:   168 passed, 168 total
Time:        1.792s
Ran all test suites.
```