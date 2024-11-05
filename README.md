
test
https://github.com/Kensuke-Hinata/statistic/tree/master
https://www.thequantizer.com/
https://cplusplus.com/doc/tutorial/
https://github.com/liyupi/code-roadmap


https://www.jorudan.co.jp/norikae/cgi/nori.cgi?eki1=%E7%B4%80%E4%B8%89%E4%BA%95%E5%AF%BA&eki2=%E9%95%B7%E5%B2%A1%E4%BA%AC&via_on=-1&eki3=&eki4=&eki5=&eki6=&Dyy=2023&Dmm=8&Ddd=22&Dhh=9&Dmn1=0&Dmn2=0&Cway=1&Cfp=2&Czu=2&C7=1&C2=0&C3=0&C1=0&sort=rec&C4=5&C5=0&C6=2&S=%E6%A4%9C%E7%B4%A2&Cmap1=&rf=nr&pg=0&eok1=R-&eok2=R-&eok3=&eok4=&eok5=&eok6=&Csg=1#id_nr_routeBlock_3

https://github.com/vinceright3

https://qiita.com/c60evaporator/items/ba41cef4b37465c39948

https://download.studio3t.com/studio-3t/windows/2024.3.1/studio-3t-x64.zip

show dbs
use db_name
db
db.dropDatabase()

db.createCollection("stu")
db.createCollection("stu",{capped:true, size:10})
show collections
db._collection_name.drop()

data type:
Object ID:12byte(auto)
String
Boolean: true/false
Integer
Double
Arrays
Object
Null
Timestamp
Date -> new Date('2024-01-01'), = python:datetime.datetime.now()

db._new_collection.insert({"name":"XXXX","age":10})
db._new_collection.insert({name:"XXXX",age:10})
db._collection.find()

db._collection.save({name:"XXXX",age:10})  if new: insert, if exist: update

db._collection.update({"name":"XXXX"}, {"name":"YYYY"}) overwrite
db._collection.update({"name":"XXXX"}, {$set:{"name":"YYYY"}})
db._collection.update({"name":"XXXX"}, {$set:{"name":"YYYY"}},{multi:true})

db._collection.remove({"name":"XXXX"},{justOne:true})

https://github.com/Befzz/blender3d_import_psk_psa
https://github.com/DarklightGames/io_scene_psk_psa
https://github.com/SirWaddles/JohnWickParse/blob/35956123aa1840d626fa79b5dfc75b4c910b8509/src/assets.rs#L2093

from UE4Parse.Assets.PackageReader import LegacyPackageReader
from UE4Parse.BinaryReader import BinaryStream
from UE4Parse.Versions import EUEVersion
from UE4Parse.Provider import DefaultFileProvider, MappingProvider
from UE4Parse.Versions import EUEVersion, VersionContainer
import logging

logging.getLogger("UE4Parse").setLevel(logging.DEBUG)

asset = r'C:\Blender\python\UE\test_samples\SM_build_czmhdst.uasset'
uasset = BinaryStream(asset)
uasset.mappings = MappingProvider("C:\\downloads\\wukong\\paks\\wk.usmap")
uasset.version = EUEVersion.GAME_BlackMythWukong

path = r'C:\Blender\python\UE\test_samples'
provider = DefaultFileProvider(path, VersionContainer(EUEVersion.GAME_BlackMythWukong))

reader = LegacyPackageReader(uasset, provider =provider) #, version=EUEVersion.GAME_BlackMythWukong
# reader = LegacyPackageReader(uasset)

print('\n-- Types --')
for export_data in reader.ExportMap:
  print(export_data.type.string)




