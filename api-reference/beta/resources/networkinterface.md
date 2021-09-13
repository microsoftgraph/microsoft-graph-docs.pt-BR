---
title: Tipo de recurso networkInterface
description: Representa uma NIC (Placa de Interface de Rede) associada a esse host.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 914d7f3484762a9b2994fe1eef06d47f4ac09f75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105787"
---
# <a name="networkinterface-resource-type"></a>Tipo de recurso networkInterface

Namespace: microsoft.graph

Representa uma NIC (Placa de Interface de Rede) associada a esse host.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|Descrição do NIC (por exemplo, adaptador Ethernet, conexão de área local de LAN sem fio *<#>, etc.).|
|ipV4Address|Cadeia de Caracteres|Último endereço IPv4 associado a essa NIC.|
|ipV6Address|Cadeia de Caracteres|Último endereço IPv6 público (também conhecido como global) associado a essa NIC.|
|localIpV6Address|Cadeia de Caracteres|Último endereço IPv6 local (link local ou local) associado a esse NIC.|
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


