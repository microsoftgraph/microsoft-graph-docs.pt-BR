---
title: tipo de recurso onPremisesAgentGroup
description: tipo de recurso onPremisesAgentGroup.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 203d914098d6b7cb0b03715accac4958bcf53870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522232"
---
# <a name="onpremisesagentgroup-resource-type"></a>tipo de recurso onPremisesAgentGroup

Namespace: Microsoft. Graph

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
|id|String| A ID de objeto do **onPremisesAgentGroup**. Somente leitura.|
|isDefault|Booliano|Indica se o **onPremisesAgentGroup** é o grupo de agente padrão. Somente um único grupo de agentes pode ser o padrão **onPremisesAgentGroup** e é definido pelo sistema.|
|publishingtype|string| Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

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
