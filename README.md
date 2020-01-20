<link href="sarcasm.css" rel="stylesheet"></link>

# Sarcasm in its own right

Sarcasm is pervasive in business and casual conversation. Identifying sarcasm audibly is usually not too difficult. But sarcasm doesn't translate very well in emails, community forums and other online communications.

Why has it not been incorporated into the current HTML5/6 specification? Does sarcasm really warrant adding a tag like <code>&lt;sarcasm&gt;&lt;/sarcasm&gt;</code> into the accepted web standard? Yes.

I'm proposing that sarcasm be represented in a common format everyone can easily identify in digital communication. Sarcasm will be represented as a combination of two familiar text decorations <strong>"bold"</strong> and <em>"italic"</em>. Sarcasm will be visually differentiated from italics by slanting text in the opposite direction (backward slanting similar to the back slash). Combining the backward slant and bolding will further visually signify the text as sarcastic not italic.

Additionally, there are included styles for quotation marks that will appear before and after the sarcastic text. These are optional and intended for use if you feel that the backward slant and bolding are not sufficient. The color of the quotation marks is over-emphasized to reinforce the sarcasm. Again, if you feel the quotation marks are unnecessary, just comment out the appropriate before and after styles.


## Regular Sarcasm
![Regular Sarcasm](1.png "Image of Regular Sarcasm")

<pre>
.sarcasm-reg {
	font-weight:400;
	font-size: 1rem;
	color: #444;
    -moz-transform: skewX(7.5deg);
    -webkit-transform: skewX(7.5deg);
    -o-transform: skewX(7.5deg);
    -ms-transform: skewX(7.5deg);
    transform: skewX(7.5deg);
}
</pre>


## Heavy Sarcasm
![Heavy Sarcasm](2.png "Image of Heavy Sarcasm")

<pre>
.sarcasm-heavy {
	font-weight:700;
	font-size: 1rem;
	color: #444;
    -moz-transform: skewX(7.5deg);
    -webkit-transform: skewX(7.5deg);
    -o-transform: skewX(7.5deg);
    -ms-transform: skewX(7.5deg);
    transform: skewX(7.5deg);
}
</pre>



## Accented Sarcasm
![Accented Sarcasm](3.png "Image of Sarcastic Comment")
<pre>
.sarcastic {
	font-weight: 700;
	font-size: 1rem;
	color: #444;
    -moz-transform: skewX(7.5deg);
    -webkit-transform: skewX(7.5deg);
    -o-transform: skewX(7.5deg);
    -ms-transform: skewX(7.5deg);
    transform: skewX(7.5deg);
}
.sarcastic:before {
	content:open-quote;
	color: #ff0000;
	font-size: 1.25em;
	padding-right: .15em;
}
.sarcastic:after {
	content:close-quote;
	color: #ff0000;
	font-size: 1.25em;
	padding-left: .15em;
}
</pre>


## License
[MIT](LICENSE.md)


## Future Roadmap

+ Tweak text spacing - Complete
+ Enable on span elements - Complete
