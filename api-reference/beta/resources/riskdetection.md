---
title: Tipo de recurso riskDetection
description: Representa todas as detecções de risco em locatários do AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 40fa938f94f5f43a61c191a3d3c14b0dbbb10d6f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440133"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD [](riskyuser.md) avalia continuamente os [](signin.md) riscos do usuário e os riscos de entrada de aplicativo ou usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskDetection](../api/riskdetection-list.md) | [Coleção riskDetection](riskdetection.md)|Listar detecções de risco e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Obter uma detecção arriscada específica e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|ID exclusiva da detecção de risco. |
|`requestId`|`string`|ID da solicitação da login associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma login.|
|`correlationId`|`string`|ID de correlação do sign-in associado à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma login. |
|`riskEventType`|`string`|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel` são , , , , , , , `anonymizedIPAddress` , , , , `maliciousIPAddress` , , `unfamiliarFeatures` , , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |
|`riskType`|`riskEventType`|Lista de tipos de eventos de risco.<br/>**Observação:** Essa propriedade é preterida. Use **riskEventTypes** em vez disso. |
|`riskState`|`riskState`|O estado de um usuário ou de login de risco detectado. Os valores possíveis são none, confirmedSafe, remediado, ignorado, atRisk, confirmedCompromised e unknownFutureValue. |
|`riskLevel`|`riskLevel`|Nível do risco detectado. Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden` .|
|`riskDetail`|`riskDetail`|Detalhes do risco detectado. Os valores possíveis não são nenhum, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden` .|
|`source`|`string`|Origem da detecção de risco. Por exemplo, "activeDirectory". |
|`detectionTimingType`|`riskDetectionTimingType`|Tempo do risco detectado (em tempo real/offline). Os valores possíveis não sãoDefined, realtime, nearRealtime, offline, unknownFutureValue. |
|`activity`|`activityType`|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são signin, user, unknownFutureValue. |
|`tokenIssuerType`|`tokenIssuerType`|Indica o tipo de emissor de token para o risco de entrar detectado. Os valores possíveis são AzureAD, ADFederationServices e unknownFutureValue. |
|`ipAddress`|`string`|Fornece o endereço IP do cliente de onde o risco ocorreu. |
|`location`|[signInLocation](signinlocation.md)|Local da assinatura. |
|`activityDateTime`|`datetimeoffset`|Data e hora em que a atividade arriscada ocorreu. |
|`detectedDateTime`|`datetimeoffset`|Data e hora em que o risco foi detectado. |
|`lastUpdatedDateTime`|`datetime`|Data e hora em que a detecção de risco foi atualizada pela última vez. |
|`userId`|`string`|ID exclusivo do usuário. |
|`userDisplayName`|`string`|Nome do usuário. |
|`userPrincipalName`|`string`|O nome UPN do usuário. |
|`additionalInfo`|`string`|Informações adicionais associadas à detecção de risco no formato JSON. |

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
