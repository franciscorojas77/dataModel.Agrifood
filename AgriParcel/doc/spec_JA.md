<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
エンティティアグリパーセル  
=============<!-- /10-Header -->  
<!-- 15-License -->  
[オープンライセンス](https://github.com/smart-data-models//dataModel.Agrifood/blob/master/AgriParcel/LICENSE.md)  
[文書が自動的に生成されます](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
グローバルな記述です：**このエンティティは、一般的な土地の区画の調和された記述を含んでいます。このエンティティは、主に農業の垂直方向と関連するIoTアプリケーションに関連している。  
バージョン：1.0.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## プロパティ一覧  

<sup><sub>[*] 属性に型がない場合は、複数の型や異なるフォーマット/パターンを持つ可能性があるためです</sub></sup>。  
- `address[object]`: 郵送先住所  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: このアイテムの別称  - `area[number]`: プロパティです。モデル：'http://schema.org/Number'.単位:'m2'.名目上の区画の面積を平方メートルで表す。  . Model: [http://schema.org/Number](http://schema.org/Number)- `areaServed[string]`: サービスまたは提供されるアイテムが提供される地理的な地域  . Model: [https://schema.org/Text](https://schema.org/Text)- `belongsTo[*]`: 関係性。アイテムが所属するエンティティ  - `category[string]`: プロパティです。モデル：'http://schema.org/Text'.土地の区画のカテゴリ 例：：**arable、grassland、vineyard、orchard、mixed crop、lowland、upland、set-aside、forestry、wetland.**。  . Model: [http://schema.org/Text](http://schema.org/Text)- `cropStatus[string]`: プロパティです。Enum：「seed, justBorn, growing, maturing, readyForHarvesting」。作物の植え付け状態を説明する列挙リストからの選択。  - `dataProvider[string]`: 調和されたデータエンティティの提供者を識別する一連の文字。  - `dateCreated[string]`: エンティティの作成タイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられる。  - `dateModified[string]`: エンティティの最終更新のタイムスタンプ。これは通常、ストレージプラットフォームによって割り当てられる。  - `description[string]`: このアイテムの説明  - `hasAgriCrop[*]`: 関係。この区画に関連する作物への言及  - `hasAgriParcelChildren[array]`: 関係。このエンティティが関係する関連サブAgriParcelレコード  - `hasAgriParcelParent[*]`: 関係性親AgriParcelへの参照  - `hasAgriSoil[*]`: 関係性。この区画の土地に関連する土壌への言及  - `hasAirQualityObserved[*]`: 関係する。この区画で観測された大気質への言及  - `hasDevices[array]`: プロパティです。この区画に関連するIoTデバイス（センサー、制御装置など）を参照する。  - `id[*]`: エンティティの一意な識別子  - `irrigationSystemType[string]`: プロパティEnum: 'Surface irrigation', 'Localized irrigation', 'Drip irrigation', 'Sprinkler irrigation', 'Center pivot irrigation', 'Lateral move irrigation', 'Sub-irrigation', 'Manual irrigation'.米国疾病管理予防センター（CDC）が定義する一般的な灌漑システムの種類に基づく： https://www.cdc.gov/healthywater/other/agricultural/types.html  - `lastPlantedAt[string]`: 特性を示す。作物の最終植え付け日を示す  - `location[*]`: アイテムへの Geojson 参照。Point, LineString, Polygon, MultiPoint, MultiLineString, MultiPolygon のいずれかである。  - `name[string]`: この項目の名称です。  - `ownedBy[*]`: 関係者であることアイテムの所有者（個人または団体）であること  - `owner[array]`: 所有者の固有IDを参照するJSONエンコードされた文字列を含むリストです。  - `relatedSource[array]`: 現在のエンティティが外部アプリケーションで持つ可能性のあるIDのリスト  - `seeAlso[*]`: アイテムに関する追加リソースを指す URI のリスト。  - `soilTextureType[string]`: プロパティです。Enum: 'Sands', 'Loamy sands', 'Sandy loams', 'Loam', 'Silt loam', 'Silt', 'Sandy clay loam', 'Clay loam', 'Silty clay loam', 'Sandy clay', 'Silty clay', 'Clay'.米国農務省（USDA）の土質分類に基づく： https://www.nrcs.usda.gov/wps/portal/nrcs/detailfull/soils/ref/?cid=nrcs142p2_054262  - `source[string]`: エンティティデータの元のソースをURLとして与える一連の文字。ソースプロバイダの完全修飾ドメイン名、またはソースオブジェクトのURLであることが推奨されます。  - `type[string]`: プロパティです。NGSI Entity Typeです。AgriParcelである必要があります。  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
必須プロパティ  
- `area`  - `hasAgriCrop`  - `id`  - `location`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
このエンティティは、主に農業の垂直方向と関連するIoTアプリケーションに関連しています。古いバージョン（0.x.x）では、文字列として単一のhasAirQualityObserved値が存在します。バージョン1.x.xでは、この属性に配列があります。  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## プロパティのデータモデル記述  
アルファベット順（クリックで詳細表示）  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
AgriParcel:    
  description: This entity contains a harmonised description of a generic parcel of land. This entity is primarily associated with the agricultural vertical and related IoT applications.    
  properties:    
    address:    
      description: The mailing address    
      properties:    
        addressCountry:    
          description: 'Property. The country. For example, Spain. Model:''https://schema.org/addressCountry'''    
          type: string    
        addressLocality:    
          description: 'Property. The locality in which the street address is, and which is in the region. Model:''https://schema.org/addressLocality'''    
          type: string    
        addressRegion:    
          description: 'Property. The region in which the locality is, and which is in the country. Model:''https://schema.org/addressRegion'''    
          type: string    
        district:    
          description: 'A district is a type of administrative division that, in some countries, is managed by the local government.'    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
        streetNr:    
          description: Number identifying a specific property on a public street.    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    alternateName:    
      description: An alternative name for this item    
      type: string    
      x-ngsi:    
        type: Property    
    area:    
      description: 'Property. Model:''http://schema.org/Number''. Units:''m2''. The area of the parcel nominally in square meters.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: http://schema.org/Number    
        type: Property    
        units: m2    
    areaServed:    
      description: The geographic area where a service or offered item is provided    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    belongsTo:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Relationship. Entity the item belongs to    
      x-ngsi:    
        type: Relationship    
    category:    
      description: 'Property. Model:''http://schema.org/Text''. The category of the parcel of land e.g.: **arable, grassland, vineyard, orchard, mixed crop, lowland, upland, set-aside, forestry, wetland.**'    
      type: string    
      x-ngsi:    
        model: http://schema.org/Text    
        type: Property    
    cropStatus:    
      description: 'Property. Enum:''seeded, justBorn, growing, maturing, readyForHarvesting''. A choice from an enumerated list describing the crop planting status'    
      enum:    
        - seeded    
        - justBorn    
        - growing    
        - maturing    
        - readyForHarvesting    
      type: string    
      x-ngsi:    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity.    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: Entity creation timestamp. This will usually be allocated by the storage platform.    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    hasAgriCrop:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Relationship. Reference to the crop associated with this parcel    
      x-ngsi:    
        type: Relationship    
    hasAgriParcelChildren:    
      description: Relationship. Related sub AgriParcel records to which this entity relates    
      items:    
        anyOf: &agriparcel_-_properties_-_hasdevices_-_items_-_anyof    
          - description: Property. Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: Property. Identifier format of any NGSI entity    
            format: uri    
            type: string    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Relationship    
    hasAgriParcelParent:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Relationship. Reference to the parent AgriParcel    
      x-ngsi:    
        type: Relationship    
    hasAgriSoil:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Relationship. Reference to the soil associated with this parcel of land    
      x-ngsi:    
        type: Relationship    
    hasAirQualityObserved:    
      description: Relationship. Reference to the air quality observed in this parcel of land    
      items:    
        anyOf:    
          - description: Property. Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: Property. Identifier format of any NGSI entity    
            format: uri    
            type: string    
      type: array    
      x-ngsi:    
        type: Relationship    
    hasDevices:    
      description: 'Property. Reference to the IoT devices associated with this parcel i.e. sensors, controls.'    
      items:    
        anyOf: *agriparcel_-_properties_-_hasdevices_-_items_-_anyof    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
    id:    
      anyOf: *agriparcel_-_properties_-_hasdevices_-_items_-_anyof    
      description: Unique identifier of the entity    
      x-ngsi:    
        type: Property    
    irrigationSystemType:    
      description: 'Property. Enum: ''Surface irrigation'', ''Localized irrigation'', ''Drip irrigation'', ''Sprinkler irrigation'', ''Center pivot irrigation'', ''Lateral move irrigation'', ''Sub-irrigation'', ''Manual irrigation''. Based on common types of irrigation systems as defined by Centers for Disease Control and Prevention (CDC): https://www.cdc.gov/healthywater/other/agricultural/types.html'    
      enum:    
        - Surface irrigation    
        - Localized irrigation    
        - Drip irrigation    
        - Sprinkler irrigation    
        - Center pivot irrigation    
        - Lateral move irrigation    
        - Sub-irrigation    
        - Manual irrigation    
      type: string    
      x-ngsi:    
        type: Property    
    lastPlantedAt:    
      description: Property. Indicates the date when the crop was last planted    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: GeoProperty. Geojson reference to the item. Point    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Point    
          type: object    
        - description: GeoProperty. Geojson reference to the item. LineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON LineString    
          type: object    
        - description: GeoProperty. Geojson reference to the item. Polygon    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Polygon    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiPoint    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPoint    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiLineString    
          type: object    
        - description: GeoProperty. Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPolygon    
          type: object    
      x-ngsi:    
        type: GeoProperty    
    name:    
      description: The name of this item.    
      type: string    
      x-ngsi:    
        type: Property    
    ownedBy:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Relationship. Owner (Person or Organization) of the item    
      x-ngsi:    
        type: Relationship    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf: *agriparcel_-_properties_-_hasdevices_-_items_-_anyof    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
    relatedSource:    
      description: List of IDs the current entity may have in external applications    
      items:    
        properties:    
          application:    
            anyOf: *agriparcel_-_properties_-_hasdevices_-_items_-_anyof    
            description: Property. Unique identifier of the entity    
          applicationEntityId:    
            type: string    
        type: object    
      type: array    
      x-ngsi:    
        type: Property    
    seeAlso:    
      description: list of uri pointing to additional resources about the item    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    soilTextureType:    
      description: 'Property. Enum: ''Sands'', ''Loamy sands'', ''Sandy loams'', ''Loam'', ''Silt loam'', ''Silt'', ''Sandy clay loam'', ''Clay loam'', ''Silty clay loam'', ''Sandy clay'', ''Silty clay'', ''Clay''. Based on the soil texture classification of the United States Department of Agriculture (USDA): https://www.nrcs.usda.gov/wps/portal/nrcs/detailfull/soils/ref/?cid=nrcs142p2_054262'    
      enum:    
        - Sands    
        - Loamy sands    
        - Sandy loams    
        - Loam    
        - Silt loam    
        - Silt    
        - Sandy clay loam    
        - Clay loam    
        - Silty clay loam    
        - Sandy clay    
        - Silty clay    
        - Clay    
      type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    type:    
      description: Property. NGSI Entity Type. It has to be AgriParcel    
      enum:    
        - AgriParcel    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
    - location    
    - area    
    - hasAgriCrop    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Agrifood/blob/master/AgriParcel/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.Agrifood/AgriParcel/schema.json    
  x-model-tags: ""    
  x-version: 1.0.2    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## ペイロードの例  
#### AgriParcel NGSI-v2 キーバリューの例  
AgriParcelをJSON-LD形式でkey-valuesとした例を示します。これは、`options=keyValues`を使用した場合にNGSI-v2と互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:AgriParcel:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
  "type": "AgriParcel",  
  "dateCreated": "2017-01-01T01:20:00Z",  
  "dateModified": "2017-05-04T12:30:00Z",  
  "location": {  
    "type": "Polygon",  
    "coordinates": [[[100, 0], [101, 0], [101, 1], [100, 1], [100, 0]]]  
  },  
  "area": 200,  
  "description": "Spring wheat",  
  "category": "arable",  
  "relatedSource": [  
    {  
      "application": "urn:ngsi-ld:AgriApp:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
      "applicationEntityId": "app:parcel1"  
    }  
  ],  
  "seeAlso": [  
    "https://example.org/concept/agriparcel",  
    "https://datamodel.org/example/agriparcel"  
  ],  
  "belongsTo": "urn:ngsi-ld:AgriFarm:f67adcbc-4479-22bc-9de1-cb228de7a765",  
  "ownedBy": "urn:ngsi-ld:Person:fce9dcbc-4479-11e8-9de1-cb228de7a15c",  
  "hasAgriParcelParent": "urn:ngsi-ld:AgriParcel:1ea0f120-4474-11e8-9919-672036642081",  
  "hasAgriParcelChildren": [  
    "urn:ngsi-ld:AgriParcel:26ba4be0-4474-11e8-8ec1-ab9e0ea93835",  
    "urn:ngsi-ld:AgriParcel:2d5b8874-4474-11e8-8d6b-dbe14425b5e4"  
  ],  
  "hasAgriCrop": "urn:ngsi-ld:AgriCrop:36021150-4474-11e8-a721-af07c5fae7c8",  
  "hasAirQualityObserved": ["urn:ngsi-ld:AirQualityObserved:B3F76EA170D030BCD9E036DCC9BEA22B"],  
  "cropStatus": "seeded",  
  "lastPlantedAt": "2016-08-23T10:18:16Z",  
  "hasAgriSoil": "urn:ngsi-ld:AgriSoil:429d1338-4474-11e8-b90a-d3e34ceb73df",  
  "hasDevice": [  
    "urn:ngsi-ld:Device:4a40aeba-4474-11e8-86bf-03d82e958ce6",  
    "urn:ngsi-ld:Device:63217d24-4474-11e8-9da2-c3dd3c36891b",  
    "urn:ngsi-ld:Device:68e091dc-4474-11e8-a398-df010c53b416",  
    "urn:ngsi-ld:6f44b54e-4474-11e8-8577-d7ff6a8ef551"  
  ],  
  "soilTextureType": "Clay",  
  "irrigationSystemType": "Drip irrigation"  
}  
```  
</details>  
#### AgriParcel NGSI-v2 正規化例  
以下は、正規化されたJSON-LD形式のAgriParcelの例である。これは、オプションを使用しない場合、NGSI-v2と互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:AgriParcel:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
  "type": "AgriParcel",  
  "dateCreated": {  
    "type": "DateTime",  
    "value": "2017-01-01T01:20:00Z"  
  },  
  "dateModified": {  
    "type": "DateTime",  
    "value": "2017-05-04T12:30:00Z"  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Polygon",  
      "coordinates": [[[100, 0], [101, 0], [101, 1], [100, 1], [100, 0]]]  
    }  
  },  
  "area": {  
    "value": 200  
  },  
  "description": {  
    "value": "Spring wheat"  
  },  
  "category": {  
    "value": "arable"  
  },  
  "relatedSource": {  
    "value": [  
      {  
        "application": "urn:ngsi-ld:AgriApp:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
        "applicationEntityId": "app:parcel1"  
      }  
    ]  
  },  
  "seeAlso": {  
    "value": [  
      "https://example.org/concept/agriparcel",  
      "https://datamodel.org/example/agriparcel"  
    ]  
  },  
  "belongsTo": {  
    "type": "URL",  
    "value": "urn:ngsi-ld:AgriFarm:f67adcbc-4479-22bc-9de1-cb228de7a765"  
  },  
  "ownedBy": {  
    "type": "URL",  
    "value": "urn:ngsi-ld:Person:fce9dcbc-4479-11e8-9de1-cb228de7a15c"  
  },  
  "hasAgriParcelParent": {  
    "type": "URL",  
    "value": "urn:ngsi-ld:AgriParcel:1ea0f120-4474-11e8-9919-672036642081"  
  },  
  "hasAgriParcelChildren": {  
    "type": "URL",  
    "value": [  
      "urn:ngsi-ld:AgriParcel:26ba4be0-4474-11e8-8ec1-ab9e0ea93835",  
      "urn:ngsi-ld:AgriParcel:2d5b8874-4474-11e8-8d6b-dbe14425b5e4"  
    ]  
  },  
  "hasAgriCrop": {  
    "type": "URL",  
    "value": "urn:ngsi-ld:AgriCrop:36021150-4474-11e8-a721-af07c5fae7c8"  
  },  
  "hasAirQualityObserved": {  
    "type": "URL",  
    "value": ["urn:ngsi-ld:AirQualityObserved:B3F76EA170D030BCD9E036DCC9BEA22B"]  
  },  
  "cropStatus": {  
    "value": "seeded"  
  },  
  "lastPlantedAt": {  
    "type": "DateTime",  
    "value": "2016-08-23T10:18:16Z"  
  },  
  "hasAgriSoil": {  
    "type": "URL",  
    "value": "urn:ngsi-ld:AgriSoil:429d1338-4474-11e8-b90a-d3e34ceb73df"  
  },  
  "hasDevice": {  
    "type": "URL",  
    "value": [  
      "urn:ngsi-ld:Device:4a40aeba-4474-11e8-86bf-03d82e958ce6",  
      "urn:ngsi-ld:Device:63217d24-4474-11e8-9da2-c3dd3c36891b",  
      "urn:ngsi-ld:Device:68e091dc-4474-11e8-a398-df010c53b416",  
      "urn:ngsi-ld:Device:6f44b54e-4474-11e8-8577-d7ff6a8ef551"  
    ]  
  },  
  "soilTextureType": {  
      "type": "string",  
      "value": "Clay"  
  },  
  "irrigationSystemType": {  
      "type": "string",  
      "value": "Drip irrigation"  
  }  
}  
```  
</details>  
#### AgriParcel NGSI-LDキーバリュー例  
AgriParcelをJSON-LD形式でkey-valuesとした例を示します。これは、`options=keyValues`を使用した場合にNGSI-LDと互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:AgriParcel:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
  "type": "AgriParcel",  
  "area": 200,  
  "belongsTo": "urn:ngsi-ld:AgriFarm:f67adcbc-4479-22bc-9de1-cb228de7a765",  
  "category": "arable",  
  "createdAt": "2017-01-01T01:20:00Z",  
  "cropStatus": "seeded",  
  "description": "Spring wheat",  
  "hasAgriCrop": "urn:ngsi-ld:AgriCrop:36021150-4474-11e8-a721-af07c5fae7c8",  
  "hasAgriParcelChildren": [  
    "urn:ngsi-ld:AgriParcel:26ba4be0-4474-11e8-8ec1-ab9e0ea93835",  
    "urn:ngsi-ld:AgriParcel:2d5b8874-4474-11e8-8d6b-dbe14425b5e4"  
  ],  
  "hasAgriParcelParent": "urn:ngsi-ld:AgriParcel:1ea0f120-4474-11e8-9919-672036642081",  
  "hasAgriSoil": "urn:ngsi-ld:AgriSoil:429d1338-4474-11e8-b90a-d3e34ceb73df",  
  "hasAirQualityObserved": [  
    "urn:ngsi-ld:AirQualityObserved:B3F76EA170D030BCD9E036DCC9BEA22B"  
  ],  
  "hasDevice": [  
    "urn:ngsi-ld:Device:4a40aeba-4474-11e8-86bf-03d82e958ce6",  
    "urn:ngsi-ld:Device:63217d24-4474-11e8-9da2-c3dd3c36891b",  
    "urn:ngsi-ld:Device:68e091dc-4474-11e8-a398-df010c53b416",  
    "urn:ngsi-ld:6f44b54e-4474-11e8-8577-d7ff6a8ef551"  
  ],  
  "lastPlantedAt": "2016-08-22T10:18:16Z",  
  "location": {  
    "coordinates": [  
      [  
        [  
          100,  
          0  
        ],  
        [  
          101,  
          0  
        ],  
        [  
          101,  
          1  
        ],  
        [  
          100,  
          1  
        ],  
        [  
          100,  
          0  
        ]  
      ]  
    ],  
    "type": "Polygon"  
  },  
  "modifiedAt": "2017-05-04T12:30:00Z",  
  "ownedBy": "urn:ngsi-ld:Person:fce9dcbc-4479-11e8-9de1-cb228de7a15c",  
  "relatedSource": [  
    {  
      "application": "urn:ngsi-ld:AgriApp:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
      "applicationEntityId": "app:parcel1"  
    }  
  ],  
  "seeAlso": [  
    "https://example.org/concept/agriparcel",  
    "https://datamodel.org/example/agriparcel"  
  ],  
  "@context": [  
    "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Agrifood/master/context.jsonld"  
  ]  
}  
```  
</details>  
#### AgriParcel NGSI-LD 正規化例  
AgriParcelをJSON-LD形式で正規化した例を示します。これはオプションを使用しない場合のNGSI-LDと互換性があり、個々のエンティティのコンテキストデータを返します。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:ngsi-ld:AgriParcel:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
    "type": "AgriParcel",  
    "area": {  
        "type": "Property",  
        "value": 200  
    },  
    "belongsTo": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:AgriFarm:f67adcbc-4479-22bc-9de1-cb228de7a765"  
    },  
    "category": {  
        "type": "Property",  
        "value": "arable"  
    },  
    "createdAt": "2017-01-01T01:20:00Z",  
    "cropStatus": {  
        "type": "Property",  
        "value": "seeded"  
    },  
    "description": {  
        "type": "Property",  
        "value": "Spring wheat"  
    },  
    "hasAgriCrop": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:AgriCrop:36021150-4474-11e8-a721-af07c5fae7c8"  
    },  
    "hasAgriParcelChildren": {  
        "type": "Relationship",  
        "object": [  
            "urn:ngsi-ld:AgriParcel:26ba4be0-4474-11e8-8ec1-ab9e0ea93835",  
            "urn:ngsi-ld:AgriParcel:2d5b8874-4474-11e8-8d6b-dbe14425b5e4"  
        ]  
    },  
    "hasAgriParcelParent": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:AgriParcel:1ea0f120-4474-11e8-9919-672036642081"  
    },  
    "hasAgriSoil": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:AgriSoil:429d1338-4474-11e8-b90a-d3e34ceb73df"  
    },  
    "hasAirQualityObserved": {  
        "type": "Relationship",  
        "object": ["urn:ngsi-ld:AirQualityObserved:B3F76EA170D030BCD9E036DCC9BEA22B"]  
    },  
    "hasDevice": {  
        "type": "Relationship",  
        "object": [  
            "urn:ngsi-ld:Device:4a40aeba-4474-11e8-86bf-03d82e958ce6",  
            "urn:ngsi-ld:Device:63217d24-4474-11e8-9da2-c3dd3c36891b",  
            "urn:ngsi-ld:Device:68e091dc-4474-11e8-a398-df010c53b416",  
            "urn:ngsi-ld:6f44b54e-4474-11e8-8577-d7ff6a8ef551"  
        ]  
    },  
    "lastPlantedAt": {  
        "type": "Property",  
        "value": {  
            "@type": "DateTime",  
            "@value": "2016-08-22T10:18:16Z"  
        }  
    },  
    "location": {  
        "type": "GeoProperty",  
        "value": {  
            "type": "Polygon",  
            "coordinates": [  
                [  
                    100,  
                    0  
                ],  
                [  
                    101,  
                    0  
                ],  
                [  
                    101,  
                    1  
                ],  
                [  
                    100,  
                    1  
                ],  
                [  
                    100,  
                    0  
                ]  
            ]  
        }  
    },  
    "modifiedAt": "2017-05-04T12:30:00Z",  
    "ownedBy": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:Person:fce9dcbc-4479-11e8-9de1-cb228de7a15c"  
    },  
    "relatedSource": {  
        "type": "Property",  
        "value": [  
            {  
                "application": "urn:ngsi-ld:AgriApp:72d9fb43-53f8-4ec8-a33c-fa931360259a",  
                "applicationEntityId": "app:parcel1"  
            }  
        ]  
    },  
    "seeAlso": {  
        "type": "Property",  
        "value": [  
            "https://example.org/concept/agriparcel",  
            "https://datamodel.org/example/agriparcel"  
        ]  
    },  
    "@context": [  
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Agrifood/master/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
マグニチュード単位の扱いについては、[FAQ 10](https://smartdatamodels.org/index.php/faqs/)を参照してください。  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
