---
title: tipo de recurso de implicitGrantSettings
description: Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 82051c3605d9815fef8a0852e0ffa9075f4a6d78
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574513"
---
# <a name="implicitgrantsettings-resource-type"></a>tipo de recurso de implicitGrantSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | Especifica se esse aplicativo web pode solicitar um token de ID usando o fluxo de implícita OAuth 2.0.|
|enableAccessTokenIssuance| Boolean | Especifica se esse aplicativo web pode solicitar um token de acesso usando o fluxo de implícita OAuth 2.0.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
