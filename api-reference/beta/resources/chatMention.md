---
title: tipo de recurso de chatMessageMention
description: 'Representa uma mencionam em uma entidade chatMessage. O mencionam pode ser usuário, equipe, bot ou canal. '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876130"
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
