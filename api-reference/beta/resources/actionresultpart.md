---
title: tipo de recurso actionResultType
description: Tipo abstrato para a modelagem de respostas de operações em massa.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a092fa4a322d0d207550947559cb5dfff4ad4625
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663996"
---
# <a name="actionresultpart-resource-type"></a>tipo de recurso actionResultPart

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato que serve como base para a modelagem de respostas de operações em massa. A propriedade **Error** é preenchida seletivamente com base em se a resposta representa um erro.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|erro|[publicError](publicerror.md) |O erro que ocorreu, se houver, durante o andamento da operação em massa.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a>Confira também

- [aadUserConversationMemberResult](aadUserConversationMemberResult.md)
- [Adicionar membros em massa à equipe](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


