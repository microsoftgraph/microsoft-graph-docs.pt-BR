---
title: tipo de recurso de domínio
description: Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório).
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d19cb940729ec0d8140f229473e11f9295e655a1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343484"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

Detalha a atividade de login do usuário e do aplicativo para um locatário (diretório). Você deve ter uma Azure AD Premium P1 ou P2 para baixar logs de login usando a API Graph Microsoft. 

A disponibilidade de logs de login é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de um objeto de domínio.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|Cadeia de caracteres|Nome do aplicativo exibido no Portal do Azure. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|appId|String|GUID exclusivo que representa a ID do aplicativo no Azure Active Directory. Suporta `$filter` (`eq` somente operador).|
|appliedConditionalAccessPolicy|[coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Fornece uma lista de políticas de acesso condicional acionada por atividade correspondente entrar.|
|clientAppUsed|Cadeia de caracteres|Identifica o cliente usado para a atividade de entrada. Os clientes de autenticação moderna incluem `Browser` e `modern clients`. Os clientes de autenticação herdou incluem `Exchange ActiveSync`, `IMAP`, `MAPI`, `SMTP`, `POP`e `other clients`. Suporta `$filter` (`eq` somente operador).|
|conditionalAccessStatus|conditionalAccessStatus| Relata o status de uma política de acesso condicional ativada. Os valores possíveis são: `success`, `failure`, `notApplied`, e `unknownFutureValue`. Suporta `$filter` (`eq` somente operador).|
|correlationId|Cadeia de caracteres|A ID de solicitação enviada do cliente quando a entrada é iniciada; usado para solucionar problemas de atividade de login. Suporta `$filter` (`eq` somente operador).|
|createdDateTime|DateTimeOffset|Data e hora (UTC) a assinatura foi iniciada. Exemplo: meia-noite de 1º de janeiro de 2014 é relatada como `2014-01-01T00:00:00Z`. Suporta `$orderby` e `$filter` (`eq`, `le`e somente `ge` operadores).|
|deviceDetail|[deviceDetail](devicedetail.md)|Informações do dispositivo de onde ocorreu a entrada; inclui iD do dispositivo, sistema operacional e navegador. Oferece `$filter` suporte (`eq` e `startsWith` somente operadores) nas **propriedades browser** **e operatingSytem** . |
|id|Cadeia de caracteres|ID exclusiva que representa a atividade de login. Suporta `$filter` (`eq` somente operador).|
|ipAddress|Cadeia de caracteres|Endereço IP do cliente usado para entrar. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|isInteractive|Booliano|Indica se uma assinatura é interativa ou não.|
|location|[signInLocation](signinlocation.md)|Fornece o código de cidade, estado e país de origem do login. Oferece `$filter` suporte (`eq` e `startsWith` somente operadores) em **propriedades city**, **state** e **countryOrRegion** .|
|resourceDisplayName|String|Nome do recurso em que o usuário entrou. Suporta `$filter` (`eq` somente operador).|
|resourceId|Cadeia de caracteres|ID do recurso em que o usuário entrou. Suporta `$filter` (`eq` somente operador).|
|riskDetail|riskDetail|Fornece o motivo por trás de um estado específico de um usuário arriscado, uma entrada arriscada ou um evento de risco. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento.  Suporta `$filter` (`eq` somente operador).<br>**Observação:** Os detalhes dessa propriedade exigem uma Azure AD Premium P2 de uso. Outras licenças retornam o valor `hidden`.|
|riskEventTypes|Coleção riskEventType|Tipos de evento de risco associados à assinatura. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` e `unknownFutureValue`. Suporta `$filter` (`eq` somente operador).|
|riskEventTypes_v2|String collection|A lista de tipos de eventos de risco associados à assinatura. Valores possíveis: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, ,  `generic`ou `unknownFutureValue`. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|riskLevelAggregated|riskLevel|Nível de risco agregado. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Suporta `$filter` (`eq` somente operador). <br> **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|Nível de risco durante a assinatura. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD.  Suporta `$filter` (`eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskState|riskState|Relata o status do usuário de risco, de entrar ou de um evento de risco. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. Suporta `$filter` (`eq` somente operador).|
|status|[signInStatus](signinstatus.md)|Status de login. Inclui o código de erro e a descrição do erro (no caso de uma falha de login). Suporta `$filter` (`eq` somente operador) na **propriedade errorCode** .|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário que iniciou a login. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|userId|Cadeia de caracteres|ID do usuário que iniciou a login. Suporta `$filter` (`eq` somente operador).|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário que iniciou a login. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|

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
  "isInteractive": true,
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

