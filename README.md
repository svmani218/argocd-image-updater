# argocd-image-updater


time="2024-12-17T07:11:48Z" level=debug msg="found 2 from 4 tags eligible for consideration" image="docker.io/svmani218/elasticsearch:8.13.4"
time="2024-12-17T07:11:48Z" level=info msg="Setting new image to docker.io/svmani218/elasticsearch:8.14.2" alias=app application=root-app image_name=svmani218/elasticsearch image_tag=8.13.4 registry=docker.io
time="2024-12-17T07:11:48Z" level=debug msg="target parameters: image-spec= image-name=elasticsearch.image.repository, image-tag=elasticsearch.image.tag" application=root-app image=docker.io/svmani218/elasticsearch namespace=kube-argocd
time="2024-12-17T07:11:48Z" level=info msg="Successfully updated image 'docker.io/svmani218/elasticsearch:8.13.4' to 'docker.io/svmani218/elasticsearch:8.14.2', but pending spec update (dry run=false)" alias=app application=root-app image_name=svmani218/elasticsearch image_tag=8.13.4 registry=docker.io
time="2024-12-17T07:11:48Z" level=debug msg="Image 'svmani218/os-shell' seems not to be live in this application, skipping" application=root-app
time="2024-12-17T07:11:48Z" level=debug msg="Using commit message: build: automatic update of root-app\n\nupdates image svmani218/elasticsearch tag '8.13.4' to '8.14.2'\n"
time="2024-12-17T07:11:48Z" level=info msg="Committing 1 parameter update(s) for application root-app" application=root-app
time="2024-12-17T07:11:48Z" level=info msg="Initializing https://github.com/svmani218/argocd-image-updater.git to /tmp/git-root-app3342553816"
time="2024-12-17T07:11:48Z" level=info msg="git fetch origin main --force --prune --depth 1" dir=/tmp/git-root-app3342553816 execID=effcd
time="2024-12-17T07:11:49Z" level=info msg=Trace args="[git fetch origin main --force --prune --depth 1]" dir=/tmp/git-root-app3342553816 operation_name="exec git" time_ms=769.7528259999999
time="2024-12-17T07:11:49Z" level=info msg="git checkout --force main" dir=/tmp/git-root-app3342553816 execID=900e6
time="2024-12-17T07:11:49Z" level=info msg=Trace args="[git checkout --force main]" dir=/tmp/git-root-app3342553816 operation_name="exec git" time_ms=21.477987
time="2024-12-17T07:11:49Z" level=info msg="git clean -ffdx" dir=/tmp/git-root-app3342553816 execID=f888f
time="2024-12-17T07:11:49Z" level=info msg=Trace args="[git clean -ffdx]" dir=/tmp/git-root-app3342553816 operation_name="exec git" time_ms=9.373222
time="2024-12-17T07:11:49Z" level=debug msg="target parameter file and marshaled data are the same, skipping commit." application=root-app
time="2024-12-17T07:11:49Z" level=info msg="Successfully updated the live application spec" application=root-app
time="2024-12-17T07:11:49Z" level=info msg="Processing results: applications=1 images_considered=1 images_skipped=1 images_updated=1 errors=0"


 annotations:
    argocd-image-updater.argoproj.io/app-volume.helm.volumePermissions.image-name: elasticsearch.volumePermissions.repository
    argocd-image-updater.argoproj.io/app-volume.helm.volumePermissions.image-tag: elasticsearch.volumePermissions.tag
    argocd-image-updater.argoproj.io/app-volume.update-strategy: latest
    argocd-image-updater.argoproj.io/app.helm.image-name: elasticsearch.image.repository
    argocd-image-updater.argoproj.io/app.helm.image-tag: elasticsearch.image.tag
    argocd-image-updater.argoproj.io/git-branch: main
    argocd-image-updater.argoproj.io/image-list: app=docker.io/svmani218/elasticsearch:8.14.x-0,app-volume=docker.io/svmani218/os-shell:12-debian-x-0
    argocd-image-updater.argoproj.io/pullsecret: pullsecret:kube-argocd/dockerhub-secret
    argocd-image-updater.argoproj.io/write-back-method: git:secret:kube-argocd/repo-1102007070
    argocd-image-updater.argoproj.io/write-back-target: helmvalues:values.yaml
  creationTimestamp: "2024-12-16T04:58:51Z"
