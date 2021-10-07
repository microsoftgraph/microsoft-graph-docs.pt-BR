---
title: tipo de recurso incident
description: Um incidente no Microsoft 365 Defender é uma coleção de alertas correlacionados e metadados associados que reflete a história de um ataque.
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e1bef3d9d62fc91cee2fe1883d564bd27eaba638
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220817"
---
# <a name="incident-resource-type"></a>tipo de recurso incident

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um incidente no Microsoft 365 Defender é uma coleção de alertas correlacionados e metadados associados que reflete a história de um ataque em um locatário.

Microsoft 365 serviços e aplicativos criam alertas quando detectam um evento ou atividade suspeito ou mal-intencionado. Alertas individuais fornecem dicas valiosas sobre um ataque concluído ou contínuo. No entanto, os ataques geralmente empregam várias técnicas contra diferentes tipos de entidades, como dispositivos, usuários e caixas de correio. O resultado são vários alertas para várias entidades em seu locatário.
Como reunir os alertas individuais para obter informações sobre um ataque pode ser desafiador e demorado, Microsoft 365 Defender agrega automaticamente os alertas e suas informações associadas a um incidente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar incidentes](../api/security-list-incidents.md)|[coleção incident](../resources/incident.md)|Obter uma lista dos objetos [de incidente](../resources/incident.md) e suas propriedades.|
|[Obter incidente](../api/incident-get.md)|[incident](../resources/incident.md)|Leia as propriedades e as relações de um [objeto incident.](../resources/incident.md)|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedTo|Cadeia de caracteres|Proprietário do incidente ou nulo se nenhum proprietário for atribuído. Texto editável gratuito.|
|classificação|[m365AlertClassification](#m365alertclassification-values)|A especificação do incidente. Os valores possíveis são: `unknown`, `falsePositive`, `truePositive`, `benignPositive`, `unknownFutureValue`.|
|comentários|[Coleção m365AlertComment](../resources/m365alertcomment.md)|Matriz de comentários criados pela equipe de Operações de Segurança (SecOps) quando o incidente é gerenciado.|
|createdDateTime|DateTimeOffset|Hora em que o incidente foi criado pela primeira vez.|
|determinação|[m365AlertDetermination](#m365alertdetermination-values)|Especifica a determinação do incidente. Os valores possíveis são: `unknown`, `apt`, `malware`, `securityPersonnel`, `securityTesting`, `unwantedSoftware`, `other`, `multiStagedAttack`, `compromisedUser`, `phishing`, `maliciousUserActivity`, `clean`, `insufficientData`, `confirmedUserActivity`, `lineOfBusinessApplication`, `unknownFutureValue`.|
|displayName|Cadeia de caracteres|O nome do incidente.|
|id|Cadeia de caracteres|Identificador exclusivo para representar o incidente.|
|incidentWebUrl|String|URL para a página de incidentes Microsoft 365 Defender portal.|
|lastUpdateDateTime|DateTimeOffset|Hora em que o incidente foi atualizado pela última vez.|
|redirectIncidentId|Cadeia de caracteres|Somente populado no caso de um incidente ser agrupado com outro incidente, como parte da lógica que processa incidentes.|
|severity|[m365AlertSeverity](#m365alertseverity-values )|Indica o possível impacto nos ativos. Quanto maior a gravidade, maior será o impacto. Normalmente, itens de severidade mais altos exigem a atenção mais imediata. Os possíveis valores são: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.|
|status|[incidentStatus](#incidentstatus-values)|O status do incidente. Os valores possíveis são: `active`, `resolved`, `redirected`, `unknownFutureValue`.|
|categorias|Coleção String|Matriz de marcas personalizadas associadas a um incidente.|


### <a name="incidentstatus-values"></a>valores incidentStatus 

| Member              | Descrição                                                                                                           |
| :-------------------| :-------------------------------------------------------------------------------------------------------------------- |
| active              | O incidente está em estado ativo.                                                                                      |
| resolvido            | O incidente está em estado resolvido.                                                                                    |
| redirecionado          | O incidente foi mesclado com outro incidente. A ID do incidente de destino aparece na **propriedade redirectIncidentId.** |
| unknownFutureValue  | Valor de sentinela de enumeração evolvável. Não usar.                                                                     |

### <a name="m365alertclassification-values"></a>Valores m365AlertClassification 

| Member              | Descrição                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------- |
| desconhecido             | O alerta ainda não foi classificado.                                                                                                     |
| falsePositive       | O alerta é um falso positivo e não detectou atividade mal-intencionada.                                                                 |
| truePositive        | O alerta é verdadeiro positivo e detectou atividade mal-intencionada.                                                                         |
| benignPositive      | O alerta é positivo benigno e detectado atividade potencialmente mal-intencionada por um usuário interno/confiável, por exemplo, teste de segurança. |
| unknownFutureValue  | Valor de sentinela de enumeração evolvável. Não usar.                                                                                   |

### <a name="m365alertdetermination-values"></a>valores m365AlertDetermination 

| Member                     | Descrição                                                                                                                  |
| :--------------------------| :--------------------------------------------------------------------------------------------------------------------------- |
| desconhecido                    | Nenhum valor de determinação foi definido ainda.                                                                                          |
| apt                        | Um alerta positivo verdadeiro que detectou uma ameaça persistente avançada.                                                           |
| malware                    | Um alerta positivo verdadeiro que detectou software mal-intencionado.                                                                      |
| securityPersonnel          | Um alerta positivo verdadeiro que detectou atividades suspeitas válidas que foram executadas por alguém na equipe de segurança do cliente. |
| securityTesting            | O alerta detectou atividade suspeita válida que foi executada como parte de um teste de segurança conhecido.                         |
| unwantedSoftware           | O alerta detectou software indesejado.                                                                                        |
| multiStagedAttack          | Um alerta positivo verdadeiro que detectou vários estágios de ataque de cadeia de morte.                                                       |
| compromisedUser            | Um alerta positivo verdadeiro que detectou que as credenciais do usuário pretendido foram comprometidas ou roubadas.                         |
| phishing                   | Um alerta positivo verdadeiro que detectou um email de phishing.                                                                        |
| maliciousUserActivity      | Um alerta positivo verdadeiro que detectou que o usuário conectado executa atividades mal-intencionadas.                                   |
| clean                      | Um alerta falso, nenhuma atividade suspeita.                                                                                       |
| insufficientData           | Um alerta falso, sem informações suficientes para provar o contrário.                                                                |
| confirmedUserActivity      | O alerta flagrou uma atividade suspeita verdadeira que é considerada OK porque é uma atividade de usuário conhecida.                       |
| lineOfBusinessApplication  | O alerta flagrou uma atividade suspeita verdadeira que é considerada OK porque é um aplicativo interno conhecido e confirmado.  |
| other                      | Outra determinação.                                                                                                         |
| unknownFutureValue         | Valor de sentinela de enumeração evolvável. Não usar.                                                                            |

### <a name="m365alertseverity-values"></a>valores m365AlertSeverity 

| Member                     | Descrição                                                                                                                  |
| :--------------------------| :--------------------------------------------------------------------------------------------------------------------------- |
| desconhecido            | Gravidade desconhecida.       |
| informational      | Alertas que podem não ser ativas ou considerados prejudiciais para a rede, mas podem impulsionar a conscientização de segurança organizacional sobre possíveis problemas de segurança.     |
| low                | Alertas sobre ameaças associadas ao malware predominante. Por exemplo, as ferramentas de hack, ferramentas de hack não malware, como a execução de comandos de exploração e a limpeza de logs, que muitas vezes não indicam uma ameaça avançada que se direciona à organização. Ele também pode vir de uma ferramenta de segurança isolada que é testada por um usuário em sua organização.  |
| medium             | Alertas gerados de comportamentos pós-violação de detecções e respostas que podem fazer parte de uma ameaça persistente avançada (APT). Isso inclui comportamentos observados típicos de estágios de ataque, alteração anômala do registro, execução de arquivos suspeitos e assim por diante. Embora alguns possam ser devido a testes internos de segurança, eles são detecções válidas e exigem investigação, pois podem fazer parte de um ataque avançado. |
| high               | Alertas comumente vistos associados a ameaças persistentes avançadas (APT). Esses alertas indicam um alto risco devido à gravidade dos danos que podem causar nos ativos. Alguns exemplos são: atividades de ferramentas de roubo de credenciais, atividades de ransomware não associadas a nenhum grupo, adulteração de sensores de segurança ou atividades mal-intencionadas indicando um adversário humano. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |



## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.incident",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incident",
  "id": "String (identifier)",
  "incidentWebUrl": "String",
  "redirectIncidentId": "String",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastUpdateDateTime": "String (timestamp)",
  "assignedTo": "String",
  "classification": "String",
  "determination": "String",
  "status": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "comments": [
    {
      "@odata.type": "microsoft.graph.m365AlertComment"
    }
  ]
}
```
