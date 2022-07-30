## Just Keep Runing 项目 README

- 获取咕咚的gpx数据
  - ```python3 scripts/codoon_sync.py --with-gpx 15810800280 ghZJsny_0810```
- 更新运动数据文件
  - ```python3 scripts/update_activities_file.py```
- 生成网页静态图片
  - grid :```python scripts/gen_svg.py --from-db --title Erosminer --type heatmap --athlete erospi --output assets/grid.svg --min-distance 1.0 --special-color yellow --special-color2 red --special-distance 5 --special-distance2 10 --use-localtime```
  - github:```python scripts/gen_svg.py --from-db --title JKR --type github --athlete erospi --special-distance 5 --special-distance2 10 --special-color yellow --special-color2 red --output assets/github.svg --use-localtime --min-distance 0.5```
- 修改颜色，网页slogan等
  - ```vim src/utils/const.js```
- 测试开发
  - ```yarn install```
  - ```yarn develop```
- 上线
  - ```yarn build```
  - 