---
title: Tipo de recurso riskyServicePrincipalHistoryItem
description: Representa o histórico de risco das entidades de serviço do Azure AD
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aaafd1236a31530c32ca9cb6f62db932a0588f9e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519919"
---
# <a name="riskyserviceprincipalhistoryitem-resource-type"></a>Tipo de recurso riskyServicePrincipalHistoryItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa o histórico de risco de uma entidade de serviço do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD. Herda [de riskyServicePrincipal](riskyserviceprincipal.md).

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Histórico de listas](../api/riskyserviceprincipal-list-history.md) | [Coleção riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md)|Obter o histórico de risco de uma entidade de serviço do Azure AD.|


## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| servicePrincipalId         | string  | O identificador da entidade de serviço. |
| initiatedBy    | bool    | O identificador do ator da operação. |
| atividade       | [riskServicePrincipalActivity](riskserviceprincipalactivity.md)| A atividade relacionada à alteração no nível de risco principal do serviço. | 

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyServicePrincipalHistoryItem",
  "baseType": "microsoft.graph.riskyServicePrincipal"
}-->

```json
{
    "servicePrincipalId": "String",
    "initiatedBy": "String",
    "activity": {"@odata.type": "microsoft.graph.riskServicePrincipalActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyServicePrincipalHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
