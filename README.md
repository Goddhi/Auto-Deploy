

cd .circleci/files
aws cloudformation deploy \
            --template-file cloudfront.yml \
            --stack-name InitialStack \
            --parameter-overrides WorkflowID=232348374 \
            --tags project=udapeople            

DB instance identifier
udapeople222
password: udapeople123
master username: postgres
Database name: udapeople222

pg_isready -d udapeople222 -h udapeople222.c8q6tnhxjlco.us-east-1.rds.amazonaws.com -p 5432 -U postgres