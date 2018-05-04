<template>
  <section>
    <v-layout column wrap class="my-5" align-center>
      <v-flex xs12 class="blue lighten-5">
        <v-container grid-list-xl>
          <v-layout row wrap align-start>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">color_lens</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">기획 파트</div>
                </v-card-title>
                <v-card-text>
                  - 아이디어 디벨롭핑 시간을 통해 본인의 아이디어를 발전시키고 기획안을 완성하는 것을 목표로 합니다.
                  <br> - 디자인 및 개발파트와의 협업을 위해 필요한 정보를 습득합니다.
                  <br> - 기획자이자 프로젝트 매니저로서의 역할 수행이 가능하도록 합니다.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">flash_on</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">디자인 파트</div>
                </v-card-title>
                <v-card-text>
                  - 매주 세미나에서의 강연과 실습을 통해 UI/ UX에 관련하여 디자이너가 알아야 할 개념을 숙지합니다.
                  <br>- 이를 디자인 툴로 적용할 수 있는 것을 목표로 합니다.
                  <br>- 개발자와의 수월한 소통을 위하여 사용되는 협업툴에 관련된 스터디를 진행합니다.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">build</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">안드로이드 파트</div>
                </v-card-title>
                <v-card-text>
                  - 안드로이드 스튜디오를 이용해 기초적인 네이티브 어플리케이션 제작 방법에 대해서 배웁니다.
                  <br>- API 사용법 및 통신에 대해서 배웁니다.
                  <br>- 기초적인 어플리케이션의 디자인 방법에 대해 배웁니다.
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-flex>
      <v-flex xs12>
        <v-container grid-list-xl>
          <v-layout row wrap align-start>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">color_lens</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">서버 파트</div>
                </v-card-title>
                <v-card-text>
                  - Node.js를 이용해 AWS상에서 서버를 구성하는 방법을 배워봅니다.
                  <br> - 클라이언트와 서버, DB 사이의 연동과정을 이해하고 구성합니다.
                  <br> - 코딩뿐만 아니라 ERD 설계, API Reference 작성 등 프로젝트에서 백엔드를 담당하여 진행하는 과정 전체를 경험합니다.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">flash_on</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">iOS 파트</div>
                </v-card-title>
                <v-card-text>
                  - Xcode(통합개발환경)와 Swift를 이용해 iOS 어플리케이션 프로그래밍을 배웁니다.
                  <br> - Interface builder를 이용한 레이아웃 구성 및 네트워크 통신 방법에 대해 배웁니다.
                  <br> - 매주 실습 세미나를 통해 iOS개발 기초부터 심화까지 1인 1앱 개발을 목표로 공부합니다.
                  <br> - Open API 사용법을 숙지합니다.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="blue--text text--lighten-2">build</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">Web Front-End 파트</div>
                </v-card-title>
                <v-card-text>
                  - 기본적인 HTML, CSS 부터 컴포넌트 기반 웹 개발에 대해서 배웁니다.
                  <br> - 매주 실습 세미나를 통해 Vue.js의 기초부터 심화까지 공부합니다.
                  <br> - API 사용법 및 통신에 대해서 배웁니다.
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
  export default {

  }

</script>
