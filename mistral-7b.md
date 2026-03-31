<div align="center">

<p><b>Table 1:</b> Efficiency evaluation on Mistral-7B-Instruct-v0.2 on NVIDIA A100 40G. Bit width is set at 2, residual length is set at
0, buffer size is set 64. BS is abbreviated for batch size. Mem is abbreviated for memory. </p>
  <table border="1" style="border-collapse: collapse; text-align: center;">
    <thead>
      <tr>
        <th rowspan="2">BS</th>
        <th rowspan="2">Seqlen</th>
        <th colspan="2">Ours</th>
        <th colspan="2">SKVQ</th>
        <th colspan="2">KIVI</th>
        <th colspan="2">FP16</th>
      </tr>
      <tr>
        <th>Mem</th>
        <th>Throughput</th>
        <th>Mem</th>
        <th>Throughput</th>
        <th>Mem</th>
        <th>Throughput</th>
        <th>Mem</th>
        <th>Throughput</th>
      </tr>
    </thead>
    <tbody>
      <tr><td rowspan="5">1</td><td>1K</td><td>13.54</td><td>19.56</td><td>14.06</td><td>1.30</td><td>13.55</td><td>15.45</td><td>13.64</td><td>48.97</td></tr>
      <tr><td>2K</td><td>13.58</td><td>18.35</td><td>14.11</td><td>1.29</td><td>13.59</td><td>15.48</td><td>13.78</td><td>46.48</td></tr>
      <tr><td>4K</td><td>13.66</td><td>11.42</td><td>14.23</td><td>2.55</td><td>13.67</td><td>14.83</td><td>14.06</td><td>41.65</td></tr>
      <tr><td>8K</td><td>13.82</td><td>6.90</td><td>14.45</td><td>21.65</td><td>13.85</td><td>14.08</td><td>14.62</td><td>32.27</td></tr>
      <tr><td>16K</td><td>14.13</td><td>4.14</td><td>14.90</td><td>16.87</td><td>14.19</td><td>11.35</td><td>15.70</td><td>23.42</td></tr>
      <tr><td rowspan="5">16</td><td>1K</td><td>14.25</td><td>70.53</td><td>15.02</td><td>258.80</td><td>14.33</td><td>158.54</td><td>15.75</td><td>440.26</td></tr>
      <tr><td>2K</td><td>14.85</td><td>38.24</td><td>15.92</td><td>175.79</td><td>15.01</td><td>138.59</td><td>18.00</td><td>311.13</td></tr>
      <tr><td>4K</td><td>16.13</td><td>19.71</td><td>17.73</td><td>105.62</td><td>16.36</td><td>119.18</td><td>22.50</td><td>194.14</td></tr>
      <tr><td>8K</td><td>18.69</td><td>9.85</td><td>21.36</td><td>12.84</td><td>19.02</td><td>96.14</td><td>31.51</td><td>108.42</td></tr>
      <tr><td>16K</td><td>23.81</td><td>4.92</td><td>28.36</td><td>9.72</td><td>24.22</td><td>74.61</td><td>OOM</td><td>OOM</td></tr>
      <tr><td rowspan="5">32</td><td>1K</td><td>15.20</td><td>126.95</td><td>16.02</td><td>36.98</td><td>15.12</td><td>300.71</td><td>18.00</td><td>611.97</td></tr>
      <tr><td>2K</td><td>16.54</td><td>68.83</td><td>17.84</td><td>32.85</td><td>16.52</td><td>273.00</td><td>22.50</td><td>385.91</td></tr>
      <tr><td>4K</td><td>19.43</td><td>35.48</td><td>21.46</td><td>25.05</td><td>19.15</td><td>189.62</td><td>31.50</td><td>218.95</td></tr>
      <tr><td>8K</td><td>25.18</td><td>17.73</td><td>28.72</td><td>18.59</td><td>24.51</td><td>75.50</td><td>OOM</td><td>OOM</td></tr>
      <tr><td>16K</td><td>36.71</td><td>8.85</td><td>OOM</td><td>OOM</td><td>35.23</td><td>22.80</td><td>OOM</td><td>OOM</td></tr>
    </tbody>
  </table>
</div>
