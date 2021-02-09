---
title: Tipo de recurso onPremisesAgentGroup
description: Tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: da089ba198b5056bdecdceba96be572366618a23
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158342"
---
# <a name="onpremisesagentgroup-resource-type"></a>Tipo de recurso onPremisesAgentGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o grupo de agentes locais. Os grupos de agentes permitem que um administrador de locatários atribua [agentes](onpremisesagent.md) específicos para atender a recursos locais [publicados específicos.](publishedresource.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | Coleção onPremisesAgentGroups | Obter uma **coleção de objetos onPremisesAgentGroup.** |
| [Obter onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Leia as propriedades e os relacionamentos de um **objeto onPremisesAgentGroup.** |
| [Criar onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | Crie um novo **onPremisesAgentGroup**. |
| [Atualizar onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Atualize **um objeto onPremisesAgentGroup.** |
| [Excluir onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | Nenhum(a) | **Exclua um objeto onPremisesAgentGroup.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Nome de exibição **do onPremisesAgentGroup**.|
|id|String| A ID de objeto do **onPremisesAgentGroup**. Somente leitura.|
|isDefault|Booliano|Indica se o **onPremisesAgentGroup é** o grupo de agentes padrão. Somente um único grupo de agentes pode ser o **onPremisesAgentGroup** padrão e é definido pelo sistema.|
|publishingType|string| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentes|[Coleção onPremisesAgent](onpremisesagent.md)| Lista de **onPremisesAgent** que são atribuídos a **um onPremisesAgentGroup**. Somente leitura. Anulável.|
|publishedResources|[Coleção publishedResource](publishedresource.md)| Lista de **publishedResource** que são atribuídos a **um onPremisesAgentGroup**. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
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



