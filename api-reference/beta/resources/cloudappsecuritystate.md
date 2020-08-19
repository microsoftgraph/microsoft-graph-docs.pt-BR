---
title: tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2b16d971aa22a51552588c96f4ddbb03f1d34142
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810570"
---
# <a name="cloudappsecuritystate-resource-type"></a>tipo de recurso cloudAppSecurityState

Namespace: microsoft.graph

Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationServiceIp|String|Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.|
|destinationServiceName|String|Nome do serviço/aplicativo na nuvem (por exemplo, "Salesforce", "DropBox", etc.).|
|riskScore|String|Pontuação de risco calculado/gerado pelo provedor do aplicativo/serviço de nuvem. O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
