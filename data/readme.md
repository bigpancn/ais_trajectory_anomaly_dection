本目录包含了实验中的航次数据和异常航迹的数据，分别存储在voyages和anomalies目录中。其中，voyages/have是有异常的航次轨迹，voyages/dont是无异常的航迹数据。
航次轨迹和异常航迹是以csv文件存储船，数据结构按照以下顺序存储：
data structure:
1. mmsi: mmsi of vessel
2. time: AIS pint timestamp UTC 
3. lat: Latitude of AIS point.
4. lon: Longitude of AIS point.
5. speed: navigate speed of vessel.
6. nav_status: Navigate status
7. cog: course over ground.
航次的文件名按照mmsi + 航次离港时间组成(voyage_id) + '.csv'存储，异常航迹按照voyage_id + '#' + 异常开始时间 + '.csv'存储。
无异常航次的轨迹数共有755个，有异常的航次轨迹数据共有143个。异常航迹数据共200个。
check.xlsx是人工核对的结果。
pab包含了Piracy and Armed Robbery中的内容，其中，pab_check.xlsx是人工阅读后，得出哪些事件会对航迹产生影响。voyages是26个航次的轨迹。anomalies是被检测到的事件的位置。

