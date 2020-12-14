---
title: tipo de recurso aadUserConversationMemberResult
description: Recurso para a modelagem de respostas de operações em massa no aadUserConversationMember.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663901"
---
# <a name="aaduserconversationmemberresult-resource-type"></a>tipo de recurso aadUserConversationMemberResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta individual para cada membro especificado em uma operação em massa que consiste em [aadUserConversationMember (s)](aadUserConversationMember.md) na solicitação.
Este recurso é a derivada do recurso [actionResultPart](actionresultpart.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|userId|`String`|A ID de objeto do usuário do Azure AD que foi adicionada como parte da operação em massa.|
|erro|[publicError](publicerror.md) |O erro que ocorreu, se houver, durante o andamento da operação em massa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a>Confira também

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


