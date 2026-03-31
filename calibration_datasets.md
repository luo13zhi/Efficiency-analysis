<div align="center">

<p align="left" style="width: 85%; margin: auto; line-height: 1.5;">
  <b>Table R6:</b> Perplexity comparison among different calibration datasets on Llama-2-7B-hf model. 
  Bit width is set at 4 and residual length is set at 0 for all datasets. 
  Calibration is performed with sample len = 4096 and nsample = 256.
</p>

<table border="1" style="border-collapse: collapse; text-align: center; width: 85%; margin-top: 12px; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;">
  <thead>
    <tr style="background-color: #f8f9fa; border-bottom: 2px solid #444;">
      <th style="padding: 12px;">Calibration Dataset</th>
      <th style="padding: 12px;">Wikitext PPL</th>
      <th style="padding: 12px;">PTB PPL</th>
      <th style="padding: 12px;">C4 PPL</th>
      <th style="padding: 12px; background-color: #f1f3f4;">Average PPL</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="font-weight: bold; background-color: #fdfdfe;">Wikitext</td>
      <td >5.131</td>
      <td>28.980</td>
      <td>6.774</td>
      <td >13.63</td>
    </tr>
    <tr>
      <td style="font-weight: bold; background-color: #fdfdfe;">PTB</td>
      <td>5.135</td>
      <td >29.490</td>
      <td>6.773</td>
      <td >13.80</td>
    </tr>
    <tr>
      <td style="font-weight: bold; background-color: #fdfdfe;">C4</td>
      <td>5.131</td>
      <td>29.240</td>
      <td >6.772</td>
      <td >13.71</td>
    </tr>
  </tbody>
</table>

</div>
