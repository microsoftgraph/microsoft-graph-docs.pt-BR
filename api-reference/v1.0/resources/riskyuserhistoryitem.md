---
title: Tipo de recurso riskyUserHistoryItem
description: item de histórico de usuário arriscado
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fa835aebf8ab5d1f4e5517ded131d7ac470927ae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108860"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Tipo de recurso riskyUserHistoryItem

Namespace: microsoft.graph

Representa o histórico de risco de um usuário do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD.


Herda de [riskyUser](../resources/riskyuser.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Histórico de listas](../api/riskyuser-list-history.md)|[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obter os riskyUserHistoryItems da propriedade de navegação histórico.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e as relações de um [objeto riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|[riskUserActivity](../resources/riskuseractivity.md)|A atividade relacionada à alteração no nível de risco do usuário.|
|id|Cadeia de caracteres|Herdado da [entidade](../resources/entity.md)|
|initiatedBy|String|A id do ator que faz a operação.|
|isDeleted|Boolean| Herdado [de riskyUser](../resources/riskyuser.md)|
|isProcessing|Booliano| Herdado [de riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|Herdado [de riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Herdado [de riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|Herdado [de riskyUser](../resources/riskyuser.md). Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Herdado [de riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Herdado [de riskyUser](../resources/riskyuser.md)|
|userId|Cadeia de caracteres|A id do usuário.|
|userPrincipalName|String|Nome principal do usuário arriscado. Herdado [de riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|history|[coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)| Herdado [de riskyUser](../resources/riskyuser.md)|

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


