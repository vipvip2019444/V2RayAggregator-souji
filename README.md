# TopFreeProxies
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alanbobs999/topfreeproxies/sub_merge?label=sub_merge)](https://github.com/alanbobs999/TopFreeProxies/actions/workflows/sub_merge.yml) 

![Watchers](https://img.shields.io/github/watchers/alanbobs999/topfreeproxies) ![Stars](https://img.shields.io/github/stars/alanbobs999/topfreeproxies) ![Forks](https://img.shields.io/github/forks/alanbobs999/topfreeproxies) ![Vistors](https://visitor-badge.laobi.icu/badge?page_id=alanbobs999.topfreeproxies) ![LICENSE](https://img.shields.io/badge/license-CC%20BY--SA%204.0-green.svg)

[仓库介绍](https://github.com/alanbobs999/TopFreeProxies#仓库介绍) | [使用方法](https://github.com/alanbobs999/TopFreeProxies#使用方法) | [节点信息](https://github.com/alanbobs999/TopFreeProxies#节点信息) | [软件推荐](https://github.com/alanbobs999/TopFreeProxies#客户端选择) | [机场推荐](https://github.com/alanbobs999/TopFreeProxies#机场推荐) | [仓库声明](https://github.com/alanbobs999/TopFreeProxies#仓库声明)

## 仓库介绍
本仓库自动化功能全部基于 `GitHub Actions` 实现，如果有需要可以自行 Fork 实现个性化需求。

对网络上各免费节点池及博主分享的节点进行测速筛选出较为稳定高速的节点，再导入到仓库中进行分享记录。所筛选的节点链接在仓库 `./sub/sub_list.json` 文件中，其中大部分为其他 `GitHub` 仓库链接，如果大家有好的订阅链接欢迎提交 PR ，这些链接包含的所有节点会合并在仓库 `./sub/sub_merge.txt` 中。

测速筛选后的节点订阅文件在仓库根目录 `Eterniy`(Base64) 和 `Eternity.yml`(Clash)。同时在仓库的 `./update` 中保留了原始节点链接的的记录。

测速功能使用 [LiteSpeedTest](https://github.com/xxf098/LiteSpeedTest) 在 `GitHub Actions` 环境下实现，所以美国节点较多，不能很好代表国内网络环境下节点可用性，目前正在解决这一问题。

虽然是测速筛选过后的节点，但仍然会出现部分节点不可用的情况，遇到这种情况建议选择`Clash`, `Shadowrocket`之类能自动切换低延迟节点的客户端。

## 使用方法
将以下订阅链接导入相应客户端即可。链接中大部分为 SS 协议节点，少量 Vmess, Trojan ,SSR 协议节点，建议选择协议支持完整的客户端。

- [多协议Base64编码](https://raw.githubusercontent.com/alanbobs999/TopFreeProxies/master/Eternity)
- [Clash](https://raw.githubusercontent.com/alanbobs999/TopFreeProxies/master/Eternity.yml)

另有国内加速链接：

- [多协议Base64编码](https://raw.fastgit.org/alanbobs999/TopFreeProxies/master/Eternity)
- [Clash](https://raw.fastgit.org/alanbobs999/TopFreeProxies/master/Eternity.yml)

>`Clash`链接所使用的配置在仓库`./update/provider/`中，有相应配置文件和以国家分类的`proxy-provider`。
>
>需要其它配置可使用订阅转换工具自行转换。
>自用在线订阅转换网址：[sub-web-modify](https://sub.v1.mk/)

## 节点信息
### 高速节点
高速节点数量: `98`
<details>
  <summary>展开复制节点</summary>

    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9KFRH6aKR6YGTOkBwb2R1dmpkKSIsImFkZCI6IjQ1Ljc2LjcxLjIzMyIsInBvcnQiOiI0Njk4MyIsInR5cGUiOiJub25lIiwiaWQiOiI2OTA5OTI1OC0xNDc2LTQ2ZGQtYTUxYi04NGU5MTVlOTQxYmUiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLzF0R0s4MmxVLyIsImhvc3QiOiI0NS43Ni43MS4yMzMiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVMt6auY6YCf6IqC54K56LSt5Lmw77yadjEubWsvdmlw77yI5rWP6KeI5Zmo5omT5byA77yJIiwiYWRkIjoiNDUuNzYuNzEuMjMzIiwicG9ydCI6IjQ2OTgzIiwidHlwZSI6Im5vbmUiLCJpZCI6IjY5MDk5MjU4LTE0NzYtNDZkZC1hNTFiLTg0ZTkxNWU5NDFiZSIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvMXRHSzgybFUvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiWzA1LTAzXXxvc2xvb2t8576O5Zu9KFVTKVVTQS9Mb3NBbmdlbGVzXzExIiwiYWRkIjoiNDUuNzYuNzEuMjMzIiwicG9ydCI6IjQ2OTgzIiwidHlwZSI6Im5vbmUiLCJpZCI6IjY5MDk5MjU4LTE0NzYtNDZkZC1hNTFiLTg0ZTkxNWU5NDFiZSIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvMXRHSzgybFUvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiNDUuNzYuNzEuMjMzIiwicG9ydCI6IjQ2OTgzIiwidHlwZSI6Im5vbmUiLCJpZCI6IjY5MDk5MjU4LTE0NzYtNDZkZC1hNTFiLTg0ZTkxNWU5NDFiZSIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvMXRHSzgybFUvIiwiaG9zdCI6IjQ1Ljc2LjcxLjIzMyIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi5pel5pysIDAxNCIsImFkZCI6IjQ1Ljc2LjcxLjIzMyIsInBvcnQiOiI0Njk4MyIsInR5cGUiOiJub25lIiwiaWQiOiI2OTA5OTI1OC0xNDc2LTQ2ZGQtYTUxYi04NGU5MTVlOTQxYmUiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLzF0R0s4MmxVLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlfXzE1M181MU1iXzE0NiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA2NiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiYWEua2F5YWxvLmNvbSIsInBvcnQiOiIyNjI2NyIsInR5cGUiOiJub25lIiwiaWQiOiI5NzU3Y2RiYS1jNzViLTRiOTQtOWUzMS03OTU2ZGM3ZDg1MmEiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL3dpcyIsImhvc3QiOiJhYS5rYXlhbG8uY29tIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi6L+Z5Lqb6IqC54K55Y+q6IO95aSH55So5oiW6ICF6Ziy5q2i5aSx6IGU77yM6Jm954S26LSo6YeP5bm25LiN5piv5b6I5aW977yM5Lmf6K+35L2O6LCD5L2/55SoOikiLCJhZGQiOiI0NS43Ni43MS4yMzMiLCJwb3J0IjoiNDY5ODMiLCJ0eXBlIjoibm9uZSIsImlkIjoiNjkwOTkyNTgtMTQ3Ni00NmRkLWE1MWItODRlOTE1ZTk0MWJlIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8xdEdLODJsVS8iLCJob3N0IjoiNDUuNzYuNzEuMjMzIiwidGxzIjoiIn0=
    trojan://f39bd244-f5fe-415c-8b98-a1e5250bf178@fhcarm2.gaox.ml:443?allowInsecure=0#%E8%BF%99%E4%BA%9B%E8%8A%82%E7%82%B9%E5%8F%AA%E8%83%BD%E5%A4%87%E7%94%A8%E6%88%96%E8%80%85%E9%98%B2%E6%AD%A2%E5%A4%B1%E8%81%94%EF%BC%8C%E8%99%BD%E7%84%B6%E8%B4%A8%E9%87%8F%E5%B9%B6%E4%B8%8D%E6%98%AF%E5%BE%88%E5%A5%BD%EF%BC%8C%E4%B9%9F%E8%AF%B7%E4%BD%8E%E8%B0%83%E4%BD%BF%E7%94%A8%3A%29
    trojan://e5d46365e25e31d94279c2bcf93390a2@o7cx6bd6t4yjiqsm.xiongsonglin.com:443?allowInsecure=1#US-Openit.ml
    trojan://05742120-ce23-4cc8-88f5-6d221ce45bf4@fhcarm1.gaox.ml:443?allowInsecure=1#US_2702%20%7C87.65Mb
    vmess://eyJ2IjoiMiIsInBzIjoiVVMiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii93cyIsImhvc3QiOiJsdnVmdC5jb20iLCJ0bHMiOiIifQ==
    trojan://e5d46365e25e31d94279c2bcf93390a2@o7cx6bd6t4yjiqsm.xiongsonglin.com:443?allowInsecure=1#US-Openit.ml
    vmess://eyJ2IjoiMiIsInBzIjoiXzE0N180NE1iXzgiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii9obHMvY2N0djVwaGQubTN1OCIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvZ28iLCJob3N0IjoidXMwMi5nb2dvZ29vLmN5b3UiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzI2NDciLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi5L+E572X5pavIDAwMSIsImFkZCI6Ijk1LjE4MS4xODkuNjAiLCJwb3J0IjoiMjg2MjkiLCJ0eXBlIjoibm9uZSIsImlkIjoiODcyODA4ZDMtYzdkZS00ZjYxLWE2MGUtOGIyYjBiZDM5OWQ5IiwiYWlkIjoiNjQiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA0MCIsImFkZCI6Ijk2LjQ1LjE4OC4xOTkiLCJwb3J0IjoiODAiLCJ0eXBlIjoibm9uZSIsImlkIjoiNWQzN2MyMGYtMjE3Ni00N2FjLWM2MWEtYTY1MjljNmZiYTQyIiwiYWlkIjoiNjQiLCJuZXQiOiJ3cyIsInBhdGgiOiIvaG9tZSIsImhvc3QiOiI5Ni40NS4xODguMTk5IiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6IjEwNC4xNjguMTMuOCIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA5OSIsImFkZCI6IjEwNC4yNDMuMjYuMTEyIiwicG9ydCI6IjIxNzM1IiwidHlwZSI6Im5vbmUiLCJpZCI6IjA0NWY1OTU3LTE1N2QtNDY2NC04YjhkLTFiMmZkYTIwMjM4OCIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzM3NDQiLCJhZGQiOiI5Ni40NS4xODguMTk5IiwicG9ydCI6IjgwIiwidHlwZSI6Im5vbmUiLCJpZCI6IjVkMzdjMjBmLTIxNzYtNDdhYy1jNjFhLWE2NTI5YzZmYmE0MiIsImFpZCI6IjY0IiwibmV0Ijoid3MiLCJwYXRoIjoiL2hvbWUiLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfOTYxIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfOTM5IiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    trojan://05742120-ce23-4cc8-88f5-6d221ce45bf4@fhcarm1.gaox.ml:443?allowInsecure=1#%E7%BE%8E%E5%9B%BD%20005
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYxN184NF8wOE1iXzYiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiXzE0N180NE1iXzgiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii9obHMvY2N0djVwaGQubTN1OCIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiMTA0LjI0My4yNi4xMTIiLCJwb3J0IjoiMjE3MzUiLCJ0eXBlIjoibm9uZSIsImlkIjoiMDQ1ZjU5NTctMTU3ZC00NjY0LThiOGQtMWIyZmRhMjAyMzg4IiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIxNDQuMzQuMjQ4LjI2IiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6IjE0NC4zNC4yNDguMjYiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIxNDQuMzQuMjQ4LjI2IiwidGxzIjoiIn0=
    trojan://e5d46365e25e31d94279c2bcf93390a2@o7cx6bd6t4yjiqsm.xiongsonglin.com:443?allowInsecure=0#github.com%2Ffreefq%20-%20%E7%BE%8E%E5%9B%BD%E4%BA%9A%E5%88%A9%E6%A1%91%E9%82%A3%E5%B7%9E%E6%96%AF%E7%A7%91%E8%8C%A8%E4%BB%A3%E5%B0%94%E5%B8%82Go%20Daddy%E9%9B%86%E5%9B%A2%E5%85%AC%E5%8F%B8%2047
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIxNDQuMzQuMjQ4LjI2IiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA2MiIsImFkZCI6Ijk2LjQ1LjE4OC4xOTkiLCJwb3J0IjoiODAiLCJ0eXBlIjoibm9uZSIsImlkIjoiNWQzN2MyMGYtMjE3Ni00N2FjLWM2MWEtYTY1MjljNmZiYTQyIiwiYWlkIjoiNjQiLCJuZXQiOiJ3cyIsInBhdGgiOiIvaG9tZSIsImhvc3QiOiI5Ni40NS4xODguMTk5IiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfOTUxIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfOTYzIiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvd3MiLCJob3N0IjoiOTUuMTgxLjE4OS42MCIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA1NiIsImFkZCI6IjE0NC4zNC4yNDguMjYiLCJwb3J0IjoiMTM5MTciLCJ0eXBlIjoibm9uZSIsImlkIjoiMDA0OTJjZDEtN2Y1ZS00ZWQ1LWI5ZWYtODIxZTliODljYTcyIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8iLCJob3N0IjoiMTQ0LjM0LjI0OC4yNiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiVVMiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiMTQ0LjM0LjI0OC4yNiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYyNiB8NzIuNzhNYiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlfXzE1M181MU1iXzE0NiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjY2MCB8MzYuNjVNYiIsImFkZCI6Ijk1LjE4MS4xODkuNjAiLCJwb3J0IjoiMjg2MjkiLCJ0eXBlIjoibm9uZSIsImlkIjoiODcyODA4ZDMtYzdkZS00ZjYxLWE2MGUtOGIyYjBiZDM5OWQ5IiwiYWlkIjoiNjQiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiXzcwOSIsImFkZCI6InVzYS1kYWxsYXMubHZ1ZnQuY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiJhYmE1MGRkNC01NDg0LTNiMDUtYjE0YS00NjYxY2FmODYyZDUiLCJhaWQiOiI0IiwibmV0Ijoid3MiLCJwYXRoIjoiL3dzIiwiaG9zdCI6InVzYS1kYWxsYXMubHZ1ZnQuY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIxNDQuMzQuMjQ4LjI2IiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYxN184NF8wOE1iXzYiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6Ijk1LjE4MS4xODkuNjAiLCJ0bHMiOiIifQ==
    trojan://e5d46365e25e31d94279c2bcf93390a2@usa-sr-105.mitoption.com:443?allowInsecure=0#github.com%2Ffreefq%20-%20%E7%BE%8E%E5%9B%BD%E4%BA%9A%E5%88%A9%E6%A1%91%E9%82%A3%E5%B7%9E%E6%96%AF%E7%A7%91%E8%8C%A8%E4%BB%A3%E5%B0%94%E5%B8%82Go%20Daddy%E9%9B%86%E5%9B%A2%E5%85%AC%E5%8F%B8%208
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfOTYxIiwiYWRkIjoiMTQ0LjM0LjI0OC4yNiIsInBvcnQiOiIxMzkxNyIsInR5cGUiOiJub25lIiwiaWQiOiIwMDQ5MmNkMS03ZjVlLTRlZDUtYjllZi04MjFlOWI4OWNhNzIiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVMiLCJhZGQiOiIxNDQuMzQuMjQ4LjI2IiwicG9ydCI6IjEzOTE3IiwidHlwZSI6Im5vbmUiLCJpZCI6IjAwNDkyY2QxLTdmNWUtNGVkNS1iOWVmLTgyMWU5Yjg5Y2E3MiIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvIiwiaG9zdCI6IjE0NC4zNC4yNDguMjYiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA4MiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA1OCIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi6L+Z5Lqb6IqC54K55Y+q6IO95aSH55So5oiW6ICF6Ziy5q2i5aSx6IGU77yM6Jm954S26LSo6YeP5bm25LiN5piv5b6I5aW977yM5Lmf6K+35L2O6LCD5L2/55SoOikiLCJhZGQiOiI0NS43Ni43MS4yMzMiLCJwb3J0IjoiNDY5ODMiLCJ0eXBlIjoibm9uZSIsImlkIjoiNjkwOTkyNTgtMTQ3Ni00NmRkLWE1MWItODRlOTE1ZTk0MWJlIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8xdEdLODJsVS8iLCJob3N0IjoiNDUuNzYuNzEuMjMzIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiMTA0LjI0My4yNi4xMTIiLCJwb3J0IjoiMjE3MzUiLCJ0eXBlIjoibm9uZSIsImlkIjoiMDQ1ZjU5NTctMTU3ZC00NjY0LThiOGQtMWIyZmRhMjAyMzg4IiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    trojan://e5d46365e25e31d94279c2bcf93390a2@o7cx6bd6t4yjiqsm.xiongsonglin.com:443?allowInsecure=1#%E7%BE%8E%E5%9B%BD%28%E6%AC%A2%E8%BF%8E%E8%AE%A2%E9%98%85Youtube%E7%A0%B4%E8%A7%A3%E8%B5%84%E6%BA%90%E5%90%9B%29
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6IjE0NC4zNC4yNDguMjYiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjY2MiB8MTI5LjgwTWIiLCJhZGQiOiJ1c2EtZGFsbGFzLmx2dWZ0LmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiYWJhNTBkZDQtNTQ4NC0zYjA1LWIxNGEtNDY2MWNhZjg2MmQ1IiwiYWlkIjoiNCIsIm5ldCI6IndzIiwicGF0aCI6Ii93cyIsImhvc3QiOiJ1c2EtZGFsbGFzLmx2dWZ0LmNvbSIsInRscyI6InRscyJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiOTUuMTgxLjE4OS42MCIsInBvcnQiOiIyODYyOSIsInR5cGUiOiJub25lIiwiaWQiOiI4NzI4MDhkMy1jN2RlLTRmNjEtYTYwZS04YjJiMGJkMzk5ZDkiLCJhaWQiOiI2NCIsIm5ldCI6InRjcCIsInBhdGgiOiIvIiwiaG9zdCI6Ijk1LjE4MS4xODkuNjAiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDEwMiIsImFkZCI6IjEwNC4yNDMuMjYuMTEyIiwicG9ydCI6IjIxNzM1IiwidHlwZSI6Im5vbmUiLCJpZCI6IjA0NWY1OTU3LTE1N2QtNDY2NC04YjhkLTFiMmZkYTIwMjM4OCIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzI2NTAiLCJhZGQiOiIxNDQuMzQuMjQ4LjI2IiwicG9ydCI6IjEzOTE3IiwidHlwZSI6Im5vbmUiLCJpZCI6IjAwNDkyY2QxLTdmNWUtNGVkNS1iOWVmLTgyMWU5Yjg5Y2E3MiIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvIiwiaG9zdCI6IiIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiZ2l0aHViLmNvbS92MnJheWZyZWUgLSDnvo7lm73lvrflhYvokKjmlq/lt57ovr7mi4nmlq9Qc3ljaHrmlbDmja7kuK3lv4MgNTAiLCJhZGQiOiI0NS4zNS44NC4xNjIiLCJwb3J0IjoiNDQzIiwidHlwZSI6Im5vbmUiLCJpZCI6ImFiYTUwZGQ0LTU0ODQtM2IwNS1iMTRhLTQ2NjFjYWY4NjJkNSIsImFpZCI6IjQiLCJuZXQiOiJ3cyIsInBhdGgiOiIvd3MiLCJob3N0IjoidXNhLWRhbGxhcy5sdnVmdC5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiczIuNTIwZ3VnZS5jb20iLCJwb3J0IjoiNDQzIiwidHlwZSI6Im5vbmUiLCJpZCI6ImNmMTgxOWM4LWU1MzAtNDYyNi1hZWMwLTg3YWMwNDIwMDM4NSIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvaGFwcHkiLCJob3N0IjoiczIuNTIwZ3VnZS5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiYWEua2F5YWxvLmNvbSIsInBvcnQiOiIyNjI2NyIsInR5cGUiOiJub25lIiwiaWQiOiI5NzU3Y2RiYS1jNzViLTRiOTQtOWUzMS03OTU2ZGM3ZDg1MmEiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL3dpcyIsImhvc3QiOiJhYS5rYXlhbG8uY29tIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlfXzE1M181MU1iXzE0NiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoiYWEua2F5YWxvLmNvbSIsInBvcnQiOiIyNjI2NyIsInR5cGUiOiJub25lIiwiaWQiOiI5NzU3Y2RiYS1jNzViLTRiOTQtOWUzMS03OTU2ZGM3ZDg1MmEiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL3dpcyIsImhvc3QiOiJhYS5rYXlhbG8uY29tIiwidGxzIjoiIn0=
    trojan://sharecentre@ussc.scsevers.cf:443?allowInsecure=1#US_2700%20%7C77.61Mb
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjY0OSB8NzcuMjhNYiIsImFkZCI6Imllc2VpMWVpLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiYWJhNTBkZDQtNTQ4NC0zYjA1LWIxNGEtNDY2MWNhZjg2MmQ1IiwiYWlkIjoiNCIsIm5ldCI6IndzIiwicGF0aCI6Ii93cyIsImhvc3QiOiJpZXNlaTFlaS5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYxNyB8NzYuNzNNYiIsImFkZCI6IjE0NC4zNC4yNDguMjYiLCJwb3J0IjoiMTM5MTciLCJ0eXBlIjoibm9uZSIsImlkIjoiMDA0OTJjZDEtN2Y1ZS00ZWQ1LWI5ZWYtODIxZTliODljYTcyIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf576O5Zu9LV8zOCIsImFkZCI6IjFjaHVhbi50b3AiLCJwb3J0IjoiNDQzIiwidHlwZSI6Im5vbmUiLCJpZCI6ImZhOGY5MGUwLTJmYWUtNGIwNS1kZjdhLWVhMzI1YmM1MTdkOCIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvZXZvIiwiaG9zdCI6IjFjaHVhbi50b3AiLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzM3MjAiLCJhZGQiOiI5NS4xODEuMTg5LjYwIiwicG9ydCI6IjI4NjI5IiwidHlwZSI6Im5vbmUiLCJpZCI6Ijg3MjgwOGQzLWM3ZGUtNGY2MS1hNjBlLThiMmIwYmQzOTlkOSIsImFpZCI6IjY0IiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiZ2l0aHViLmNvbS9mcmVlZnEgLSDnvo7lm71DbG91ZEZsYXJl6IqC54K5IDE5IiwiYWRkIjoiMWNodWFuLnRvcCIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiZmE4ZjkwZTAtMmZhZS00YjA1LWRmN2EtZWEzMjViYzUxN2Q4IiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii9ldm8iLCJob3N0IjoiMWNodWFuLnRvcCIsInRscyI6InRscyJ9
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf576O5Zu9LV8zNzM4IiwiYWRkIjoiYWEua2F5YWxvLmNvbSIsInBvcnQiOiIyNjI2NyIsInR5cGUiOiJub25lIiwiaWQiOiI5NzU3Y2RiYS1jNzViLTRiOTQtOWUzMS03OTU2ZGM3ZDg1MmEiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL3dpcyIsImhvc3QiOiJhYS5rYXlhbG8uY29tIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9KOasoui/juiuoumYhVlvdXR1YmXnoLTop6PotYTmupDlkJspIiwiYWRkIjoidXMzLjMxdnBuLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiMmVmNjRkYzgtY2EzYy00NWI4LWFkNWYtMjA4NzE0NTIxNDNiIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii9mYXN0c3NoLzMxMDI2Mzc0OTNxcWNvbS82MjZjZjdkOGJkNDliLyIsImhvc3QiOiJ1czMuMzF2cG4uY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiVVMtT3Blbml0Lm1sIiwiYWRkIjoibWcubGFveW91djIudG9wIiwicG9ydCI6IjEwMDgwIiwidHlwZSI6Im5vbmUiLCJpZCI6IjI5NDMwYjNkLWY4M2YtM2M3NC05NGEyLWU4YzFhNDU5MjE5ZiIsImFpZCI6IjAiLCJuZXQiOiJ3cyIsInBhdGgiOiIvIiwiaG9zdCI6Im1nLmxhb3lvdXYyLnRvcCIsInRscyI6IiJ9
    trojan://e23f408a-012e-4030-8b31-02022031cb50@fhcamd1.gaox.ml:443?allowInsecure=0#%E8%BF%99%E4%BA%9B%E8%8A%82%E7%82%B9%E5%8F%AA%E8%83%BD%E5%A4%87%E7%94%A8%E6%88%96%E8%80%85%E9%98%B2%E6%AD%A2%E5%A4%B1%E8%81%94%EF%BC%8C%E8%99%BD%E7%84%B6%E8%B4%A8%E9%87%8F%E5%B9%B6%E4%B8%8D%E6%98%AF%E5%BE%88%E5%A5%BD%EF%BC%8C%E4%B9%9F%E8%AF%B7%E4%BD%8E%E8%B0%83%E4%BD%BF%E7%94%A8%3A%29
    vmess://eyJ2IjoiMiIsInBzIjoi6L+Z5Lqb6IqC54K55Y+q6IO95aSH55So5oiW6ICF6Ziy5q2i5aSx6IGU77yM6Jm954S26LSo6YeP5bm25LiN5piv5b6I5aW977yM5Lmf6K+35L2O6LCD5L2/55SoOikiLCJhZGQiOiJ1czMuMzF2cG4uY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiIyZWY2NGRjOC1jYTNjLTQ1YjgtYWQ1Zi0yMDg3MTQ1MjE0M2IiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL2Zhc3Rzc2gvMzEwMjYzNzQ5M3FxY29tLzYyNmNmN2Q4YmQ0OWIvIiwiaG9zdCI6InVzMy4zMXZwbi5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYxNCB8NzIuNTJNYiIsImFkZCI6ImFhLmtheWFsby5jb20iLCJwb3J0IjoiMjYyNjciLCJ0eXBlIjoibm9uZSIsImlkIjoiOTc1N2NkYmEtYzc1Yi00Yjk0LTllMzEtNzk1NmRjN2Q4NTJhIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii93aXMiLCJob3N0IjoiYWEua2F5YWxvLmNvbSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA2MiIsImFkZCI6IjY3LjIxLjcyLjQxIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLCJhaWQiOiI2NCIsIm5ldCI6IndzIiwicGF0aCI6Ii9wYXRoLzE3MzQxODE0MTEyMyIsImhvc3QiOiJ3d3cuMTcwODAxMDAueHl6IiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi5qKm5q2MfEJHUOS4rei9rHzop6PplIHmtYHlqpLkvZNfNzAiLCJhZGQiOiJ1czMuMzF2cG4uY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiIyZWY2NGRjOC1jYTNjLTQ1YjgtYWQ1Zi0yMDg3MTQ1MjE0M2IiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL2Zhc3Rzc2gvMzEwMjYzNzQ5M3FxY29tLzYyNmNmN2Q4YmQ0OWIvIiwiaG9zdCI6InVzMy4zMXZwbi5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiWzA1LTAzXXxvc2xvb2t8576O5Zu9KFVTKVVTQS9DbGlmdG9uXzE4IiwiYWRkIjoidXMzLjMxdnBuLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiMmVmNjRkYzgtY2EzYy00NWI4LWFkNWYtMjA4NzE0NTIxNDNiIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii9mYXN0c3NoLzMxMDI2Mzc0OTNxcWNvbS82MjZjZjdkOGJkNDliLyIsImhvc3QiOiJ1czMuMzF2cG4uY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiZ2l0aHViLmNvbS9mcmVlZnEgLSDnvo7lm73nur3nuqbluIJEaWdpdGFsT2NlYW7kupHlhazlj7ggMjIiLCJhZGQiOiJ1czMuMzF2cG4uY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiIyZWY2NGRjOC1jYTNjLTQ1YjgtYWQ1Zi0yMDg3MTQ1MjE0M2IiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL2Zhc3Rzc2gvMzEwMjYzNzQ5M3FxY29tLzYyNmNmN2Q4YmQ0OWIvIiwiaG9zdCI6InVzMy4zMXZwbi5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf8J+HuvCfh7hVUy3wn4e68J+HuFVTXzQ2IiwiYWRkIjoidXMzLjMxdnBuLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiMmVmNjRkYzgtY2EzYy00NWI4LWFkNWYtMjA4NzE0NTIxNDNiIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii9mYXN0c3NoLzMxMDI2Mzc0OTNxcWNvbS82MjZjZjdkOGJkNDliLyIsImhvc3QiOiJ1czMuMzF2cG4uY29tIiwidGxzIjoidGxzIn0=
    trojan://e23f408a-012e-4030-8b31-02022031cb50@fhcamd1.gaox.ml:443?allowInsecure=1#US-Openit.ml
    trojan://sharecentre@ussc.scsevers.cf:443?allowInsecure=1#US_2663%20%7C53.81Mb
    trojan://sharecentre@ussc.scsevers.cf:443?allowInsecure=1#US_2700%20%7C77.61Mb
    trojan://dbf9bf9c-2c3f-474a-8031-d4c00666a989@fhcamd2.gaox.ml:443?allowInsecure=1&sni=fhcamd2.gaox.ml#%28Youtube%E6%8A%80%E6%9C%AF%E5%88%86%E4%BA%AB%E5%AE%A4%29%F0%9F%87%BA%F0%9F%87%B8%E7%BE%8E%E5%9B%BD%2039
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzM3MzEiLCJhZGQiOiIxNTAuMjMwLjQzLjY1IiwicG9ydCI6IjE0NTY0IiwidHlwZSI6Im5vbmUiLCJpZCI6IjE1NTZlMDQwLTMxZDMtNGM0Ny1iMGQyLWRkZjg4ODAxMGI0ZSIsImFpZCI6IjAiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiVVNfMjYyMSB8NDYuNDhNYiIsImFkZCI6Imllc2VpMWVpLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiYWJhNTBkZDQtNTQ4NC0zYjA1LWIxNGEtNDY2MWNhZjg2MmQ1IiwiYWlkIjoiNCIsIm5ldCI6IndzIiwicGF0aCI6Ii93cyIsImhvc3QiOiJpZXNlaTFlaS5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiZ2l0aHViLmNvbS9mcmVlZnEgLSDnvo7lm73nur3nuqbluIJEaWdpdGFsT2NlYW7kupHlhazlj7ggMjIiLCJhZGQiOiJ1czMuMzF2cG4uY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiIyZWY2NGRjOC1jYTNjLTQ1YjgtYWQ1Zi0yMDg3MTQ1MjE0M2IiLCJhaWQiOiIwIiwibmV0Ijoid3MiLCJwYXRoIjoiL2Zhc3Rzc2gvMzEwMjYzNzQ5M3FxY29tLzYyNmNmN2Q4YmQ0OWIvIiwiaG9zdCI6InVzMy4zMXZwbi5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA1OSIsImFkZCI6Imllc2VpMWVpLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiYWJhNTBkZDQtNTQ4NC0zYjA1LWIxNGEtNDY2MWNhZjg2MmQ1IiwiYWlkIjoiNCIsIm5ldCI6IndzIiwicGF0aCI6Ii93cyIsImhvc3QiOiJpZXNlaTFlaS5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf576O5Zu9LV8yMjY3IiwiYWRkIjoidXNhLXdhc2hpbmd0b24ubHZ1ZnQuY29tIiwicG9ydCI6IjQ0MyIsInR5cGUiOiJub25lIiwiaWQiOiJhYmE1MGRkNC01NDg0LTNiMDUtYjE0YS00NjYxY2FmODYyZDUiLCJhaWQiOiI0IiwibmV0Ijoid3MiLCJwYXRoIjoiL3dzIiwiaG9zdCI6InVzYS13YXNoaW5ndG9uLmx2dWZ0LmNvbSIsInRscyI6InRscyJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IDA2NyIsImFkZCI6InVzYS13YXNoaW5ndG9uLmx2dWZ0LmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiYWJhNTBkZDQtNTQ4NC0zYjA1LWIxNGEtNDY2MWNhZjg2MmQ1IiwiYWlkIjoiNCIsIm5ldCI6IndzIiwicGF0aCI6Ii93cyIsImhvc3QiOiJ1c2Etd2FzaGluZ3Rvbi5sdnVmdC5jb20iLCJ0bHMiOiJ0bHMifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiXzE0MV83Nk1iXzY2IiwiYWRkIjoiMTUwLjIzMC40My42NSIsInBvcnQiOiIxNDU2NCIsInR5cGUiOiJub25lIiwiaWQiOiIxNTU2ZTA0MC0zMWQzLTRjNDctYjBkMi1kZGY4ODgwMTBiNGUiLCJhaWQiOiIwIiwibmV0IjoidGNwIiwicGF0aCI6Ii9hVHRoYjhaeC8iLCJob3N0IjoiIiwidGxzIjoiIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu957q957qm5biCRGlnaXRhbE9jZWFu5LqR5YWs5Y+4IDMwIiwiYWRkIjoidXMzLjMxdnBuLmNvbSIsInBvcnQiOiI0NDMiLCJ0eXBlIjoibm9uZSIsImlkIjoiMmVmNjRkYzgtY2EzYy00NWI4LWFkNWYtMjA4NzE0NTIxNDNiIiwiYWlkIjoiMCIsIm5ldCI6IndzIiwicGF0aCI6Ii9mYXN0c3NoLzMxMDI2Mzc0OTNxcWNvbS82MjZjZjdkOGJkNDliLyIsImhvc3QiOiJ1czMuMzF2cG4uY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf8J+HuvCfh7hVUy3wn4e68J+HuFVTXzEzNDZfNDNfNjBNYl8xMDQiLCJhZGQiOiJ1c2Etd2FzaGluZ3Rvbi5sdnVmdC5jb20iLCJwb3J0IjoiNDQzIiwidHlwZSI6Im5vbmUiLCJpZCI6ImFiYTUwZGQ0LTU0ODQtM2IwNS1iMTRhLTQ2NjFjYWY4NjJkNSIsImFpZCI6IjQiLCJuZXQiOiJ3cyIsInBhdGgiOiIvd3MiLCJob3N0IjoidXNhLXdhc2hpbmd0b24ubHZ1ZnQuY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi5qyn5rSyIiwiYWRkIjoiMTUwLjIzMC40My42NSIsInBvcnQiOiIxNDU2NCIsInR5cGUiOiJub25lIiwiaWQiOiIxNTU2ZTA0MC0zMWQzLTRjNDctYjBkMi1kZGY4ODgwMTBiNGUiLCJhaWQiOiIwIiwibmV0IjoidGNwIiwicGF0aCI6Ii8iLCJob3N0IjoiMTUwLjIzMC40My42NSIsInRscyI6IiJ9
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9NeW5tO+8iOiHqueUqO+8iV8xIiwiYWRkIjoiMTg1LjIwMi4xNzIuMjQzIiwicG9ydCI6IjQwOTQxIiwidHlwZSI6Im5vbmUiLCJpZCI6IjQ4NTM3ODIwLTE0ZjMtNGRlNy1kMjZlLWEzYjg4YmNmMDE1YSIsImFpZCI6IjAiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9IiwiYWRkIjoiMTg1LjIwMi4xNzIuMjQzIiwicG9ydCI6IjQwOTQxIiwidHlwZSI6Im5vbmUiLCJpZCI6IjQ4NTM3ODIwLTE0ZjMtNGRlNy1kMjZlLWEzYjg4YmNmMDE1YSIsImFpZCI6IjAiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIxODUuMjAyLjE3Mi4yNDMiLCJ0bHMiOiIifQ==
    vmess://eyJ2IjoiMiIsInBzIjoiUmVsYXlf576O5Zu9LV8yMjQ3IiwiYWRkIjoiMTkyLjk2LjIwNC4yNTAiLCJwb3J0IjoiNDQzIiwidHlwZSI6Im5vbmUiLCJpZCI6ImFiYTUwZGQ0LTU0ODQtM2IwNS1iMTRhLTQ2NjFjYWY4NjJkNSIsImFpZCI6IjQiLCJuZXQiOiJ3cyIsInBhdGgiOiIvd3MiLCJob3N0IjoidXNhLXdhc2hpbmd0b24ubHZ1ZnQuY29tIiwidGxzIjoidGxzIn0=
    vmess://eyJ2IjoiMiIsInBzIjoi576O5Zu9XzM3NDUiLCJhZGQiOiIxNTAuMjMwLjQzLjY1IiwicG9ydCI6IjE0NTY0IiwidHlwZSI6Im5vbmUiLCJpZCI6IjE1NTZlMDQwLTMxZDMtNGM0Ny1iMGQyLWRkZjg4ODAxMGI0ZSIsImFpZCI6IjAiLCJuZXQiOiJ0Y3AiLCJwYXRoIjoiLyIsImhvc3QiOiIiLCJ0bHMiOiIifQ==

</details>

### 所有节点
合并节点总数: `7119`
[节点链接](https://raw.githubusercontent.com/alanbobs999/TopFreeProxies/master/sub/sub_merge.txt)

### 节点来源
- [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), 节点数量: `78`
- [chfchf0306/clash](https://github.com/chfchf0306/clash), 节点数量: `498`
- [xiyaowong/freeFQ](https://github.com/xiyaowong/freeFQ), 节点数量: `185`
- [freefq/free](https://github.com/freefq/free), 节点数量: `47`
- [learnhard-cn/free_proxy_ss](https://github.com/learnhard-cn/free_proxy_ss), 节点数量: `181`
- [vpei/Free-Node-Merge](https://github.com/vpei/Free-Node-Merge), 节点数量: `100`
- [colatiger/v2ray-nodes](https://github.com/colatiger/v2ray-nodes), 节点数量: `59`
- [oslook/clash-freenode](https://github.com/oslook/clash-freenode), 节点数量: `42`
- [ssrsub/ssr](https://github.com/ssrsub/ssr), 节点数量: `35`
- [Leon406/SubCrawler](https://github.com/Leon406/SubCrawler), 节点数量: `2445`
- [yu-steven/openit](https://github.com/yu-steven/openit), 节点数量: `303`
- [alanbobs999/TopFreeProxies](https://github.com/alanbobs999/TopFreeProxies), 节点数量: `99`
- [ldir92664/Vmess-Actions](https://github.com/ldir92664/Vmess-Actions), 节点数量: `79`
- [gooooooooooooogle/Clash-Config](https://github.com/gooooooooooooogle/Clash-Config), 节点数量: `1`
- [Jsnzkpg/Jsnzkpg](https://github.com/Jsnzkpg/Jsnzkpg), 节点数量: `79`
- [ermaozi/get_subscribe](https://github.com/ermaozi/get_subscribe), 节点数量: `145`
- [wrfree/free](https://github.com/wrfree/free), 节点数量: `47`
- [GreenFishStudio/GreenFish](https://github.com/GreenFishStudio/GreenFish), 节点数量: `28`
- [ObcbO/auto-subscribe](https://github.com/ObcbO/auto-subscribe), 节点数量: `1`
- [tomdegnan/clashrule](https://github.com/tomdegnan/clashrule), 节点数量: `214`
- [TG@getv2ray](https://t.me/getv2ray), 节点数量: `7`
- [changfengoss](https://github.com/ronghuaxueleng/get_v2), 节点数量: `902`
- [anaer/Sub](https://github.com/anaer/Sub), 节点数量: `177`
- [xrayfree/free-ssr-ss-v2ray-vpn-clash](https://github.com/xrayfree/free-ssr-ss-v2ray-vpn-clash), 节点数量: `155`
- [KYLELI1991/subscription_vless](https://github.com/KYLELI1991/subscription_vless), 节点数量: `1`
- [mhmhone/shadowrocket-free-subscribe](https://github.com/mhmhone/shadowrocket-free-subscribe), 节点数量: `31`
- [aiboboxx/v2rayfree](https://github.com/aiboboxx/v2rayfree), 节点数量: `47`
- [moneyfly1/sublist](https://github.com/moneyfly1/sublist), 节点数量: `32`
- [poduv/poduv](https://github.com/poduv/poduv), 节点数量: `82`
- [ok1991/v2ray](https://github.com/ok1991/v2ray), 节点数量: `134`
- [parkerpa/jsfxs](https://github.com/parkerpa/jsfxs), 节点数量: `582`
- [Pawdroid/Free-servers](https://github.com/Pawdroid/Free-servers), 节点数量: `0`
- [songkaik/Sub](https://github.com/songkaik/Sub), 节点数量: `135`
- [yosefwang/subscription](https://github.com/yosefwang/subscription), 节点数量: `25`
- [Nodefree.org](https://github.com/Fukki-Z/nodefree), 节点数量: `134`

## 客户端选择
### 主流桌面客户端
|                            MacOS                             |                            Linux                             |                           Windows                            | 简易描述                                           |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :------------------------------------------------- |
| [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW(Clash For Windows)](https://github.com/Fndroid/clash_for_windows_pkg/releases) | SS, SSR, Trojan, Vmess, VLESS协议支持，策略分流能力强。            |
|     [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)      |     [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)      |     [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)      | SS, SSR, Trojan, Vmess, VLESS, Trojan-Go协议支持（需安装相关插件）。 |
|                              ×                               |                              ×                               |      [V2rayN](https://github.com/2dust/v2rayN/releases)      | SS, Trojan, Vmess, VLESS协议支持，有测速，测延迟功能，支持订阅，二维码，剪贴板导入及手动配置。                 |
|                              ×                               |                              ×                               |    [WinXray](https://github.com/TheMRLL/winxray/releases)    | SS, SSR, Trojan, Vmess, VLESS协议支持，支持自动连接最快节点。            |
|                              ×                               |                              ×                               | [Shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows/releases) | SS协议支持， SS 专用客户端。                                       |
|                              ×                               |                              ×                               | [ShadowsocksR-windows](https://github.com/HMBSbige/ShadowsocksR-Windows/releases) | SSR协议支持，SSR 专用客户端。                                      |
|                [Surge](https://nssurge.com/)                 |                              ×                               |                              ×                               | SS, Trojan, Vmess协议支持，著名网络调试工具，策略分流能力强大，需付费。                        |
|   [ClashX](https://github.com/yichengchen/clashX/releases)   |                              ×                               |                              ×                               | SS, SSR, Trojan, Vmess协议支持，占用资源较少。                   |
|      [V2rayU](https://github.com/yanue/V2rayU/releases)      |                              ×                               |                              ×                               | SS, Trojan, Vmess协议支持，支持订阅，二维码，剪贴板导入，手动配置，二维码分享，与 V2RayN 类似。                        |

### 主流移动客户端
|                          iOS/iPadOS                          |                           Android                            | 简易描述                                                     |
| :----------------------------------------------------------: | :----------------------------------------------------------: | ------------------------------------------------------------ |
| [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118) | [Shadowrocket](https://play.google.com/store/apps/details?id=com.v2cross.proxy) | SS, SSR, Trojan, Vmess, VLESS协议支持，iOS端需在非国区 App Store 购买，美区售价 $2.99；安卓端非与 iOS 端同一作者，不支持 SSR 协议，免费且内置免费节点。 |
|                [Surge](https://nssurge.com/)                 |                              ×                               | SS, Trojan, Vmess协议支持，iOS 端著名网络调试工具，需付费。                                  |
| [Quantumult X](https://apps.apple.com/us/app/quantumult-x/id1443988620) |                              ×                               | SS, SSR, Trojan, Vmess协议支持，需在非国区AppStore购买，美区售价$4.99。 |
| [Potatso Lite](https://apps.apple.com/us/app/potatso-lite/id1239860606) |                              ×                               | SS, SSR协议支持，需在非国区AppStore购买，免费。              |
|                              ×                               | [Surfboard](https://play.google.com/store/apps/details?id=com.getsurfboard) | SS, SSR, Vmess协议支持，安卓端网络调试软件，兼容 Surge 2 配置。 |
|                              ×                               | [CFA(Clash For Android)](https://github.com/Kr328/ClashForAndroid/releases) | SS, SSR, Trojan, Vmess协议支持。                             |
|                              ×                               |  [SagerNet](https://github.com/SagerNet/SagerNet/releases)   | SS, SSR, Trojan, Vmess, VLESS协议支持。                      |
|                              ×                               | [Shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android/releases) | SS协议支持，安卓专用 SS 客户端。                                                 |
|                              ×                               | [ShadowsocksR-android](https://github.com/HMBSbige/ShadowsocksR-Android/releases) | SSR协议支持，安卓专用 SSR 客户端。                                                |
|                              ×                               |     [V2rayNG](https://github.com/2dust/v2rayNG/releases)     | SS, Trojan, Vmess, VLESS协议支持，v2ray 内核。                           |

## 机场推荐
免费节点失效太快，推荐一些性价比高的机场应急使用。
- [魔戒.net](https://www.mojie.cyou/#/register?code=sAbl0qtT)
  - 按量计费机场, 1¥10G, 10¥130G
  - 所有套餐均是一样的节点与一样的服务，所有套餐流量永不过期，用完为止，不限制客户端数量，最高可提供 2Gbps 峰值。
- [大迅云](https://daxun.club/#/register?code=JPmAFPav)
  - 最低月付 5¥50G, 购买 12¥ 及以上套餐免费领取奈飞 + 迪士尼 Plus 共享号
  - 原生IP负载均衡，流媒体解锁晚高峰油管秒开，主打性价比，有试用
- [阿伟云](https://awslcn.xyz/#/register?code=8C18uZwl)
  - 最低月付 1¥ 起, 9.99¥100G
  - 无带宽速率限制，有流媒体解锁，香港 BGP 中继线路

## 仓库声明
订阅节点仅作学习交流使用，只是对网络上节点的优选排序，用于查找资料，学习知识，不做任何违法行为。所有资源均来自互联网，仅供大家交流学习使用，出现违法问题概不负责。

## 星标统计
[![Stargazers over time](https://starchart.cc/alanbobs999/TopFreeProxies.svg)](https://starchart.cc/alanbobs999/TopFreeProxies)