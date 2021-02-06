---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório.
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: 6d5c8680d93c5fd480efae9c3f11bcbe4475e05b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133039"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório. Você deve ter uma licença P1 ou P2 do Azure AD Premium para baixar logs de login usando a API do Microsoft Graph.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Ler propriedades e relações de um objeto signIn.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|alternateSignInName|String|A identidade de login alternativa sempre que você usar o número de telefone para entrar.|
|appDisplayName|String|O nome do aplicativo exibido no Portal do Azure.|
|appId|String|O identificador de aplicativo no Azure Active Directory.|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto|Uma lista de políticas de acesso condicional que são disparadas pela atividade de entrada correspondente.|
|authenticationDetails|[Coleção authenticationDetail](authenticationdetail.md)|O resultado da tentativa de autenticação e detalhes adicionais sobre o método de autenticação.|
|authenticationMethodsUsed|Coleção de cadeias de caracteres|Os métodos de autenticação usados. Valores possíveis: `SMS` , , , , ou `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Coleção [KeyValue](keyvalue.md)|Detalhes adicionais de processamento de autenticação, como o nome do agente no caso de PTA/PHS ou nome de servidor/farm em caso de autenticação federada.|
|authenticationRequirement | string | Isso mantém o nível mais alto de autenticação necessário por meio de todas as etapas de login para que a login seja bem-sucedida.|
|clientAppUsed|Cadeia de caracteres|O cliente herddo usado para atividade de entrada. Por exemplo, Navegador, Exchange Active Sync, Clientes modernos, IMAP, MAPI, SMTP ou POP.|
|conditionalAccessStatus|cadeia de caracteres| O status da política de acesso condicional acionada. Valores possíveis: `success` `failure` , , ou `notApplied` `unknownFutureValue` .|
|correlationId|Cadeia de caracteres|O identificador que é enviado do cliente quando a entrada é iniciada. Isso é usado para solucionar problemas da atividade de login correspondente ao chamar o suporte.|
|createdDateTime|DateTimeOffset|A data e a hora em que a login foi iniciada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|As informações do dispositivo de onde ocorreu a entrada. Inclui informações como deviceId, SO e navegador. |
|id|String|O identificador que representa a atividade de login.|
|ipAddress|Cadeia de caracteres|O endereço IP do cliente de onde ocorreu a entrada.|
|isInteractive|Booliano|Indica se uma assinatura é interativa ou não.|
|location|[signInLocation](signinlocation.md)|A cidade, o estado e o código do país de duas letras de onde ocorreu a login.|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Os detalhes do local de rede, como endereço IP, local da login, o tipo de rede usado e seus nomes. Valores possíveis: `Named Netowrk` `Extranet` , , ou `Intranet` `Trusted Network` .|
|originalRequestId|Cadeia de caracteres|O identificador de solicitação da primeira solicitação na sequência de autenticação.|
|processingTimeInMilliseconds|Int|O tempo de processamento da solicitação em milissegundos no AD STS.|
|resourceDisplayName|String|O nome do recurso em que o usuário se inscreveu.|
|resourceId|Cadeia de caracteres|O identificador do recurso em que o usuário se inscreveu.|
|riskDetail|riskDetail|O motivo por trás de um estado específico de um usuário arriscado, login ou um evento de risco. Valores possíveis: `none` , , , , , , , `adminGeneratedTemporaryPassword` ou `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são `hidden` retornados.|
|riskEventTypes|Coleção riskEventType|A lista de tipos de eventos de risco associados à login. Valores possíveis: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskEventTypes_v2|Coleção de cadeias de caracteres|A lista de tipos de eventos de risco associados à login. Valores possíveis: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|O nível de risco agregado. Valores possíveis: `none` , , , ou `low` `medium` `high` `hidden` `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são `hidden` retornados.|
|riskLevelDuringSignIn|riskLevel|O nível de risco durante a login. Valores possíveis: `none` , , , ou `low` `medium` `high` `hidden` `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são `hidden` retornados.|
|riskState|riskState|O estado de risco de um usuário arriscado, entrar ou um evento de risco. Valores possíveis: `none` , , , , ou `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` .|
|servicePrincipalId|String|O identificador do aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo.|
|servicePrincipalName|Cadeia de caracteres|O nome do aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo.|
|status|[signInStatus](signinstatus.md)|O status de login. Inclui o código de erro e a descrição do erro (em caso de falha de login).|
|tokenIssuerName|Cadeia de caracteres|O nome do provedor de identidade. Por exemplo, `sts.microsoft.com`.|
|tokenIssuerType|Cadeia de caracteres|O tipo de provedor de identidade. Valores possíveis: `AzureAD` `ADFederationServices` , ou `UnknownFutureValue` .|
|userAgent|String|As informações do agente do usuário relacionadas à login.|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário.|
|userId|Cadeia de caracteres|O identificador do usuário.|
|userPrincipalName|String|O UPN do usuário.|

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
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "authenticationDetails": [{"@odata.type": "microsoft.graph.authenticationDetail"}],
  "authenticationMethodsUsed": ["String"],
  "authenticationProcessingDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "string",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "id": "String (identifier)",
  "ipAddress": "String",
  "isInteractive": true,
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": 1024,
  "resourceDisplayName": "String",
  "resourceId": "String",
  "riskDetail": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "tokenIssuerName": "String",
  "tokenIssuerType": "string",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String"
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


