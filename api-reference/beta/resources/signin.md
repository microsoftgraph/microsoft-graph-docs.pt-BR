---
title: tipo de recurso de logon
description: 'Este recurso fornece detalhes sobre o usuário ou aplicativo entrar atividade em seu diretório. '
ms.openlocfilehash: 2bc6c8b961f0626a6409d9be868235f285f48e52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040004"
---
# <a name="signin-resource-type"></a>tipo de recurso de logon
Este recurso fornece detalhes sobre o usuário ou aplicativo entrar atividade em seu diretório. 

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Entrando de lista](../api/signin-list.md) | [Entrando](signin.md) |Leia as propriedades e os relacionamentos de objetos de logon.|
|[Fazer logon](../api/signin-get.md) | [Entrando](signin.md) |Leia as propriedades e relações de objeto de entrar.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|String|Refere-se ao nome do aplicativo exibido no Portal do Windows Azure.|
|appId|Cadeia de caracteres|Refere-se o GUID exclusivo que representa a Id do aplicativo no Windows Azure Active Directory.|
|authenticationProcessingDetails|`authenticationProcessingDetails`|Fornece detalhes associados ao processador de autenticação.|
|clientAppUsed|String|Fornece o cliente herdado usado para entrar activty.E.g. inclui um navegador, Exchange Active Sync, clientes modernos, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicy|coleção [conditionalAccessPolicy](conditionalaccesspolicy.md)|Fornece uma lista de políticas de acesso condicional que são acionadas pela atividade de entrada correspondente.|
|conditionalAccessStatus|string| Fornece o status da política de acesso condicional disparado. Os valores possíveis são: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|originalRequestId|String|O id de solicitação da primeira solicitação na sequência de autenticação.|
|isInteractive|Booliano|Indica se um logon é interativo ou não.|
|tokenIssuerName|String|Nome da identidade do provedor (por exemplo, sts.microsoft.com)|
|tokenIssuerType|String|Fornece o tipo de identityProvider. Os valores possíveis são `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|Cadeia de caracteres|Refere-se a ID que é enviada pelo cliente quando o sign-in é iniciado. Isso é usado para solução de problemas da atividade de entrada correspondente ao chamar suporte ou da assistência técnica.|
|createdDateTime|DateTimeOffset|Fornece a data e hora que o sign-in tenha sido iniciado. O tipo de carimbo de hora é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|Fornece as informações do dispositivo de onde a entrar ocorreu. Ele inclules informações como deviceId, sistema operacional, navegador. |
|id|String|Indica a identificação exclusiva que representa a atividade de entrada.|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde a entrar ocorreu.|
|location|[signInLocation](signinlocation.md)|Fornece a cidade, estado e código do país 2 de carta do qual a entrar ocorreu.|
|processingTimeInMilliseconds|Int|Fornece o tempo em milissegundos no AD STS de processamento de solicitação|
|riskDetail|`riskDetail`|Fornece o motivo por trás de um estado específico de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada no usuário ou entrar até o momento.|
|riskLevelAggregated|`riskLevel`|Fornece o nível de risco agregados. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.|
|riskLevelDuringSignIn|`riskLevel`|Fornece o nível de risco durante a entrada. Os valores possíveis são: `none`, `low`, `medium`, `high`, `hidden`, e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.|
|riskEventTypes|`riskEventTypes`|Fornece a lista de tipos de evento de risco associados a entrar. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecurePasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`e `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrar não foi habilitada para a proteção de identidade do Windows Azure AD.|
|riskState|`riskState`|Fornece o 'estado de risco' de um usuário riscado, entrar ou um evento de risco. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Fornece o MFA relacionado informações como MFA, MFA Status Requerido para a entrada correspondente.|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|Fornece detalhes sobre o local de rede.|
|riskLevel|string| Fornece o nível de risco associado a entrar. Os valores possíveis são: `low`, `medium`, `high`.|
|status|[signInStatus](signinstatus.md)|Fornece o status de entrada. Os valores possíveis incluem `Success` e `Failure`.|
|userDisplayName|String|Indica a exibição do nome do usuário.|
|userId|String|Indica o ID de usuário do usuário.|
|userPrincipalName|String|Indica o UPN do usuário.|
|resourceDisplayName|String|Indica o nome do recurso que o usuário entrado na|
|resourceId|Cadeia de caracteres|Indica a identificação do recurso que o usuário entrado na.|
|authenticationMethodsUsed|String|Indica a lista de métodos de autenticação usado|

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
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskLevel": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
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