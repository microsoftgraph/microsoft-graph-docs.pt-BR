---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7808d014ee2ab19fda9eceb6064375cf5904d52
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704147"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="bf380-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="bf380-103">configuration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf380-104">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar o externalConnection e indexar o conteúdo em um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="bf380-104">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="bf380-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf380-105">Properties</span></span>

| <span data-ttu-id="bf380-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf380-106">Property</span></span>       | <span data-ttu-id="bf380-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf380-107">Type</span></span>              | <span data-ttu-id="bf380-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf380-108">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="bf380-109">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="bf380-109">authorizedApps</span></span> | <span data-ttu-id="bf380-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf380-110">String collection</span></span> | <span data-ttu-id="bf380-111">Uma coleção de IDs de aplicativo para aplicativos registrados do Active Directory do Azure que têm permissão para gerenciar o externalConnection e indexar o conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="bf380-111">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bf380-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf380-112">JSON representation</span></span>

<span data-ttu-id="bf380-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf380-113">The following is a JSON representation of the resource.</span></span>

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
