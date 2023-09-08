<div align="center">
 
 ![火箭.png](https://s2.loli.net/2023/09/06/ZipkBhjlL1y4seR.png)
 
</div>

# The mechanism of improving the generalization computation performance of strawberry ripeness using the coupling TOOD model

<div align="center">

<b><font size="5">OpenMMLab website</font></b>
    <sup>
      <a href="https://openmmlab.com/">
        <i><font size="4">HOT</font></i>
      </a>
    </sup>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <b><font size="5">OpenMMLab platform</font></b>
    <sup>
      <a href="https://openmmlab.com/">
        <i><font size="4">TRY IT OUT</font></i>
      </a>
    </sup>
    <b><font size="5">NVIDIA Tesla P100</font></b>
    <sup>
      <a href="https://www.nvidia.cn/data-center/tesla-p100/">
        <i><font size="4">GET IT</font></i>
      </a>
    </sup>

  ![](https://img.shields.io/badge/python-3.7-red)
  [![](https://img.shields.io/badge/pytorch-1.10-red)](https://pytorch.org/)
  [![](https://img.shields.io/badge/torchvision-0.11.0-red)](https://pypi.org/project/torchvision/)
  [![](https://img.shields.io/badge/MMDetection-2.28.2-red)](https://github.com/open-mmlab/)
  
  

  [🛠️Installation Dependencies](https://blog.csdn.net/m0_46556474/article/details/130778016) |
  [🎤Introduction](https://github.com/open-mmlab/mmdetection) |
 
  [👀Download Dataset](https://pan.baidu.com/s/1kxS0curbX3XJ9gp_G6lt4A) |
  
  [🌊a Simple Anchor alignment metric](https://github.com/0811yu/0811yu.github.io) |
  [🚀Small Object detection improved](https://github.com/0811yu/0811yu.github.io) |
  
  [🤔Model generalization ability improved](https://github.com/0811yu/0811yu.github.io) |
 

</div>

## Dependencies:

 - Python 3.7
 - [PyTorch](https://pytorch.org/) 1.10
 - [Torchvision](https://pypi.org/project/torchvision/) 0.11.0
 - [OpenCV](https://opencv.org/) 4.7.0
 - Ubuntu 20.04.5 LTS 
 - [MMCV](https://github.com/open-mmlab/mmcv)
 - NVIDIA Tesla P100

## Introduction

We have developed an innovative algorithm based on TOOD, aiming to enhance the performance of strawberry ripeness detection. This algorithm incorporates the CARAFE-FPN + Swin-B + MST + Albu + Saam modules and improves the model in the following ways: Firstly, the introduction of the Swin-B module in the backbone network enhances the accuracy of feature extraction. Secondly, the traditional feature pyramid network is replaced by CARAFE-FPN to improve detection efficacy across different scales. Additionally, we employ the MST training method to enhance the detection capability of small objects. Furthermore, the utilization of the albu library for feature augmentation empowers the model with better generalization ability. Lastly, by improving the S-aam header, we mitigate the impact of parameters on network performance and determine the optimal network parameters to achieve the highest detection accuracy. Through this series of improvements, our model achieves an average precision (AP) of 74.1% on the LSDS strawberry dataset, surpassing the performance of currently advanced single-stage and two-stage networks.

![单阶段双阶段网络对比图.png](https://s2.loli.net/2023/09/06/bQ2hM5aBeqJmTKo.png)

## Ours Strawberries dataset
We have the largest strawberry dataset of our own, with a total of 5600 photos. We used the dataset augmentation method (https://roboflow.com/) to expand to 16800 images. The training set contains 13,800 images and the test set contains 3,000 images. The data set is named "LSDS".
<a href="https://pan.baidu.com/s/1kxS0curbX3XJ9gp_G6lt4A">Click here to view and download the dataset</a>
### LSDS Dataset example

![最新.jpg](https://s2.loli.net/2023/09/06/r2G9ODnwQ8aomIx.jpg)

</div>


## Result of experiment
The conducted experiment validated the contributions of novel upsampling pyramid (CARAFE-FPN), self-attention neural network model (Swin-B), multi-scale training (MST), feature enhancement tool (Albu), and simple anchor alignment metric (S-aam) in improving the performance of strawberry ripeness detection.

### Ablation experiments in LSDS dataset

<html xmlns:v="urn:schemas-microsoft-com:vml"
xmlns:o="urn:schemas-microsoft-com:office:office"
xmlns:w="urn:schemas-microsoft-com:office:word"
xmlns:m="http://schemas.microsoft.com/office/2004/12/omml"
xmlns="http://www.w3.org/TR/REC-html40">

<head>
<meta http-equiv=Content-Type content="text/html; charset=gb2312">
<meta name=ProgId content=Word.Document>
<meta name=Generator content="Microsoft Word 15">
<meta name=Originator content="Microsoft Word 15">
<link rel=File-List href="不同数据集的.files/filelist.xml">
<!--[if gte mso 9]><xml>
 <o:DocumentProperties>
  <o:Author>刘 欢</o:Author>
  <o:Template>Normal</o:Template>
  <o:LastAuthor>刘 欢</o:LastAuthor>
  <o:Revision>2</o:Revision>
  <o:TotalTime>0</o:TotalTime>
  <o:Created>2023-09-08T07:29:00Z</o:Created>
  <o:LastSaved>2023-09-08T07:29:00Z</o:LastSaved>
  <o:Pages>1</o:Pages>
  <o:Words>41</o:Words>
  <o:Characters>235</o:Characters>
  <o:Lines>1</o:Lines>
  <o:Paragraphs>1</o:Paragraphs>
  <o:CharactersWithSpaces>275</o:CharactersWithSpaces>
  <o:Version>16.00</o:Version>
 </o:DocumentProperties>
 <o:OfficeDocumentSettings>
  <o:AllowPNG/>
 </o:OfficeDocumentSettings>
</xml><![endif]-->
<link rel=themeData href="不同数据集的.files/themedata.thmx">
<link rel=colorSchemeMapping href="不同数据集的.files/colorschememapping.xml">
<!--[if gte mso 9]><xml>
 <w:WordDocument>
  <w:SpellingState>Clean</w:SpellingState>
  <w:GrammarState>Clean</w:GrammarState>
  <w:TrackMoves>false</w:TrackMoves>
  <w:TrackFormatting/>
  <w:PunctuationKerning/>
  <w:DrawingGridVerticalSpacing>7.8 磅</w:DrawingGridVerticalSpacing>
  <w:DisplayHorizontalDrawingGridEvery>0</w:DisplayHorizontalDrawingGridEvery>
  <w:DisplayVerticalDrawingGridEvery>2</w:DisplayVerticalDrawingGridEvery>
  <w:ValidateAgainstSchemas/>
  <w:SaveIfXMLInvalid>false</w:SaveIfXMLInvalid>
  <w:IgnoreMixedContent>false</w:IgnoreMixedContent>
  <w:AlwaysShowPlaceholderText>false</w:AlwaysShowPlaceholderText>
  <w:DoNotPromoteQF/>
  <w:LidThemeOther>EN-US</w:LidThemeOther>
  <w:LidThemeAsian>ZH-CN</w:LidThemeAsian>
  <w:LidThemeComplexScript>X-NONE</w:LidThemeComplexScript>
  <w:Compatibility>
   <w:SpaceForUL/>
   <w:BalanceSingleByteDoubleByteWidth/>
   <w:DoNotLeaveBackslashAlone/>
   <w:ULTrailSpace/>
   <w:DoNotExpandShiftReturn/>
   <w:AdjustLineHeightInTable/>
   <w:BreakWrappedTables/>
   <w:SnapToGridInCell/>
   <w:WrapTextWithPunct/>
   <w:UseAsianBreakRules/>
   <w:DontGrowAutofit/>
   <w:SplitPgBreakAndParaMark/>
   <w:EnableOpenTypeKerning/>
   <w:DontFlipMirrorIndents/>
   <w:OverrideTableStyleHps/>
   <w:UseFELayout/>
  </w:Compatibility>
  <m:mathPr>
   <m:mathFont m:val="Cambria Math"/>
   <m:brkBin m:val="before"/>
   <m:brkBinSub m:val="&#45;-"/>
   <m:smallFrac m:val="off"/>
   <m:dispDef/>
   <m:lMargin m:val="0"/>
   <m:rMargin m:val="0"/>
   <m:defJc m:val="centerGroup"/>
   <m:wrapIndent m:val="1440"/>
   <m:intLim m:val="subSup"/>
   <m:naryLim m:val="undOvr"/>
  </m:mathPr></w:WordDocument>
</xml><![endif]--><!--[if gte mso 9]><xml>
 <w:LatentStyles DefLockedState="false" DefUnhideWhenUsed="false"
  DefSemiHidden="false" DefQFormat="false" DefPriority="99"
  LatentStyleCount="376">
  <w:LsdException Locked="false" Priority="0" QFormat="true" Name="Normal"/>
  <w:LsdException Locked="false" Priority="9" QFormat="true" Name="heading 1"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 2"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 3"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 4"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 5"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 6"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 7"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 8"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 9"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 9"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 1"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 2"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 3"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 4"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 5"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 6"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 7"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 8"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 9"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footnote text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="header"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footer"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index heading"/>
  <w:LsdException Locked="false" Priority="35" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="caption"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="table of figures"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="envelope address"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="envelope return"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footnote reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="line number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="page number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="endnote reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="endnote text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="table of authorities"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="macro"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="toa heading"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 5"/>
  <w:LsdException Locked="false" Priority="10" QFormat="true" Name="Title"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Closing"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Signature"/>
  <w:LsdException Locked="false" Priority="1" SemiHidden="true"
   UnhideWhenUsed="true" Name="Default Paragraph Font"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Message Header"/>
  <w:LsdException Locked="false" Priority="11" QFormat="true" Name="Subtitle"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Salutation"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Date"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text First Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text First Indent 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Note Heading"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Block Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Hyperlink"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="FollowedHyperlink"/>
  <w:LsdException Locked="false" Priority="22" QFormat="true" Name="Strong"/>
  <w:LsdException Locked="false" Priority="20" QFormat="true" Name="Emphasis"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Document Map"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Plain Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="E-mail Signature"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Top of Form"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Bottom of Form"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal (Web)"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Acronym"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Address"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Cite"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Code"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Definition"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Keyboard"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Preformatted"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Sample"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Typewriter"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Variable"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal Table"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation subject"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="No List"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Contemporary"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Elegant"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Professional"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Subtle 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Subtle 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Balloon Text"/>
  <w:LsdException Locked="false" Priority="39" Name="Table Grid"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Theme"/>
  <w:LsdException Locked="false" SemiHidden="true" Name="Placeholder Text"/>
  <w:LsdException Locked="false" Priority="1" QFormat="true" Name="No Spacing"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 1"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 1"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 1"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 1"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 1"/>
  <w:LsdException Locked="false" SemiHidden="true" Name="Revision"/>
  <w:LsdException Locked="false" Priority="34" QFormat="true"
   Name="List Paragraph"/>
  <w:LsdException Locked="false" Priority="29" QFormat="true" Name="Quote"/>
  <w:LsdException Locked="false" Priority="30" QFormat="true"
   Name="Intense Quote"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 1"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 1"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 1"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 1"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 1"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 2"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 2"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 2"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 2"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 2"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 2"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 2"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 3"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 3"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 3"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 3"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 3"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 3"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 3"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 4"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 4"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 4"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 4"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 4"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 4"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 4"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 5"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 5"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 5"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 5"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 5"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 5"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 5"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 6"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 6"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 6"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 6"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 6"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 6"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 6"/>
  <w:LsdException Locked="false" Priority="19" QFormat="true"
   Name="Subtle Emphasis"/>
  <w:LsdException Locked="false" Priority="21" QFormat="true"
   Name="Intense Emphasis"/>
  <w:LsdException Locked="false" Priority="31" QFormat="true"
   Name="Subtle Reference"/>
  <w:LsdException Locked="false" Priority="32" QFormat="true"
   Name="Intense Reference"/>
  <w:LsdException Locked="false" Priority="33" QFormat="true" Name="Book Title"/>
  <w:LsdException Locked="false" Priority="37" SemiHidden="true"
   UnhideWhenUsed="true" Name="Bibliography"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="TOC Heading"/>
  <w:LsdException Locked="false" Priority="41" Name="Plain Table 1"/>
  <w:LsdException Locked="false" Priority="42" Name="Plain Table 2"/>
  <w:LsdException Locked="false" Priority="43" Name="Plain Table 3"/>
  <w:LsdException Locked="false" Priority="44" Name="Plain Table 4"/>
  <w:LsdException Locked="false" Priority="45" Name="Plain Table 5"/>
  <w:LsdException Locked="false" Priority="40" Name="Grid Table Light"/>
  <w:LsdException Locked="false" Priority="46" Name="Grid Table 1 Light"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark"/>
  <w:LsdException Locked="false" Priority="51" Name="Grid Table 6 Colorful"/>
  <w:LsdException Locked="false" Priority="52" Name="Grid Table 7 Colorful"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 1"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 1"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 1"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 2"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 2"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 2"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 3"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 3"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 3"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 4"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 4"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 4"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 5"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 5"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 5"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 6"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 6"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 6"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="46" Name="List Table 1 Light"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark"/>
  <w:LsdException Locked="false" Priority="51" Name="List Table 6 Colorful"/>
  <w:LsdException Locked="false" Priority="52" Name="List Table 7 Colorful"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 1"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 1"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 1"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 2"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 2"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 2"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 3"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 3"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 3"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 4"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 4"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 4"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 5"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 5"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 5"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 6"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 6"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 6"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Mention"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Smart Hyperlink"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Hashtag"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Unresolved Mention"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Smart Link"/>
 </w:LatentStyles>
</xml><![endif]--><![if !supportAnnotations]>
<style id="dynCom" type="text/css"><!-- --></style>
<script language="JavaScript"><!--
function msoCommentShow(anchor_id, com_id)
{
	if(msoBrowserCheck()) 
		{
		c = document.all(com_id);
		a = document.all(anchor_id);
		if (null != c && null == c.length && null != a && null == a.length)
			{
			var cw = c.offsetWidth;
			var ch = c.offsetHeight;
			var aw = a.offsetWidth;
			var ah = a.offsetHeight;
			var x  = a.offsetLeft;
			var y  = a.offsetTop;
			var el = a;
			while (el.tagName != "BODY") 
				{
				el = el.offsetParent;
				x = x + el.offsetLeft;
				y = y + el.offsetTop;
				}
			var bw = document.body.clientWidth;
			var bh = document.body.clientHeight;
			var bsl = document.body.scrollLeft;
			var bst = document.body.scrollTop;
			if (x + cw + ah / 2 > bw + bsl && x + aw - ah / 2 - cw >= bsl ) 
				{ c.style.left = x + aw - ah / 2 - cw; }
			else 
				{ c.style.left = x + ah / 2; }
			if (y + ch + ah / 2 > bh + bst && y + ah / 2 - ch >= bst ) 
				{ c.style.top = y + ah / 2 - ch; }
			else 
				{ c.style.top = y + ah / 2; }
			c.style.visibility = "visible";
}	}	}
function msoCommentHide(com_id) 
{
	if(msoBrowserCheck())
		{
		c = document.all(com_id);
		if (null != c && null == c.length)
		{
		c.style.visibility = "hidden";
		c.style.left = -1000;
		c.style.top = -1000;
		} } 
}
function msoBrowserCheck()
{
	ms = navigator.appVersion.indexOf("MSIE");
	vers = navigator.appVersion.substring(ms + 5, ms + 6);
	ie4 = (ms > 0) && (parseInt(vers) >= 4);
	return ie4;
}
if (msoBrowserCheck())
{
	document.styleSheets.dynCom.addRule(".msocomanchor","background: infobackground");
	document.styleSheets.dynCom.addRule(".msocomoff","display: none");
	document.styleSheets.dynCom.addRule(".msocomtxt","visibility: hidden");
	document.styleSheets.dynCom.addRule(".msocomtxt","position: absolute");
	document.styleSheets.dynCom.addRule(".msocomtxt","top: -1000");
	document.styleSheets.dynCom.addRule(".msocomtxt","left: -1000");
	document.styleSheets.dynCom.addRule(".msocomtxt","width: 33%");
	document.styleSheets.dynCom.addRule(".msocomtxt","background: infobackground");
	document.styleSheets.dynCom.addRule(".msocomtxt","color: infotext");
	document.styleSheets.dynCom.addRule(".msocomtxt","border-top: 1pt solid threedlightshadow");
	document.styleSheets.dynCom.addRule(".msocomtxt","border-right: 2pt solid threedshadow");
	document.styleSheets.dynCom.addRule(".msocomtxt","border-bottom: 2pt solid threedshadow");
	document.styleSheets.dynCom.addRule(".msocomtxt","border-left: 1pt solid threedlightshadow");
	document.styleSheets.dynCom.addRule(".msocomtxt","padding: 3pt 3pt 3pt 3pt");
	document.styleSheets.dynCom.addRule(".msocomtxt","z-index: 100");
}
// --></script>
<![endif]>
<style>
<!--
 /* Font Definitions */
 @font-face
	{font-family:"Cambria Math";
	panose-1:2 4 5 3 5 4 6 3 2 4;
	mso-font-charset:0;
	mso-generic-font-family:roman;
	mso-font-pitch:variable;
	mso-font-signature:-536869121 1107305727 33554432 0 415 0;}
@font-face
	{font-family:等线;
	panose-1:2 1 6 0 3 1 1 1 1 1;
	mso-font-alt:DengXian;
	mso-font-charset:134;
	mso-generic-font-family:auto;
	mso-font-pitch:variable;
	mso-font-signature:-1610612033 953122042 22 0 262159 0;}
@font-face
	{font-family:"\@等线";
	panose-1:2 1 6 0 3 1 1 1 1 1;
	mso-font-charset:134;
	mso-generic-font-family:auto;
	mso-font-pitch:variable;
	mso-font-signature:-1610612033 953122042 22 0 262159 0;}
 /* Style Definitions */
 p.MsoNormal, li.MsoNormal, div.MsoNormal
	{mso-style-unhide:no;
	mso-style-qformat:yes;
	mso-style-parent:"";
	margin:0cm;
	text-align:justify;
	text-justify:inter-ideograph;
	mso-pagination:none;
	font-size:10.5pt;
	mso-bidi-font-size:11.0pt;
	font-family:等线;
	mso-ascii-font-family:等线;
	mso-ascii-theme-font:minor-latin;
	mso-fareast-font-family:等线;
	mso-fareast-theme-font:minor-fareast;
	mso-hansi-font-family:等线;
	mso-hansi-theme-font:minor-latin;
	mso-bidi-font-family:"Times New Roman";
	mso-bidi-theme-font:minor-bidi;
	mso-font-kerning:1.0pt;}
p.MsoHeader, li.MsoHeader, div.MsoHeader
	{mso-style-priority:99;
	mso-style-link:"页眉 字符";
	margin:0cm;
	text-align:center;
	mso-pagination:none;
	tab-stops:center 207.65pt right 415.3pt;
	layout-grid-mode:char;
	font-size:9.0pt;
	font-family:等线;
	mso-ascii-font-family:等线;
	mso-ascii-theme-font:minor-latin;
	mso-fareast-font-family:等线;
	mso-fareast-theme-font:minor-fareast;
	mso-hansi-font-family:等线;
	mso-hansi-theme-font:minor-latin;
	mso-bidi-font-family:"Times New Roman";
	mso-bidi-theme-font:minor-bidi;
	mso-font-kerning:1.0pt;}
p.MsoFooter, li.MsoFooter, div.MsoFooter
	{mso-style-priority:99;
	mso-style-link:"页脚 字符";
	margin:0cm;
	mso-pagination:none;
	tab-stops:center 207.65pt right 415.3pt;
	layout-grid-mode:char;
	font-size:9.0pt;
	font-family:等线;
	mso-ascii-font-family:等线;
	mso-ascii-theme-font:minor-latin;
	mso-fareast-font-family:等线;
	mso-fareast-theme-font:minor-fareast;
	mso-hansi-font-family:等线;
	mso-hansi-theme-font:minor-latin;
	mso-bidi-font-family:"Times New Roman";
	mso-bidi-theme-font:minor-bidi;
	mso-font-kerning:1.0pt;}
span.a
	{mso-style-name:"页眉 字符";
	mso-style-priority:99;
	mso-style-unhide:no;
	mso-style-locked:yes;
	mso-style-link:页眉;
	mso-ansi-font-size:9.0pt;
	mso-bidi-font-size:9.0pt;}
span.a0
	{mso-style-name:"页脚 字符";
	mso-style-priority:99;
	mso-style-unhide:no;
	mso-style-locked:yes;
	mso-style-link:页脚;
	mso-ansi-font-size:9.0pt;
	mso-bidi-font-size:9.0pt;}
.MsoChpDefault
	{mso-style-type:export-only;
	mso-default-props:yes;
	font-family:等线;
	mso-bidi-font-family:"Times New Roman";
	mso-bidi-theme-font:minor-bidi;
	mso-ligatures:none;}
 /* Page Definitions */
 @page
	{mso-page-border-surround-header:no;
	mso-page-border-surround-footer:no;
	mso-footnote-separator:url("不同数据集的.files/header.htm") fs;
	mso-footnote-continuation-separator:url("不同数据集的.files/header.htm") fcs;
	mso-endnote-separator:url("不同数据集的.files/header.htm") es;
	mso-endnote-continuation-separator:url("不同数据集的.files/header.htm") ecs;}
@page WordSection1
	{size:595.3pt 841.9pt;
	margin:72.0pt 90.0pt 72.0pt 90.0pt;
	mso-header-margin:42.55pt;
	mso-footer-margin:49.6pt;
	mso-paper-source:0;
	layout-grid:15.6pt;}
div.WordSection1
	{page:WordSection1;}
-->
</style>
<!--[if gte mso 10]>
<style>
 /* Style Definitions */
 table.MsoNormalTable
	{mso-style-name:普通表格;
	mso-tstyle-rowband-size:0;
	mso-tstyle-colband-size:0;
	mso-style-noshow:yes;
	mso-style-priority:99;
	mso-style-parent:"";
	mso-padding-alt:0cm 5.4pt 0cm 5.4pt;
	mso-para-margin:0cm;
	mso-pagination:widow-orphan;
	font-size:10.5pt;
	mso-bidi-font-size:11.0pt;
	font-family:等线;
	mso-ascii-font-family:等线;
	mso-ascii-theme-font:minor-latin;
	mso-fareast-font-family:等线;
	mso-fareast-theme-font:minor-fareast;
	mso-hansi-font-family:等线;
	mso-hansi-theme-font:minor-latin;
	mso-font-kerning:1.0pt;}
</style>
<![endif]--><!--[if gte mso 9]><xml>
 <o:shapedefaults v:ext="edit" spidmax="2050"/>
</xml><![endif]--><!--[if gte mso 9]><xml>
 <o:shapelayout v:ext="edit">
  <o:idmap v:ext="edit" data="2"/>
 </o:shapelayout></xml><![endif]-->
</head>

<body lang=ZH-CN style='tab-interval:21.0pt;word-wrap:break-word;text-justify-trim:
punctuation'>

<div class=WordSection1 style='layout-grid:15.6pt'>

<table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 width="100%"
 style='width:100.0%;border-collapse:collapse;border:none;mso-border-top-alt:
 solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext 1.5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;height:14.25pt'>
  <td width="32%" nowrap style='width:32.04%;border-top:solid windowtext 1.5pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Dataset</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="2%" valign=top style='width:2.86%;border:none;border-top:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border-top:solid windowtext 1.5pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Models</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border-top:solid windowtext 1.5pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>AP</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap valign=bottom style='width:13.2%;border-top:solid windowtext 1.5pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;mso-font-kerning:0pt'>AP@50<o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap valign=bottom style='width:13.2%;border-top:solid windowtext 1.5pt;
  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;
  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;mso-font-kerning:0pt'>AP@75<o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:1;height:14.25pt'>
  <td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;mso-border-top-alt:
  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><a
  name="_Hlk140258770"><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;color:black;
  mso-color-alt:windowtext;mso-font-kerning:0pt'>LSDS</span></a><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;mso-border-top-alt:
  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:
  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>71.9</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:
  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>91.8</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:
  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>82.1</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:2;height:14.25pt'>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>74.1</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>93.9</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>84.1</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:3;height:14.25pt'>
  <td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;background:
  white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:
  0pt'>StrawDI_Db1</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:
  0pt'><o:p></o:p></span></p>
  </td>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>71.3</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>91.2</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>81.6</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:4;height:14.25pt'>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>72.6</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>92.4</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>82.7</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:5;height:14.25pt'>
  <td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;background:
  white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:
  0pt'>Internet</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:
  0pt'><o:p></o:p></span></p>
  </td>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>63.8</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>86.3</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>77.2</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:6;height:14.25pt'>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>65.6</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>88.9</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>79.4</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:7;height:14.25pt'>
  <td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;border-bottom:
  solid windowtext 1.5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;
  height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:
  0pt'>COCO</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="2%" valign=top style='width:2.86%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>51.1</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>69.4</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;background:white;
  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>55.5</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
 <tr style='mso-yfti-irow:8;mso-yfti-lastrow:yes;height:14.25pt'>
  <td width="2%" valign=top style='width:2.86%;border:none;border-bottom:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p>
  </td>
  <td width="25%" nowrap style='width:25.5%;border:none;border-bottom:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>51.8</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;
  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:
  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>70.2</span><span
  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:
  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
  <td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;
  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'>
  <p class=MsoNormal align=center style='text-align:center;line-height:150%;
  mso-pagination:widow-orphan;page-break-after:avoid'><span lang=EN-US
  style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:"Times New Roman",serif;
  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:
  0pt'>56.4</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:
  150%;font-family:"Times New Roman",serif;mso-fareast-font-family:等线;
  mso-font-kerning:0pt'><o:p></o:p></span></p>
  </td>
 </tr>
</table>

<p class=MsoNormal><span lang=EN-US><o:p>&nbsp;</o:p></span></p>

</div>

</body>

</html>




### The outcomes of our proposed model testing are denoted by b and d, whereas the results from the baseline model testing are represented by a and c.



We have observed that the parameters α and β in the formula t=s^α×u^β, as well as the threshold for non-maximum suppression (NMS), have a significant impact on the experimental results. We have chosen values of α as 0.5, 1, 1.5, and 2, and values of β as four times, five times, six times, seven times, and eight times α. Lastly, we have experimented with NMS threshold IOU set at 0.6, 0.65, 0.7, and 0.75. By adjusting these parameters, we aim to uncover the relationships among them.
##Multidimensional graph

![987.png](https://s2.loli.net/2023/09/07/n6eA3RHLIZWMFDu.png)

Detailed experimental results can be found by clicking the link below
<a href="https://s2.loli.net/2023/09/08/SBYqaCUVGrWcsPL.jpg">Click here to view </a>


In order to further scrutinize the relationship between them, we apply the method of analysis of variance (ANOVA) using the single-factor ANOVA feature available in the SPSS software to evaluate whether there are disparities between the various magnitudes of measurement and the experimental outcomes.
#### Results of homogeneity test of variance<a href="https://s2.loli.net/2023/09/08/e9XsxpOdgqy2n4v.jpg">Click here to view </a>
#### Table of significant differences between different multiples of α<a href="https://s2.loli.net/2023/09/08/eIavwKHz9RZr6ob.jpg">Click here to view </a>


## The outcomes of our model tested on various datasets.
To assess the efficacy of the improved model on a variety of datasets, experiments were conducted on four different datasets for both the improved model and the baseline model. The following table presents diverse performance metrics, namely AP, AP50, and AP75, during training on the LSDS, StrawDI_Db1, Internet, and COCO datasets.



<html xmlns:v="urn:schemas-microsoft-com:vml"xmlns:o="urn:schemas-microsoft-com:office:office"xmlns:w="urn:schemas-microsoft-com:office:word"xmlns:m="http://schemas.microsoft.com/office/2004/12/omml"xmlns="http://www.w3.org/TR/REC-html40"><head><meta http-equiv=Content-Type content="text/html; charset=gb2312"><meta name=ProgId content=Word.Document><meta name=Generator content="Microsoft Word 15"><meta name=Originator content="Microsoft Word 15"><link rel=File-List href="不同数据集999.files/filelist.xml"><link rel=themeData href="不同数据集999.files/themedata.thmx"><link rel=colorSchemeMapping href="不同数据集999.files/colorschememapping.xml"><![if !supportAnnotations]><style id="dynCom" type="text/css"></style><script language="JavaScript"></script><![endif]><style></style></head><body lang=ZH-CN style='tab-interval:21.0pt;word-wrap:break-word;text-justify-trim:punctuation'><div class=WordSection1 style='layout-grid:15.6pt'><table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0 width="100%" style='width:100.0%;border-collapse:collapse;border:none;mso-border-top-alt: solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext 1.5pt; mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'><tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;height:14.25pt'><td width="32%" nowrap style='width:32.04%;border-top:solid windowtext 1.5pt;  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:150%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Dataset</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:150%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="2%" valign=top style='width:2.86%;border:none;border-top:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:150%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:150%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border-top:solid windowtext 1.5pt;  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Models</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border-top:solid windowtext 1.5pt;  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>AP</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap valign=bottom style='width:13.2%;border-top:solid windowtext 1.5pt;  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;mso-font-kerning:0pt'>AP@50<o:p></o:p></span></p></td><td width="13%" nowrap valign=bottom style='width:13.2%;border-top:solid windowtext 1.5pt;  border-left:none;border-bottom:solid windowtext 1.0pt;border-right:none;  mso-border-top-alt:solid windowtext 1.5pt;mso-border-bottom-alt:solid windowtext .5pt;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;mso-font-kerning:0pt'>AP@75<o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:1;height:14.25pt'><td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;mso-border-top-alt:  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><a  name="_Hlk140258770"><span lang=EN-US style='mso-bidi-font-size:10.5pt;  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;color:black;  mso-color-alt:windowtext;mso-font-kerning:0pt'>LSDS</span></a><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;mso-border-top-alt:  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>71.9</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>91.8</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;mso-border-top-alt:  solid windowtext .5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>82.1</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:2;height:14.25pt'><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>74.1</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>93.9</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>84.1</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:3;height:14.25pt'><td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;background:  white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:  0pt'>StrawDI_Db1</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:  0pt'><o:p></o:p></span></p></td><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>71.3</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>91.2</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>81.6</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:4;height:14.25pt'><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>72.6</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>92.4</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>82.7</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:5;height:14.25pt'><td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;background:  white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:  0pt'>Internet</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;  font-family:"Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:  0pt'><o:p></o:p></span></p></td><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>63.8</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>86.3</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>77.2</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:6;height:14.25pt'><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>65.6</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>88.9</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>79.4</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:7;height:14.25pt'><td width="32%" nowrap rowspan=2 style='width:32.04%;border:none;border-bottom:  solid windowtext 1.5pt;background:white;padding:0cm 5.4pt 0cm 5.4pt;  height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:  0pt'>COCO</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="2%" valign=top style='width:2.86%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Baseline</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>51.1</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>69.4</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;background:white;  padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>55.5</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr><tr style='mso-yfti-irow:8;mso-yfti-lastrow:yes;height:14.25pt'><td width="2%" valign=top style='width:2.86%;border:none;border-bottom:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;mso-pagination:widow-orphan'><span  lang=EN-US style='mso-bidi-font-size:10.5pt;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p>&nbsp;</o:p></span></p></td><td width="25%" nowrap style='width:25.5%;border:none;border-bottom:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>Improved</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>51.8</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan'><span lang=EN-US style='mso-bidi-font-size:10.5pt;  line-height:200%;font-family:"Times New Roman",serif;mso-fareast-font-family:  等线;color:black;mso-color-alt:windowtext;mso-font-kerning:0pt'>70.2</span><span  lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:  "Times New Roman",serif;mso-fareast-font-family:等线;mso-font-kerning:0pt'><o:p></o:p></span></p></td><td width="13%" nowrap style='width:13.2%;border:none;border-bottom:solid windowtext 1.5pt;  background:white;padding:0cm 5.4pt 0cm 5.4pt;height:14.25pt'><p class=MsoNormal align=center style='text-align:center;line-height:200%;  mso-pagination:widow-orphan;page-break-after:avoid'><span lang=EN-US  style='mso-bidi-font-size:10.5pt;line-height:200%;font-family:"Times New Roman",serif;  mso-fareast-font-family:等线;color:black;mso-color-alt:windowtext;mso-font-kerning:  0pt'>56.4</span><span lang=EN-US style='mso-bidi-font-size:10.5pt;line-height:  200%;font-family:"Times New Roman",serif;mso-fareast-font-family:等线;  mso-font-kerning:0pt'><o:p></o:p></span></p></td></tr></table><p class=MsoNormal><span lang=EN-US><o:p>&nbsp;</o:p></span></p></div></body></html>


 ## Our model structure diagram
 ![论文图5555.jpg](https://s2.loli.net/2023/09/07/9Fp7vQY8lbxjS3u.jpg)
 
 
 ## Test result
 The results obtained from testing were based on the models proposed in b and d, while a and c represent the results obtained from the baseline models. The LDSD dataset was employed for experimentation.
![新的ours对比.jpg](https://s2.loli.net/2023/09/07/IC2zEQT7paADX5r.jpg)
