---
title: tipo de recurso riskyUserHistoryItem
description: item de histórico de usuários arriscados
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 551f008696b3c9507f1cae414c34de5a8779ab24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984156"
---
# <a name="riskyuserhistoryitem-resource-type"></a>tipo de recurso riskyUserHistoryItem

Namespace: microsoft.graph

Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.


Herda de [riskyUser](../resources/riskyuser.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Histórico de lista](../api/riskyuser-list-history.md)|coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obtenha o riskyUserHistoryItems da propriedade de navegação History.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e os relacionamentos de um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|[riskUserActivity](../resources/riskuseractivity.md)|A atividade relacionada à alteração no nível de risco do usuário.|
|id|String|Herdado da [entidade](../resources/entity.md)|
|initiatedBy|String|A ID do ator que faz a operação.|
|isDeleted|Boolean| Herdado de [riskyUser](../resources/riskyuser.md)|
|isprocessoing|Boolean| Herdado de [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|Herdado de [riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Herdado de [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|Herdado de [riskyUser](../resources/riskyuser.md). Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Herdado de [riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Herdado de [riskyUser](../resources/riskyuser.md)|
|userId|Cadeia de caracteres|A ID do usuário.|
|userPrincipalName|String|Nome UPN de usuário arriscado. Herdado de [riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|histórico|coleção [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)| Herdado de [riskyUser](../resources/riskyuser.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


