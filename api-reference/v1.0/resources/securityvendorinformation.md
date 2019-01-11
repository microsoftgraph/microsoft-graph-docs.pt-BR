---
title: tipo de recurso de securityVendorInformation
description: " subProvider = AppLocker)."
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820143"
---
# <a name="securityvendorinformation-resource-type"></a>tipo de recurso de securityVendorInformation

Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|provedor |Cadeia de caracteres|Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.|
|providerVersion|Cadeia de caracteres|Versão do provedor ou subprovider, se ela existir, que gerou o alerta. *Required*|
|subProvider|Cadeia de caracteres|Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.|
|fornecedor |Cadeia de caracteres|Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye). *Required*|


## <a name="json-representation"></a>Representação JSON

A seguinte é uma representação de JSON do recurso.
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
