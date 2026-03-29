<div align="center">

<p align="left" style="width: 85%; margin: auto; line-height: 1.5;">
  <b>Table 4:</b> Performance scaling analysis of buffer size on the Qwen2.5-7B-Instruct model. 
  Experiments are conducted under 2-bit KV cache quantization with a fixed residual window = 64. 
  Throughput (tokens/s) and Peak Memory (GB) are reported across various sequence lengths (2K and 4K) to evaluate the efficiency of the proposed buffering strategy.
</p>

<table border="1" style="border-collapse: collapse; text-align: center; width: 85%; margin-top: 12px; font-family: sans-serif;">
  <thead>
    <tr style="background-color: #f1f3f4; border-bottom: 2px solid #333;">
      <th style="padding: 12px;">Seqlen</th>
      <th style="padding: 12px;">Metric</th>
      <th>BS=0</th>
      <th>BS=16</th>
      <th>BS=32</th>
      <th>BS=64</th>
      <th>BS=128</th>
      <th>BS=256</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2" style="font-weight: bold; background-color: #f8f9fa;">2K</td>
      <td align="left" style="padding: 8px;">Throughput (↑)</td>
      <td>38.27</td>
      <td>212.30</td>
      <td>253.35</td>
      <td>279.14</td>
      <td>291.70</td>
      <td>299.66</td>
    </tr>
    <tr>
      <td align="left" style="padding: 8px;">Memory Peak (GB)</td>
      <td>16.98</td>
      <td>16.98</td>
      <td>17.01</td>
      <td>16.98</td>
      <td>17.05</td>
      <td>16.99</td>
    </tr>
    <tr style="border-top: 2px solid #ccc;">
      <td rowspan="2" style="font-weight: bold; background-color: #f8f9fa;">4K</td>
      <td align="left" style="padding: 8px;">Throughput (↑)</td>
      <td>26.43</td>
      <td>145.28</td>
      <td>165.59</td>
      <td>171.76</td>
      <td>169.36</td>
      <td>163.57</td>
    </tr>
    <tr>
      <td align="left" style="padding: 8px;">Memory Peak (GB)</td>
      <td>19.24</td>
      <td>19.22</td>
      <td>19.26</td>
      <td>19.26</td>
      <td>19.34</td>
      <td>19.28</td>
    </tr>
  </tbody>
</table>

</div>
