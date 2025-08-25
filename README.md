
# tidy-tuesday

Repository for lab hacky hours

## 2025-08-26

### Visualizing flounder MSE metrics

Visualize results of the summer flounder MSE using a common results data
frame, in `data/MSE_median_metrics.rds`.

#### Data Dictionary

<table style="width:99%;">
<colgroup>
<col style="width: 7%" />
<col style="width: 13%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr>
<th>Variable</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>om</td>
<td>NA</td>
<td>not used</td>
</tr>
<tr>
<td>mp</td>
<td>character</td>
<td>Management Procedure. One of four candidate MPs:<br />
“BBM” - biomass-based matrix<br />
“BRP” - biological reference point<br />
“NCA” - no change approach<br />
“PCA” - percent change approach</td>
</tr>
<tr>
<td>metric</td>
<td>character</td>
<td><p>Name of performance metric or regulation. One of 22 values:</p>
<p>“bag” - bag limit (number of fish)<br />
“change_cs” - overall change in consumer surplus<br />
“cs_per_trip” - consumer surplus per trip<br />
“exp_keep” - expected number of fish kept<br />
“expense” - total recreational fishing costs<br />
“keep_one” - probability of a trip with at least one keeper<br />
“keep_to_exp” - number of kept fish compared to expected<br />
“kept per trip” - number of kept fish per trip<br />
“kept:released” - ratio of number of kept fish to numbers released<br />
“minlen” - minimum size limit (inches)<br />
“mulen_keep” - mean length of kept fish<br />
“mulen_release” - mean length of released fish<br />
“not overfished” - probability that the stock is not overfished (i.e
P(SSB&gt;0.5 BMSY) )<br />
“not overfishing” - probability that overfishing is not occurring
(i.e. P(F &lt; FMSY) )<br />
“ntrips” - total number of recreational fishing trips<br />
“prop_female” - proportion of the stock that are female fish<br />
“rec_removals” - total recreational removals (number of fish)<br />
“rel per trip” - number of fish released per trip<br />
“seaslen” - season length (days)<br />
“spawning biomass” - magnitude of spawning stock biomass<br />
“total catch” - total catch (from both commercial and
recreational)<br />
“trophy” - probability that a trip includes a large ‘trophy size’
fish.</p></td>
</tr>
<tr>
<td>value</td>
<td>numeric (real number)</td>
<td>Median (over simulations) value for the performance metric</td>
</tr>
<tr>
<td>StartBBMSY</td>
<td>numeric (real number)</td>
<td><p>Value for the scenario stock status relative to BMSY at the start
of the projection period in the simulations. One of three values:<br />
1.0 - (base case, stock starts the simulations around B/BMSY)</p>
<p>2.0 - (stock starts above BMSY)</p>
<p>0.3 - (stock starts close to the overfished limit)</p></td>
</tr>
</tbody>
</table>
