#  사용하는 방법 
## 실행 

이것은 원본의 `house-sitter2` 앱을 Meteor Version 1.4.2.1로 수정해 본 것이다. 


이 깃저장소를 클론닝 한 이후에 다음과 같이 시행한다.


    $ git clone https://github.com/koseokbum/chap7_workoutTracker_1.3.git

그리고 해당 앱 디렉터리로 이동한 다음, 다음을 실행한다.


    $ meteor npm install
    $ meteor remove autopublish
    $ meteor remove insecure
    $ meteor add acccounts-ui
    $ meteor add accounts-password
    $ meteor add audit-argument-checks
    $ meteor run


## 원본과 비교하여 수정한 부분들 

- 앱의 전반적인 패턴은 책의 앞 부분 부록에 실린 `imports` 디렉터리를 만들어 사용하는 패턴을 따랐다. `api` 서브디렉터리에서 컬렉션을 정의하였고, `ui` 디렉터리에서 UI를 정의하였다.  

- 원본의 `fixtures.js`를 `main.js`로 옮겨 놓았다. 디폴트 앱에 있는 `Meteor.startup()` 부분을 ES2015의 애로우 함수(arrow function)을 사용하지 않고 클래식한 패턴을 따랐다. 

- 필요한 패키지들을 필요한 부분에서 임포트하였다. 





