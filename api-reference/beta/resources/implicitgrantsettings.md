---
title: tipo de recurso implicitGrantSettings
description: Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506219"
---
# <a name="implicitgrantsettings-resource-type"></a>tipo de recurso implicitGrantSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica se este aplicativo Web pode solicitar tokens usando o fluxo implícito do OAuth 2,0. Propriedades separadas estão disponíveis para solicitar tokens de ID e acesso como parte do fluxo implícito. Para habilitar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Booliano | Especifica se este aplicativo Web pode solicitar um token de ID usando o fluxo implícito do OAuth 2,0.|
|enableAccessTokenIssuance| Booliano | Especifica se este aplicativo Web pode solicitar um token de acesso usando o fluxo implícito do OAuth 2,0.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

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
