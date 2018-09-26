

```python
import FinanceDataReader as fdr

df  = fdr.DataReader('KS11', '2000', '2016')
dfm = df.resample('BMS').first()
dfm.head(20)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Close</th>
      <th>Open</th>
      <th>High</th>
      <th>Low</th>
      <th>Volume</th>
      <th>Change</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2000-12-01</th>
      <td>504.62</td>
      <td>509.09</td>
      <td>509.95</td>
      <td>501.64</td>
      <td>252890000.0</td>
      <td>0.0080</td>
    </tr>
    <tr>
      <th>2001-01-01</th>
      <td>520.95</td>
      <td>503.31</td>
      <td>521.34</td>
      <td>500.97</td>
      <td>231010000.0</td>
      <td>0.0324</td>
    </tr>
    <tr>
      <th>2001-02-01</th>
      <td>612.30</td>
      <td>606.49</td>
      <td>620.78</td>
      <td>605.42</td>
      <td>396010000.0</td>
      <td>-0.0091</td>
    </tr>
    <tr>
      <th>2001-03-01</th>
      <td>559.44</td>
      <td>574.61</td>
      <td>574.61</td>
      <td>557.20</td>
      <td>329690000.0</td>
      <td>-0.0323</td>
    </tr>
    <tr>
      <th>2001-04-02</th>
      <td>515.20</td>
      <td>520.56</td>
      <td>522.09</td>
      <td>512.40</td>
      <td>231820000.0</td>
      <td>-0.0153</td>
    </tr>
    <tr>
      <th>2001-05-01</th>
      <td>583.70</td>
      <td>586.27</td>
      <td>587.18</td>
      <td>580.39</td>
      <td>594620000.0</td>
      <td>0.0110</td>
    </tr>
    <tr>
      <th>2001-06-01</th>
      <td>607.07</td>
      <td>615.67</td>
      <td>617.09</td>
      <td>603.84</td>
      <td>358790000.0</td>
      <td>-0.0083</td>
    </tr>
    <tr>
      <th>2001-07-02</th>
      <td>596.74</td>
      <td>593.03</td>
      <td>598.24</td>
      <td>592.90</td>
      <td>201670000.0</td>
      <td>0.0027</td>
    </tr>
    <tr>
      <th>2001-08-01</th>
      <td>562.79</td>
      <td>546.30</td>
      <td>563.67</td>
      <td>542.00</td>
      <td>441170000.0</td>
      <td>0.0392</td>
    </tr>
    <tr>
      <th>2001-09-03</th>
      <td>541.83</td>
      <td>545.02</td>
      <td>547.63</td>
      <td>539.17</td>
      <td>415210000.0</td>
      <td>-0.0060</td>
    </tr>
    <tr>
      <th>2001-10-01</th>
      <td>500.64</td>
      <td>498.87</td>
      <td>501.22</td>
      <td>494.76</td>
      <td>547900000.0</td>
      <td>0.0437</td>
    </tr>
    <tr>
      <th>2001-11-01</th>
      <td>544.09</td>
      <td>540.63</td>
      <td>546.12</td>
      <td>536.20</td>
      <td>461560000.0</td>
      <td>0.0117</td>
    </tr>
    <tr>
      <th>2001-12-03</th>
      <td>650.66</td>
      <td>643.61</td>
      <td>654.00</td>
      <td>631.87</td>
      <td>888590000.0</td>
      <td>0.0105</td>
    </tr>
    <tr>
      <th>2002-01-01</th>
      <td>724.95</td>
      <td>698.00</td>
      <td>725.06</td>
      <td>690.36</td>
      <td>618720000.0</td>
      <td>0.0450</td>
    </tr>
    <tr>
      <th>2002-02-01</th>
      <td>742.42</td>
      <td>757.07</td>
      <td>761.85</td>
      <td>739.15</td>
      <td>758400000.0</td>
      <td>-0.0076</td>
    </tr>
    <tr>
      <th>2002-03-01</th>
      <td>834.21</td>
      <td>842.21</td>
      <td>847.39</td>
      <td>834.21</td>
      <td>621760000.0</td>
      <td>0.0173</td>
    </tr>
    <tr>
      <th>2002-04-01</th>
      <td>875.83</td>
      <td>900.47</td>
      <td>900.47</td>
      <td>874.90</td>
      <td>489780000.0</td>
      <td>-0.0221</td>
    </tr>
    <tr>
      <th>2002-05-01</th>
      <td>859.86</td>
      <td>855.41</td>
      <td>860.72</td>
      <td>844.20</td>
      <td>695010000.0</td>
      <td>0.0208</td>
    </tr>
    <tr>
      <th>2002-06-03</th>
      <td>804.93</td>
      <td>793.53</td>
      <td>807.15</td>
      <td>787.04</td>
      <td>566880000.0</td>
      <td>0.0107</td>
    </tr>
    <tr>
      <th>2002-07-01</th>
      <td>746.23</td>
      <td>722.58</td>
      <td>750.60</td>
      <td>720.70</td>
      <td>430080000.0</td>
      <td>0.0047</td>
    </tr>
  </tbody>
</table>
</div>



# 참고 자료
* http://pandas.pydata.org/pandas-docs/stable/timeseries.html#offset-aliases



```python
    
```