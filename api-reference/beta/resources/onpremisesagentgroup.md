---
title: tipo de recurso onPremisesAgentGroup
description: tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f0236c2c2e52742a84f19eae8eb7693f1b559b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052593"
---
# <a name="onpremisesagentgroup-resource-type"></a>tipo de recurso onPremisesAgentGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o grupo de agentes local. Os grupos de agentes permitem que um administrador de locatários atribua [agentes](onpremisesagent.md) específicos para atender [recursos locais publicados](publishedresource.md)específicos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | coleção onPremisesAgentGroups | Obtenha uma coleção de objetos **onPremisesAgentGroup** . |
| [Obter onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Leia as propriedades e os relacionamentos de um objeto **onPremisesAgentGroup** . |
| [Criar onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | Criar um novo **onPremisesAgentGroup**. |
| [Atualizar onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Atualize um objeto **onPremisesAgentGroup** . |
| [Excluir onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | Nenhum | Excluir um objeto **onPremisesAgentGroup** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome para exibição do **onPremisesAgentGroup**.|
|id|Cadeia de caracteres| A ID de objeto do **onPremisesAgentGroup**. Somente leitura.|
|isDefault|Booliano|Indica se o **onPremisesAgentGroup** é o grupo de agente padrão. Somente um único grupo de agentes pode ser o padrão **onPremisesAgentGroup** e é definido pelo sistema.|
|publishingtype|cadeia de caracteres| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|SNMP|coleção [onPremisesAgent](onpremisesagent.md)| Lista de **onPremisesAgent** que são atribuídas a um **onPremisesAgentGroup**. Somente leitura. Anulável.|
|publishedResources|coleção [publishedResource](publishedresource.md)| Lista de **publishedResource** que são atribuídas a um **onPremisesAgentGroup**. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


