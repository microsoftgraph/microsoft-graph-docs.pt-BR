---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 519e2a7fdb6662496cdb660095ec63ce81b849f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521051"
---
# <a name="riskyuserhistoryitem-resource-type"></a>tipo de recurso riskyUserHistoryItem

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD. 

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Histórico de lista](../api/riskyuser-list-history.md) | coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)|Obter o histórico de riscos de um usuário do Azure AD.|


## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| userId         | cadeia de caracteres  | A ID do usuário. |
| initiatedBy    | bool    | A ID do ator que faz a operação. |
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
