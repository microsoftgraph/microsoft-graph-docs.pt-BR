---
title: Tipo de recurso onPremisesAgentGroup
description: Tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5751e01ab6e7645416a8a8fde5c30f09c38a3d22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956915"
---
# <a name="onpremisesagentgroup-resource-type"></a>Tipo de recurso onPremisesAgentGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o grupo de agentes locais. Os grupos de agentes permitem que um administrador de locatário atribua [agentes](onpremisesagent.md) específicos para atender a recursos [locais publicados específicos.](publishedresource.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | Coleção onPremisesAgentGroups | Obter uma **coleção de objetos onPremisesAgentGroup.** |
| [Obter onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Leia as propriedades e as relações de um **objeto onPremisesAgentGroup.** |
| [Criar onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | Crie um novo **onPremisesAgentGroup**. |
| [Atualizar onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Atualize um **objeto onPremisesAgentGroup.** |
| [Excluir onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | Nenhum | **Exclua um objeto onPremisesAgentGroup.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome de exibição **do onPremisesAgentGroup**.|
|id|Cadeia de caracteres| A ID do objeto **do onPremisesAgentGroup**. Somente leitura.|
|isDefault|Booliano|Indica se **o onPremisesAgentGroup** é o grupo de agente padrão. Somente um único grupo de agentes pode ser o **padrão onPremisesAgentGroup** e é definido pelo sistema.|
|publishingType|Cadeia de caracteres| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentes|[Coleção onPremisesAgent](onpremisesagent.md)| Lista de **onPremisesAgent** atribuídos a **um onPremisesAgentGroup**. Somente leitura. Anulável.|
|publishedResources|[coleção publishedResource](publishedresource.md)| Lista de **publishedResource** que são atribuídos a **um onPremisesAgentGroup**. Somente leitura. Anulável.|

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



