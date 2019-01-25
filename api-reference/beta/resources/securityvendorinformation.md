---
title: tipo de recurso de securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512175"
---
# <a name="securityvendorinformation-resource-type"></a>tipo de recurso de securityVendorInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|Provider= |String|Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.|
|providerVersion|String|Versão do provedor ou subprovider, se ela existir, que gerou o alerta. *Required*|
|subProvider|String|Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.|
|fornecedor |String|Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye). *Required*|

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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
