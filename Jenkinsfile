pipeline {
 agent any  //环境maven、jdk等

 stages {  			//项目构建
  stage('pull code') { 	//拉取代码 
   steps {    	//具体实施步骤
    git pull 	// 拉取代码命令
   }
  }
  stage('build project') {		// 编译打包 
   steps {   		 	//具体实施步骤
    mvn clean package 	 	// 打包命令
   }
  }
  stage('publish project') { 		// 部署上线 
   steps {    		//具体实施步骤
    echo 'build is success' 	// 部署命令
   }
  }
 }
}
