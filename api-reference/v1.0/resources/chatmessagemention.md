---
title: Tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chatMessage. A menção pode ser para um usuário, equipe, bot ou canal. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2891a555666f7265050ec4e9b12f4d8f02500c4f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53206990"
---
# <a name="chatmessagemention-resource-type"></a>Tipo de recurso chatMessageMention

Namespace: microsoft.graph

Representa uma menção em uma [entidade chatMessage.](chatmessage.md) A menção pode ser para um [usuário](user.md), [equipe,](team.md)bot ou [canal](channel.md). 

Em um **objeto chatMessage** que contém uma ou  mais menções, a propriedade de conteúdo do corpo da mensagem representa a mensagem de chat em HTML. Ele inclui o **mentionText** de cada menção em um elemento HTML, com um atributo que corresponde à propriedade `at` `id` **id** da menção.

Como exemplo, uma mensagem de chat contém duas menções, com o texto de menção "Megan" e "Alex" respectivamente. Sua propriedade **de conteúdo** do corpo especifica elementos para as `at` duas menções da seguinte forma:

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

Na propriedade **content,** a primeira menção tem um atributo HTML `id` de 0. Isso corresponde à propriedade **id** da primeira instância **do chatMessageMention**, que também é 0.

A segunda menção tem um atributo 1, que corresponde à `id` **propriedade id** da segunda instância, que é 1.

Para um contexto mais completo do exemplo, consulte [List channel message replies](../api/chatmessage-list-replies.md#example).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Int32|Índice de uma entidade que está sendo mencionada no **chatMessage especificado.** Corresponde ao valor {index} na `<at id="{index}">` marca correspondente no corpo da mensagem.|
|mentionText|cadeia de caracteres|Cadeia de caracteres usada para representar a menção. Por exemplo, o nome de exibição de um usuário, um nome de equipe.|
|mencionado|[chatMessageMentionedIdentitySet](chatmessagementionedidentityset.md)|A entidade (usuário, aplicativo, equipe ou canal) que foi @mentioned.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"}
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
  "suppressions": []
}
-->


