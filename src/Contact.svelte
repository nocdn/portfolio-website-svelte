<script>
  import MailChip from "./lib/MailChip.svelte";
  import SocialChip from "./lib/SocialChip.svelte";

  import ContentHeader from "./lib/ContentHeader.svelte";

  import MorphingText from "./lib/MorphingText.svelte";
</script>

<contact class="flex flex-col gap-12 motion-opacity-in-0">
  <ContentHeader title="You can reach me on">
    {#snippet customElement()}
      <MorphingText />
    {/snippet}
  </ContentHeader>
  <div id="contact-chip-grid" class="flex flex-col gap-7">
    <div class="grid grid-cols-2 gap-3">
      <SocialChip
        socialIcon="github"
        primaryColor="#EFDFFC"
        backgroundColor="#FCF3FF"
        textColor="#8A24DF"
        link="github.com/nocdn"
      />
      <SocialChip
        socialIcon="linkedin"
        primaryColor="#E0E1FD"
        backgroundColor="#F4F4FF"
        textColor="#2E38F1"
        link="linkedin.com/in/bartosz-bak-2b8a1b1b3/"
      />
      <SocialChip
        socialIcon="instagram"
        primaryColor="#FCE0F8"
        backgroundColor="#FFF5FE"
        textColor="#DD20BA"
        link="instagram.com/bartek_front/"
      />
      <SocialChip
        socialIcon="twitter"
        primaryColor="#DEEDFF"
        backgroundColor="#F4F9FF"
        textColor="#217EE0"
        link="x.com/AKBB071"
      />
    </div>
    <p class="font-geist">Or, most directly through e-mail</p>
    <div class="grid">
      <MailChip />
    </div>
  </div>
</contact>
