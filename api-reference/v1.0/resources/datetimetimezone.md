# <a name="datetimetimezone-resource-type"></a>tipo de recurso dateTimeTimeZone

Descreve a data, a hora e o fuso horário de um ponto no tempo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|DateTime|String|Um único ponto de tempo em uma representação combinada de data e hora (`<date>T<time>`).|
|TimeZone|String|Um dos seguintes nomes de fuso horário.|

A propriedade _TimeZone_ pode ser definida para qualquer um dos fusos horários com suporte no Windows, bem como os nomes de fusos horários a seguir.

Etc/GMT+12

Etc/GMT+11

Pacífico/Honolulu

América/Anchorage

América/Santa_Isabel

América/Los_Angeles

América/Phoenix

América/Chihuahua

América/Denver

América/Guatemala

América/Chicago

América/Mexico_City

América/Regina

América/Bogotá

América/New_York

América/Indiana/Indianápolis

América/Caracas

América/Asunción

América/Halifax

América/Cuiabá

América/La_Paz

América/Santiago

América/St_Johns

América/São_Paulo

América/Argentina/Buenos_Aires

América/Cayenne

América/Godthab

América/Montevidéu

América/Bahia

Etc/GMT+2

Atlântico/Açores

Atlântico/Cape_Verde

África/Casablanca

Etc/GMT

Europa/Londres

Atlântico/Reykjavik

Europa/Berlim

Europa/Budapeste

Europa/Paris

Europa/Varsóvia

África/Lagos

África/Windhoek

Europa/Bucareste

Ásia/Beirute

África/Cairo

Ásia/Damasco

África/Joanesburgo

Europa/Kiev (Kiev)

Europa/Istambul

Ásia/Jerusalém

Ásia/Amman

Ásia/Bagdá

Europa/Caliningrado

Ásia/Riad

África/Nairóbi

Ásia/Teerã

Ásia/Dubai

Ásia/Baku

Europa/Moscou

Índia/Maurício

Ásia/Tbilisi

Ásia/Ierevan

Ásia/Cabul

Ásia/Karachi

Ásia/Toshkent (Tashkent)

Ásia/Kolkata (Calcutá)

Ásia/Colombo

Ásia/Katmandu

Ásia/Astana (Almaty)

Ásia/Dacca

Ásia/Ecaterimburgo

Ásia/Yakutsk (Yangon)

Ásia/Bangcoc

Ásia/Novosibirsk

Ásia/Shanghai

Ásia/Krasnoyarsk

Ásia/Cingapura

Austrália/Perth

Ásia/Taipé

Ásia/Ulan Bator

Ásia/Irkutsk

Ásia/Tóquio

Ásia/Seul

Austrália/Adelaide

Austrália/Darwin

Austrália/Brisbane

Austrália/Sidney

Pacífico/Port_Moresby

Austrália/Hobart

Ásia/Yakutsk

Pacífico/Guadalcanal

Ásia/Vladivostok

Pacífico/Auckland

Etc/GMT-12

Pacífico/Fiji

Ásia/Magadã

Pacífico/Tongatapu

Pacífico/Apia

Pacífico/Kiritimati

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
