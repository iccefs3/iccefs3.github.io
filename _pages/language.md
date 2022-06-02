---
permalink: /language/
title: "The SAGE Objective Editor Language"
excerpt: "The SAGE Objective Editor Language"
author_profile: false
redirect_from: 
  - /language
  - /language.html
---
# SAGE Objective Editor Language

The SAGE Objective Editor Language was implemented using Google's Blockly library for building 
visual programming editors (Google, 2016). This section will describe the design of the language 
and the implementation of the editor that can be used to write assessments using the language.

## Language Reference

The SAGE Objective Editor Language grammar is provided below. Terminals in this grammar are 
represented using **bold** font and described with more detail in the following section. The &#8595; symbol 
represents a vertical connection between two blocks. The &#8594; symbol represents a horizontal 
connection between two blocks. Productions that have the suffix *opt* are optional. As assessment 
begins with the "assessment" non-terminal.

assessment:

&nbsp;&nbsp;&nbsp;&nbsp;expectation &#8595; trigger-list<sub>opt</sub>

expectation:

&nbsp;&nbsp;&nbsp;&nbsp;**expect** &#8594; actual &#8594; assert &#8594; matcher
    
actual:

&nbsp;&nbsp;&nbsp;&nbsp;**actl-sprite**
&nbsp;&nbsp;&nbsp;&nbsp;**actl-block**
&nbsp;&nbsp;&nbsp;&nbsp;**actl-block-type**
&nbsp;&nbsp;&nbsp;&nbsp;**actl-key-pressed**
&nbsp;&nbsp;&nbsp;&nbsp;**actl-sprite-touch-sprite**
&nbsp;&nbsp;&nbsp;&nbsp;**actl-sprite-touch-color**

assert:

&nbsp;&nbsp;&nbsp;&nbsp;**asrt-should**
&nbsp;&nbsp;&nbsp;&nbsp;**asrt-should-not**

matcher:

&nbsp;&nbsp;&nbsp;&nbsp;**mtch-be-present**
&nbsp;&nbsp;&nbsp;&nbsp;**mtch-be-on-x-y**
&nbsp;&nbsp;&nbsp;&nbsp;**mtch-point-direction**
&nbsp;&nbsp;&nbsp;&nbsp;**mtch-move-steps**
&nbsp;&nbsp;&nbsp;&nbsp;**mtch-say**

trigger-list:

&nbsp;&nbsp;&nbsp;&nbsp;trigger
&nbsp;&nbsp;&nbsp;&nbsp;trigger-list &#8595; trigger

trigger:

&nbsp;&nbsp;&nbsp;&nbsp;condition action

condition:

&nbsp;&nbsp;&nbsp;&nbsp;**cnd-if-pass**
&nbsp;&nbsp;&nbsp;&nbsp;**cnd-if-fail**

action:

&nbsp;&nbsp;&nbsp;&nbsp;**actn-say**
&nbsp;&nbsp;&nbsp;&nbsp;**actn-include-block**
&nbsp;&nbsp;&nbsp;&nbsp;**actn-exclude-block**
 
## Terminals
 
Every terminal in the grammar corresponds to a block that is described below.
 
### expect 

![expect](/images/fs3/language/expect.png)

The Expect blog signifies the beginning of an assessment. It connects horizontally to an actual 
block and connects vertically to a trigger block.
 
### actl-sprite 

![actl-sprite](/images/fs3/language/actl-sprite.png)

The Actual Sprite block is used to reference a sprite. It takes a single string argument for the 
ID of the sprite that is being referenced. It connects horizontally to an assert block.
 
### actl-block

![actl-block](/images/fs3/language/actl-block.png)

The Actual Block block is used to reference a block. It takes a single string argument for the ID 
of the block that is being referenced. It connects horizontally to an assert block.
 
### actl-block-type
 
![actl-block-type](/images/fs3/language/actl-block-type.png)

The Actual Block Type block is used to reference a block type. It takes a single string argument 
for the type of block that is being references. It connects horizontally to an assert block.
 
### actl-key-pressed 

![actl-key-pressed](/images/fs3/language/actl-key-pressed.png)

The Actual Key Pressed block is used to express a mapping between a key on a keyboard being 
pressed and a sprite. It takes two arguments. The first argument must be selected from a drop 
down menu that is pre-populated with single keyboard characters. The second argument is of 
type string for the ID of the sprite that is being referenced. It connects horizontally to an assert 
block.

### actl-sprite-touch-sprite 

![actl-sprite-touch-sprite](/images/fs3/language/actl-sprite-touch-sprite.png)

The Actual Sprite Touching Sprite block is used to express a mapping between two sprites. It 
takes two arguments. Each argument is of type string for the ID of each of the sprites that are 
being referenced. It connects horizontally to an assert block.

### actl-sprite-touch-color 

![actl-sprite-touch-color](/images/fs3/language/actl-sprite-touch-color.png)

The Actual Sprite Touching Color block is used to express a mapping between a sprite and a 
color. It takes two arguments. The first argument is of type string for the ID of the sprite being 
referenced. The second argument is from a drop down menu that is pre-populated with a list 
of colors. It connects horizontally to an assert block.
 
### asrt-should 

![asrt-should](/images/fs3/language/asrt-should.png)

The Should block is used to express an assessment where an action should occur. It connects 
horizontally to a matcher block.
 
### asrt-should-not

![asrt-should-not](/images/fs3/language/asrt-should-not.png)
 
The Should Not block is used to express an assessment where an action should not occur. It 
connects horizontally to a matcher block.
 
### mtch-be-present

![mtch-be-present](/images/fs3/language/mtch-be-present.png)
 
The Be Present block is used to express an assessment that verifies a sprite, block, or block 
type is present.
 
### mtch-be-on-x-y

![mtch-be-on-x-y](/images/fs3/language/mtch-be-on-x-y.png)
 
The Be on X and Y block is used to express an assessment that verifies a sprite is on specific 
coordinate in the Scratch stage. It takes two arguments. Each argument is of the integer data 
type and represents the X or Y coordinate.
 
### mtch-point-direction

![mtch-point-direction](/images/fs3/language/mtch-point-direction.png)

The Point in Direction block is used to express an assessment that verifies a sprite is pointing 
in a specific direction. It takes one argument. The argument must be chosen from a drop down 
menu that is pre-populated with the following options: right, left, down, up. 
 
### mtch-move-steps

![mtch-move-steps](/images/fs3/language/mtch-move-steps.png)

The Move Steps block is used to express an assessment that verifies a sprite moves a certain 
number of steps. It takes one argument. The argument is of type integer and represent the 
number of steps.
 
### mtch-say

![mtch-say](/images/fs3/language/mtch-say.png)
 
The Say block is used to express an assessment that verifies the sprite says, or prints a message 
to the screen. It takes one argument. The argument is of type string and represents the 
message. 
 
### cnd-if-pass

![cnd-if-pass](/images/fs3/language/cnd-if-pass.png)

The block If Pass is used to express a trigger that is invoked if the assessment passes. It 
connects vertically to an expect or another trigger block. It connects horizontally to an action 
block.
 
### cnd-if-fail

![cnd-if-fail](/images/fs3/language/cnd-if-fail.png)

The block If Fail is used to express a trigger that is invoked if the assessment fails. It connects 
vertically to an expect or another trigger block. It connects horizontally to an action block.

### actn-say

![actn-say](/images/fs3/language/actn-say.png)
 
The Say block is used to say, or print a message on the dashboard if the previous trigger is 
invoked. It takes one argument. The argument is of data type string and represents the 
message that should be printed on the dashboard.
 
### actn-include-block

![actn-include-block](/images/fs3/language/actn-include-block.png)

The Include Block block is used to include one block on the Scratch palette builder if the 
previous trigger is invoked. It takes one argument. The argument is of data type string and 
represents the ID of the block that should be included.

### actn-exclude-blocks

![actn-exclude-blocks](/images/fs3/language/actn-exclude-blocks.png)
 
The Exclude Block block is used to exclude one block on the Scratch palette builder if the 
previous trigger is invoked. It takes one argument. The argument is of data type string and 
represents the ID of the block that should be excluded.
 
## Editor

The SAGE Objective Editor Language editor is implemented using HTML and JavaScript. It extends the 
Blockly Code editor example on the Blockly website (Google, 2016) by enabling users to upload 
assessments to the assessment server. When a user requests that an assessment be uploaded, 
the editor executes an HTTP POST request against the assessment server with the XML-encoded 
assessments as the HTTP request body.