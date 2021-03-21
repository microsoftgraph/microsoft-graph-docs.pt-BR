---
title: Tipo de recurso onPremisesAgent
description: Tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74128ab48e023f066f259fea5f326d5e1642eb14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956929"
---
# <a name="onpremisesagent-resource-type"></a>Tipo de recurso onPremisesAgent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agente local. Agentes locais instalados por um administrador de locatários podem ser configurados para acessar/manipular solicitações para um determinado [recurso publicado.](publishedresource.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgents](../api/onpremisesagent-list.md) | [Coleção onPremisesAgent](onpremisesagent.md) | Obter uma **coleção de objetos onPremisesAgents.** |
| [Obter onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | Leia as propriedades e as relações de um **objeto onPremisesAgent.** |
| [Atribuir onPremisesAgent ao onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | Nenhum | Atribua **um onPremisesAgent** a **um onPremisesAgentGroup**.|
| [Remover onpremisesAgent de um onPremisesAgentGroup](../api/onpremisesagent-delete-agentgroups.md) | Nenhum | Remova um **onPremisesAgent** de **um onPremisesAgentGroup**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|Cadeia de caracteres|O endereço IP externo, conforme detectado pelo serviço para o computador do agente. Somente leitura|
|id|Cadeia de caracteres| A id do objeto do onPremisesAgent. Somente leitura.|
|machineName|Cadeia de caracteres|O nome do computador em que o aggent está sendo executado. Somente leitura|
|status|agentStatus| Os valores possíveis são: `active` e `inactive`.|
|publishingType|Cadeia de caracteres| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de **onPremisesAgentGroups** aos que um **onPremisesAgent** é atribuído. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



