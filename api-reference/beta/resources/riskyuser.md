---
title: Tipo de recurso riskyUser
description: Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.
author: cloudhandler
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: ff09c334f4d7301b54d70fd2527b1884bb67019e
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060532"
---
# <a name="riskyuser-resource-type"></a>Tipo de recurso riskyUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco no Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Usar a API riskyUsers requer uma licença Azure AD Premium P2 segurança.
> 2. A disponibilidade de dados de usuário arriscados é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskyUsers](../api/riskyusers-list.md) | [coleção riskyUser](riskyuser.md)|Listar usuários arriscados e suas propriedades.|
|[Obter riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|Obtenha um usuário arriscado específico e suas propriedades.|
|[Histórico de lista](../api/riskyuser-list-history.md) | [Coleção riskyUserHistoryItem](riskyuserhistoryitem.md)|Obtenha o histórico de risco de um usuário do Azure AD.|
|[Confirmar riskyUsers comprometidos](../api/riskyusers-confirmcompromised.md)|Nenhum |Confirme um usuário arriscado como comprometido.|
|[Ignorar riskyUsers](../api/riskyusers-dismiss.md)|Nenhum | Ignore o risco de um usuário arriscado.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|id|string|ID exclusiva do usuário em risco.|
|isDeleted|boolean|Indica se o usuário foi excluído. Os valores possíveis são: `true` e `false`.|
|isProcessing|booliano|Indica se o estado arriscado de um usuário está sendo processado pelo back-end.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que o usuário suspeito foi atualizado pela última vez.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel| Nível do usuário arriscado detectado. Os valores possíveis são `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.  |
|riskState|riskState| Estado do risco do usuário. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.  |
|riskDetail|riskDetail| Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, , `adminConfirmedUserCompromised`, `unknownFutureValue`.  |
|userDisplayName|string|Nome de exibição de usuário arriscado.|
|userPrincipalName|string|Nome principal do usuário suspeito.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
