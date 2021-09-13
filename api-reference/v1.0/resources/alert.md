---
title: tipo de alerta do recurso
description: Representa possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros. Use alertas para unificar e agilizar o gerenciamento de problemas de segurança em todas as soluções integradas. Para saber mais, veja exemplos de consulta no Explorador de Gráfico.
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ac7198b4f45e9e79e12da878d28c3d245cefdf7a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089890"
---
# <a name="alert-resource-type"></a>tipo de alerta do recurso

Namespace: microsoft.graph

Representa possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros. Use alertas para unificar e agilizar o gerenciamento de problemas de segurança em todas as soluções integradas. Para saber mais, veja exemplos de consulta no [Explorador de Gráfico](https://developer.microsoft.com/graph/graph-explorer).

Os alertas podem ser recuperados de diferentes provedores de segurança listados na [Visão Geral de Segurança do Microsoft Graph](security-api-overview.md).

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Obter alerta](../api/alert-get.md) | [alert](alert.md) |Leia as propriedades e os relacionamentos do objeto de alerta.|
|[Atualizar alertas](../api/alert-update.md) | [alert](alert.md) |Atualize um objeto de alerta. |
|[Listar alertas](../api/alert-list.md) | conjunto [alerta](alert.md)  |Obtenha uma coleção de objetos de alerta.|

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                                         | Descrição                                                                                                                                                                                                                                                                                          |
|:---------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityGroupName    | String                                                       | Nome ou alias do grupo de atividades (invasor) a que este alerta é atribuído.                                                                                                                                                                                                                          |
| assignedTo           | String                                                       | Nome do analista ao qual o alerta está atribuído para triagem, investigação ou remediação (suporta [atualização](../api/alert-update.md)).                                                                                                                                                                  |
| azureSubscriptionId  | String                                                       | ID da assinatura do Azure, presente se o alerta estiver relacionado a um recurso do Azure.                                                                                                                                                                                                                        |
| azureTenantId        | String                                                       | ID do Locatário do Azure Active Directory. Obrigatório.                                                                                                                                                                                                                                                          |
| category             | String                                                       | Categoria de alerta (por exemplo, credentialTheft ransomware, etc.).                                                                                                                                                                                                                              |
| closedDateTime       | DateTimeOffset                                               | Tempo em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z` (suporta [atualização](../api/alert-update.md)).                    |
| cloudAppStates       | conjunto [cloudAppSecurityState](cloudappsecuritystate.md) | Informações com estado relacionadas à segurança geradas pelo provedor sobre os aplicativos de nuvem relacionados a esse alerta.                                                                                                                                                                                 |
| comentários             | String collection                                            | Comentários fornecidos pelo cliente no alerta (gerenciamento de alerta de cliente) (suporta [atualização](../api/alert-update.md)).                                                                                                                                                                                     |
| confidence           | Int32                                                        | Confiança da lógica de detecção (porcentagem entre 1 e 100).                                                                                                                                                                                                                                        |
| createdDateTime      | DateTimeOffset                                               | Hora em que o alerta foi criado pelo provedor de alerta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Obrigatório.                               |
| description          | String                                                       | Descrição de alerta.                                                                                                                                                                                                                                                                                   |
| detectionIds         | String collection                                            | Conjunto de alertas relacionados a essa entidade de alerta (cada alerta é enviado ao SIEM como um registro separado).                                                                                                                                                                                                  |
| eventDateTime        | DateTimeOffset                                               | Tempo no qual o(s) evento(s) que serviu (serviram) como acionador(es) para gerar o alerta ocorreu. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Obrigatório. |
| comentários             | alertFeedback                                                | Comentários do analista no alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (suporta [atualização](../api/alert-update.md))                                                                                                                                        |
| fileStates           | [fileSecurityState](filesecuritystate.md)         | Informações com estado relacionadas à segurança geradas pelo provedor sobre os arquivos relacionados a esse alerta.                                                                                                                                                                                             |
| hostStates           | Conjunto [hostSecurityState](hostsecuritystate.md)         | Informações com estado relacionadas à segurança geradas pelo provedor sobre o(s) host(s) relacionados a esse alerta.                                                                                                                                                                                             |
| id                   | String                                                       | Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.                                                                                                                                                                                                                                      |
| incidentIds          | Coleção de cadeias de caracteres                                            | IDs de incidentes relacionados ao alerta atual.                                                                                                                                                                                                                                                           |
| lastModifiedDateTime | DateTimeOffset                                               | Hora na qual entidade alerta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.                                                  |
| malwareStates        | conjunto [malwareState](malwarestate.md)                   | Inteligência contra ameaças referentes ao malware relacionado a esse alerta.                                                                                                                                                                                                                                     |
| networkConnections   | conjunto [networkConnection](networkconnection.md)         | Informações com estado relacionadas à segurança geradas pelo provedor sobre as conexões de rede relacionadas a esse alerta.                                                                                                                                                                               |
| processos            | conjunto [processo](process.md)                             | Informações com estado relacionadas à segurança geradas pelo provedor sobre o processo ou processos relacionados a esse alerta.                                                                                                                                                                                |
| recommendedActions   | String collection                                            | Ações recomendadas pelo provedor/fornecedor a serem tomadas como resultado do alerta (por exemplo, isolar máquina, enforce2FA, host de imagem de imagem).                                                                                                                                                                     |
| registryKeyStates    | conjunto [registryKeyState](registrykeystate.md)           | Informações com estado relacionadas à segurança geradas pelo provedor sobre as chaves de registro relacionadas a esse alerta.                                                                                                                                                                                       |
| securityResources    | Coleção de [securityResource](securityResource.md)           | Recursos relacionados ao alerta atual. Por exemplo, para alguns alertas, isso pode ter o valor do Recurso do Azure.                                                                                                                                                                                             |
| severity             | alertSeverity                                                | Gravidade de alerta, definida pelo provedor/fornecedor. Os valores possíveis são: `unknown`, `informational`, `low`, `medium`, `high`. Obrigatório.                                                                                                                                                                         |
| sourceMaterials      | String collection                                            | Hiperlinks (URIs) para o material de origem relacionado ao alerta, por exemplo, a interface do usuário do provedor para alertas ou pesquisa de log, etc.                                                                                                                                                                 |
| status               | alertStatus                                                  | Status de alerta de ciclo de vida (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`. (suporta [atualização](../api/alert-update.md)). Obrigatório.                                                                                                                                         |
| marcações                 | String collection                                            | Etiquetas definidas pelo usuário que podem ser aplicadas a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SAW", etc.) (suporta [atualização](../api/alert-update.md)).                                                                                                                               |
| title                | String                                                       | Título do alerta. Obrigatório.                                                                                                                                                                                                                                                                               |
| gatilhos             | Conjunto [alertTrigger](alerttrigger.md)                   | Informações de segurança sobre propriedades específicas que dispararam o alerta (Propriedades aparecendo no alerta). Os alertas podem conter informações sobre vários usuários hosts, arquivos, endereços ip. Este campo indica quais propriedades acionaram a geração de alertas.                    |
| userStates           | Conjunto [userSecurityState](usersecuritystate.md)         | Informações com estado relacionadas à segurança geradas pelo provedor sobre as contas de usuários relacionadas a esse alerta.                                                                                                                                                                                       |
| vendorInformation    | [securityVendorInformation](securityvendorinformation.md)    | Tipo complexo que contém detalhes do fornecedor, provedor e subprovedor de produtos/serviços de segurança (por exemplo, fornecedor=Microsoft; provedor=Windows Defender ATP; subProvedor=AppLocker).                                                                                                |
| vulnerabilityStates  | conjunto [vulnerabilityState](vulnerabilitystate.md)       | Inteligência de ameaças referente a uma ou mais vulnerabilidades relacionadas a este alerta.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "incidentIds": ["String"],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "securityResources": [{"@odata.type": "microsoft.graph.securityResource"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

