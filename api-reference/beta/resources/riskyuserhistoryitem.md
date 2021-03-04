---
title: Tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos dos usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ae6d5fbc28e8dddb4c782aa9e9b2fad79b347ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442849"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Tipo de recurso riskyUserHistoryItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa o histórico de risco de um usuário do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD. 

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Histórico de listas](../api/riskyuser-list-history.md) | [coleção riskyUserHistoryItem](riskyuserhistoryitem.md)|Obter o histórico de risco de um usuário do Azure AD.|


## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| userId         | cadeia de caracteres  | A id do usuário. |
| initiatedBy    | bool    | A id do ator que faz a operação. |
| atividade       | [riskUserActivity](riskuseractivity.md)| A atividade relacionada à alteração no nível de risco do usuário. | 

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->


