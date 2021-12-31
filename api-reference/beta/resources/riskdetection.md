---
title: Tipo de recurso riskDetection
description: Representa todas as detecções de risco em locatários do AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d0acaeb29f80e38cb9a1ce88d2e15878a294a65
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647109"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD [](riskyuser.md) avalia continuamente os [](signin.md) riscos do usuário e os riscos de entrada de aplicativo ou usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Você deve ter uma Azure AD Premium P1 ou P2 para usar a API de detecção de risco.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskDetection](../api/riskdetection-list.md) | [Coleção riskDetection](riskdetection.md)|Listar detecções de risco e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Obter uma detecção arriscada específica e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|id|string|ID exclusiva da detecção de risco. |
|requestId|string|ID da solicitação da login associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma login.|
|correlationId|string|ID de correlação do sign-in associado à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma login. |
|riskEventType|string|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel` são , , , , , , , , `anonymizedIPAddress` , , , `maliciousIPAddress` , , `unfamiliarFeatures` , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |
|riskState|riskState|O estado de um usuário ou de login de risco detectado. Os valores possíveis `none` são , , , , , e `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` . |
|riskLevel|riskLevel|Nível do risco detectado. Os valores possíveis `low` são , , , , , `medium` `high` `hidden` `none` `unknownFutureValue` . <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden` .|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis `none` são , , , , , , , `adminGeneratedTemporaryPassword` , , , `userPerformedSecuredPasswordChange` , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` . <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden` .|
|source|string|Origem da detecção de risco. Por exemplo, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado (em tempo real/offline). Os valores possíveis `notDefined` são , , , , `realtime` `nearRealtime` `offline` `unknownFutureValue` . |
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são `signin` `user` , , `unknownFutureValue` . |
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor de token para o risco de entrar detectado. Os valores possíveis são `AzureAD`, `ADFederationServices` e `unknownFutureValue`. |
|ipAddress|string|Fornece o endereço IP do cliente de onde o risco ocorreu. |
|location|[signInLocation](signinlocation.md)|Local da assinatura. |
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z` |
|lastUpdatedDateTime|DateTimeOffset|Data e hora em que a detecção de risco foi atualizada pela última vez. |
|userId|cadeia de caracteres|ID exclusivo do usuário.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|userDisplayName|string|Nome do usuário. |
|userPrincipalName|string|O nome UPN do usuário. |
|additionalInfo|string|Informações adicionais associadas à detecção de risco no formato JSON. |
|riskType (preterido)|riskEventType|Lista de tipos de eventos de risco.<br />**Observação:** Essa propriedade é preterida. Use **riskEventType** em vez disso. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
