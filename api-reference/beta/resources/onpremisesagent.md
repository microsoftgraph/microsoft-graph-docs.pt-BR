---
title: tipo de recurso onPremisesAgent
description: tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ec125e52eaf9eba3423f70dd47cc7dd1562716bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052588"
---
# <a name="onpremisesagent-resource-type"></a>tipo de recurso onPremisesAgent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agente local. Os agentes locais instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgents](../api/onpremisesagent-list.md) | coleção [onPremisesAgent](onpremisesagent.md) | Obtenha uma coleção de objetos **onPremisesAgents** . |
| [Obter onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | Leia as propriedades e os relacionamentos de um objeto **onPremisesAgent** . |
| [Atribuir onPremisesAgent a onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | Nenhum | Atribua um **onPremisesAgent** a um **onPremisesAgentGroup**.|
| [Remover o onpremisesAgent de um onPremisesAgentGroup](../api/onpremisesagent-delete-agentgroups.md) | Nenhum | Remover um **onPremisesAgent** de um **onPremisesAgentGroup**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|Cadeia de caracteres|O endereço IP externo, conforme detectado pelo serviço para o computador do agente. Somente leitura|
|id|Cadeia de caracteres| A ID de objeto do onPremisesAgent. Somente leitura.|
|Nomecomputador|Cadeia de caracteres|O nome da máquina na qual o aggent está sendo executado. Somente leitura|
|status|cadeia de caracteres| Os valores possíveis são: `active` e `inactive`.|
|publishingtype|cadeia de caracteres| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|coleção [onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de **onPremisesAgentGroups** aos quais um **onPremisesAgent** é atribuído. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
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


