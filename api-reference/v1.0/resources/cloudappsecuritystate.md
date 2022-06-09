---
title: Tipo de recurso cloudAppSecurityState
description: Contém informações com estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
author: preetikr
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b367766b7605a0c0444c17d962e9e034269683f2
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65970934"
---
# <a name="cloudappsecuritystate-resource-type"></a>Tipo de recurso cloudAppSecurityState

Namespace: microsoft.graph

Contém informações com estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationServiceIp|Cadeia de caracteres|Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.|
|destinationServiceName|String|Nome do aplicativo/serviço de nuvem (por exemplo, "Salesforce", "DropBox", etc.).|
|riskScore|Cadeia de caracteres|Pontuação de risco calculada/gerada pelo provedor do Aplicativo/Serviço de Nuvem. Intervalo de valor recomendado de 0 a 1, que equivale a um percentual.|

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

