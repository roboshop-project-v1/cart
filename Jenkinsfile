node('workstation'){
    print '************'
    sh 'env'
    print '******************'
    sh 'find .'
    print '*****************'
    stage("Compile Code"){
        print "Hello Compile "
    }
    stage("Test"){
        print "Hello test"
    }
    stage("Code Quality"){
        print "Heloo Quality"
        print env.BRANCH_NAME
    }
    if (env.BRANCH_NAME == 'main')
        {
            stage("code security"){
            print "Hello security"
            }
        }
    
    if (env.TAG_NAME !=~ '.*' )
        {
        stage("Release"){
            print " Release"
        }
    }
}