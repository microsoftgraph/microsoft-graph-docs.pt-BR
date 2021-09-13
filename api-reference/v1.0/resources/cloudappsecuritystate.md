---
title: Tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d04a23bb38c9f5264057d56d43de0f053dd58b9c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118754"
---
# <a name="cloudappsecuritystate-resource-type"></a>Tipo de recurso cloudAppSecurityState

Namespace: microsoft.graph

Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationServiceIp|Cadeia de caracteres|Endereço IP de destino da conexão com o aplicativo/serviço na nuvem.|
|destinationServiceName|String|Nome do aplicativo/serviço na nuvem (por exemplo, "Salesforce", "DropBox", etc.).|
|riskScore|String|Pontuação de risco gerada/calculada pelo provedor do Aplicativo/Serviço na Nuvem. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|

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

