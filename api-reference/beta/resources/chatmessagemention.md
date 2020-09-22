---
title: tipo de recurso chatMessageMention
description: 'Representa uma menção em uma entidade chat. A menção pode ser a um usuário, uma equipe, um bot ou um canal. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b6a63380475be8bd0e669851f7e760a9f645d18d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064271"
---
# <a name="chatmessagemention-resource-type"></a>tipo de recurso chatMessageMention

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma menção em uma entidade [chat](chatmessage.md) . A menção pode ser a um [usuário](user.md), uma [equipe](team.md), um bot ou um [canal](channel.md). 

Em um objeto **chat** que contém uma ou mais menciona, a propriedade de **conteúdo** do corpo da mensagem representa a mensagem de chat em HTML. Ele inclui o **mentionText** de cada menção em um `at` elemento HTML, com um `id` atributo que corresponde à propriedade **ID** da menção.

Por exemplo, uma mensagem de chat contém duas menção, com o texto de menção "Megan" e "Alex", respectivamente. A propriedade de **conteúdo** do corpo especifica `at` os elementos das duas mencionas da seguinte maneira:

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

Na propriedade **Content** , a primeira menção tem um atributo HTML `id` de 0. Isso corresponde à propriedade **ID** dessa primeira instância de **chatMessageMention**, que também é 0.

A segunda menção tem um `id` atributo de 1, correspondendo à propriedade **ID** da segunda instância, que é 1.

Para obter um contexto mais completo do exemplo, consulte [listar respostas de mensagens de canal](../api/channel-list-messagereplies.md#example).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Int32|Índice de uma entidade que está sendo mencionada no **chat**especificado. Corresponde ao valor {index} na marca correspondente `<at id="{index}">` no corpo da mensagem.|
|mentionText|cadeia de caracteres|Cadeia de caracteres usada para representar a menção. Por exemplo, o nome de exibição de um usuário, o nome de uma equipe.|
|foi|[identitySet](identityset.md)|A entidade (usuário, aplicativo, equipe ou canal) que foi mencionada.  Se fosse um canal ou uma equipe que foi @mentioned, o identityset contém uma propriedade de **conversa** que concede a ID da equipe/canal, e uma propriedade **conversationIdentityType** que representa a equipe ou o canal.|


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
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
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


