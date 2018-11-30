---
title: tipo de recurso networkInterface
description: Representa uma placa de Interface de rede (NIC) associado a este host.
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033843"
---
# <a name="networkinterface-resource-type"></a>tipo de recurso networkInterface

Representa uma placa de Interface de rede (NIC) associado a este host.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição do NIC (adaptador de Ethernet por exemplo, Conexão de área Local de adaptador de LAN sem fio * <> #, etc.).|
|ipV4Address|String|Último endereço IPv4 associado a este NIC.|
|ipV6Address|String|Última (também conhecido como global) endereço IPv6 público associado a este NIC.|
|localIpV6Address|String|Últimos local endereço IPv6 (conexão local ou de site local) associado a este NIC.|
|macAddress|String|Endereço MAC da NIC nesse host.|

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