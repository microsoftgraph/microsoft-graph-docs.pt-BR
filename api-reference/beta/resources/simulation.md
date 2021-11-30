---
title: tipo de recurso de simulação
description: Represente a simulação de ataque e a campanha de treinamento de um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e0cee15f6298ce67ca8be3cf8f6b2aef9302ac2a
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224794"
---
# <a name="simulation-resource-type"></a>tipo de recurso de simulação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma simulação de ataque e uma campanha de treinamento de um locatário.

Simulação e treinamento de ataque é um serviço disponível como parte do [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). Esse serviço permite que os usuários em um locatário experimentem um ataque de phishing benigno realista e aprendam com ele. O serviço permite que os administradores de locatários simulem, atribuam treinamentos e leiam informações derivadas sobre comportamentos online dos usuários nas simulações de phishing. O serviço fornece relatórios de simulação de ataque que ajudam os locatários a identificar lacunas de conhecimento de segurança, para que eles possam treinar ainda mais seus usuários para diminuir sua suscetibilidade a ataques. 

A _API_ de simulação e treinamento de  ataque permite que os [](report-m365defender-reports-overview.md) administradores de locatários listem exercícios e treinamentos de simulação lançados e recebam relatórios sobre informações derivadas sobre comportamentos online dos usuários nas simulações de phishing.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[coleção simulation](../resources/simulation.md)|Obter uma lista dos objetos [de simulação](../resources/simulation.md) e suas propriedades.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attackTechnique|[simulationAttackTechnique](#simulationattacktechnique-values)|A técnica de engenharia social usada na campanha de simulação e treinamento de ataques. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `credentialHarvesting`, `attachmentMalware`, `driveByUrl`, `linkInAttachment`, `linkToMalwareFile`, `unknownFutureValue`. Para obter mais informações sobre os tipos de técnicas de ataque de engenharia social, consulte [simulações](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).|
|attackType|[simulationAttackType](#simulationattacktype-values)|Tipo de ataque da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `social`, `cloud`, `endpoint`, `unknownFutureValue`.|
|cleanupArtifacts|Booleano|Sinalizador representando se artefatos foram limpos na campanha de simulação e treinamento de ataque.|
|completionDateTime|DateTimeOffset|Data e hora de conclusão da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que criou a campanha de simulação e treinamento de ataque.|
|createdDateTime|DateTimeOffset|Data e hora da criação da campanha de simulação e treinamento de ataque.|
|description|String|Descrição da campanha de simulação e treinamento de ataque.|
|displayName|String|Nome de exibição da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|enableRegionTimezoneDelivery|Booliano|Sinalizador representando se é possível habilitar ou desabilitar a entrega ciente de zona de tempo da carga de phishing na campanha de treinamento e simulação de ataque.|
|id|String|ID da campanha de treinamento e simulação de ataque.|
|includeAllAccountTargets|Booleano|Sinalizador representando a inclusão de todos os usuários de um locatário na campanha de simulação e treinamento de ataque.|
|isAutomated|Booleano|Sinalizador representando se a campanha de simulação e treinamento de ataque foi criada a partir de um fluxo de automação de simulação. Oferece suporte para `$filter` e `$orderby`. |
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que modificou a campanha de treinamento e simulação de ataque mais recentemente.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da modificação mais recente da campanha de simulação e treinamento de ataque.|
|launchDateTime|DateTimeOffset|Data e hora do início/início da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|payloadDeliveryPlatform|payloadDeliveryPlatform|Método de entrega da carga de phishing usada na campanha de simulação e treinamento de ataques. Os valores possíveis são: `unknown`, `sms`, `email`, `teams`, `unknownFutureValue`.|
|payloadSource|[payloadSource](#payloadsource-values)|Fonte de carga de phishing na campanha de simulação e treinamento de ataques. Os valores possíveis são: `unknown`, `global`, `tenant`, `unknownFutureValue`.|
|report|[simulationReport](../resources/simulationreport.md)|Relatório da campanha de simulação e treinamento de ataque.|
|status|simulationStatus|Status da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `draft`, `inProgress`, `scheduled`, `completed`, `partiallyCompleted`, `failed`, `cancelled`, `excluded`, `deleted`, `included`, `unknownFutureValue`.|
|trainingAssignmentPreference|[trainingAssignmentPreference](#trainingassignmentpreference-values)|Preferência do administrador do locatário para atribuir treinamento aos usuários na campanha de simulação e treinamento de ataque. Os valores possíveis são: `unknown`, `auto`, `manual`, `unknownFutureValue`.|
|trainingContentPreference|[trainingContentPreference](#trainingcontentpreference-values)|Preferência do administrador do locatário para a origem do conteúdo de treinamento a ser atribuído aos usuários na campanha de simulação e treinamento de ataque. Os valores possíveis são: `unknown`, `microsoft`, `custom`, `noTraining`, `unknownFutureValue`.|
|trainingDueDateTime|DateTimeOffset|Data e hora antes das quais os treinamentos precisam ser concluídos pelos usuários na campanha de simulação e treinamento de ataque.|

### <a name="simulationattacktechnique-values"></a>valores simulationAttackTechnique

|Member|Descrição |
|:---|:---|
|desconhecido| Técnica de ataque não definida. |
|credentialHarvesting| Técnica de ataque que envolve um usuário final fornecendo credenciais. |
|attachmentMalware| Técnica de ataque que envolve um usuário final clicando em um anexo. |
|driveByUrl| Técnica de ataque que envolve um usuário final clicando em um link de URL na carga de phishing. |
|linkInAttachment| Técnica de ataque que envolve um usuário final clicando em um link de URL em um anexo. |
|linkToMalwareFile| Técnica de ataque que envolve um usuário final clicando em um link de URL para um arquivo de malware. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

### <a name="simulationattacktype-values"></a>valores simulationAttackType

|Member|Descrição |
|:---|:---|
|desconhecido| Tipo de ataque não identificado. |
|social| Ataque que usa habilidades sociais para manipular as vítimas de forma psicológica, criando uma falsa sensação de curiosidade, urgência ou medo. |
|cloud| Ataque a um host ou usuário em um ambiente de nuvem, por exemplo, ataques de negação de serviço.|
|ponto de extremidade| Ataque aos pontos de extremidade de uma rede corporativa, como desktops, laptops, telefones celulares, dispositivos de Internet das coisas. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

### <a name="payloadsource-values"></a>valores payloadSource

|Member|Descrição |
|:---|:---|
|desconhecido| Fonte de carga não identificada. |
|global| Carga de uma coleção de cargas fornecidas pela Microsoft. |
|locatário| Carga de uma coleção de cargas fornecidas pelo locatário. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

### <a name="trainingassignmentpreference-values"></a>trainingAssignmentPreference values

|Member|Descrição |
|:---|:---|
|desconhecido| Preferência de atribuição de treinamento não identificada. |
|Automático| Atribua treinamentos aos usuários finais com base em critérios pré-definidos. |
|Manual| Atribua treinamentos aos usuários finais com base em critérios definidos pelo administrador. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

### <a name="trainingcontentpreference-values"></a>trainingContentPreference values

|Member|Descrição |
|:---|:---|
|desconhecido| Preferência de conteúdo de treinamento não identificada. |
|microsoft| Conteúdo de treinamento de uma coleção de treinamentos fornecidos pela Microsoft. |
|custom| Conteúdo de treinamento fornecido pelo locatário. |
|noTraining| Nenhuma atribuição de treinamento para usuários finais como parte da campanha. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulation",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "attackType": "String",
  "attackTechnique": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "launchDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "includeAllAccountTargets": "Boolean",
  "enableRegionTimezoneDelivery": "Boolean",
  "isAutomated": "Boolean",
  "cleanupArtifacts": "Boolean",
  "payloadSource": "String",
  "payloadDeliveryPlatform": "String",
  "trainingAssignmentPreference": "String",
  "trainingContentPreference": "String",
  "trainingDueDateTime": "String (timestamp)",
  "report": {
    "@odata.type": "microsoft.graph.simulationReport"
  }
}
```


## <a name="see-also"></a>Confira também
- [Simular um ataque de phishing](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true)
- [Começar a usar o treinamento de simulação de ataque](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).
