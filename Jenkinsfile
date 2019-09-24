pipeline
{
	agent any
	stages{
		stage('Upload to AWS'){
			steps{
            			withAWS(region:'us-west-2',credentials:'AKIAUO64LQLX4BSMMTZL') {
                			s3Upload(bucket:'staticwebarik', file:'index.html', path:'/index.html');
            			}
			}
		}
	}
}
