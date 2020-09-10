# Google Store Analytics Transactions Revenue Prediction

### Problem Statement:

The 80/20 rule has proven true for many businesses, only a small percentage of customers produce most of the revenue. 
Understanding how much each customer spends will allow companies to place actionable operations 
to better allocate their 
marketing budgets.

### Objective:

Predict a how much GStore customer will spend. In addition, to predict the natural log of the sum of all transactions per user.

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <msub>
    <mi>y</mi>
    <mrow class="MJX-TeXAtom-ORD">
      <mi>u</mi>
      <mi>s</mi>
      <mi>e</mi>
      <mi>r</mi>
    </mrow>
  </msub>
  <mo>=</mo>
  <munderover>
    <mo>&#x2211;<!-- ∑ --></mo>
    <mrow class="MJX-TeXAtom-ORD">
      <mi>i</mi>
      <mo>=</mo>
      <mn>1</mn>
    </mrow>
    <mrow class="MJX-TeXAtom-ORD">
      <mi>n</mi>
    </mrow>
  </munderover>
  <mi>t</mi>
  <mi>r</mi>
  <mi>a</mi>
  <mi>n</mi>
  <mi>s</mi>
  <mi>a</mi>
  <mi>c</mi>
  <mi>t</mi>
  <mi>i</mi>
  <mi>o</mi>
  <msub>
    <mi>n</mi>
    <mrow class="MJX-TeXAtom-ORD">
      <mi>u</mi>
      <mi>s</mi>
      <mi>e</mi>
      <msub>
        <mi>r</mi>
        <mi>i</mi>
      </msub>
    </mrow>
  </msub>
</math>

target_{user} = \ln({y_{user}+1})

### Data:

- fullVisitorId- A unique identifier for each user of the Google Merchandise Store.
- channelGrouping - The channel via which the user came to the Store.
- date - The date on which the user visited the Store.
- device - The specifications for the device used to access the Store.
- geoNetwork - This section contains information about the geography of the user.
- socialEngagementType - Engagement type, either "Socially Engaged" or "Not Socially Engaged".
- totals - This section contains aggregate values across the session.
- trafficSource - This section contains information about the Traffic Source from which the session originated.
- visitId - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.
- visitNumber - The session number for this user. If this is the first session, then this is set to 1.
- visitStartTime - The timestamp (expressed as POSIX time).
- hits - This row and nested fields are populated for any and all types of hits. Provides a record of all page visits.
- customDimensions - This section contains any user-level or session-level custom dimensions that are set for a session. This is a repeated field and has an entry for each dimension that is set.
- totals - This set of columns mostly includes high-level aggregate data.


 
