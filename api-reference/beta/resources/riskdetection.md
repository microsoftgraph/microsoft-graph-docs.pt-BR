---
title: Tipo de recurso riskDetection
description: Representa todas as detecções de risco em locatários do AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5e27d1df57ac4242f74cca746b7dc8890f004c7a
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060483"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD avalia continuamente [](riskyuser.md) os riscos do usuário e os riscos [](signin.md) de entrada do aplicativo ou do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Você deve ter uma licença Azure AD Premium P1 ou P2 para usar a API de detecção de risco.
> 2. A disponibilidade dos dados de detecção de risco é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Listar riskDetection](../api/riskdetection-list.md) | [coleção riskDetection](riskdetection.md)|Listar detecções de risco e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Obtenha uma detecção de risco específica e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|id|string|ID exclusiva da detecção de risco. |
|Requestid|string|ID da solicitação da entrada associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma entrada.|
|correlationId|string|ID de correlação da entrada associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma entrada. |
|riskEventType|string|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel`são , `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, , `leakedCredentials`, `investigationsThreatIntelligence`, `generic`,`adminConfirmedUserCompromised` , `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, , , `maliciousIPAddressValidCredentialsBlockedIP`, e `unknownFutureValue`. <br/> Para obter mais informações sobre cada valor, consulte [valores riskEventType](#riskeventtype-values).|
|riskState|riskState|O estado de um usuário arriscado detectado ou entrada. Os valores possíveis são `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`e `confirmedCompromised``unknownFutureValue`. |
|riskLevel|riskLevel|Nível do risco detectado. Os valores possíveis são `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, , `adminConfirmedUserCompromised`, `unknownFutureValue`. <br />**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`.|
|source|string|Origem da detecção de risco. Por exemplo, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado (em tempo real/offline). Os valores possíveis são `notDefined`, `realtime`, `nearRealtime`, `offline`. `unknownFutureValue` |
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são `signin`, `user`. `unknownFutureValue` |
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor do token para o risco de entrada detectado. Os valores possíveis são `AzureAD`, `ADFederationServices` e `unknownFutureValue`. |
|ipAddress|string|Fornece o endereço IP do cliente de onde o risco ocorreu. |
|location|[signInLocation](signinlocation.md)|Local da entrada. |
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z` |
|lastUpdatedDateTime|DateTimeOffset|Data e hora em que a detecção de risco foi atualizada pela última vez. |
|userId|cadeia de caracteres|ID exclusivo do usuário.  O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|userDisplayName|string|Nome do usuário. |
|userPrincipalName|string|O nome UPN do usuário. |
|additionalInfo|string|Informações adicionais associadas à detecção de risco no formato JSON. |
|riskType (preterido)|riskEventType|Lista de tipos de evento de risco.<br />**Nota:** Essa propriedade foi preterida. Em **vez disso, use riskEventType** . |

### <a name="riskeventtype-values"></a>Valores riskEventType

| Member | Descrição |
|--|--|
| unlikelyTravel | Identifica duas entradas originadas de locais geograficamente distantes, em que pelo menos um dos locais também pode ser atípico para o usuário, dado o comportamento passado.  |
| anonymizedIPAddress | Indica entradas de um endereço IP anônimo, por exemplo, usando um navegador anônimo ou VPN. |
| maliciousIPAddress | Indica entradas de endereços IP conhecidos como mal-intencionados. Preterido e não gerado mais para novas detecções. |
| unfamiliarFeatures | Indica entradas com características que se desviam das propriedades de entrada anteriores. |
| malwareInfectedIPAddress | Indica entradas de endereços IP infectados com malware |
| suspiciousIPAddress | Identifica logons de endereços IP que são conhecidos como mal-intencionados no momento da entrada. |
| leakedCredentials | Indica que as credenciais válidas do usuário foram vazadas. Esse compartilhamento normalmente é feito postando publicamente na Dark Web, colando sites ou negociando e vendendo as credenciais no mercado negro. Quando o serviço de credenciais vazadas da Microsoft adquire credenciais de usuário da Web escura, colar sites ou outras fontes, elas são verificadas em relação às credenciais válidas atuais dos usuários do Azure AD para localizar as correspondentes válidas. |
| investigationsThreatIntelligence | Indica uma atividade de entrada incomum para o usuário determinado ou que é consistente com padrões de ataque conhecidos com base nas fontes internas e externas de inteligência contra ameaças da Microsoft. |
| Genérico | Indica que o usuário não estava habilitado para o Identity Protection. |
| adminConfirmedUserCompromised | Indica que um administrador confirmou [que o usuário está comprometido](../api/riskyusers-confirmcompromised.md). |
| mcasImpossibleTravel | Descoberto por Microsoft Defender para Nuvem Aplicativos (MDCA). Identifica duas atividades do usuário (uma única ou várias sessões) originadas de locais geograficamente distantes em um período menor do que o tempo que levaria o usuário a viajar do primeiro local para o segundo, indicando que um usuário diferente está usando as mesmas credenciais. |
| mcasSuspiciousInboxManipulationRules | Descoberto por Microsoft Defender para Nuvem Aplicativos (MDCA). Identifica regras suspeitas de encaminhamento de email, por exemplo, se um usuário criou uma regra de caixa de entrada que encaminha uma cópia de todos os emails para um endereço externo.|
| investigationsThreatIntelligenceSigninLinked | Identifica a atividade que é incomum com padrões de ataque conhecidos com base na inteligência contra ameaças |
| maliciousIPAddressValidCredentialsBlockedIP | Indica que a entrada foi feita com credenciais válidas de um endereço IP mal-intencionado. |
| unknownFutureValue | Valor de sentinel de enumeração evolvável. Não usar. |


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
