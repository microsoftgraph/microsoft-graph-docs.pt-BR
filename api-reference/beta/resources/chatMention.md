---
title: tipo de recurso de chatMessageMention
description: 'Representa uma mencionam em uma entidade chatMessage. O mencionam pode ser usuário, equipe, bot ou canal. '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033429"
---
# <a name="chatmessagemention-resource-type"></a>tipo de recurso de chatMessageMention

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
