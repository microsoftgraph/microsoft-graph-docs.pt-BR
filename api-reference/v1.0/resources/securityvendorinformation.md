---
title: Tipo de recurso securityVendorInformation
description: " subProvider=AppLocker)."
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ed666cb4948d658dc877567bbbf31a0e6d551778
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142506"
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
|vendor |String|Nome do fornecedor de alerta (por exemplo, Microsoft, Dell, FireEye). *Required*|


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

