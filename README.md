{
    "AWSTemplateFormatVersion": "2010-09-09",
    "Description": "A template is for creating lambda from s3 buckets",
    "Resources": {
        "LambdaFunResource": {
            "Type": "AWS::Lambda::Function",
            "Properties": {
                "FunctionName": "Srirangam",
                
                "Code": {
        "S3Bucket" : "abcdefgd",
        "S3Key" : "index.zip"
      },
                "Description": "Used to run job",
                "Handler": "index.lambda_handler",
                "Role": "arn:aws:iam::13015229333333455024:role/lambda_basic_execution",
                "Runtime": "python3.6",
                "Timeout": 120
            }
        }
  }
}

