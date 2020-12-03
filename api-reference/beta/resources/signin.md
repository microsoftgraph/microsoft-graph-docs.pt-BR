---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório.
author: besiler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 97a3c3807c4abe25594ad918b8717efad4ce7770
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563678"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

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
|alternateSignInName|String|A identidade de entrada alternativa sempre que você usa o número de telefone para entrar.|
|appDisplayName|String|O nome do aplicativo exibido no portal do Azure.|
|appId|String|O identificador de aplicativo no Azure Active Directory.|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto|Uma lista de políticas de acesso condicional disparadas pela atividade de entrada correspondente.|
|authenticationDetails|coleção [authenticationDetail](authenticationdetail.md)|O resultado da tentativa de autenticação e detalhes adicionais sobre o método de autenticação.|
|authenticationMethodsUsed|Conjunto de cadeias de caracteres|Os métodos de autenticação usados. Valores possíveis: `SMS` ,,,,, `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` ou `PHS` .|
|authenticationProcessingDetails|Coleção [KeyValue](keyvalue.md)|Detalhes de processamento de autenticação adicionais, como o nome do agente em caso de PTA/PHS ou nome do servidor/farm, no caso de autenticação federada.|
|authenticationRequirement | cadeia de caracteres | Isso mantém o nível mais alto de autenticação necessário por meio de todas as etapas de entrada para que a entrada tenha êxito.|
|clientAppUsed|Cadeia de caracteres|O cliente herdado usado para a atividade de entrada. Por exemplo, navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP ou POP.|
|conditionalAccessStatus|cadeia de caracteres| O status da política de acesso condicional disparado. Valores possíveis: `success` , `failure` , `notApplied` ou `unknownFutureValue` .|
|correlationId|Cadeia de caracteres|O identificador que é enviado do cliente quando o logon é iniciado. Isso é usado para solucionar problemas de atividade de entrada correspondente ao chamar o suporte.|
|createdDateTime|DateTimeOffset|A data e a hora em que o logon foi iniciado. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|As informações sobre o dispositivo de onde o logon ocorreu. Inclui informações como DeviceID, so e navegador. |
|id|String|O identificador que representa a atividade de entrada.|
|ipAddress|Cadeia de caracteres|O endereço IP do cliente de onde a conexão ocorreu.|
|isInteractive|Booliano|Indica se um logon é interativo ou não.|
|location|[signInLocation](signinlocation.md)|O código do país de cidade, estado e 2 letras de onde o logon ocorreu.|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Os detalhes do local de rede, como o endereço IP, o local da entrada, o tipo de rede usado e seus nomes. Valores possíveis: `Named Netowrk` , `Extranet` , `Intranet` ou `Trusted Network` .|
|originalRequestId|Cadeia de caracteres|O identificador de solicitação da primeira solicitação na sequência de autenticação.|
|processingTimeInMilliseconds|Int|O tempo de processamento da solicitação em milissegundos no AD STS.|
|resourceDisplayName|String|O nome do recurso no qual o usuário entrou.|
|resourceId|Cadeia de caracteres|O identificador do recurso para o qual o usuário entrou.|
|riskDetail|riskDetail|O motivo por trás de um estado específico de um usuário arriscado, entrar ou um evento de risco. Valores possíveis: `none` ,,,,, `adminGeneratedTemporaryPassword` ,, `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` , ou `unknownFutureValue` . O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskEventTypes|coleção riskEventType|A lista de tipos de eventos de risco associados à entrada. Valores possíveis: `unlikelyTravel` ,,,,, `anonymizedIPAddress` ,, `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` , ou `unknownFutureValue` .|
|riskEventTypes_v2|Conjunto de cadeias de caracteres|A lista de tipos de eventos de risco associados à entrada. Valores possíveis: `unlikelyTravel` ,,,,, `anonymizedIPAddress` ,, `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` , ou `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|O nível de risco agregado. Valores possíveis: `none` , `low` ,,, `medium` `high` `hidden` ou `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskLevelDuringSignIn|riskLevel|O nível de risco durante a entrada. Valores possíveis: `none` , `low` ,,, `medium` `high` `hidden` ou `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskState|riskState|O estado de risco de um usuário arriscado, logon ou um evento de risco. Valores possíveis: `none` ,,,,, `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` ou `unknownFutureValue` .|
|servicePrincipalName|String|O identificador de aplicativo usado para entrar. Este campo será preenchido quando você estiver fazendo logon usando um aplicativo.|
|servicePrincipalName|Cadeia de caracteres|O nome do aplicativo usado para entrar. Este campo será preenchido quando você estiver fazendo logon usando um aplicativo.|
|status|[signInStatus](signinstatus.md)|O status de entrada. Inclui o código de erro e a descrição do erro (em caso de falha de entrada).|
|tokenIssuerName|Cadeia de caracteres|O nome do provedor de identidade. Por exemplo, `sts.microsoft.com`.|
|tokenIssuerType|Cadeia de caracteres|O tipo de provedor de identidade. Valores possíveis: `AzureAD` , `ADFederationServices` , ou `UnknownFutureValue` .|
|userAgent|String|As informações do agente do usuário relacionadas à entrada.|
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


