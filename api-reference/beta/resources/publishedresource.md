---
title: tipo de recurso publishedResource
description: tipo de recurso publishedResource.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841357"
---
# <a name="publishedresource-resource-type"></a>tipo de recurso publishedResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso publicado no local. Um administrador de locatários pode publicar vários tipos de recursos locais-aplicativos corporativos, controladores de domínio, servidores, etc. [os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um recurso publicado específico.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar publishedResources](../api/publishedresource-list.md) | coleção Objects [publishedResource](publishedresource.md) | Obtenha uma coleção de objetos **publishedResources** . |
| [Obter publishedResource](../api/publishedresource-get.md) | [publishedResource](publishedresource.md) | Leia as propriedades e os relacionamentos de um objeto **publishedResource** . |
| [Criar publishedResource](../api/publishedresource-post.md) |  [publishedResource](publishedresource.md)  | Criar um novo **publishedResource**. |
| [Atualizar publishedResource](../api/publishedresource-update.md) | [publishedResource](publishedresource.md) | Atualizar um objeto **publishedResource** . |
| [Excluir publishedResource](../api/publishedresource-delete.md) | Nenhum | Excluir um objeto **publishedResource** . |
| [Atribuir publishedResource a onPremisesAgentGroup](../api/publishedresource-post-agentgroups.md) | Nenhum | Atribua um objeto **publishedResource** a um **onPremisesAgentGroup**. |
| [Remover o publishedResource do onPremisesAgentGroup](../api/publishedresource-delete-agentgroups.md) | Nenhum |  Remover um objeto **publishedResource** de um **onPremisesAgentGroup**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String| Nome para exibição do publishedResource.|
|id|String| A ID de objeto do publishedResource. Somente leitura.|
|publishingtype|string| Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|
|resourceName|Cadeia de caracteres|Nome do publishedResource.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|coleção [onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de **onPremisesAgentGroups** aos quais um **publishedResource** é atribuído. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
