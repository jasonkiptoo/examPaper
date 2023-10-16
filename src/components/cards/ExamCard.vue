<template>
  <q-card>
    <q-card-section>
      <div class="row">
        <div class="col">
          <h6 class="qt">
            <a
              href="https://www.kenyaplex.com/exams/1822-form-4-drawing--design-paper-2-end-of-term-2-examination-2023.aspx"
            >
              Form 4 Drawing & Design Paper 2 End of Term 2 Examination 2023
            </a>
          </h6>
          <p class="qa">
            Download Form 4 Drawing & Design Paper 2 End of Term 2 Examination
            2023. This exam document has the question paper and its marking
            scheme in both PDF and Word formats.
          </p>
          <input
            type="hidden"
            name="ctl00$ContentPlaceHolder1$lvQuestions$ctrl0$hiddenID"
            id="ContentPlaceHolder1_lvQuestions_hiddenID_0"
            value="1822"
          />
          <p class="qa">
            High School, Form 4, Drawing and Design, Term 2, 2023
          </p>
          <p>
            <span
              id="ContentPlaceHolder1_lvQuestions_lblPrice_0"
              style="color: Green; font-size: 14px; font-weight: bold"
            >
              Price: KES: 50
            </span>
          </p>
          <div class="col-auto">
            <q-btn
              class="btn1"
              icon="cloud_download"
              label="Download"
              color="primary"
              @click="redirectToLink"
            />
          </div>
          <!-- Uncomment the following section if you want to display the date posted -->
          <!--
          <p class="qs">
            Date posted: <span class="c-green">July 25, 2023</span>.
          </p>
          -->
        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  methods: {
    redirectToLink() {
      window.location.href =
        "https://www.kenyaplex.com/exams/1822-form-4-drawing--design-paper-2-end-of-term-2-examination-2023.aspx";
    },
  },
};
</script>
