Universal Character Set 
=======================
This is an extract from [wikipedia](https://en.wikipedia.org/wiki/Universal_Character_Set_characters).

see also:   
Unicode 13.0 Character Code [Charts]( https://unicode.org/charts/ )



## Unicode Blocks

Unicode adds a block property to UCS that further divides each plane into separate blocks. Each block is a grouping of characters by their use such as "mathematical operators" or "Hebrew script characters". When assigning characters to previously unassigned code points, the Consortium typically allocates entire blocks of similar characters: for example all the characters belonging to the same script or all similarly purposed symbols get assigned to a single block. Blocks may also maintain unassigned or reserved code points when the Consortium expects a block to require additional assignments.

The first 256 code points in the UCS correspond with those of ISO 8859-1, the most popular 8-bit character encoding in the Western world. As a result, the first 128 characters are also identical to *ASCII*. Though Unicode refers to these as a Latin script block, these two blocks contain many characters that are commonly useful outside of the Latin script. In general, not all characters in a given block need be of the same script, and a given script can occur in several different blocks. 

## Character reference overview in HTML or XML 

See also: 
: [character entity]( https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references ) a List of XML and HTML character entity references Unicode input
: [Unicode input]( https://en.wikipedia.org/wiki/Unicode_input ) 
is the insertion method, of a specific Unicode character, on a computer by a user;

An HTML or XML numeric character reference refers to a character by its Universal Character Set/Unicode code point, and uses the decimal format:

    	&#nnnn;

or in the exadecimal format:

    	&#xhhhh;

where `nnnn` is the code point in decimal form, and `hhhh` is the code point in hexadecimal form. The `x` must be lowercase in XML documents. The `nnnn` or `hhhh` may be any number of digits and may include leading zeros. The `hhhh` may mix uppercase and lowercase, though **uppercase** is the usual style.

In contrast, a character *entity* reference refers to a character by the name of an entity which has the desired character as its replacement text. 
The entity must either be predefined (built into the markup language) or explicitly declared in a *Document Type Definition* (DTD). 
The format is the same as for any entity reference:

    	&name;

where `name` is the case-sensitive name of the entity. The semicolon is required. 



## *Unicode block* - Box Drawing

UTF-8 characters in the *Box Drawing Unicode block*.
They can be generated in browser and Markdown with the HTML command: `&#xNNNN;`, where `NNNN` is a four digit exadecimal in the range `[2500..257F]`.

>Unicode Block  
>: *Category*:	Box Drawing  
>: From: 	U+2500  
>: To: 		U+257F  
>: \#chars:(128)  

```
        0x00 0x01 0x02 0x03 0x04 0x05 0x06 0x07	0x08 0x09 0x0A 0x0B 0x0C 0x0D 0x0E 0x0F
				  
0x2500  ─    ━    │    ┃    ┄    ┅    ┆    ┇    ┈    ┉    ┊    ┋    ┌    ┍    ┎    ┏

0x2510 	┐    ┑    ┒    ┓    └    ┕    ┖    ┗    ┘    ┙    ┚    ┛    ├    ┝    ┞    ┟

0x2520 	┠    ┡    ┢    ┣    ┤    ┥    ┦    ┧    ┨    ┩    ┪    ┫    ┬    ┭    ┮    ┯

0x2530 	┰    ┱    ┲    ┳    ┴    ┵    ┶    ┷    ┸    ┹    ┺    ┻    ┼    ┽    ┾    ┿

0x2540 	╀    ╁    ╂    ╃    ╄    ╅    ╆    ╇    ╈    ╉    ╊    ╋    ╌    ╍    ╎    ╏

0x2550 	═    ║    ╒    ╓    ╔    ╕    ╖    ╗    ╘    ╙    ╚    ╛    ╜    ╝    ╞    ╟

0x2560 	╠    ╡    ╢    ╣    ╤    ╥    ╦    ╧    ╨    ╩    ╪    ╫    ╬    ╭    ╮    ╯

0x2570 	╰    ╱    ╲    ╳    ╴    ╵    ╶    ╷    ╸    ╹    ╺    ╻    ╼    ╽    ╾    ╿

```

## *Unicode block* - Supplemental Mathematical Operators

```
        0	1	2	3	4	5	6	7	8	9	A	B	C	D	E	F
		
U+270x  ✀ 	✁ 	✂ 	✃ 	✄ 	✅ 	✆ 	✇ 	✈ 	✉ 	✊ 	✋ 	✌ 	✍ 	✎ 	✏
U+271x 	✐ 	✑ 	✒ 	✓ 	✔ 	✕ 	✖ 	✗ 	✘ 	✙ 	✚ 	✛ 	✜ 	✝ 	✞ 	✟
U+272x 	✠ 	✡ 	✢ 	✣ 	✤ 	✥ 	✦ 	✧ 	✨ 	✩ 	✪ 	✫ 	✬ 	✭ 	✮ 	✯
U+273x 	✰ 	✱ 	✲ 	✳ 	✴ 	✵ 	✶ 	✷ 	✸ 	✹ 	✺ 	✻ 	✼ 	✽ 	✾ 	✿
U+274x 	❀ 	❁ 	❂ 	❃ 	❄ 	❅ 	❆ 	❇ 	❈ 	❉ 	❊ 	❋ 	❌ 	❍ 	❎ 	❏
U+275x 	❐ 	❑ 	❒ 	❓ 	❔ 	❕ 	❖ 	❗ 	❘ 	❙ 	❚ 	❛ 	❜ 	❝ 	❞ 	❟
U+276x 	❠ 	❡ 	❢ 	❣ 	❤ 	❥ 	❦ 	❧ 	❨ 	❩ 	❪ 	❫ 	❬ 	❭ 	❮ 	❯
U+277x 	❰ 	❱ 	❲ 	❳ 	❴ 	❵ 	❶ 	❷ 	❸ 	❹ 	❺ 	❻ 	❼ 	❽ 	❾ 	❿
U+278x 	➀ 	➁ 	➂ 	➃ 	➄ 	➅ 	➆ 	➇ 	➈ 	➉ 	➊ 	➋ 	➌ 	➍ 	➎ 	➏
U+279x 	➐ 	➑ 	➒ 	➓ 	➔ 	➕ 	➖ 	➗ 	➘ 	➙ 	➚ 	➛ 	➜ 	➝ 	➞ 	➟
U+27Ax 	➠ 	➡ 	➢ 	➣ 	➤ 	➥ 	➦ 	➧ 	➨ 	➩ 	➪ 	➫ 	➬ 	➭ 	➮ 	➯
U+27Bx 	➰ 	➱ 	➲ 	➳ 	➴ 	➵ 	➶ 	➷ 	➸ 	➹ 	➺ 	➻ 	➼ 	➽ 	➾ 	➿
```

        
```   
        0	1	2	3	4	5	6	7	8	9	A	B	C	D	E	F
		
U+2A0x  ⨀	⨁	⨂ 	⨃ 	⨄ 	⨅ 	⨆ 	⨇ 	⨈ 	⨉ 	⨊ 	⨋ 	⨌ 	⨍ 	⨎ 	⨏
U+2A1x  ⨐	⨑	⨒	⨓	⨔	⨕	⨖	⨗	⨘	⨙	⨚	⨛	⨜	⨝	⨞	⨟
U+2A2x  ⨠	⨡	⨢	⨣	⨤	⨥	⨦	⨧	⨨	⨩	⨪	⨫	⨬	⨭	⨮	⨯
U+2A3x  ⨰	⨱	⨲	⨳	⨴	⨵	⨶	⨷	⨸	⨹	⨺	⨻	⨼	⨽	⨾	⨿
U+2A4x  ⩀	⩁	⩂	⩃	⩄	⩅	⩆	⩇	⩈	⩉	⩊	⩋	⩌	⩍	⩎	⩏
U+2A5x  ⩐	⩑	⩒	⩓	⩔	⩕	⩖	⩗	⩘	⩙	⩚	⩛	⩜	⩝	⩞	⩟
U+2A6x  ⩠	⩡	⩢	⩣	⩤	⩥	⩦	⩧	⩨	⩩	⩪	⩫	⩬	⩭	⩮	⩯
U+2A7x  ⩰	⩱	⩲	⩳	⩴	⩵	⩶	⩷	⩸	⩹	⩺	⩻	⩼	⩽	⩾	⩿
U+2A8x  ⪀	⪁	⪂	⪃	⪄	⪅	⪆	⪇	⪈	⪉	⪊	⪋	⪌	⪍	⪎	⪏
U+2A9x  ⪐	⪑	⪒	⪓	⪔	⪕	⪖	⪗	⪘	⪙	⪚	⪛	⪜	⪝	⪞	⪟
U+2AAx  ⪠	⪡	⪢	⪣	⪤	⪥	⪦	⪧	⪨	⪩	⪪	⪫	⪬	⪭	⪮	⪯
U+2ABx  ⪰	⪱	⪲	⪳	⪴	⪵	⪶	⪷	⪸	⪹	⪺	⪻	⪼	⪽	⪾	⪿
U+2ACx  ⫀	 ⫁	⫂	⫃	⫄	⫅	⫆	⫇	⫈	⫉	⫊	⫋	⫌	⫍	⫎	⫏
U+2ADx  ⫐	⫑	⫒	⫓	⫔	⫕	⫖	⫗	⫘	⫙	⫚	⫛	⫝̸	⫝	⫞	⫟
U+2AEx  ⫠ 	⫡ 	⫢ 	⫣ 	⫤	⫥	⫦	⫧	⫨	⫩	⫪	⫫	⫬	⫭	⫮	⫯
U+2AFx  ⫰ 	⫱ 	⫲ 	⫳ 	⫴	⫵	⫶	⫷	⫸	⫹	⫺	⫻	⫼	⫽	⫾	⫿ 

```

## *Unicode block* - Geometric shapes

```
        0	1	2	3	4	5	6	7	8	9	A	B	C	D	E	F
U+25Ax 	■ 	□ 	▢ 	▣ 	▤ 	▥ 	▦ 	▧ 	▨ 	▩ 	▪ 	▫ 	▬ 	▭ 	▮ 	▯
U+25Bx 	▰ 	▱ 	▲ 	△ 	▴ 	▵ 	▶ 	▷ 	▸ 	▹ 	► 	▻ 	▼ 	▽ 	▾ 	▿
U+25Cx 	◀ 	◁ 	◂ 	◃ 	◄ 	◅ 	◆ 	◇ 	◈ 	◉ 	◊ 	○ 	◌ 	◍ 	◎ 	●
U+25Dx 	◐ 	◑ 	◒ 	◓ 	◔ 	◕ 	◖ 	◗ 	◘ 	◙ 	◚ 	◛ 	◜ 	◝ 	◞ 	◟
U+25Ex 	◠ 	◡ 	◢ 	◣ 	◤ 	◥ 	◦ 	◧ 	◨ 	◩ 	◪ 	◫ 	◬ 	◭ 	◮ 	◯
U+25Fx 	◰ 	◱ 	◲ 	◳ 	◴ 	◵ 	◶ 	◷ 	◸ 	◹ 	◺ 	◻ 	◼ 	◽  ◾  ◿

```

## *Unicode block* - 

```


```

## *Unicode block* - 

```


```
## Samples - 

─ ⟶  🠆🡢⯈ ⟶ ⭢ →◌⃔ 

```
	┌───┐
	┢━━━┷━━━━━━━┓
	┃           ┃
	┃           ┃
	┃           ┃
	┗━━━━━━━━━━━┛
```

 ```	
        ⌠₅⁷ ᵉ
      🡪 ⎪  x²
        ⌡₁ 
```



