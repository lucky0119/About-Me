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

