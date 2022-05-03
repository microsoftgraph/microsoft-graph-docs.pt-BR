---
title: Tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: preetikr
ms.openlocfilehash: 9c2d2b8558730a832d6658ce6ef137d609a13d04
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176812"
---
# <a name="networkinterface-resource-type"></a>Tipo de recurso networkInterface

Namespace: microsoft.graph

Representa uma placa de interface de rede (NIC) associada a esse host.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio *<#> etc.).|
|ipV4Address|Cadeia de Caracteres|Último endereço IPv4 associado a essa NIC.|
|Endereço_ipv6|Cadeia de Caracteres|Último endereço IPv6 público (também conhecido como global) associado a essa NIC.|
|localIpV6Address|Cadeia de Caracteres|Último endereço IPv6 local (link local ou local) associado a essa NIC.|
|macAddress|Cadeia de Caracteres|Endereço MAC da NIC neste host.|

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


