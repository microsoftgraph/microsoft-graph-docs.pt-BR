---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
ms.openlocfilehash: 7f678cdbd48a3d5f013c22120d01c28bb61738e6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324696"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="e8fca-103">tipo de recurso synchronizationError</span><span class="sxs-lookup"><span data-stu-id="e8fca-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fca-104">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e8fca-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="e8fca-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8fca-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="e8fca-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8fca-106">Property</span></span>     | <span data-ttu-id="e8fca-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8fca-107">Type</span></span>   |<span data-ttu-id="e8fca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8fca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8fca-109">código</span><span class="sxs-lookup"><span data-stu-id="e8fca-109">code</span></span>|<span data-ttu-id="e8fca-110">String</span><span class="sxs-lookup"><span data-stu-id="e8fca-110">String</span></span>||
|<span data-ttu-id="e8fca-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="e8fca-111">message</span></span>|<span data-ttu-id="e8fca-112">String</span><span class="sxs-lookup"><span data-stu-id="e8fca-112">String</span></span>||
|<span data-ttu-id="e8fca-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="e8fca-113">tenantActionable</span></span>|<span data-ttu-id="e8fca-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8fca-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="e8fca-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8fca-115">JSON representation</span></span>

<span data-ttu-id="e8fca-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8fca-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
