---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5fd40bec964a73579863b8222cd4c90d58991502
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522572"
---
# <a name="networkinterface-resource-type"></a>tipo de recurso networkInterface

Namespace: Microsoft. Graph

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
