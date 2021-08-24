---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório.
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: 03beb5f18106469f9e20c602aecb771142d6a7bc
ms.sourcegitcommit: c6f7a931a8d83ac54f577b7bec08237fd17ce51a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2021
ms.locfileid: "58490123"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório. Você deve ter uma Azure AD Premium P1 ou P2 para baixar logs de login usando a API Graph Microsoft.

A disponibilidade de logs de login é governada pelas políticas de retenção de dados do [Azure AD.](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Ler propriedades e relações de um objeto signIn.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|alternateSignInName|Cadeia de caracteres|A identidade de login alternativa sempre que você usa o número de telefone para entrar. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|appDisplayName|Cadeia de caracteres|O nome do aplicativo exibido no Portal do Azure. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|appId|Cadeia de caracteres|O identificador do aplicativo no Azure Active Directory. Suporta `$filter` ( `eq` somente operador).|
|appliedConditionalAccessPolicies|[coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Uma lista de políticas de acesso condicional que são disparadas pela atividade de entrada correspondente.|
|authenticationDetails|[Coleção authenticationDetail](authenticationdetail.md)|O resultado da tentativa de autenticação e detalhes adicionais sobre o método de autenticação.|
|authenticationMethodsUsed|String collection|Os métodos de autenticação usados. Valores possíveis: `SMS` , , , , , , ou `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Coleção [KeyValue](keyvalue.md)|Detalhes adicionais de processamento de autenticação, como o nome do agente em caso de PTA/PHS ou nome de servidor/farm em caso de autenticação federada.|
|authenticationRequirement | String | Isso mantém o nível mais alto de autenticação necessário por meio de todas as etapas de login, para que a assinatura seja bem-sucedida. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|clientAppUsed|Cadeia de caracteres|O cliente herddo usado para atividades de entrada. Por exemplo: `Browser` , , , , , , ou `Exchange Active Sync` `Modern clients` `IMAP` `MAPI` `SMTP` `POP` . Suporta `$filter` ( `eq` somente operador). |
|conditionalAccessStatus|conditionalAccessStatus| O status da política de acesso condicional disparada. Valores possíveis: `success` `failure` , , ou `notApplied` `unknownFutureValue` . Suporta `$filter` ( `eq` somente operador).|
|correlationId|Cadeia de caracteres|O identificador enviado do cliente quando a entrada é iniciada. Isso é usado para solucionar problemas da atividade de login correspondente ao chamar o suporte. Suporta `$filter` ( `eq` somente operador).|
|createdDateTime|DateTimeOffset|A data e a hora em que a assinatura foi iniciada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece `$orderby` suporte e ( , e somente `$filter` `eq` `le` `ge` operadores).|
|deviceDetail|[deviceDetail](devicedetail.md)|As informações do dispositivo de onde ocorreu a entrada. Inclui informações como deviceId, so e navegador. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores) nas **propriedades browser** **e operatingSytem.**|
|id|Cadeia de caracteres|O identificador que representa a atividade de login. Suporta `$filter` ( `eq` somente operador).|
|ipAddress|Cadeia de caracteres|O endereço IP do cliente de onde ocorreu a entrada. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|isInteractive|Booliano|Indica se uma assinatura é interativa ou não.|
|location|[signInLocation](signinlocation.md)|A cidade, o estado e o código de país de duas letras de onde ocorreu a login. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores) em **propriedades city**, **state** e **countryOrRegion.**|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Os detalhes do local da rede, incluindo o tipo de rede usada e seus nomes.|
|originalRequestId|Cadeia de caracteres|O identificador de solicitação da primeira solicitação na sequência de autenticação. Suporta `$filter` ( `eq` somente operador).|
|processingTimeInMilliseconds|Int|O tempo de processamento da solicitação em milissegundos no AD STS.|
|resourceDisplayName|Cadeia de caracteres|O nome do recurso ao que o usuário se inscreveu. Suporta `$filter` ( `eq` somente operador).|
|resourceId|Cadeia de caracteres|O identificador do recurso ao que o usuário se inscreveu. Suporta `$filter` ( `eq` somente operador).|
|riskDetail|riskDetail|O motivo por trás de um estado específico de um usuário arriscado, de entrar ou de um evento de risco. Valores possíveis: `none` , , , , , , , , , `adminGeneratedTemporaryPassword` ou `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. Suporta `$filter` ( `eq` somente operador).<br> **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskEventTypes|Coleção riskEventType|A lista de tipos de eventos de risco associados à assinatura. Valores possíveis: `unlikelyTravel` , , , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Suporta `$filter` ( `eq` somente operador).|
|riskEventTypes_v2|String collection|A lista de tipos de eventos de risco associados à assinatura. Valores possíveis: `unlikelyTravel` , , , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|riskLevelAggregated|riskLevel|O nível de risco agregado. Valores possíveis: `none` , , , , ou `low` `medium` `high` `hidden` `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Suporta `$filter` ( `eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskLevelDuringSignIn|riskLevel|O nível de risco durante a assinatura. Valores possíveis: `none` , , , , ou `low` `medium` `high` `hidden` `unknownFutureValue` . O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Suporta `$filter` ( `eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden` .|
|riskState|riskState|O estado de risco de um usuário arriscado, de entrar ou de um evento de risco. Valores possíveis: `none` , , , , , , ou `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` . Suporta `$filter` ( `eq` somente operador).|
|servicePrincipalId|Cadeia de caracteres|O identificador de aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|servicePrincipalName|Cadeia de caracteres|O nome do aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|status|[signInStatus](signinstatus.md)|O status de login. Inclui o código de erro e a descrição do erro (no caso de uma falha de login). Suporta `$filter` ( `eq` somente operador) na propriedade **errorCode.**|
|tokenIssuerName|Cadeia de caracteres|O nome do provedor de identidade. Por exemplo, `sts.microsoft.com`. Suporta `$filter` ( `eq` somente operador).|
|tokenIssuerType|tokenIssuerType|O tipo de provedor de identidade. Valores possíveis: `AzureAD` `ADFederationServices` , ou `UnknownFutureValue` .|
|userAgent|Cadeia de caracteres|As informações do agente do usuário relacionadas à login. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|
|userId|Cadeia de caracteres|O identificador do usuário. Suporta `$filter` ( `eq` somente operador).|
|userPrincipalName|String|O UPN do usuário. Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).|

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


