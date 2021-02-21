# aws_codebuild_codedeploy_nodeJs_demo
This repository contains sample codes to work with AWS 

This Project build_script directory contains build related script, check buildspec.yml file I have integrated the same. 

Deployment related scripts are in deployment_scripts directory, check appspec.yml file. 


This is a node.js project same, but change config as per your project requirement 


In codebuild.yml file in post build phase, line:
      - aws deploy push --application-name "${CODE_DEPLOY_APPLICATION_NAME}" --s3-location "s3://${CODE_DEPLOY_S3_BUCKET}/codedeploydemo/app.zip" --ignore-hidden-files --region us-west-2

You can enavironment variable in code build : CODE_DEPLOY_APPLICATION_NAME, CODE_DEPLOY_S3_BUCKET and the value will reflect in the command. 

Check Previous Videos to make sense of this implementation:

AWS CodeCommit (Ep.1): https://www.youtube.com/watch?v=0649R_Fk9_E

AWS CodeBuild (Ep.2): https://www.youtube.com/watch?v=rxZniDstaa

AWS CodeDeploy(Ep.3): https://www.youtube.com/watch?v=mtby2y2aSeU

Keep learning , Keep improving 
