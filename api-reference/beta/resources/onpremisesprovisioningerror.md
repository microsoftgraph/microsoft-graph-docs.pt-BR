---
title: tipo de recurso de onPremisesProvisioningError
description: Representa os erros de sincronização de diretório para o usuário, grupo ou organizacionais entidades visita quando a sincronização local diretórios no Windows Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512728"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>tipo de recurso de onPremisesProvisioningError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os erros de sincronização de diretório para as entidades de [usuário](user.md), [grupo](group.md)ou [contato organizacional](orgcontact.md) quando a sincronização local diretórios no Windows Azure Active Directory.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|Ferramentas para desenvolvedores|String| Categoria do erro provisionamento. Observação: No momento, há apenas um valor possível. Valores possíveis: *PropertyConflict* - indica um valor de propriedade não é exclusivo. Outros objetos contenham o mesmo valor da propriedade. |
|occurredDateTime|DateTimeOffset| A data e hora em que o erro ocorreu. |
|propertyCausingError|String| Nome da propriedade diretório que causou o erro. Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress* |
|valor|String| Valor da propriedade que causou o erro. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
