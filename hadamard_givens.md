<div align="center">

<p align="left" style="width: 80%; margin: auto;">
  <b>Table 3:</b> Ablation study of different transformation and smoothing components on the <b>Llama-2-7B-hf</b> model. 
  Perplexity (PPL) is evaluated on the <b>WikiText-2</b> dataset with <b>4-bit</b> KV cache quantization. 
  Hyper-parameters are fixed at <b>buffer size = 64</b>, <b>group size = 64</b>, and <b>residual window = 0</b>. 
  The configuration with both Hadamard and Givens transformations (Smooth Factor 2.5) achieves the optimal PPL.
</p>

<table border="1" style="border-collapse: collapse; text-align: center; width: 85%; margin-top: 10px;">
  <thead>
    <tr style="background-color: #f8f9fa;">
      <th style="padding: 12px;">Method Components</th>
      <th>1</th>
      <th style="background-color: #fff3e0;">2 (Best)</th>
      <th>3</th>
      <th>4</th>
      <th>5</th>
      <th>6</th>
      <th>7</th>
      <th>8</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="left" style="padding: 10px; font-weight: 500;">Use Hadamard</td>
      <td>✓</td>
      <td style="background-color: #fff3e0;">✓</td>
      <td>✗</td>
      <td>✗</td>
      <td>✗</td>
      <td>✗</td>
      <td>✗</td>
      <td>✗</td>
    </tr>
    <tr>
      <td align="left" style="padding: 10px; font-weight: 500;">Use Givens</td>
      <td>✗</td>
      <td style="background-color: #fff3e0;">✓</td>
      <td>✓</td>
      <td>✓</td>
      <td>✓</td>
      <td>✓</td>
      <td>✓</td>
      <td>✗</td>
    </tr>
    <tr>
      <td align="left" style="padding: 10px; font-weight: 500;">Smooth Factor</td>
      <td>-</td>
      <td style="background-color: #fff3e0;">2.5</td>
      <td>2.5</td>
      <td>3.5</td>
      <td>4.5</td>
      <td>5.5</td>
      <td>6.5</td>
      <td>-</td>
    </tr>
    <tr style="border-top: 2px solid #333; font-weight: bold;">
      <td align="left" style="padding: 10px; background-color: #f8f9fa;">PPL (WikiText-2) </td>
      <td>5.133</td>
      <td style="color: #d32f2f; background-color: #ffebee;">5.131</td>
      <td>5.139</td>
      <td>5.137</td>
      <td>5.138</td>
      <td>5.138</td>
      <td>5.139</td>
      <td>5.139</td>
    </tr>
  </tbody>
</table>

</div>
