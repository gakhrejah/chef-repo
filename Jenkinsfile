#!/usr/bin/groovy
/**
  * ROCC Jenkins Pipeline as a code by InfraDevOps
  * Author: Amit Patil, Saurabh Singhal and Neeraj Sharama
  * Function: pipeline as code fetches the shared library and start implementing the pipeline
  **/

/**
  * Importing the custom library before run by calling explicitly
  */
@Library('DevOps@RoccDevOpsFramework') _

node ('master'){
  def RUN_UNIT_TESTS = params.RUN_UNIT_TESTS
  def RUN_SONAR      = params.RUN_SONAR
  def RUN_FUNC_TESTS = params.RUN_FUNC_TESTS
  def Environment    = params.env
  def Deployment     = params.RUN_DEPLOYMENT
  def ZAP_TESTING    = params.ZAP_SECURITY_TESTING
  def JMET_TESTING   = params.JMET_PERF_TESTING

  ATG {
    JAVA_HOME        = "/usr/java/jdk1.8.0_73"
    MAVEN_HOME       = "/u02/opt/apache_maven/apache-maven-3.2.5"
    ANT_HOME         = "/u02/app/ci/ant/apache-ant-1.9.6"
    ZAP_HOME         = "/u02/app/ci/ZAP_2.6.0"
    EXEC_UNIT_TESTS  = RUN_UNIT_TESTS
    EXEC_SONAR       = RUN_SONAR
    EXEC_FUNC_TESTS  = RUN_FUNC_TESTS
    CURRENT_Env      = Environment
    EXEC_DEPLOYMENT  = Deployment	 
    EXEC_ZAP         = ZAP_TESTING
	EXEC_JMET		 = JMET_TESTING
  }
}


