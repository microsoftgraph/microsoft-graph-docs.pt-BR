---
title: tipo de recurso chatThread
description: Um chatThread é uma coleção de chatMessages no Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399602"
---
# <a name="chatthread-resource-type"></a>tipo de recurso chatThread

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
