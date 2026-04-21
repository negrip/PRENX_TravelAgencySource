<H1 class=page-title>Intersection Observer</H1></HEADER>
<DIV class=page-body><FIGURE id=76979060-f539-49b4-856f-3a0cd192161d class="block-color-gray_background callout" style="WHITE-SPACE: pre-wrap; DISPLAY: flex">
<DIV style="FONT-SIZE: 1.5em"><SPAN class=icon>💡</SPAN></DIV>
<DIV style="WIDTH: 100%">This control allows the user to wrap another component and use the Javascript Intersection Observer on it.</DIV></FIGURE>
<H2 id=c491e685-09bb-42db-9027-f3d11512285a>Properties:</H2>
<UL id=6514cfdc-450b-40d7-b1bc-f25e3ad12ee8 class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"><MARK class=highlight-gray_background><STRONG>Root:</STRONG></MARK> String: Set the ID of the component that is used as the viewport, default is the browser.</LI></UL>
<H3 id=22efe259-70c4-4335-8818-133f7bb685a3>Root Margin</H3>
<P id=7ce80f29-9f97-4f66-b8cf-c675bbbf2540>Margin around the root. The values can be percentages or dip, default value is zero. 
<DIV class=indented>
<UL id=357e73e6-919c-4a1d-a018-2736be624cfd class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"><MARK class=highlight-gray_background><STRONG>TopRootMargin: </STRONG></MARK>Top margin around the root</LI></UL>
<UL id=d062796e-85d8-44b3-ba35-aa92b64a60c5 class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"></MARK><MARK class=highlight-gray_background><STRONG>LeftRootMargin: </STRONG></MARK>Left margin around the root</LI></UL>
<UL id=ddeec778-03b2-4beb-b0b4-c449abc4833d class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"></MARK><MARK class=highlight-gray_background><STRONG>BottomRootMargin: </STRONG></MARK>Bottom margin around the root</LI></UL>
<UL id=383fc262-a0b4-4e7c-9d96-c0fd688964d8 class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"></MARK><MARK class=highlight-gray_background><STRONG>RightRootMargin: </STRONG></MARK>Right margin around the root</LI></UL></DIV>
<P></P>
<UL id=5d470360-803f-4d21-bd16-1d39e64c8de2 class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"><MARK class=highlight-gray_background><STRONG>Threshold:</STRONG></MARK> An string of colon separated&nbsp;percentage values&nbsp;which indicate at what percentage of the target's visibility the observer's callback should be executed, default is [0]. Example "10%,50%"</LI></UL>
<UL id=36308b4f-5a91-43c5-8e68-7f87584f6ec8 class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"><MARK class=highlight-gray_background><STRONG>IntersectionRatio:</STRONG></MARK> The degree of intersection between the target element and its root, its a read-only property that change its value when the <MARK class=highlight-gray_background><STRONG>IntersectionUpdate</STRONG></MARK> event its triggered. Default value is zero.</LI></UL>
<H2 id=d2439906-c7c5-4481-b0f4-e8e8ba8e6a7c>Events:</H2>
<UL id=96ec6739-87d5-4806-a583-7c1a145547ea class=bulleted-list>
<LI style="LIST-STYLE-TYPE: disc"><MARK class=highlight-gray_background><STRONG>IntersectionUpdate:</STRONG></MARK> This event is triggered when the page load, and every time that an intercepton occurs.</LI></UL>
<P id=7f9b875d-670b-42d9-b507-0c7faf0aea9c></P></DIV></ARTICLE>