---
title: tipo de recurso de chatThread
description: Um chatThread é uma coleção de chatMessages em Teams da Microsoft.
localization_priority: Priority
ms.openlocfilehash: 5060d7ea846f5aedec5551aaf247642a36f73c1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833240"
---
# <a name="chatthread-resource-type"></a>tipo de recurso de chatThread

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um chatThread é uma coleção de [chatMessages](chatmessage.md) em Teams da Microsoft.

> Atualmente, chatThreads pode ser [criado no canais](../api/channel-post-chatthreads.md).  Versões de futuro API dará suporte a chatThreads existente, bem como leitura/gravação chats diretos entre os usuários que estão fora do escopo de uma equipe ou canal de leitura.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar thread](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |Inicie um novo segmento no canal especificado, fornecendo a primeira mensagem.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Anulável.|
|chatMessages|coleção [chatMessage](chatmessage.md)| Anulável.|

> Atualmente essas relações existe implicitamente, mas não pode ler ou gravados.  Versões beta futuras API dará suporte a isso.

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
  "id": "string (identifier)",
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
