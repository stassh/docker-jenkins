node {
    stage("Checkout") {
        echo 'Checkout stage'
    }

    stage("Verify Packages") {
        echo 'Verify stage'
    }

    stage("Build") {
        when {
            branch "master"
        }
        steps {
            echo 'Build stage'
        }
    }

    stage("Test") {
        when {
            branch "develop"
        }
        steps {
            echo 'Test stage'
        }
    }

    stage("Archive") {
        echo 'Archive stage'
    }
}
