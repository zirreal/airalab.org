<template>
  <LayoutEN>
    <MetaInfo
      :metaSiteName = "this.$static.metadata.siteNameEN"
      :metaTitle = "'Public blockchain stamp for data in your production'"
      :metaDescription = "'Use the service from NPO robotics research centre Airalab Rus “Blockchain stamp”: issue web3 digital certificates and product passports and increase confidence in your products or services.'"
    />

    <PageContent
      :title = "'Service Public blockchain stamp for data in your production'"
      :description = "'Use the service from NPO robotics research centre Airalab Rus “Blockchain stamp”: issue web3 digital certificates and product passports and increase confidence in your products or services.'"
      breadcrumb = "Our research"
      breadcrumbLink = "en/services"
      :button1 = "'Write to us'"
      :block1title = "'How it works'"
      :block1description = "'You have 2 options for issuing a digital blockchain certificate for your product or service:'"
      :block1opt1 = "'Manual issuance of a certificate by an operator in a pre-prepared decentralized application'"
      :block1opt2 = "'Issuing a certificate in the background automatically, based on data received from configured IoT devices'"

      :block2title = "'Cooperation scheme'"
      :block2step1 = "'Send sample data to create a blockchain stamp'"
      :block2step2 = "'Sign a contract with NPO robotics research centre Airalab Rus'"
      :block2step3 = "'Within a week you will issue your first certificate'"
      :block2button = "'Submit your application'"
      :block2buttonLink = "this.$static.metadata.formBlockchainStampEN"

      :block3title = "'Areas of application'"
      :block3opt1title = "'Asset tracking'"
      :block3opt1description = "'Monitoring compliance with the conditions of transportation and storage of products with increased requirements for conditions (vaccines, freezing, raw materials).'"
      :block3opt2title = "'Monitoring of equipment wear'"
      :block3opt2description = "'Control of operating conditions and warranty period of complex technical equipment based on data from IoT devices.'"
      :block3opt3title = "'Technical Data Sheet'"
      :block3opt3description = "'Keep the most important data for consumers and counterparties in the most confidential way.'"
      :block3opt4title = "'Carbon footprint compensation'"
      :block3opt4description = "'Attach the carbon footprint and trace off transaction data to your unique product identifier.'"

      :block4text = "'If you have any questions, please write to email'"
    />
  </LayoutEN>
</template>

<static-query>
  query {
    metadata {
      siteNameEN,
      formBlockchainStampEN
    }
  }
</static-query>

<script>
export default {
  components: {
    PageContent: () => import('~/components/PageServiceBlockchainStamp.vue'),
    MetaInfo: () => import('~/components/MetaInfo.vue')
  }
}
</script>