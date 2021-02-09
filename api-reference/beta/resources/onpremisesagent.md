---
title: Tipo de recurso onPremisesAgent
description: Tipo de recurso onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158349"
---
# <a name="onpremisesagent-resource-type"></a>Tipo de recurso onPremisesAgent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agente local. Agentes locais instalados por um administrador de locatários podem ser configurados para acessar/manipular solicitações para um determinado [recurso publicado.](publishedresource.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgents](../api/onpremisesagent-list.md) | [Coleção onPremisesAgent](onpremisesagent.md) | Obter uma **coleção de objetos onPremisesAgents.** |
| [Obter onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | Leia as propriedades e os relacionamentos de um **objeto onPremisesAgent.** |
| [Atribuir onPremisesAgent a onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | Nenhum(a) | Atribua **um onPremisesAgent** a **um onPremisesAgentGroup**.|
| [Remover onpremisesAgent de um onPremisesAgentGroup](../api/onpremisesagent-delete-agentgroups.md) | Nenhum(a) | Remover um **onPremisesAgent** de **um onPremisesAgentGroup**. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|externalIp|String|O endereço IP externo conforme detectado pelo serviço para o computador do agente. Somente leitura|
|id|String| A ID do objeto do onPremisesAgent. Somente leitura.|
|machineName|String|O nome do computador em que o agregação está sendo executado. Somente leitura|
|status|cadeia de caracteres| Os valores possíveis são: `active` e `inactive`.|
|publishingType|string| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de **onPremisesAgentGroups** aos que um **onPremisesAgent** está atribuído. Somente leitura. Anulável.|

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



