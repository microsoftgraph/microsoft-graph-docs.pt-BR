---
title: Tipo de recurso riskDetection
description: Representa todas as detecções de risco em locatários do AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 231141c3ff679af50b5f42652c64b3da18edc005
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335210"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD avalia continuamente [](riskyuser.md) os riscos do usuário e os riscos [](signin.md) de entrada de aplicativo ou usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

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
|riskEventType|string|O tipo de evento de risco detectado. Os valores possíveis são , , , , , , , `investigationsThreatIntelligence``leakedCredentials`, , `generic`,`adminConfirmedUserCompromised``mcasImpossibleTravel` , , `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, e .`unknownFutureValue``suspiciousIPAddress``malwareInfectedIPAddress``unfamiliarFeatures``maliciousIPAddress``anonymizedIPAddress``unlikelyTravel` <br/> Para obter mais informações sobre cada valor, consulte [riskEventType values](#riskeventtype-values).|
|riskState|riskState|O estado de um usuário ou de login de risco detectado. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`e `unknownFutureValue`. |
|riskLevel|riskLevel|Nível do risco detectado. Os valores possíveis são `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, , `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`. <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`.|
|source|string|Origem da detecção de risco. Por exemplo, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado (em tempo real/offline). Os valores possíveis são , , , , `unknownFutureValue``offline`. `nearRealtime``realtime``notDefined` |
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são `signin`, `user`, `unknownFutureValue`. |
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

### <a name="riskeventtype-values"></a>valores riskEventType

| Member | Descrição |
|--|--|
| unlikelyTravel | Identifica dois sign-ins provenientes de locais geograficamente distantes, onde pelo menos um dos locais também pode ser atípico para o usuário, dado o comportamento passado.  |
| anonymizedIPAddress | Indica as insereções de um endereço IP anônimo, por exemplo, usando um navegador anônimo ou VPN. |
| maliciousIPAddress | Indica as logins de endereços IP conhecidos como mal-intencionados. Preterido e não mais gerado para novas detecções. |
| unfamiliarFeatures | Indica sign-ins com características que se desviam das propriedades de login anteriores. |
| malwareInfectedIPAddress | Indica as logins de endereços IP infectados por malware |
| suspiciousIPAddress | Identifica logons de endereços IP que são conhecidos como mal-intencionados no momento da sessão. |
| leakedCredentials | Indica que as credenciais válidas do usuário foram vazadas. Esse compartilhamento geralmente é feito postando publicamente na Web escura, colar sites ou comercializando e vendendo as credenciais no mercado negro. Quando o serviço de credenciais vazadas da Microsoft adquire credenciais de usuário da Web escura, sites de colar ou outras fontes, eles são verificados em relação às credenciais válidas atuais dos usuários do Azure AD para encontrar as combinações válidas. |
| investigationsThreatIntelligence | Indica uma atividade de login incomum para o usuário determinado ou consistente com padrões de ataque conhecidos com base nas fontes de inteligência de ameaças internas e externas da Microsoft. |
| generic | Indica que o usuário não estava habilitado para a Proteção de Identidade. |
| adminConfirmedUserCompromised | Indica que um administrador confirmou [que o usuário está comprometido](../api/riskyusers-confirmcompromised.md). |
| mcasImpossibleTravel | Descoberto pelo Microsoft Defender para Aplicativos de Nuvem (MDCA). Identifica duas atividades do usuário (uma única ou várias sessões) provenientes de locais geograficamente distantes em um período menor do que o tempo que ele teria levado o usuário a viajar do primeiro local para o segundo, indicando que um usuário diferente está usando as mesmas credenciais. |
| mcasSuspiciousInboxManipulationRules | Descoberto pelo Microsoft Defender para Aplicativos de Nuvem (MDCA). Identifica regras suspeitas de encaminhamento de email, por exemplo, se um usuário criou uma regra de caixa de entrada que encaminha uma cópia de todos os emails para um endereço externo.|
| investigationsThreatIntelligenceSigninLinked | Identifica atividade incomum com padrões de ataque conhecidos com base na inteligência contra ameaças |
| maliciousIPAddressValidCredentialsBlockedIP | Indica que a assinatura foi feita com credenciais válidas de um endereço IP mal-intencionado. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |


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
