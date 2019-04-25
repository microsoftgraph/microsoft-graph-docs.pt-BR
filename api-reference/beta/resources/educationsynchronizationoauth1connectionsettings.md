---
title: recurso educationSynchronizationOAuth1ConnectionSettings
description: Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 71e45033c022061b72c1ea0be815ff3e0b611475
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542817"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>recurso educationSynchronizationOAuth1ConnectionSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.

Derivado de [Microsoft. Graph. educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Propriedades

Nenhuma propriedade adicional é exposta por esse tipo.

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth1connectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
