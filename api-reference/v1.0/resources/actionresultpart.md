---
title: Tipo de recurso actionResultPart
description: Tipo abstrato para modelar respostas de operações em massa.
author: abshar-teams
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb09088bfdd298d286447b63453f1965f38a9e6a
ms.sourcegitcommit: 30fca91ed203a9ab7b0562833ce0c20c7fb7b7b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/27/2021
ms.locfileid: "59932057"
---
# <a name="actionresultpart-resource-type"></a>Tipo de recurso actionResultPart

Namespace: microsoft.graph

Um tipo abstrato que serve como base para modelar respostas de operações em massa. A **propriedade** error é preenchida seletivamente com base em se a resposta representa um erro.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|erro|[publicError](publicerror.md) |O erro que ocorreu, se for o caso, durante o curso da operação em massa.|

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

- [Adicionar membros em massa a uma equipe](../api/conversationmembers-add.md)

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


