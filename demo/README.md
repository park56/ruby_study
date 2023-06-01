# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version
3.7.4
* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

<h1> [명령어 모음] </h1>
mac에는 기본적으로 ruby가 설치되어 있음.

gem update --system

gem install rails

rails new [프로젝트이름]

cd [프로젝트이름]

// 뭔갈 설치하면 다시  해야함
bundle install
bundle

rails server 

// 실행 폴더 안에서
rails console
    - Post.first
    - Post.create! title: "제목", content: "내용"

// Action Text 설치. 다양한 텍스트 에디터를 쉽게 통합해 애플리케이션에서 리치 텍스트(이미지, 동영상, 서식 있는 텍스트 등)를 다룰 수 있도록 도와준다.
rails action_text:install
// 모델과 생성자에 따라 db 생성
rails db:migrate

// generate 모델 설치
rails generate scaffold post title:string content:text

// 다른 모듈을 사용하고 싶을 떄 
./bin/importmap pin local-time --download

// rails에서 commment 모델과 리소스에 대한 생성자를 만드는 명령어
rails g resource comment post:references content:text 