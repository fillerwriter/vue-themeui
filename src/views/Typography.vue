<template>
  <section class="l-content">
    <h2>Typography</h2>
    <p>Set the values associated with your chosen fonts.</p>
    <div class="c-panel">
      <h2>Graphik</h2>
      <p>Regular, Bold</p>
      <hr />
      <h3>Line Heights</h3>
      <div class="flex margin-lg">
        <res-input
          ><label>Tight</label
          ><input
            type="text"
            :placeholder="lineHeight.tight"
            v-model="lineHeight.tight"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:24px;"
          v-bind:style="{ lineHeight: lineHeight.tight }"
          >This line height applies to larger font sizes, such as those used in
          headlines. Here's some sample text for you to test this value. Let's
          use this example text to also tell the user how this works</span
        >
      </div>
      <div class="flex margin-lg">
        <res-input
          ><label>Medium</label
          ><input
            type="text"
            :placeholder="lineHeight.medium"
            v-model="lineHeight.medium"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:16px;"
          v-bind:style="{ lineHeight: lineHeight.medium }"
          >This line height applies to medium font sizes. Here's some sample
          text for you to test this value. Lorem ipsum dolor sit amet,
          consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
          labore et dolore magna aliqua.</span
        >
      </div>
      <div class="flex margin-lg">
        <res-input
          ><label>Loose</label
          ><input
            type="text"
            :placeholder="lineHeight.loose"
            v-model="lineHeight.loose"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:12px;"
          v-bind:style="{ lineHeight: lineHeight.loose }"
          >This line height applies to small font sizes. Here's some sample text
          for you to test this value. Lorem ipsum dolor sit amet, consectetur
          adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
          magna aliqua.</span
        >
      </div>
      <div class="flex margin-lg">
        <res-input
          ><label>Body</label
          ><input
            type="text"
            :placeholder="lineHeight.body"
            v-model="lineHeight.body"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:16px;"
          v-bind:style="{ lineHeight: lineHeight.body }"
          >This line height applies to the body copy in an article, which we
          think is a little different than other text. Here's some sample text
          for you to test this value.</span
        >
      </div>
      <h3>Letterspacing</h3>
      <div class="flex margin-lg">
        <res-input
          ><label>Default</label
          ><input
            type="text"
            :placeholder="letterSpacing.default"
            v-model="letterSpacing.default"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:16px;"
          v-bind:style="{ letterSpacing: letterSpacing.default }"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.</span
        >
      </div>
      <div class="flex margin-lg">
        <res-input
          ><label>Caps</label
          ><input
            type="text"
            :placeholder="letterSpacing.caps"
            v-model="letterSpacing.caps"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:12px;text-transform:uppercase;"
          v-bind:style="{ letterSpacing: letterSpacing.caps }"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.</span
        >
      </div>
      <div class="flex margin-lg">
        <res-input
          ><label>Expressive</label
          ><input
            type="text"
            :placeholder="letterSpacing.expressive"
            v-model="letterSpacing.expressive"/></res-input
        ><span
          class="c-typography-text"
          style="font-size:16px;"
          v-bind:style="{ letterSpacing: letterSpacing.expressive }"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.</span
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Typography",
  data: () => ({
    lineHeight: {
      tight: 1.1,
      medium: 1.3,
      loose: 1.5,
      body: 1.7
    },
    letterSpacing: {
      default: "0",
      caps: ".04em",
      expressive: ".02em"
    }
  })
};
</script>

<style scoped></style>
