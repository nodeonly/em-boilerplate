# em-boilerplate

express + mongodb 

## npm 

这里放一些常用的npm，以及好的实践

### 测试

http://www.infoq.com/cn/news/2012/06/nodejs-mongo-app-autotest

- mocha
- chai
- sinon（Standalone test spies, stubs and mocks for JavaScript.）
- 页面事件模拟zombie(Zombie.js is a lightweight framework for testing client-side JavaScript code in a simulated environment. No browser required.)
- 接口测试supertest(Super-agent driven library for testing node.js HTTP servers using a fluent API)


```
npm install --save-dev mocha
npm install --save-dev chai
npm install --save-dev sinon
npm install --save-dev supertest
npm install --save-dev zombie
```

## 相关网址

- https://github.com/mochajs/mocha
- https://github.com/chaijs/chai
- http://chaijs.com/
- http://mochajs.org/
- http://sinonjs.org/
- http://zombie.labnotes.org/
- passportjs.org认证中间件
- https://github.com/madhums/node-express-mongoose 参考
- nodemon非常实用的工具,用来监控你 node.js 源代码的任何变化和自动重启你的服务器
- https://github.com/tj/supertest（api test文档）
- https://github.com/tj/superagent/blob/master/test/node/agency.js（api test示例）



## api

http://chaijs.com/guide/styles/#should


	should.exist
	should.not.exist
	should.equal
	should.not.equal
	should.Throw
	should.not.Throw
	
	
	var should = require('chai').should() //actually call the the function
	  , foo = 'bar'
	  , beverages = { tea: [ 'chai', 'matcha', 'oolong' ] };

	foo.should.be.a('string');
	foo.should.equal('bar');
	foo.should.have.length(3);
	beverages.should.have.property('tea').with.length(3);
