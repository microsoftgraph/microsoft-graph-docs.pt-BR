---
title: tipo de recurso riskDetection
description: Representa todas as detecções de riscos em locatários do AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ac9606b0b1d2a5bd49ac25f25ce43996b9bb60a1
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400729"
---
# <a name="riskdetection-resource-type"></a>tipo de recurso riskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD avalia continuamente [os riscos do usuário](riskyuser.md) e os riscos de [entrada do](signin.md) aplicativo ou do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskDetection](../api/riskdetection-list.md) | coleção [riskDetection](riskdetection.md)|Listar detecções de risco e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Obtenha uma detecção arriscada específica e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|`id`|`string`|ID exclusiva da detecção de risco. |
|`requestId`|`string`|ID de solicitação da entrada associada à detecção de risco. Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada.|
|`correlationId`|`string`|ID de correlação da entrada associada à detecção de risco. Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada. |
|`riskEventType`|`string`|O tipo de evento de risco detectado. Os valores possíveis são:,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` e `unknownFutureValue` . |
|`riskType`|`riskEventType`|Lista de tipos de eventos de risco.<br/>**Observação:** Essa propriedade foi preterida. Use **riskEventTypes** em vez disso. |
|`riskState`|`riskState`|O estado de um usuário ou logon arriscado detectado. Os valores possíveis são nenhum, confirmedSafe, corrigido, descartado, atRisk, confirmedCompromised e unknownFutureValue. |
|`riskLevel`|`riskLevel`|Nível do risco detectado. Os valores possíveis são baixo, médio, alto, oculto, nenhum, unknownFutureValue. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Os clientes P1 serão retornados `hidden` .|
|`riskDetail`|`riskDetail`|Detalhes do risco detectado. Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue. **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Os clientes P1 serão retornados `hidden` .|
|`source`|`string`|Fonte da detecção de risco. Por exemplo, "activeDirectory". |
|`detectionTimingType`|`riskDetectionTimingType`|Intervalo do risco detectado (em tempo real/offline). Os valores possíveis são não definidos, em tempo real, nearRealtime, offline, unknownFutureValue. |
|`activity`|`activityType`|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são entrar, User, unknownFutureValue. |
|`tokenIssuerType`|`tokenIssuerType`|Indica o tipo de emissor de token para o risco de entrada detectado. Os valores possíveis são AzureAD, ADFederationServices e unknownFutureValue. |
|`ipAddress`|`string`|Fornece o endereço IP do cliente de onde o risco ocorreu. |
|`location`|[signInLocation](signinlocation.md)|Local de entrada. |
|`activityDateTime`|`datetimeoffset`|Data e hora em que a atividade arriscada ocorreu. |
|`detectedDateTime`|`datetimeoffset`|Data e hora em que o risco foi detectado. |
|`lastUpdatedDateTime`|`datetime`|Data e hora da última atualização do risco. |
|`userId`|`string`|ID exclusivo do usuário. |
|`userDisplayName`|`string`|Nome do usuário. |
|`userPrincipalName`|`string`|O nome UPN do usuário. |
|`additionalInfo`|`string`|Informações adicionais associadas à detecção de riscos no formato JSON. |

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