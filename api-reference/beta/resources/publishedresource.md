---
title: Tipo de recurso publishedResource
description: Tipo de recurso publishedResource.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1090e985fc9ffdec0c27f9793a361851d2fa5216
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155563"
---
# <a name="publishedresource-resource-type"></a>Tipo de recurso publishedResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso publicado no local. Um administrador de locatários pode publicar vários tipos de recursos locais - aplicativos corporativos, controladores de domínio, servidores etc. Agentes locais instalados por um administrador de locatários podem ser [configurados](onpremisesagent.md) para acessar/manipular solicitações para um recurso publicado específico.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar publishedResources](../api/publishedresource-list.md) | [Coleção de objetos publishedResource](publishedresource.md) | Obter uma **coleção de objetos publishedResources.** |
| [Obter publishedResource](../api/publishedresource-get.md) | [publishedResource](publishedresource.md) | Leia as propriedades e os relacionamentos de um **objeto publishedResource.** |
| [Criar publishedResource](../api/publishedresource-post.md) |  [publishedResource](publishedresource.md)  | Crie um novo **publishedResource**. |
| [Atualizar publishedResource](../api/publishedresource-update.md) | [publishedResource](publishedresource.md) | Atualize **um objeto publishedResource.** |
| [Excluir publishedResource](../api/publishedresource-delete.md) | Nenhum(a) | **Exclua um objeto publishedResource.** |
| [Atribuir publishedResource a onPremisesAgentGroup](../api/publishedresource-post-agentgroups.md) | Nenhum(a) | Atribuir um **objeto publishedResource** a **um onPremisesAgentGroup**. |
| [Remover publishedResource de onPremisesAgentGroup](../api/publishedresource-delete-agentgroups.md) | Nenhum(a) |  Remover um **objeto publishedResource** de **um onPremisesAgentGroup**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String| Nome de exibição do publishedResource.|
|id|String| A ID do objeto do publishedResource. Somente leitura.|
|publishingType|string| Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|
|resourceName|Cadeia de caracteres|Nome do publishedResource.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de **onPremisesAgentGroups** aos que um **publishedResource** é atribuído. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
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


