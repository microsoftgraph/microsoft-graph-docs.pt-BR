---
title: tipo de recurso de domínio
description: Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório).
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0c450ad78ca91ed49300f94f5bf96b2e2a6fbfe6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137148"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório). Você deve ter uma licença P1 ou P2 do Azure AD Premium para baixar logs de login usando a API do Microsoft Graph.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de um objeto de domínio.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|String|Nome do aplicativo exibido no Portal do Azure.|
|appId|String|GUID exclusivo que representa a ID do aplicativo no Azure Active Directory.|
|appliedConditionalAccessPolicy|[Coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Fornece uma lista de políticas de acesso condicional acionada por atividade correspondente entrar.|
|clientAppUsed|Cadeia de caracteres|Identifica o cliente herddo usado para atividade de entrada.  Inclui Navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP e POP.|
|conditionalAccessStatus|cadeia de caracteres| Relata o status de uma política de acesso condicional ativada. Os valores possíveis `success` são: `failure` , e `notApplied` `unknownFutureValue` .|
|correlationId|Cadeia de caracteres|A ID de solicitação enviada do cliente quando a entrada é iniciada; usado para solucionar problemas de atividade de login.|
|createdDateTime|DateTimeOffset|Data e hora (UTC) em que a login foi iniciada. Exemplo: meia-noite em 1º de janeiro de 2014 é relatado como `'2014-01-01T00:00:00Z'` .|
|deviceDetail|[deviceDetail](devicedetail.md)|Informações do dispositivo de onde ocorreu a entrada; inclui a ID do dispositivo, o sistema operacional e o navegador. |
|id|String|ID exclusiva que representa a atividade de login.|
|ipAddress|Cadeia de caracteres|Endereço IP do cliente usado para entrar.|
|isInteractive|Booliano|Indica se uma assinatura é interativa ou não.|
|location|[signInLocation](signinlocation.md)|Fornece a cidade, o estado e o código do país de origem do login.|
|resourceDisplayName|String|Nome do recurso em que o usuário entrou.|
|resourceId|Cadeia de caracteres|ID do recurso em que o usuário entrou.|
|riskDetail|riskDetail|Fornece o motivo por trás de um estado específico de um usuário arriscado, uma entrada arriscada ou um evento de risco. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. <br>**Observação:** Os detalhes dessa propriedade exigem uma licença do Azure AD Premium P2. Outras licenças retornam o `hidden` valor.|
|riskEventTypes|Coleção riskEventType|Tipos de evento de risco associados à login. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` e `unknownFutureValue`.|
|riskEventTypes_v2|String collection|A lista de tipos de eventos de risco associados à login. Valores possíveis: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Nível de risco agregado. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|Nível de risco durante a login. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskState|riskState|Relata o status do usuário arriscado, de entrar ou de um evento de risco. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Status de login. Inclui o código de erro e a descrição do erro (em caso de falha de login).|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário que iniciou a login.|
|userId|Cadeia de caracteres|ID do usuário que iniciou a login.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário que iniciou a login.|

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
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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

