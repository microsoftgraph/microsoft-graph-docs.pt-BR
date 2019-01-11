---
title: tipo de recurso networkInterface
description: Representa uma placa de Interface de rede (NIC) associado a este host.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823300"
---
# <a name="networkinterface-resource-type"></a>tipo de recurso networkInterface

Representa uma placa de Interface de rede (NIC) associado a este host.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|Descrição do NIC (adaptador de Ethernet por exemplo, Conexão de área Local de adaptador de LAN sem fio * <> #, etc.).|
|ipV4Address|Cadeia de caracteres|Último endereço IPv4 associado a este NIC.|
|ipV6Address|Cadeia de caracteres|Última (também conhecido como global) endereço IPv6 público associado a este NIC.|
|localIpV6Address|Cadeia de caracteres|Últimos local endereço IPv6 (conexão local ou de site local) associado a este NIC.|
|macAddress|Cadeia de caracteres|Endereço MAC da NIC nesse host.|

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
