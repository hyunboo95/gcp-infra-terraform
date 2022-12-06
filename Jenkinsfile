#!groovy

pipeline {
    //선언적 문법의 코드
    agent any
    // 파이프라인 혹은 스테이지를 실행하기 위해 사용할 노드를 지정
    // agent 디렉티브에 명시한 매개변수는 젠킨스 시스템에 존재하는 노드의 label을 찾아가서 연결

    stages {
        // 파이프라인의 중심 로직을 정의하는 개별 stage들을 묶은 것.
        stage("Git checkout") {
            steps {
                script {
                    checkout scm
                    echo "=================checkout scm================="
                }
            }
        }
        // stage("Environment Select") {
        //     steps {
        //         script {
        //             if(BRANCH_NAME == 'stage'){
        //                 env.stagechk = "STG"
        //             }else if(BRANCH_NAME == 'master'){
        //                 env.stagechk = "PRD"
        //             }else if(BRANCH_NAME == 'master'){
        //                 env.stagechk = "PRD"
        //             }
        //         }
        //     }
        // }
    }
}