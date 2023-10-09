# PLM synthetic data generator
This data set allows to evaluate PLM synthetic data generator provided by my research works.

A “Xbox demo” CAD Design authored by Ernesto FLORES in 2021 and downloaded from site <a href="https://grabcad.com/library/xbox-controller-solidworks-surfaces-1">https://grabcad.com/library/xbox-controller-solidworks-surfaces-1</a> has been loaded into PTC Windchill PDMLink. GrabCAD models are free for non-commercial public use as soon as the author and download URL are mentioned. 

The original data set has been built by a manual Bottom/Up approach. The first product has been saved 3 times by using “re-use” function during save-as. When “re-use” option is selected, save-as stop duplicating parts and links upper parts to non-duplicated part, thus creating components.

Several “kits” have been created; they connect top parts of products within a dense graph. This way produces a layer 3 data package graph (components, products, kits).

A pure graph export format has been selected in order be domain agnostic. Graphs are provided in GraphML format (Brandes et al., 2002) which can be manipulated by <a href="https://www.yworks.com/products/yed">YeD grapher software</a>

Data generator is applied on demonstration initial data and generated graph is provided. For both graphs, the same D6 multi-pass analysis is executed, 2 output graphs are provided. For all graphs, PDF prints are provided for convenience. 

Content is described in following table:

<table style="width: 100%">
	<tr>
		<th>Folder</th><th>Sub-Folded</th><th>File</th><th>Description</th>
	</tr>
	<!-- Original -->
	<tr>
		<td>Orginal</td><td colspan="2"/><td>Original data set</td>
	</tr>
	<tr>
		<td/>
		<td>input-data-graph</td>
		<td>original-data.graphml<br/>original-data-withGraphLayout.pdf</td>
		<td>Original data set in GraphML format<br/>Convenience PDF print</td>
	</tr>
	<tr>
		<td/>
		<td>D6-analysis</td>
		<td>original-D6-analysis.graphml<br/>original-D6-analysis.pdf</td>
		<td>Original data set analysed by D6, inGraphML format<br/>Convenience PDF print</td>
	</tr>
	<!-- Generated -->
	<tr>
		<td>Generated</td><td colspan="2"/><td>Generated data set</td>
	</tr>
	<tr>
		<td/>
		<td>input-data-graph</td>
		<td>generated-data.graphml<br/>generated-data-withGraphLayout.pdf</td>
		<td>Generated data set in GraphML format<br/>Convenience PDF print</td>
	</tr>
	<tr>
		<td/>
		<td>D6-analysis</td>
		<td>generated-D6-analysis.graphml<br/>Original data set analysed by D6, in GraphML format</td>
		<td>Original data set analysed by D6, in GraphML format<br/>Convenience PDF print</td>
	</tr>
</table>

## Bibliography

Brandes, U., Eiglsperger, M., Herman, I., Himsolt, M., Marshall, M.S., 2002. GraphML Progress Report Structural Layer Proposal, in: Mutzel, P., Jünger, M., Leipert, S. (Eds.), Graph Drawing,<br/> 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Lecture Notes in Computer Science. Springer Berlin Heidelberg, Berlin, Heidelberg, pp. 501–512. https://doi.org/10.1007/3-540-45848-4_59
