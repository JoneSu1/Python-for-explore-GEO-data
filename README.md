# Python-for-explore-GEO-data

**Using python to load the GEO data**

The first step is insall package: GEOparse

```
import GEOparse
import GEOparse

# GEO数据集的ID，例如"GSEXXXXX"
gse_id = 'GSEXXXXX'

# 下载并读取GEO数据集
gse = GEOparse.get_GEO(geo=gse_id)

# 查看GEO数据集的摘要信息
print(gse.metadata)

# 查看样本信息
for gsm_name, gsm in gse.gsms.items():
    print(gsm_name)
    print(gsm.metadata)

# 查看平台信息
for gpl_name, gpl in gse.gpls.items():
    print(gpl_name)
    print(gpl.metadata)


```
