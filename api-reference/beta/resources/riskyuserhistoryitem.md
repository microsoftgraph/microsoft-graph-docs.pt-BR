---
title: Tipo de recurso riskyUserHistoryItem
description: Representa o histórico de risco de usuários do Azure AD
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6a415325c26226ad2400ce572146bbfaa5beb8c7
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060665"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Tipo de recurso riskyUserHistoryItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa o histórico de risco de um usuário do Azure AD, conforme determinado pelo Azure AD Identity Protection.

>[!NOTE]
> 1. Usar essa API requer uma licença Azure AD Premium P2 aplicativo.
> 2. A disponibilidade dos dados do histórico de riscos é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Histórico de lista](../api/riskyuser-list-history.md) | [Coleção riskyUserHistoryItem](riskyuserhistoryitem.md)|Obtenha o histórico de risco de um usuário do Azure AD.|


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


