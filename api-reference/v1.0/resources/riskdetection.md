---
title: tipo de recurso riskDetection
description: detecções de risco
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e6766d300ab3fd179ce5a684740cfcd25f672cc8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991877"
---
# <a name="riskdetection-resource-type"></a>tipo de recurso riskDetection

Namespace: Microsoft. Graph representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD avalia continuamente [os riscos do usuário](riskyuser.md) e os riscos de [entrada do](signin.md) aplicativo ou do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).

>[!NOTE]
>Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskDetections](../api/riskdetection-list.md)|coleção [riskDetection](../resources/riskdetection.md)|Obtenha uma lista dos objetos [riskDetection](../resources/riskdetection.md) e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Leia as propriedades e os relacionamentos de um objeto [riskDetection](../resources/riskdetection.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. . Os valores possíveis são: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu.|
|additionalInfo|String|Informações adicionais associadas à detecção de riscos no formato JSON.|
|correlationId|Cadeia de caracteres|ID de correlação da entrada associada à detecção de risco. Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada.|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado.|
|detectionTimingType|riskDetectionTimingType|Intervalo do risco detectado (em tempo real/offline). Os valores possíveis são: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|ID exclusiva da detecção de risco. Herdado da [entidade](../resources/entity.md)|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde o risco ocorreu.|
|lastUpdatedDateTime|DateTimeOffset|Data e hora da última atualização do risco.|
|location|[signInLocation](../resources/signinlocation.md)|Local de entrada.|
|Identificação|String|ID de solicitação da entrada associada à detecção de risco. Essa propriedade será NULL se a detecção de risco não estiver associada a uma entrada.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|String|O tipo de evento de risco detectado. Os valores possíveis são:,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` e `unknownFutureValue` . Se a detecção de risco for Premium, mostrará `generic`|
|riskLevel|riskLevel|Nível do risco detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|O estado de um usuário ou logon arriscado detectado. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Fonte da detecção de risco. Por exemplo, "activeDirectory". |
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor de token para o risco de entrada detectado. Os valores possíveis são: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|O nome UPN do usuário. |
|userId|Cadeia de caracteres|ID exclusivo do usuário.|
|userPrincipalName|String|O nome UPN do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```


