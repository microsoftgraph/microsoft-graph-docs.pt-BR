---
title: tipo de recurso de riskyUsers
description: Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 2e4cf47ea78583958c79750e0b2ad4fa12230d22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950729"
---
# <a name="riskyusers-resource-type"></a>tipo de recurso de riskyUsers

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os usuários do Windows Azure AD que estão em risco. Azure AD continuamente avalia o risco de usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários em risco em sua Azure AD.

> **Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Proteção de identidade do Windows Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Lista riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyuser.md) |Listar usuários riscados e suas propriedades.|
|[Obter riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyuser.md)|Obtenha um usuário riscado específico e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|Id exclusiva do usuário em risco|
|`isDeleted`|`bool`|Indica se o usuário é excluído. Os valores possíveis são: `true`,`false`|
|`isGuest`|`bool`|Indica se o usuário é um usuário convidado. Os valores possíveis são: `true` e `false`. True se a identidade do usuário encontra-se fora do locatário em consideração. Esse usuário pode ser uma B2B ou um usuário B2C com identidade no Azure AD, MSA ou 3º provedor de identidade de terceiros. False se a identidade do usuário estiver dentro do locatário em consideração|
|`riskDetail`|`riskDetail`|Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.|
|`riskLevel`|`riskLevel`|Fornece o nível de risco geral de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.|
|`riskState`|`riskState`|Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|`riskLastUpdatedDateTime`|`datetime`|A data e hora em que o usuário riscado foi atualizada pela última vez|
|`userDisplayName`|`string`|Nome de exibição do usuário riscado|
|`userPrincipalName`|`string`|Nome principal de usuário riscado|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|UserObjectId| O identificador exclusivo do usuário com a qual um evento de determinado risco está associado.|
|isGuest|isGuest| Um usuário riscado poderia ser um usuário Home (B2E) ou um usuário convidado (B2B, B2C).|
|isDeleted|isDeleted| Um usuário pode ou não pode ser excluído. |
|riskState|riskState| Um usuário riscado pode existir em um dos vários estados. |
|riskDetail|riskDetail| Um usuário riscado poderia ser em um determinado estado por vários motivos. |
|riskLevel|riskLevel| Um usuário riscado poderia ser considerado um dos vários níveis de risco. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
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
