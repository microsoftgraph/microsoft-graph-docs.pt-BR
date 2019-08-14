---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Descreve o recurso signIn da API do Microsoft Graph (REST), que ajuda a auditar a atividade de login de usuário e de aplicativo (versão beta).
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0f3977c14ce8e0e53cdbd296ea28c4b79f5762
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396741"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Ler propriedades e relações de um objeto signIn.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|Cadeia de caracteres|Refere-se ao nome do aplicativo exibido no Portal do Azure.|
|appId|Cadeia de caracteres|Se refere a GUID exclusivo que representa o Id de aplicativo no Azure Active Directory.|
|clientAppUsed|Cadeia de caracteres|Fornece o cliente herdado usado para entrar na atividade E.g. inclui o navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto|Fornece uma lista de políticas de acesso condicional acionada por atividade correspondente entrar.|
|conditionalAccessStatus|cadeia de caracteres| Fornece o status da política de acesso condicional disparado. Os valores possíveis são: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|originalRequestId|Cadeia de caracteres|A id de solicitação da primeira solicitação na sequência de autenticação.|
|isInteractive|Booliano|Indica se uma entrada é interativa ou não.|
|tokenIssuerName|Cadeia de caracteres|Nome do provedor da identidade (por exemplo, sts.microsoft.com)|
|tokenIssuerType|Cadeia de caracteres|Fornece o tipo de identityProvider. Os valores possíveis são `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|Cadeia de caracteres|Refere-se a ID que é enviada do cliente quando é iniciado a entrada. Isso é usado para solução de problemas da atividade de entrada correspondente ao chamar o suporte ou obter assistência técnica.|
|createdDateTime|DateTimeOffset|Fornece a data e hora que a entrada foi iniciada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|Fornece as informações de dispositivo do qual a entrada ocorreu. Ele inclue informações como deviceId, OS, navegador. |
|id|Cadeia de caracteres|Indica que representa a atividade de ID exclusiva.|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde a entrada ocorreu.|
|location|[signInLocation](signinlocation.md)|Fornece a cidade, código de estado e 2 letras do país de onde a entrada ocorreu.|
|processingTimeInMilliseconds|Int|Fornece a solicitação de processamento de tempo em milissegundos no AD STS|
|riskDetail|`riskDetail`|Fornece o motivo por trás de um estado específico de um usuário arriscado, uma entrada arriscada ou um evento de risco. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelAggregated|`riskLevel`|Fornece o nível de risco agregado. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelDuringSignIn|`riskLevel`|Fornece o nível de risco durante a entrada. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskEventTypes|coleção `riskEventType`|Fornece a lista de tipos de evento de risco associados à entrada. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` e `unknownFutureValue`.|
|riskState|`riskState`|Fornece o motivo atrás de um estado específico de um usuário arriscado, entrada ou um evento de risco. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Fornece a MFA relacionada a informações como a MFA, MFA Status Requerido para a entrada correspondente.|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Fornece detalhes sobre o local de rede.|
|status|[signInStatus](signinstatus.md)|Fornece o status de entrada. Os valores possíveis incluem `Success` e `Failure`.|
|userDisplayName|Cadeia de caracteres|Indica o nome de exibição do usuário.|
|userId|Cadeia de caracteres|Indica que o userId do usuário.|
|userPrincipalName|Cadeia de caracteres|Indica o userId do usuário.|
|resourceDisplayName|Cadeia de caracteres|Indica o nome do recurso que o usuário entrou|
|resourceId|Cadeia de caracteres|Indica o Id do recurso que o usuário entrou.|
|authenticationMethodsUsed|Cadeia de caracteres|Indica a lista de métodos de autenticação usado|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "processingTimeInMilliseconds": 12356,
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
