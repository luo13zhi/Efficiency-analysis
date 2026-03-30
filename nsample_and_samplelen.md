<div align="center">

<p align="left" style="width: 85%; margin: auto; line-height: 1.5;">
  <b>Table 5:</b> Ablation study of sample length and nsample (number of samples) on Llama-2-7B-hf perplexity (PPL). 
  Evaluated on the WikiText-2 dataset. The table is divided into two control groups to study the impact of calibration setting on quantization performance.
</p>

<table border="1" style="border-collapse: collapse; text-align: center; width: 85%; margin-top: 12px;">
  <thead>
    <tr style="background-color: #f2f2f2; border-bottom: 2px solid #333;">
      <th style="padding: 10px;">Group</th>
      <th style="padding: 10px;">Variable</th>
      <th colspan="7">Wikitext2 PPL</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2" style="font-weight: bold; background-color: #f9f9f9;">Group A<br>nsample=256</td>
      <td style="padding: 8px; background-color: #f9f9f9;">sample len</td>
      <td>64</td>
      <td>128</td>
      <td>256</td>
      <td>512</td>
      <td>1024</td>
      <td>2048</td>
      <td>4096</td>
    </tr>
    <tr>
      <td style="padding: 8px;">PPL</td>
      <td>5.130</td>
      <td>5.132</td>
      <td>5.132</td>
      <td>5.132</td>
      <td>5.131</td>
      <td>5.131</td>
      <td>5.131</td>
    </tr>
    <tr style="border-top: 2px solid #ccc;">
      <td rowspan="2" style="font-weight: bold; background-color: #f9f9f9;">Group B<br>sample len=4096</td>
      <td style="padding: 8px; background-color: #f9f9f9;">nsample</td>
      <td>32</td>
      <td>64</td>
      <td>128</td>
      <td>256</td>
      <td>512</td>
      <td>1024</td>
      <td style="background-color: #eee; color: #999;">-</td>
    </tr>
    <tr>
      <td style="padding: 8px;">PPL</td>
      <td>5.134</td>
      <td>5.133</td>
      <td>5.133</td>
      <td>5.131</td>
      <td>5.131</td>
      <td>5.130</td>
      <td style="background-color: #eee; color: #999;">-</td>
    </tr>
  </tbody>
</table>

</div>
