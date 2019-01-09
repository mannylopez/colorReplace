# colorReplace

## Notes
January 07, 2019
10:19 PM
# colorReplace project

<tr>
	<td class="wysiwyg-text-align-center highlight-red" colspan="1" data-highlight-colour="red">
		<br/>
	</td>
		<td class="wysiwyg-text-align-center" colspan="1">
	<br/>
	</td>
</tr>



<tr>
	<td class="wysiwyg-text-align-center" style="width: 5.0%;text-align: center;vertical-align: top;background-color: rgb(174,214,241);">
		<span class="wysiwyg-color-black wysiwyg-font-size-medium">1.1</span>
	</td>
	<td class="wysiwyg-text-align-center" style="width: 95.0%;text-align: left;vertical-align: top;background-color: rgb(247,247,247);">
		<p>Sub-step one-one. </p>
	</td>
</tr>

replace 
	data-highlight-colour="red"
with
	style="background-color: rgb(174,214,241);"


while read a ; do echo ${a//data-highlight-colour="red"/style="background-color: rgb(174,214,241);"} ; done < 001.html > 001.html.t ; mv 001.html{.t,}


while read a ; do echo ${a//abc/XYZ} ; done < 001.html > 001.html.t ; mv 001.html{.t,}



sed -i -e 's/XYZ/123/g' 001.html

sed -i -e 's/data-highlight-colour="green"/style="background-color: rgb(174,214,241);"/g' 001.html

# Yellow
sed -i -e 's/data-highlight-colour="yellow"/style="background-color: rgb(249,231,159);"/g' 001.html

# Red
sed -i -e 's/data-highlight-colour="red"/style="background-color: rgb(245,183,177);"/g' 001.html

# Green
sed -i -e 's/data-highlight-colour="green"/style="background-color: rgb(171,235,198);"/g' 001.html

# Blue
sed -i -e 's/data-highlight-colour="blue"/style="background-color: rgb(174,214,241);"/g' 001.html

# Grey
sed -i -e 's/data-highlight-colour="grey"/style="background-color: rgb(247,247,247);"/g' 001.html


# Multiple at once (with blue and grey)

sed -i -e 's/data-highlight-colour="blue"/style="background-color: rgb(174,214,241);"/g;s/data-highlight-colour="grey"/style="background-color: rgb(247,247,247);"/g' 001.html

# Multiple with all colors
sed -i -e 's/data-highlight-colour="yellow"/style="background-color: rgb(249,231,159);"/g;s/data-highlight-colour="red"/style="background-color: rgb(245,183,177);"/g;s/data-highlight-colour="green"/style="background-color: rgb(171,235,198);"/g;s/data-highlight-colour="blue"/style="background-color: rgb(174,214,241);"/g;s/data-highlight-colour="grey"/style="background-color: rgb(247,247,247);"/g' 001.html



```
sed -i -e 's/data-highlight-colour="yellow"/style="background-color: rgb(249,231,159);"/g;s/data-highlight-colour="red"/style="background-color: rgb(245,183,177);"/g;s/data-highlight-colour="green"/style="background-color: rgb(171,235,198);"/g;s/data-highlight-colour="blue"/style="background-color: rgb(174,214,241);"/g;s/data-highlight-colour="grey"/style="background-color: rgb(247,247,247);"/g' 001.html
```