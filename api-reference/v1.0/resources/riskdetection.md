---
title: Tipo de recurso riskDetection
description: detecções de risco
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 855d8b34da6c8cc24bd01f448164dc0b0b68b521d40c78bc6a3b06b95235423c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154879"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD [](riskyuser.md) avalia continuamente os [](signin.md) riscos do usuário e os riscos de entrada de aplicativo ou usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Você deve ter uma Azure AD Premium P1 ou P2 para usar a API de detecção de risco.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskDetections](../api/riskdetection-list.md)|[Coleção riskDetection](../resources/riskdetection.md)|Obter uma lista dos [objetos riskDetection](../resources/riskdetection.md) e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Leia as propriedades e as relações de um [objeto riskDetection.](../resources/riskdetection.md)|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. . Os valores possíveis são: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é assim: `2014-01-01T00:00:00Z`|
|additionalInfo|Cadeia de caracteres|Informações adicionais associadas à detecção de risco no formato JSON.|
|correlationId|Cadeia de caracteres|ID de correlação do sign-in associado à detecção de risco. Essa propriedade é `null` se a detecção de risco não estiver associada a uma login.|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é assim: `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado (em tempo real/offline). Os valores possíveis são: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|Cadeia de caracteres|ID exclusiva da detecção de risco. Herdado da [entidade](../resources/entity.md)|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde o risco ocorreu.|
|lastUpdatedDateTime|DateTimeOffset|Data e hora em que a detecção de risco foi atualizada pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é assim: `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|Local da assinatura.|
|requestId|Cadeia de caracteres|ID da solicitação da login associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma login.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|String|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel` são , , , , , , , , `anonymizedIPAddress` , , , `maliciousIPAddress` , , `unfamiliarFeatures` , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . Se a detecção de risco for uma detecção premium, mostrará `generic`|
|riskLevel|riskLevel|Nível do risco detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|O estado de um usuário ou de login de risco detectado. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|Cadeia de caracteres|Origem da detecção de risco. Por exemplo, `activeDirectory`. |
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor de token para o risco de entrar detectado. Os valores possíveis são: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|Cadeia de caracteres|O nome UPN do usuário. |
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
