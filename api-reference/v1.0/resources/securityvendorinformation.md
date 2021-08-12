---
title: Tipo de recurso securityVendorInformation
description: " subProvider=AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a0b0d5ece58a1db1ce929b4bc72de7e8f9c1a44fdd8ccab15aee0d2c47143dcc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216550"
---
# <a name="securityvendorinformation-resource-type"></a>Tipo de recurso securityVendorInformation

Namespace: microsoft.graph

Contém detalhes sobre o fornecedor de produto/serviço de segurança, provedor e subprovider (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|provider |Cadeia de caracteres|Provedor específico (produto/serviço - não empresa de fornecedor); por exemplo, WindowsDefenderATP.|
|providerVersion|Cadeia de caracteres|Versão do provedor ou subprovider, se existir, que gerou o alerta. *Required*|
|subProvider|String|Subprovider específico (em provedor agregador); por exemplo, WindowsDefenderATP.SmartScreen.|
|vendor |Cadeia de caracteres|Nome do fornecedor de alerta (por exemplo, Microsoft, Dell, FireEye). *Required*|


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

