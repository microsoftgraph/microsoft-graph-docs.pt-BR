---
title: tipo de recurso de simulação
description: Representa uma campanha de treinamento de simulação de ataque em um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: fbd043bd16176834c523d3b5083fab5ce69c406d
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757833"
---
# <a name="simulation-resource-type"></a>tipo de recurso de simulação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma campanha de treinamento de simulação de ataque em um locatário.

Simulação e treinamento de ataque é um serviço disponível como parte do [Microsoft Defender para](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) Office 365. Esse serviço permite que os usuários em um locatário experimentem um ataque de phishing benigno realista e aprendam com ele. O serviço permite que os administradores de locatários simulem, atribuam treinamentos e leiam informações derivadas sobre comportamentos online dos usuários nas simulações de phishing. O serviço fornece relatórios de simulação de ataque que ajudam os locatários a identificar lacunas de conhecimento de segurança, para que eles possam treinar ainda mais seus usuários para diminuir sua suscetibilidade a ataques.

A API de simulação e treinamento de ataque permite que os administradores de  locatários listem exercícios e treinamentos de simulação lançados e recebam relatórios sobre informações derivadas sobre comportamentos online dos usuários nas simulações de phishing.[](report-m365defender-reports-overview.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[coleção simulation](../resources/simulation.md)|Obter uma lista dos objetos [de simulação](../resources/simulation.md) e suas propriedades.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attackTechnique|[simulationAttackTechnique](#simulationattacktechnique-values)|A técnica de engenharia social usada na campanha de simulação e treinamento de ataques. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `credentialHarvesting`, `attachmentMalware`, `driveByUrl`, `linkInAttachment`, `linkToMalwareFile`, `unknownFutureValue`. Para obter mais informações sobre os tipos de técnicas de ataque de engenharia social, consulte [simulações](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).|
|attackType|[simulationAttackType](#simulationattacktype-values)|Tipo de ataque da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `social`, `cloud`, `endpoint`, `unknownFutureValue`.|
|automationId|Cadeia de Caracteres|Identificador exclusivo para a automação de simulação de ataque.|
|completionDateTime|DateTimeOffset|Data e hora de conclusão da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|createdBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que criou a campanha de simulação e treinamento de ataque.|
|createdDateTime|DateTimeOffset|Data e hora da criação da campanha de simulação e treinamento de ataque.|
|descrição|Cadeia de caracteres|Descrição da campanha de simulação e treinamento de ataque.|
|displayName|String|Nome de exibição da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|id|Cadeia de caracteres|Identificador exclusivo para a campanha de simulação e treinamento de ataque.|
|isAutomated|Boolean|Sinalizador representando se a campanha de simulação e treinamento de ataque foi criada a partir de um fluxo de automação de simulação. Oferece suporte para `$filter` e `$orderby`. |
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|Identidade do usuário que modificou a campanha de treinamento e simulação de ataque mais recentemente.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da modificação mais recente da campanha de simulação e treinamento de ataque.|
|launchDateTime|DateTimeOffset|Data e hora do início/início da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`.|
|payloadDeliveryPlatform|payloadDeliveryPlatform|Método de entrega da carga de phishing usada na campanha de simulação e treinamento de ataques. Os valores possíveis são: `unknown`, `sms`, `email`, `teams`, `unknownFutureValue`.|
|report|[simulationReport](../resources/simulationreport.md)|Relatório da campanha de simulação e treinamento de ataque.|
|status|[simulationStatus](#simulationstatus-values)|Status da campanha de simulação e treinamento de ataque. Oferece suporte para `$filter` e `$orderby`. Os valores possíveis são: `unknown`, `draft`, `running`, `scheduled`, `succeeded`, `failed`, `cancelled`, `excluded`, `unknownFutureValue`.|

### <a name="simulationstatus-values"></a>valores simulationStatus

|Member|Descrição |
|:---|:---|
|desconhecido| O status da simulação não está definido. |
|draft| A simulação está no modo de rascunho. |
|running| A simulação está em execução. |
|agendado| A simulação está agendada. |
|bem-sucedido| A simulação foi bem-sucedida. |
|failed| A simulação falhou. |
|cancelado| A simulação foi cancelada. |
|excluded| A simulação é excluída. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

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
  "isAutomated": "Boolean",
  "automationId": "String",
  "payloadDeliveryPlatform": "String",
  "report": {
    "@odata.type": "microsoft.graph.simulationReport"
  }
}
```


## <a name="see-also"></a>Confira também
- [Simular um ataque de phishing](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true)
- [Começar a usar o treinamento de simulação de ataque](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).
