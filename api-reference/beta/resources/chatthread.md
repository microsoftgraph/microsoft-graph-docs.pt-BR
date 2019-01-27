---
title: tipo de recurso chatThread
description: Um chatThread é uma coleção de chatMessages no Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521338"
---
# <a name="chatthread-resource-type"></a>tipo de recurso chatThread

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chatThread é uma coleção de [chatMessages](chatmessage.md) no Microsoft Teams.

> Atualmente, os chatThreads podem ser[criados em canais](../api/channel-post-chatthreads.md).  Os lançamentos futuros da API terão suporte para leitura dos chatThreads existentes, além de chats diretos de leitura/escrita entre os usuários que estão fora do escopo da equipe ou do canal.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar thread](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Inicia uma nova thread no canal especificado, fornecendo a primeira mensagem.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Anulável.|
|chatMessages|coleção de [chatMessage](chatmessage.md)| Anulável.|

> Atualmente essas relações existem implicitamente, mas não podem ler ou escreveu.  As versões Beta futuras da API oferecerão suporte para isso.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
