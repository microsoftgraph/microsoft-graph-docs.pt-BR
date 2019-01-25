---
title: tipo de recurso de chatMessageMention
description: 'Representa uma mencionam em uma entidade chatMessage. O mencionam pode ser usuário, equipe, bot ou canal. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515346"
---
# <a name="chatmessagemention-resource-type"></a>tipo de recurso de chatMessageMention

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mencionam em uma entidade [chatMessage](chatmessage.md) . O mencionam pode ser usuário, equipe, bot ou canal. 

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|ID da entidade que está sendo mencionada|
|mentionText|string|Cadeia de caracteres usada para representar o mencionam ex.: nome de exibição do usuário, o nome da equipe etc.|
|mencionado|[identitySet](identityset.md)|O usuário que tenha sido mencionado|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
