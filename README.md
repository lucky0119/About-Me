# Salted-fish-code

纵使疾风起，人生不言弃

咸鱼代码：海滨墓园

- 👋 Hi, I’m @luckly2000
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
luckly2000/luckly2000 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




import pyecharts.options as opts
from pyecharts.charts import MapGlobe
from pyecharts.faker import POPULATION
data = [x for _, x in POPULATION[1:]]
low, high = min(data), max(data)
c = (
    MapGlobe(init_opts=opts.InitOpts())
    .add_schema()
    .add(
        maptype="world",
        series_name="World Population",
        data_pair=POPULATION[1:],
        is_map_symbol_show=False,
        label_opts=opts.LabelOpts(is_show=False),
    )
    .set_global_opts(
        visualmap_opts=opts.VisualMapOpts(
            min_=low,
            max_=high,
            range_text=["max", "min"],
            is_calculable=True,
            is_piecewise=True,
            range_color=["lightskyblue", "yellow", "orangered"],
        )
    )
)
c.render_notebook()



wskey=AAJjcgXXAEBB6PhAUhm4llIcmwG5bB_OTne4ePit6ypbuRqjjlAsQVYL400IvWm_4ZNKjbwe4UbC3VtbAO7yck1Ck8O8SR2n;whwswswws=JD0111d47dFzgFzB0JcR166848542490102VSoT29bkDIOlhUVJtjQa7nqnyAdyTACakWovL7OwBZsjwzMegGCHG-v-FM5pBDupJlUG0GVWualOkoWCynOrY7z_LwBzUIt0Gye5wvfMKeU1ukt8kd~q5SHs/18XFhhcVJutisUPyZFzx9eYNhXP1iwi7YZkLx9HfM/45cVveX51y2HrklqlgK/uhOmiw7d2oy/PYAkrSA==;unionwsws={"jmafinger":"JD0111d47dFzgFzB0JcR166848542490102VSoT29bkDIOlhUVJtjQa7nqnyAdyTACakWovL7OwBZsjwzMegGCHG-v-FM5pBDupJlUG0GVWualOkoWCynOrY7z_LwBzUIt0Gye5wvfMKeU1ukt8kd~q5SHs\/18XFhvhcVJutisUPyZFzx9eYNhXP1iwi7YZkLx9HfM\/45cVveX51y2HrklqlgK\/uhOmiw7d2oy\/PYAkrSA==","devicefinger":"eidIbe918121a1sdZ47ZhI5nQU+JWW4E+K62SmeO2v0tknaEsZnDoxZyQ0QYupH65sUmjERPYa3ySlIy7+Hy6u9lnrRm0zICKQPGMdY7T7ycjFgBE5FR"};pin_hash=-785329248
J-E-C: 
