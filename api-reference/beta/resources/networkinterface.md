---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d7b712c50d8cc19951f583cb8c9af7e185dba7ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029159"
---
# <a name="networkinterface-resource-type"></a>tipo de recurso networkInterface

Namespace: microsoft.graph

Representa uma placa de interface de rede (NIC) associada a esse host.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio * < # >, etc.).|
|ipV4Address|String|Último endereço IPv4 associado a esta NIC.|
|ipV6Address|String|Último endereço IPv6 público (aka global) associado a esta NIC.|
|localIpV6Address|String|Último endereço IPv6 local (link-local ou site-local) associado a esta NIC.|
|macAddress|String|Endereço MAC da NIC neste host.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


