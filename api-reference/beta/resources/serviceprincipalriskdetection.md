---
title: Tipo de recurso servicePrincipalRiskDetection
description: Representa informações sobre uma entidade de serviço em risco detectada em um locatário do Azure AD.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 63eb90a7147394eb6639083f7f965e8759262901
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519921"
---
# <a name="serviceprincipalriskdetection-resource-type"></a>Tipo de recurso servicePrincipalRiskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre entidades de serviço de risco detectadas em um locatário do Azure AD. O Azure AD avalia continuamente os riscos com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco principal do serviço em seu ambiente do Azure AD.

Herda da [entidade](../resources/entity.md).

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection). 

>**Observação:** Você deve ter uma Azure AD Premium P1 ou P2 para usar a API servicePrincipalRiskDetection.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar servicePrincipalRiskDetections](../api/identityprotectionroot-list-serviceprincipalriskdetections.md)|[Coleção servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md)|Listar as detecções de risco principal do serviço e suas propriedades.|
|[Obter servicePrincipalRiskDetection](../api/serviceprincipalriskdetection-get.md)|[servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md)|Obter uma detecção de risco de entidade de serviço específica e suas propriedades.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado.  Os valores possíveis são: `signin`, `unknownFutureValue`, `servicePrincipal`. Observe que você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter os seguintes valores neste [número evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipal`. |
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|additionalInfo|Cadeia de caracteres|Informações adicionais associadas à detecção de risco. Esse valor de cadeia de caracteres é representado como um objeto JSON com as aspas escapam. |
|appId|Cadeia de caracteres|O identificador exclusivo do aplicativo associado.|
|correlationId|Cadeia de caracteres|ID de correlação da atividade de login associada à detecção de risco. Essa propriedade é `null` se a detecção de risco não estiver associada a uma atividade de login.|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado , seja em tempo real ou offline). Os valores possíveis são: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|Cadeia de caracteres|Identificador exclusivo da detecção de risco. Herdado da [entidade](../resources/entity.md).|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde o risco ocorreu.|
|keyIds|String collection|O identificador exclusivo (GUID) da credencial de chave associada à detecção de risco.|
|lastUpdatedDateTime|DateTimeOffset|Data e hora em que a detecção de risco foi atualizada pela última vez.|
|location|[signInLocation](signinlocation.md)|Local de onde a assinatura foi iniciada. |
|requestId|Cadeia de caracteres|Identificador de solicitação da atividade de login associada à detecção de risco. Essa propriedade é `null` se a detecção de risco não estiver associada a uma atividade de login. Suporta `$filter` (`eq`).|
|riskDetail|riskDetail|Detalhes do risco detectado. <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`. <br/>Os valores possíveis são: `none`, `hidden`, `unknownFutureValue`, `adminConfirmedServicePrincipalCompromised`, `adminDismissedAllRiskForServicePrincipal`. Observe que você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter os seguintes valores nesta [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `adminConfirmedServicePrincipalCompromised` , `adminDismissedAllRiskForServicePrincipal`.|
|riskEventType|String|O tipo de evento de risco detectado. Os valores possíveis são: `investigationsThreatIntelligence`, `generic`, `adminConfirmedServicePrincipalCompromised`, , `suspiciousSignins`, `leakedCredentials`. `unknownFutureValue` Suporta `$filter` (`eq`).|
|riskLevel|riskLevel|Nível do risco detectado. <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`. Os valores possíveis são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|O estado de uma principal de serviço ou atividade de login de risco detectada. Os valores possíveis são: `none`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalDisplayName|String|    O nome de exibição da entidade de serviço.|
|servicePrincipalId|Cadeia de caracteres|O identificador exclusivo da entidade de serviço. Suporta `$filter` (`eq`).|
|source|String|Origem da detecção de risco. Por exemplo, `identityProtection`.|
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor de token para o risco de entrar detectado. Os valores possíveis são: `AzureAD`, `UnknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipalRiskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
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
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String",
  "keyIds": [
    "String"
  ],
  "additionalInfo": "String"
}
```

