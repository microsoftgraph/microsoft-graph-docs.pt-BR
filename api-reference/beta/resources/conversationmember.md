---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 796bbe9f64342f97a9ae18363fdc01dc1712d015
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507398"
---
# <a name="conversationmember-resource-type"></a>tipo de recurso conversationMember

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros do bate-papo](../api/conversationmember-list.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.|
|[Obter membro do bate-papo](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Obter um único usuário no bate-papo.|
|[Listar membros](../api/conversationmember-list.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no chat ou canal.|
|[Obter membro](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Obter um único usuário no chat ou canal.|
|[Adicionar membro](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Adicionar um membro a um canal.|
|[Atualizar membro](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Atualizar um membro no canal.|
|[Excluir membro](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Excluir um membro do canal.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusivo do usuário.|
|displayName| cadeia de caracteres | O nome de exibição do usuário. |
|funções| coleção de cadeias de caracteres | As funções desse usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
