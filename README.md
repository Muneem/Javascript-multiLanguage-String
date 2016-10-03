# Javascript-multiLanguage-String
In javascript if you want to concatenate multilanguage string like there comes ARABIC text in english sentence or there comes ENGLISH word in ARABIC sentnce then you have to explicitly tell the compiler that these texts are being treated as embedded from left-to-right text or vicevers.

If you want left-to-right embedding then you have to use following format for that

var String  = '\u202A'+ARABICSTRING+'\u202C'+ENGLISHSTRING.
u202A = LEFT-TO-RIGHT EMBEDDING. Treat the following text as embedded left to right
u202C = End scope. This indicates end of embedded text.

and for RIght-to-left embedding 

var String  = '\u202B'+EnglishString+'\u202C'+ArabicString.
u202B = RIGHT-TO-LEFT EMBEDDING. Treat the following text as embedded left to right
u202C = End scope. This indicates end of embedded text.

You can further read about this embeddng by clicking on following link
http://unicode.org/reports/tr9/#Directional_Formatting_Codes


