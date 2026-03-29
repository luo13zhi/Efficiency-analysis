<div align="center">

<p><b>Table 1: Efficiency evaluation on Llama-3.1-8B-Instruct on NVIDIA A100 40G. Bit width is set at 2, residual length is set at
0, buffer size is set 64. BS is abbreviated for batch size. Mem is abbreviated for memory. </p>

<table border="1">
  <thead>
    <tr align="center">
      <th rowspan="2">BS</th>
      <th rowspan="2">Seqlen</th>
      <th colspan="2">Ours</th>
      <th colspan="2">KIVI</th>
      <th colspan="2">SKVQ</th>
    </tr>
    <tr align="center">
      <th>Mem</th>
      <th>Throughput</th>
      <th>Mem</th>
      <th>Throughput</th>
      <th>Mem</th>
      <th>Throughput</th>
    </tr>
  </thead>
  <tbody align="center">
    <tr>
      <td rowspan="5">1</td>
      <td>1K</td><td>15.01</td><td>2.75</td><td>15.01</td><td>18.44</td><td>15.01</td><td>5.11</td>
    </tr>
    <tr><td>2K</td><td>15.06</td><td>8.84</td><td>15.06</td><td>17.81</td><td>15.06</td><td>5.03</td></tr>
    <tr><td>4K</td><td>15.15</td><td>7.95</td><td>15.14</td><td>18.80</td><td>15.15</td><td>4.71</td></tr>
    <tr><td>8K</td><td>15.31</td><td>6.78</td><td>15.32</td><td>16.35</td><td>15.33</td><td>2.08</td></tr>
    <tr><td>16K</td><td>15.65</td><td>3.97</td><td>15.66</td><td>13.67</td><td>15.67</td><td>0.76</td></tr>
    <tr style="border-top: 2px solid #ccc;">
      <td rowspan="5">16</td>
      <td>1K</td><td>15.77</td><td>66.22</td><td>15.79</td><td>204.72</td><td>15.81</td><td>110.99</td>
    </tr>
    <tr><td>2K</td><td>16.44</td><td>38.57</td><td>16.46</td><td>146.71</td><td>16.46</td><td>89.91</td></tr>
    <tr><td>4K</td><td>17.81</td><td>20.17</td><td>17.81</td><td>103.33</td><td>17.83</td><td>63.44</td></tr>
    <tr><td>8K</td><td>20.48</td><td>10.05</td><td>20.48</td><td>52.15</td><td>20.50</td><td>31.22</td></tr>
    <tr><td>16K</td><td>25.89</td><td>8.91</td><td>25.90</td><td>24.88</td><td>25.90</td><td>14.50</td></tr>
    <tr style="border-top: 2px solid #ccc;">
      <td rowspan="5">32</td>
      <td>1K</td><td>16.56</td><td>44.97</td><td>16.61</td><td>334.76</td><td>16.56</td><td>353.65</td>
    </tr>
    <tr><td>2K</td><td>17.93</td><td>39.09</td><td>17.96</td><td>237.95</td><td>17.94</td><td>201.22</td></tr>
    <tr><td>4K</td><td>20.56</td><td>20.80</td><td>20.56</td><td>115.40</td><td>20.57</td><td>98.45</td></tr>
    <tr><td>8K</td><td>25.92</td><td>12.93</td><td>25.93</td><td>58.20</td><td>25.93</td><td>45.10</td></tr>
    <tr><td>16K</td><td>36.54</td><td>11.85</td><td>36.54</td><td>28.15</td><td>36.56</td><td>21.30</td></tr>
  </tbody>
</table>

</div>
