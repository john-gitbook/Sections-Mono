---
cover:
  light: ../.gitbook/assets/CleanShot 2026-05-20 at 09.33.31@2x.png
  dark: ../.gitbook/assets/CleanShot 2026-05-20 at 09.33.31@2x.png
coverY: -19.445314947042384
coverHeight: 371
layout:
  width: wide
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
---

# Accordion

{% tabs %}
{% tab title="Usage" %}
An accordion is a vertically stacked list of headers that reveal or hide associated sections of content.

* [Live demo](https://carbondesignsystem.com/components/accordion/usage/#live-demo)
* [Overview](https://carbondesignsystem.com/components/accordion/usage/#overview)
* [Formatting](https://carbondesignsystem.com/components/accordion/usage/#formatting)
* [Content](https://carbondesignsystem.com/components/accordion/usage/#content)
* [Behaviors](https://carbondesignsystem.com/components/accordion/usage/#behaviors)
* [Related](https://carbondesignsystem.com/components/accordion/usage/#related)
* [References](https://carbondesignsystem.com/components/accordion/usage/#references)
* [Feedback](https://carbondesignsystem.com/components/accordion/usage/#feedback)

### Live demo <a href="#live-demo" id="live-demo"></a>

Theme selector

This live demo contains only a preview of functionality and styles available for this component. View the [full demo](https://react.carbondesignsystem.com/?path=/story/components-accordion--default\&globals=theme:white) on Storybook for additional information such as its version, controls, and API documentation.

#### Accessibility testing status <a href="#accessibility-testing-statusobject-objectobject-object" id="accessibility-testing-statusobject-objectobject-object"></a>

[**Default state**Tested](https://carbondesignsystem.com/components/accordion/accessibility/#accessibility-testing-status)[**Advanced states**Tested](https://carbondesignsystem.com/components/accordion/accessibility/#accessibility-testing-status)[**Screen reader**Manually tested](https://carbondesignsystem.com/components/accordion/accessibility/#accessibility-testing-status)[**Keyboard navigation**Tested](https://carbondesignsystem.com/components/accordion/accessibility/#accessibility-testing-status)

### Overview <a href="#overview" id="overview"></a>

The accordion component delivers large amounts of content in a small space through progressive disclosure. The header title gives the user a high level overview of the content allowing the user to decide which sections to read.

Accordions can make information processing and discovering more effective. However, it does hide content from users and it’s important to account for a user not noticing or reading all of the included content.

#### When to use <a href="#when-to-use" id="when-to-use"></a>

* To organize related information.
* To shorten pages and reduce scrolling when content is not crucial to read in full.
* When space is at a premium and long content cannot be displayed all at once, like on a mobile interface or in a side panel.

#### When not to use <a href="#when-not-to-use" id="when-not-to-use"></a>

* When organizing large amounts of information that can be nested, consider using [tree view](https://carbondesignsystem.com/components/tree-view/usage) instead.
* If a user is likely to read all of the content, then don’t use an accordion as it adds the burden of an extra click; instead use a full scrolling page with normal headers.

### Formatting <a href="#formatting" id="formatting"></a>

#### Anatomy <a href="#anatomy" id="anatomy"></a>

![accordion anatomy](https://carbondesignsystem.com/static/ae35a758a11df1aac5e36b906bdba7ee/3cbba/accordion-anatomy.png)

1. **Header**: contains the section title and is control for revealing the panel.
2. **Icon**: indicates if the panel is open or closed.
3. **Panel**: the section of content associated with an accordion header.

#### Alignment <a href="#alignment" id="alignment"></a>

**Flush alignment**

Use flush alignment when designing within smaller spaces on a page such as side panels or sidebars to achieve better text alignment with other content. Flush alignment is also used to help avoid converging rule lines between components that are close to each other on a page.

![accordion flush alignment](https://carbondesignsystem.com/static/d8180944f68f06c4d7091008e5a2e145/3cbba/accordion-flush.png)

Flush alignment places the row title and chevron icons with 0px padding, keeping them flush to the rule dividers. For hover and focus interactive states, the left and right padding receives an additional 16px padding.

![accordion flush alignment spec](https://carbondesignsystem.com/static/5b32620155b0e5e770a8478f9504075f/3cbba/accordion-flush-spec.png)

**Icon alignment**

By default the chevron icon is placed on the `end` side of the header. This allows for the title on the `start` side to align with other type elements in the layout, which is the preferred alignment scenario.

However, in some rare scenarios, the accordion may be modified to place the icon in `start` front of the title to function more like a tree. Most instances should use the default `end` alignment, especially for any pure content or documentation purposes. Icon placement in accordions should be consistent throughout your page and should not alternate.

![Do use the default end icon alignment to keep accordion text aligned with other content on the page.](https://carbondesignsystem.com/static/46032636069a150c17ff78d873d0f821/a5df1/accordion-alignment-do.png)

In most cases, use the default end icon alignment to keep accordion text aligned with other content on the page.

![Do place icons on the start side for tree like functionality.](https://carbondesignsystem.com/static/5550cbceec4c21d9c318346df63198ef/a5df1/accordion-alignment-do-2.png)

In rare cases, you can place icons on the start side for tree like functionality.

#### Placement <a href="#placement" id="placement"></a>

Accordions can be placed with main page content or placed inside of a container such as a side panel or tile.

![accordion placement](https://carbondesignsystem.com/static/8c15d04534079e729403fa13ceea31a9/3cbba/accordion-placement-2.png)

**Grid placement**

When placing an accordion on the 2x Grid with its default alignment, the indented title and content align to the grid columns, and the top and bottom borders hang into the gutter. However, the accordion can be modified to have a [flush alignment](https://carbondesignsystem.com/components/accordion/usage#alignment) where the titles and content are instead flush aligned with the top and bottom borders having 0px padding.

![accordion grid placement](https://carbondesignsystem.com/static/c2ebd73fe035bfdb41a1c57e42a4c4f3/3cbba/accordion-placement-1.png)

### Content <a href="#content" id="content"></a>

#### Main elements <a href="#main-elements" id="main-elements"></a>

**Title**

* The title should be as brief as possible while still being clear and descriptive.
* Each title should be wrapped in a [role heading](https://www.w3.org/TR/wai-aria-practices-1.1/#wai-aria-roles-states-and-properties) (h1-h6) that is appropriate for the information architecture of the page.

**Body copy**

* Content inside of a section may be split into paragraphs and include sub-headers if needed.

#### Scrolling content <a href="#scrolling-content" id="scrolling-content"></a>

When the accordion content is longer than the viewport the whole accordion should vertically scroll. Content should not scroll inside of an individual panel. Content should never scroll horizontally in an accordion.

#### Further guidance <a href="#further-guidance" id="further-guidance"></a>

For further content guidance, see Carbon’s [content guidelines](https://carbondesignsystem.com/components/accordion/usage/\[https:/www.carbondesignsystem.com/guidelines/content/general]\(https://www.carbondesignsystem.com/guidelines/content/general\)).

### Behaviors <a href="#behaviors" id="behaviors"></a>

#### States <a href="#states" id="states"></a>

The accordion component has two main states: **collapsed** and **expanded**. The chevron icon at the end of the accordion indicates which state the accordion is in. The chevron points down to indicate collapsed and up to indicate expanded.

Accordions begin by default in the collapsed state with all content panels closed. Starting in a collapsed state gives the user a high level overview of the available information.

![accordion states](https://carbondesignsystem.com/static/0465ab97827ebd522ea8c08f0a8c3caf/3cbba/accordion-state-1.png)

A user can then independently expand each section of the accordion allowing for multiple sections to be open at once.

![multiple sections expanded](https://carbondesignsystem.com/static/6fadbea750f3062a60e105c24918838e/3cbba/accordion-state-2.png)

In addition to the collapsed and expanded states, accordions also have interactive states for focus, hover, and disabled. See the [style tab](https://carbondesignsystem.com/components/accordion/style) for more details.

![accordion interactives states](https://carbondesignsystem.com/static/ba0f151088fc214aa62b5dfa50ba3ac0/3cbba/accordion-state-3.png)

#### Interactions <a href="#interactions" id="interactions"></a>

**Mouse**

Users can trigger a state change by clicking on the chevron or clicking anywhere in the header area.

![accordion click targets](https://carbondesignsystem.com/static/beea227653c4258701275f8391664c5e/3cbba/accordion-click-target.png)

**Keyboard**

Users can navigate between accordion headers by pressing `Tab` or `Shift-Tab`. Users can trigger a state change by pressing `Enter` or `Space` while the header area has focus. For additional keyboard interactions, see the [accessibility tab](https://carbondesignsystem.com/components/accordion/accessibility#keyboard-interactions).

### Related <a href="#related" id="related"></a>

The following components are additional ways to organize content. Consider the type and length of content you are working with when choosing a content container. Longer form content may benefit from tabs or a content switcher while very short content might do better in a structured list.

* [Content switchers](https://carbondesignsystem.com/components/content-switcher/usage) allow users to toggle between two or more content sections within the same space on the screen.
* [Progress indicators](https://carbondesignsystem.com/components/progress-indicator/usage) guide users through any linear, multistep task by showing the user their completed, current, and future steps.
* [Structured lists](https://carbondesignsystem.com/components/structured-list/usage) group content that is similar or related, such as terms and definitions.
* [Tabs](https://carbondesignsystem.com/components/tabs/usage) organize related content by allowing the user to navigate between groups of information that appear within the same context.
* [Tree view](https://carbondesignsystem.com/components/tree-view/usage) is a hierarchical structure that provides nested levels of navigation.

### References <a href="#references" id="references"></a>

* Hoa Loranger, [Accordions Are Not Always the Answer for Complex Content on Desktops](https://www.nngroup.com/articles/accordions-complex-content/) (Nielsen Norman Group, 2014)

<br>
{% endtab %}

{% tab title="Style" %}
### Color <a href="#color" id="color"></a>

| Element | Property      | Color token      |
| ------- | ------------- | ---------------- |
| Title   | color         | `$text-primary`  |
| Content | color         | `$text-primary`  |
| Icon    | fill          | `$icon-primary`  |
| Header  | border-top    | `$border-subtle` |
|         | background    | Transparent      |
| Panel   | border-bottom | `$border-subtle` |
|         | background    | Transparent      |

#### Interactive states <a href="#interactive-states" id="interactive-states"></a>

| Element | State    | Property   | Color token      |
| ------- | -------- | ---------- | ---------------- |
| Header  | Hover    | background | `$layer-hover`   |
|         | Focus    | border     | `$focus`         |
|         | Disabled | border-top | `$border-subtle` |
| Title   | Disabled | background | `$text-disabled` |
| Icon    | Disabled | fill       | `$icon-disabled` |

* Default
* Flush

![default accordion alignment interactive states](https://carbondesignsystem.com/static/d364faa050c2b2e7b9f5b63315c737a9/3cbba/accordion-style-2.png)

### Typography <a href="#typography" id="typography"></a>

All accordion titles are set in sentence case. See the accordion [content guidelines](https://carbondesignsystem.com/components/accordion/usage#content) for more details.

| Element | Font-size (px/rem) | Font-weight   | Type token |
| ------- | ------------------ | ------------- | ---------- |
| Title   | 14 / 0.875         | Regular / 400 | `$body-01` |
| Content | 14 / 0.875         | Regular / 400 | `$body-01` |

### Structure <a href="#structure" id="structure"></a>

There is no max-height for an open panel but an accordion may [scroll](https://carbondesignsystem.com/components/accordion/usage#scrolling-content) if constrained by vertical space. The width of an accordion varies based on the content, layout, and page design. The icon used in the header is a `chevron`. The accordion has an indented default alignment but can also be set to have a flush alignment.

#### Default alignment <a href="#default-alignment" id="default-alignment"></a>

| Element | Property       | px/rem   | Spacing token |
| ------- | -------------- | -------- | ------------- |
| Header  | height         | 40 / 2.5 | –             |
| Item    | border-top     | 1        | –             |
| Title   | margin-left    | 16 / 1   | `$spacing-05` |
| Panel   | padding-top    | 8 / 0.5  | `$spacing-03` |
|         | padding-bottom | 24 / 1.5 | `$spacing-06` |
|         | padding-right  | 25%      | –             |
|         | padding-left   | 16 / 1   | `$spacing-05` |
| Icon    | size           | 16 / 1   | –             |
|         | padding-right  | 16 / 1   | `$spacing-05` |

![Structure measurements for default accordion alignment](https://carbondesignsystem.com/static/00ad888b595ced3f314dd467c5dc20f4/3cbba/accordion-style-4.png)

Structure measurements for default accordion alignment. | px / rem

\
![Spacing measurements for default accordion alignment](https://carbondesignsystem.com/static/a3ce6ea1502806a0228fdb4eca7744c4/3cbba/accordion-style-5.png)

Spacing measurements for default accordion alignment. | px / rem

#### Flush alignment <a href="#flush-alignment" id="flush-alignment"></a>

| Element | Property       | px/rem   | Spacing token |
| ------- | -------------- | -------- | ------------- |
| Header  | height         | 40 / 2.5 | –             |
| Item    | border-top     | 1        | –             |
| Title   | margin-left    | 0        | –             |
| Panel   | padding-top    | 8 / 0.5  | `$spacing-03` |
|         | padding-bottom | 24 / 1.5 | `$spacing-06` |
|         | padding-right  | 25%      | –             |
|         | padding-left   | 0        | –             |
| Icon    | size           | 16 / 1   | –             |
|         | padding-right  | 0        | –             |

![Structure measurements for flush accordion alignment](https://carbondesignsystem.com/static/9139501b19bbc3274f2f0e32bf8b3c58/3cbba/accordion-style-6.png)

Structure measurements for flush accordion alignment. | px / rem

\
![Spacing measurements for flush accordion alignment](https://carbondesignsystem.com/static/153019fcccab481ad3cefadc07c5a182/3cbba/accordion-style-7.png)

Spacing measurements for flush accordion alignment. | px / rem
{% endtab %}

{% tab title="Code" %}
Preview the accordion component with the React live demo. For detailed code usage documentation, see the Storybooks for each framework below.

### Documentation <a href="#documentation" id="documentation"></a>

[**React**](https://react.carbondesignsystem.com/?path=/story/components-accordion--default)[**Web Components**](https://web-components.carbondesignsystem.com/?path=/story/components-accordion--default)[**Angular (Community)**](https://angular.carbondesignsystem.com/?path=/story/components-accordion--basic)[**Vue (Community)**](http://vue.carbondesignsystem.com/?path=/story/components-cvaccordion--default)

### Live demo <a href="#live-demo" id="live-demo"></a>

Theme selector

This live demo contains only a preview of functionality and styles available for this component. View the [full demo](https://react.carbondesignsystem.com/?path=/story/components-accordion--default\&globals=theme:white) on Storybook for additional information such as its version, controls, and API documentation.
{% endtab %}
{% endtabs %}
