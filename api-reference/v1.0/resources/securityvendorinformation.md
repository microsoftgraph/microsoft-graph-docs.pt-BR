---
title: tipo de recurso securityVendorInformation
description: " subfornecedor = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 536ed37cfe8ba190a22ef86e190af2b171d352ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983981"
---
# <a name="securityvendorinformation-resource-type"></a>tipo de recurso securityVendorInformation

Namespace: microsoft.graph

Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|provedor |String|Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.|
|providerVersion|String|Versão do provedor ou do subfornecedor, se existir, que gerou o alerta. *Required*|
|subprovedor|String|Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.|
|fornecedor |String|Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye). *Required*|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

