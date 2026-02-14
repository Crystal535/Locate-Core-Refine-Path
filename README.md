## LCRP: Locate-Core-Refine-Path
### Demo Video
**Note:** The demo video is large, please wait patiently.
<p align="center">
  <img src="demo/video_1.gif" width="45%" />
  <img src="demo/video_2.gif" width="45%" />
</p>


### Segmentation Result
<p align="center">
   <img src="demo/figure3.png" width=600 />
</p>


### More ablation studies
- Ref-DAVIS17

<table cellspacing="16" cellpadding="0" border="0">
  <tr>
    <td valign="top">
      <table border="1" cellspacing="0" cellpadding="6">
        <thead>
          <tr>
            <th><var>N</var></th>
            <th><var>K</var></th>
            <th>J &amp; F</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>5</td><td>5</td><td>75.1</td></tr>
          <tr><td>7</td><td>3</td><td>75.0</td></tr>
          <tr><td>5</td><td>3</td><td>75.9</td></tr>
          <tr><td><strong>10</strong></td><td><strong>3</strong></td><td><strong>76.7</strong></td></tr>
          <tr><td>10</td><td>5</td><td>76.3</td></tr>
        </tbody>
      </table>
    </td>
    <td valign="top">
      <table border="1" cellspacing="0" cellpadding="6">
        <thead>
          <tr>
            <th><var>H</var></th>
            <th>&delta;</th>
            <th>J &amp; F</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>1</td><td>0.1%</td><td>76.5</td></tr>
          <tr><td>2</td><td>0.3%</td><td>76.6</td></tr>
          <tr><td><strong>3</strong></td><td><strong>0.3%</strong></td><td><strong>76.7</strong></td></tr>
          <tr><td>2</td><td>0.2%</td><td>76.5</td></tr>
          <tr><td>3</td><td>0.2%</td><td>76.5</td></tr>
        </tbody>
      </table>
    </td>
  </tr>
</table>

- MeViS

<table cellspacing="16" cellpadding="0" border="0">
  <tr>
    <td valign="top">
      <table border="1" cellspacing="0" cellpadding="6">
        <thead>
          <tr>
            <th><var>N</var></th>
            <th><var>K</var></th>
            <th>J &amp; F</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>5</td><td>5</td><td>47.8</td></tr>
          <tr><td>10</td><td>10</td><td>48.8</td></tr>
          <tr><td>10</td><td>3</td><td>48.7</td></tr>
          <tr><td><strong>10</strong></td><td><strong>5</strong></td><td><strong>49.1</strong></td></tr>
        </tbody>
      </table>
    </td>
    <td valign="top">
      <table border="1" cellspacing="0" cellpadding="6">
        <thead>
          <tr>
            <th><var>H</var></th>
            <th>&delta;</th>
            <th>J &amp; F</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>3</td><td>0.1%</td><td>48.9</td></tr>
          <tr><td><strong>3</strong></td><td><strong>0.3%</strong></td><td><strong>49.1</strong></td></tr>
          <tr><td>2</td><td>0.3%</td><td>48.9</td></tr>
          <tr><td>2</td><td>0.2%</td><td>48.7</td></tr>
        </tbody>
      </table>
    </td>
  </tr>
</table>


### Model Complexity and Resource Usage on Ref-Youtube-VOS
| Method | Learnable params | Training GPU Memory Usage |Inference GPU Memory Usage |
|:--------:|:-----------------:|:--------------:|:--------------:|
| SOC | ~110.0 M | ~26 G | ~19 G |
| ReferDINO | ~15.3 M | ~21 G | ~12 G |
| Ours | 0 | 0 | ~15 G |
> **Note:** Both SOC and ReferDINO are trained and inferred on an **A100-40G GPU** with `batch_size=1`.  
> Our model is inferred on a single **RTX 4090-24G GPU** with `batch_size=1`.

### Segmentation Results 
- Binary Segmentation Results of Fig. 4.
![](demo/Figure%204.png)

### The code will be released soon





