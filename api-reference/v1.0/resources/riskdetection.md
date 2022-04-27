---
title: Tipo de recurso riskDetection
description: detecções de risco
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6dad1999a6b0cea913f02bb1a072fa501a241157
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061101"
---
# <a name="riskdetection-resource-type"></a>Tipo de recurso riskDetection

Namespace: microsoft.graph

Representa informações sobre um risco detectado em um locatário do Azure AD. 

O Azure AD avalia continuamente [](riskyuser.md) os riscos do usuário e os riscos [](signin.md) de entrada do aplicativo ou do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todas as detecções de risco em seu ambiente do Azure AD.

Para obter mais informações sobre eventos de risco, [consulte Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Você deve ter uma licença Azure AD Premium P1 ou P2 para usar a API de detecção de risco.
> 2. A disponibilidade dos dados de detecção de risco é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskDetections](../api/riskdetection-list.md)|[coleção riskDetection](../resources/riskdetection.md)|Obtenha uma lista dos [objetos riskDetection](../resources/riskdetection.md) e suas propriedades.|
|[Obter riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Leia as propriedades e as relações de um [objeto riskDetection](../resources/riskdetection.md) .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|atividade|activityType|Indica o tipo de atividade ao qual o risco detectado está vinculado. Os valores possíveis são: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Data e hora em que a atividade arriscada ocorreu. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: `2014-01-01T00:00:00Z`|
|additionalInfo|String|Informações adicionais associadas à detecção de risco no formato JSON. Por exemplo, `"[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"`. As chaves possíveis na cadeia de caracteres JSON additionalInfo são: `userAgent`, , , `relatedEventTimeInUtc`, `relatedUserAgent`, `deviceInformation`, `relatedLocation``requestId`, `correlationId`, `lastActivityTimeInUtc`, `malwareName`, `clientIp``clientLocation``riskReasons`. `alertUrl` <br/>Para obter mais informações sobre riskReasons e valores possíveis, consulte [valores riskReasons](#riskreasons-values). |
|correlationId|Cadeia de caracteres|ID de correlação da entrada associada à detecção de risco. Essa propriedade será `null` se a detecção de risco não estiver associada a uma entrada.|
|detectedDateTime|DateTimeOffset|Data e hora em que o risco foi detectado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|Tempo do risco detectado (em tempo real/offline). Os valores possíveis são: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|Cadeia de caracteres|ID exclusiva da detecção de risco. Herdado da [entidade](../resources/entity.md)|
|ipAddress|Cadeia de caracteres|Fornece o endereço IP do cliente de onde o risco ocorreu.|
|lastUpdatedDateTime|DateTimeOffset|Data e hora em que a detecção de risco foi atualizada pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|Local da entrada.|
|Requestid|Cadeia de caracteres|ID da solicitação da entrada associada à detecção de risco. Essa propriedade será nula se a detecção de risco não estiver associada a uma entrada.|
|riskDetail|riskDetail|Detalhes do risco detectado. Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|String|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel`são , `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, , , `leakedCredentials`, `investigationsThreatIntelligence`,`adminConfirmedUserCompromised``generic` , `passwordSpray`, , `impossibleTravel`, `newCountry`, , `anomalousToken``tokenIssuerAnomaly`, , `riskyIPAddress``suspiciousBrowser`, , `mcasSuspiciousInboxManipulationRules``suspiciousInboxForwarding``unknownFutureValue` Se a detecção de risco for uma detecção premium, mostrará `generic`. <br/>Para obter mais informações sobre cada valor, consulte [valores riskEventType](#riskeventtype-values).|
|riskLevel|riskLevel|Nível do risco detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|O estado de um usuário arriscado detectado ou entrada. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Origem da detecção de risco. Por exemplo, `activeDirectory`. |
|tokenIssuerType|tokenIssuerType|Indica o tipo de emissor do token para o risco de entrada detectado. Os valores possíveis são: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|O nome UPN do usuário. |
|userId|Cadeia de caracteres|ID exclusivo do usuário.|
|userPrincipalName|String|O nome UPN do usuário.|

### <a name="riskeventtype-values"></a>Valores riskEventType

| Nome | Nome de exibição da interface do usuário | Descrição |
|--|--|--|
| unlikelyTravel | Viagem atípica | Identifica duas entradas originadas de locais geograficamente distantes, em que pelo menos um dos locais também pode ser atípico para o usuário, dado o comportamento passado.  |
| anonymizedIPAddress | Endereço IP anônimo | Indica entradas de um endereço IP anônimo, por exemplo, usando um navegador anônimo ou VPN. |
| maliciousIPAddress | Endereço IP mal-intencionado | Indica entradas de um endereço IP mal-intencionado. Um endereço IP é considerado mal-intencionado com base em altas taxas de falha devido a credenciais inválidas recebidas do endereço IP ou de outras fontes de reputação de IP. |
| unfamiliarFeatures | Propriedades de entrada desconhecidas | Indica entradas com características que se desviam das propriedades de entrada anteriores. |
| malwareInfectedIPAddress | Endereço IP vinculado a malware | Indica entradas de endereços IP infectados com malware. Preterido e não gerado mais para novas detecções. |
| suspiciousIPAddress | Endereço IP mal-intencionado | Identifica logons de endereços IP que são conhecidos como mal-intencionados no momento da entrada. |
| leakedCredentials | Vazamento de credenciais | Indica que as credenciais válidas do usuário foram vazadas. Esse compartilhamento normalmente é feito postando publicamente na Dark Web, colando sites ou negociando e vendendo as credenciais no mercado negro. Quando o serviço de credenciais vazadas da Microsoft adquire credenciais de usuário da Web escura, colar sites ou outras fontes, elas são verificadas em relação às credenciais válidas atuais dos usuários do Azure AD para localizar as correspondentes válidas. |
| investigationsThreatIntelligence | Inteligência contra ameaças do Azure AD | Indica uma atividade de entrada incomum para o usuário determinado ou que é consistente com padrões de ataque conhecidos com base nas fontes internas e externas de inteligência contra ameaças da Microsoft. |
| Genérico | Risco adicional detectado | Indica que o usuário não estava habilitado para o Identity Protection. |
| adminConfirmedUserCompromised | Usuário confirmado pelo administrador comprometido | Indica que um administrador confirmou [que o usuário está comprometido](../api/riskyuser-confirmcompromised.md). |
| passwordSpray | Pulverização de senha | Indica que vários nomes de usuário são atacados usando senhas comuns de maneira unificada de força bruta para obter acesso não autorizado. |
| anomalousToken | Token anômalo | Indica que há características anormais no token, como um tempo de vida de token incomum ou um token que é reproduzido de um local desconhecido. |
| tokenIssuerAnomaly | Anomalia do emissor do token | Indica que o emissor do token SAML para o token SAML associado está potencialmente comprometido. As declarações incluídas no token são incomuns ou correspondem a padrões de invasores conhecidos. |
| suspiciousBrowser | Navegador suspeito | Atividade suspeita de entrada em vários locatários de países diferentes no mesmo navegador. |
| impossibleTravel | Viagem impossivel | Descoberto por Microsoft Defender para Nuvem Aplicativos (MDCA). Identifica duas atividades do usuário (uma única ou várias sessões) originadas de locais geograficamente distantes em um período menor do que o tempo que levaria o usuário a viajar do primeiro local para o segundo, indicando que um usuário diferente está usando as mesmas credenciais. | 
| newCountry | Novo país | Essa detecção é descoberta por Microsoft Cloud App Security (MCAS). A entrada ocorreu de um local que não foi visitado recentemente ou nunca pelo usuário fornecido. |
| riskyIPAddress | Atividade de endereço IP anônimo | Essa detecção é descoberta por Microsoft Cloud App Security (MCAS). Os usuários estavam ativos de um endereço IP que foi identificado como um endereço IP de proxy anônimo. |
| mcasSuspiciousInboxManipulationRules | Regras de manipulação de caixa de entrada suspeita | Descoberto por Microsoft Defender para Nuvem Aplicativos (MDCA). Identifica regras suspeitas de encaminhamento de email, por exemplo, se um usuário criou uma regra de caixa de entrada que encaminha uma cópia de todos os emails para um endereço externo.|
| suspiciousInboxForwarding | Encaminhamento suspeito de caixa de entrada | Essa detecção é descoberta por Microsoft Cloud App Security (MCAS). Ele procura regras suspeitas de encaminhamento de email, por exemplo, se um usuário criou uma regra de caixa de entrada que encaminha uma cópia de todos os emails para um endereço externo. |
| unknownFutureValue | N/D | Valor de sentinel de enumeração evolvável. Não usar. |

### <a name="riskreasons-values"></a>valores riskReasons

| riskEventType | Valor | Cadeia de caracteres de exibição da interface do usuário |
|--|--|--|
| `investigationsThreatIntelligence` | `suspiciousIP` | Essa entrada foi de um endereço IP suspeito |
| `investigationsThreatIntelligence` | `passwordSpray` | Essa conta de usuário foi atacada por uma pulverização de senha. |

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
