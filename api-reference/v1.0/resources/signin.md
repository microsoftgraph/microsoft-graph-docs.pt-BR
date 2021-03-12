---
title: tipo de recurso de domínio
description: Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório).
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d4ce200ba33cbc3896c967d85c6b83ce21a2bc63
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721744"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório). Você deve ter uma licença do Azure AD Premium P1 ou P2 para baixar logs de login usando a API do Microsoft Graph.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de um objeto de domínio.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|Cadeia de caracteres|Nome do aplicativo exibido no Portal do Azure.|
|appId|Cadeia de caracteres|GUID exclusivo que representa a ID do aplicativo no Azure Active Directory.|
|appliedConditionalAccessPolicy|[coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Fornece uma lista de políticas de acesso condicional acionada por atividade correspondente entrar.|
|clientAppUsed|Cadeia de caracteres|Identifica o cliente herddo usado para a atividade de entrada.  Inclui Navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP e POP.|
|conditionalAccessStatus|cadeia de caracteres| Relata o status de uma política de acesso condicional ativada. Os valores possíveis são: `success` `failure` , , e `notApplied` `unknownFutureValue` .|
|correlationId|Cadeia de caracteres|A ID de solicitação enviada do cliente quando a entrada é iniciada; usado para solucionar problemas de atividade de login.|
|createdDateTime|DateTimeOffset|Data e hora (UTC) a assinatura foi iniciada. Exemplo: meia-noite de 1º de janeiro de 2014 é relatada como `2014-01-01T00:00:00Z` .|
|deviceDetail|[deviceDetail](devicedetail.md)|Informações do dispositivo de onde ocorreu a entrada; inclui iD do dispositivo, sistema operacional e navegador. |
|id|Cadeia de caracteres|ID exclusiva que representa a atividade de login.|
|ipAddress|Cadeia de caracteres|Endereço IP do cliente usado para entrar.|
|isInteractive|Booliano|Indica se uma assinatura é interativa ou não.|
|location|[signInLocation](signinlocation.md)|Fornece o código de cidade, estado e país de origem do login.|
|resourceDisplayName|Cadeia de caracteres|Nome do recurso em que o usuário entrou.|
|resourceId|Cadeia de caracteres|ID do recurso em que o usuário entrou.|
|riskDetail|riskDetail|Fornece o motivo por trás de um estado específico de um usuário arriscado, uma entrada arriscada ou um evento de risco. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. <br>**Observação:** Os detalhes dessa propriedade exigem uma licença do Azure AD Premium P2. Outras licenças retornam o valor `hidden` .|
|riskEventTypes|Coleção riskEventType|Tipos de evento de risco associados à assinatura. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` e `unknownFutureValue`.|
|riskEventTypes_v2|Coleção de cadeias de caracteres|A lista de tipos de eventos de risco associados à assinatura. Valores possíveis: `unlikelyTravel` , , , , , , , , , `anonymizedIPAddress` ou `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Nível de risco agregado. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|Nível de risco durante a assinatura. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskState|riskState|Relata o status do usuário de risco, de entrar ou de um evento de risco. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Status de login. Inclui o código de erro e a descrição do erro (no caso de uma falha de login).|
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

