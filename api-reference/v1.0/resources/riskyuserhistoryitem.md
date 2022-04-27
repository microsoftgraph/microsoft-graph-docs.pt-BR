---
title: Tipo de recurso riskyUserHistoryItem
description: item de histórico de usuário arriscado
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5853ec669c4b8ed1e048dce701ac65b3fbc1dc4
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060976"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Tipo de recurso riskyUserHistoryItem

Namespace: microsoft.graph

Representa o histórico de risco de um usuário do Azure AD, conforme determinado pelo Azure AD Identity Protection.

Herda de [riskyUser](../resources/riskyuser.md).

>[!NOTE]
> 1. Usar essa API requer uma licença Azure AD Premium P2 aplicativo.
> 2. A disponibilidade dos dados do histórico de riscos é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Histórico de lista](../api/riskyuser-list-history.md)|[Coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obtenha riskyUserHistoryItems da propriedade de navegação de histórico.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e as relações de um [objeto riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|[riskUserActivity](../resources/riskuseractivity.md)|A atividade relacionada à alteração no nível de risco do usuário.|
|id|String|Herdado da [entidade](../resources/entity.md)|
|initiatedBy|String|A ID do ator que faz a operação.|
|isDeleted|Boolean| Herdado de [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| Herdado de [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|Herdado de [riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Herdado de [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|Herdado de [riskyUser](../resources/riskyuser.md). Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Herdado de [riskyUser](../resources/riskyuser.md). Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Herdado de [riskyUser](../resources/riskyuser.md)|
|userId|Cadeia de caracteres|A ID do usuário.|
|userPrincipalName|String|Nome principal do usuário suspeito. Herdado de [riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|História|[Coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)| Herdado de [riskyUser](../resources/riskyuser.md)|

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


