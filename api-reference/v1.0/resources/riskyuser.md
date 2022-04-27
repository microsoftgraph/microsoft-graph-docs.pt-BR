---
title: Tipo de recurso riskyUser
description: item de usuários arriscados
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 222ff5f10fdb7ddf9ebd80209551d5e3f44ce83b
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060783"
---
# <a name="riskyuser-resource-type"></a>Tipo de recurso riskyUser

Namespace: microsoft.graph

Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Usar a API riskyUsers requer uma licença Azure AD Premium P2 segurança.
> 2. A disponibilidade de dados de usuário arriscados é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskyUsers](../api/riskyuser-list.md)|[coleção riskyUser](../resources/riskyuser.md)|Obtenha uma lista dos **objetos riskyUser** e suas propriedades.|
|[Obter riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Leia as propriedades e as relações de um **objeto riskyUser** .|
|[Ignorar um riskyUser](../api/riskyuser-dismiss.md)|Nenhum|Ignore o risco de um ou mais **objetos riskyUser** . |
|[Confirmar um riskyUser como comprometido](../api/riskyuser-confirmcompromised.md)|Nenhum|Confirme um ou mais **objetos riskyUser** como comprometidos.|
|[Histórico de lista](../api/riskyuser-list-history.md)|[Coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Obtenha **riskyUserHistoryItems** da propriedade de navegação de histórico.|
|[Obter histórico](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Leia as propriedades e as relações de um [objeto riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva do usuário em risco.|
|isDeleted|Boolean|Indica se o usuário foi excluído. Os valores possíveis são: `true` e `false`.|
|isProcessing|Boolean|Indica se o estado arriscado de um usuário está sendo processado pelo back-end.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário suspeito foi atualizado pela última vez.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel|Nível do usuário arriscado detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Estado do risco do usuário. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|Nome de exibição de usuário arriscado.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário suspeito.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|História|[Coleção riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|   A atividade relacionada à alteração no nível de risco do usuário|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
