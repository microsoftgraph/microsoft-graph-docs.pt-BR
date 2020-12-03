---
title: tipo de recurso de domínio
description: Detalha a atividade de entrada do usuário e do aplicativo para um locatário (diretório).
author: besiler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b86ae228a888ce32ca79053f46ff4e7a04505bcc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563657"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

Detalha a atividade de entrada do usuário e do aplicativo para um locatário (diretório).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de um objeto de domínio.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|String|Nome do aplicativo exibido no portal do Azure.|
|appId|String|GUID exclusivo que representa a ID do aplicativo no Azure Active Directory.|
|appliedConditionalAccessPolicy|coleção [appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Fornece uma lista de políticas de acesso condicional acionada por atividade correspondente entrar.|
|clientAppUsed|Cadeia de caracteres|Identifica o cliente herdado usado para a atividade de entrada.  Inclui navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP e POP.|
|conditionalAccessStatus|cadeia de caracteres| Relata o status de uma política de acesso condicional ativada. Os valores possíveis são: `success` , `failure` , `notApplied` , e `unknownFutureValue` .|
|correlationId|Cadeia de caracteres|A ID de solicitação enviada do cliente quando o logon é iniciado; usado para solucionar problemas de atividade de entrada.|
|createdDateTime|DateTimeOffset|Data e hora (UTC) a entrada foi iniciada. Exemplo: meia-noite em 1º de janeiro de 2014 é reportada como `'2014-01-01T00:00:00Z'` .|
|deviceDetail|[deviceDetail](devicedetail.md)|Informações do dispositivo de onde a entrada ocorreu; inclui ID de dispositivo, sistema operacional e navegador. |
|id|String|ID exclusiva que representa a atividade de entrada.|
|ipAddress|Cadeia de caracteres|Endereço IP do cliente usado para entrar.|
|isInteractive|Booliano|Indica se um logon é interativo ou não.|
|location|[signInLocation](signinlocation.md)|Fornece a cidade, o estado e o código do país onde a entrada se originou.|
|resourceDisplayName|String|Nome do recurso do usuário conectado.|
|resourceId|Cadeia de caracteres|ID do recurso que o usuário entrou.|
|riskDetail|riskDetail|Fornece o motivo por trás de um estado específico de um usuário arriscado, uma entrada arriscada ou um evento de risco. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. <br>**Observação:** Os detalhes dessa propriedade exigem uma licença do Azure AD Premium P2. Outras licenças retornam o valor `hidden` .|
|riskEventTypes|coleção riskEventType|Tipos de eventos de risco associados à entrada. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` e `unknownFutureValue`.|
|riskEventTypes_v2|Conjunto de cadeias de caracteres|A lista de tipos de eventos de risco associados à entrada. Valores possíveis: `unlikelyTravel` ,,,,, `anonymizedIPAddress` ,, `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` , ou `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Nível de risco agregado. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|Nível de risco durante a entrada. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Outros clientes serão retornados `hidden`.|
|riskState|riskState|Relata o status do usuário arriscado, de entrada ou de um evento de risco. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Status de logon. Inclui o código de erro e a descrição do erro (em caso de falha de entrada).|
|userDisplayName|Cadeia de caracteres|Nome para exibição do usuário que iniciou a entrada.|
|userId|Cadeia de caracteres|ID do usuário que iniciou a entrada.|
|userPrincipalName|String|Nome principal do usuário que iniciou a entrada.|

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

