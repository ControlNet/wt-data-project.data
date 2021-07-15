# WT-DATA-PROJECT.DATA
Data collected in wt-data-project.

<table>
    <tr>
        <th>Repository</th>
        <th>Info</th>
    </tr>
    <tr>
        <td><a href="https://github.com/ControlNet/wt-data-project.data">wt-data-project.data</a></td>
        <td>
            <img src="https://img.shields.io/github/forks/ControlNet/wt-data-project.data?style=flat-square" alt="">
            <img src="https://img.shields.io/github/stars/ControlNet/wt-data-project.data?style=flat-square" alt="">
            <img src="https://img.shields.io/github/last-commit/ControlNet/wt-data-project.data/master?style=flat-square" alt="">
            <img src="https://img.shields.io/github/workflow/status/ControlNet/wt-data-project.data/push-to-gitee?label=push-to-gitee&style=flat-square" alt="">
        </td>
    </tr>
    <tr>
        <td><a href="https://github.com/ControlNet/wt-data-project.web">wt-data-project.web</a></td>
        <td>
            <img src="https://img.shields.io/github/forks/ControlNet/wt-data-project.web?style=flat-square" alt="">
            <img src="https://img.shields.io/github/stars/ControlNet/wt-data-project.web?style=flat-square" alt="">
            <img src="https://img.shields.io/github/last-commit/ControlNet/wt-data-project.web?style=flat-square" alt="">
            <img src="https://img.shields.io/website?style=flat-square&up_message=online&url=https%3A%2F%2Fwt.controlnet.space" alt="">
        </td>
    </tr>
    <tr>
        <td><a href="https://github.com/ControlNet/wt-data-project.visualization">wt-data-project.visualization</a></td>
        <td>
            <img src="https://img.shields.io/github/forks/ControlNet/wt-data-project.visualization?style=flat-square" alt="">
            <img src="https://img.shields.io/github/stars/ControlNet/wt-data-project.visualization?style=flat-square" alt="">
            <img src="https://img.shields.io/github/last-commit/ControlNet/wt-data-project.visualization/master?style=flat-square" alt="">
        </td>
    </tr>
</table>

## Visualization
The visualization part is in this [webpage](https://wt.controlnet.space).

## Gitee mirror
[https://gitee.com/controlnet/wt-data-project.data](https://gitee.com/controlnet/wt-data-project.data)

## Time-series RB battle ranks data
File `rb_ranks_1.csv`: containing a time-series from 2019-11-22 until now, and grouped as battle rating ranges = 1.0.

File `rb_ranks_0.csv`: time-series data for each battle rating and nation

File `rb_ranks_all.csv`: time-series data for each nation, aggregated by all battle ratings

The overall stats is calculated with weighted average, and the weight is the `battles` in thunderskill data.

### Content
 * nation: USA, USSR...
 * cls: Aviation, Ground_vehicles, Fleet
 * date: 2020-08-13, 2020-05-10...
 * rb_br: 9.7 ~ 10.7
 * rb_lower_br: 9.7
 * rb_battles_sum 
 * rb_battles_mean 
 * rb_win_rate 
 * rb_air_frags_per_battle 
 * rb_air_frags_per_death 
 * rb_ground_frags_per_battle 
 * rb_ground_frags_per_death

## Thunderskill data
Directory `ts`: containing content from [thunderskill](http://thunderskill.com/en)

#### Content
 * name: ts url name
 * ab_battles 
 * ab_win_rate 
 * ab_air_frags_per_battle 
 * ab_air_frags_per_death 
 * ab_ground_frags_per_battle 
 * ab_ground_frags_per_death 
 * rb_battles 
 * rb_win_rate 
 * rb_air_frags_per_battle 
 * rb_air_frags_per_death 
 * rb_ground_frags_per_battle 
 * rb_ground_frags_per_death 
 * sb_battles 
 * sb_win_rate 
 * sb_air_frags_per_battle 
 * sb_air_frags_per_death 
 * sb_ground_frags_per_battle 
 * sb_ground_frags_per_death 
 * alt_name: alternative name

## War Thunder Wiki data
Directory `wk`: containing content from [war thunder wiki](https://wiki.warthunder.com/)

#### Content
 * name: displayed name in wiki page
 * nation: USA, USSR...
 * cls: Aviation, Ground_vehicles, Fleet
 * ab_br 
 * rb_br 
 * sb_br 
 * ab_repair
 * rb_repair 
 * sb_repair 
 * is_premium: True if the vehicle is premium else False
 * ab_rp_rate 
 * ab_sl_rate 
 * rb_rp_rate 
 * rb_sl_rate 
 * sb_rp_rate 
 * sb_sl_rate
 
## Joined data
Directory `joined`

To utilize both the battle stats like `rb_win_rate` and the information of `nation` and `rb_br`, the joined data is 
joined by the Thunderskill data and WT Wiki data.

Please acknowledge the join process is not perfectly accurate. Please report if there is any join issue.

#### Content
**TS Part**
 * name: ts url name
 * ab_battles 
 * ab_win_rate 
 * ab_air_frags_per_battle 
 * ab_air_frags_per_death 
 * ab_ground_frags_per_battle 
 * ab_ground_frags_per_death 
 * rb_battles 
 * rb_win_rate 
 * rb_air_frags_per_battle 
 * rb_air_frags_per_death 
 * rb_ground_frags_per_battle 
 * rb_ground_frags_per_death 
 * sb_battles 
 * sb_win_rate 
 * sb_air_frags_per_battle 
 * sb_air_frags_per_death 
 * sb_ground_frags_per_battle 
 * sb_ground_frags_per_death 
 * alt_name: alternative name

**Wiki Part**
 * wk_name: displayed name in wiki page
 * nation: USA, USSR...
 * cls: Aviation, Ground_vehicles, Fleet
 * ab_br 
 * rb_br 
 * sb_br 
 * ab_repair 
 * rb_repair 
 * sb_repair 
 * is_premium: True if the vehicle is premium else False
 * ab_rp_rate 
 * ab_sl_rate 
 * rb_rp_rate 
 * rb_sl_rate 
 * sb_rp_rate 
 * sb_sl_rate
