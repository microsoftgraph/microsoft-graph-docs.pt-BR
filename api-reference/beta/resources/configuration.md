---
title: tipo de recurso de configuração
description: Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a82c5e9e4cbd915d5a7e11b9e162bc510628ecf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366771"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="e0f28-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="e0f28-103">configuration resource type</span></span>

<span data-ttu-id="e0f28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0f28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0f28-105">Especifica IDs de aplicativo adicionais que podem gerenciar o externalConnection e indexar conteúdo em [um externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="e0f28-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e0f28-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0f28-106">Properties</span></span>

| <span data-ttu-id="e0f28-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0f28-107">Property</span></span>       | <span data-ttu-id="e0f28-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0f28-108">Type</span></span>              | <span data-ttu-id="e0f28-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0f28-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="e0f28-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="e0f28-110">authorizedApps</span></span> | <span data-ttu-id="e0f28-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0f28-111">String collection</span></span> | <span data-ttu-id="e0f28-112">Uma coleção de IDs de aplicativos para aplicativos Azure Active Directory registrados que podem gerenciar o externalConnection e indexar conteúdo no externalConnection.</span><span class="sxs-lookup"><span data-stu-id="e0f28-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e0f28-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0f28-113">JSON representation</span></span>

<span data-ttu-id="e0f28-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0f28-114">The following is a JSON representation of the resource.</span></span>

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


