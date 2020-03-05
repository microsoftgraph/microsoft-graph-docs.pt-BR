---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be4fa7bd8f4b44842bd6dbc9876d0dd19fe466fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507496"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="b6ef6-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="b6ef6-103">configuration resource type</span></span>

<span data-ttu-id="b6ef6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6ef6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6ef6-105">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="b6ef6-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="b6ef6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6ef6-106">Properties</span></span>

| <span data-ttu-id="b6ef6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6ef6-107">Property</span></span>       | <span data-ttu-id="b6ef6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6ef6-108">Type</span></span>              | <span data-ttu-id="b6ef6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6ef6-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="b6ef6-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="b6ef6-110">authorizedApps</span></span> | <span data-ttu-id="b6ef6-111">String collection</span><span class="sxs-lookup"><span data-stu-id="b6ef6-111">String collection</span></span> | <span data-ttu-id="b6ef6-112">Uma coleção de IDs de aplicativo para aplicativos registrados do Active Directory do Azure que têm permissão para gerenciar o externalConnection e indexar o conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="b6ef6-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6ef6-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6ef6-113">JSON representation</span></span>

<span data-ttu-id="b6ef6-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6ef6-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
