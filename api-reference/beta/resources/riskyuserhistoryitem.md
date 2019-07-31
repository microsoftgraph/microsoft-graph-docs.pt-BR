---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 586fdb046adc8977550cc386a27284752cf487c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965331"
---
# <a name="riskyuserhistoryitem-resource-type"></a>tipo de recurso riskyUserHistoryItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD. 

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Histórico de lista](../api/riskyuser-list-history.md) | coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)|Obter o histórico de riscos de um usuário do Azure AD.|


## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| userId         | string  | A ID do usuário. |
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
