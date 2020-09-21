---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c32f3bc22d2357c0eca88e6f693cd958a6dd5ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013451"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="bb04e-103">tipo de recurso synchronizationError</span><span class="sxs-lookup"><span data-stu-id="bb04e-103">synchronizationError resource type</span></span>

<span data-ttu-id="bb04e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bb04e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb04e-105">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="bb04e-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="bb04e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb04e-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="bb04e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb04e-107">Property</span></span>     | <span data-ttu-id="bb04e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb04e-108">Type</span></span>   |<span data-ttu-id="bb04e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb04e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb04e-110">código</span><span class="sxs-lookup"><span data-stu-id="bb04e-110">code</span></span>|<span data-ttu-id="bb04e-111">String</span><span class="sxs-lookup"><span data-stu-id="bb04e-111">String</span></span>||
|<span data-ttu-id="bb04e-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="bb04e-112">message</span></span>|<span data-ttu-id="bb04e-113">String</span><span class="sxs-lookup"><span data-stu-id="bb04e-113">String</span></span>||
|<span data-ttu-id="bb04e-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="bb04e-114">tenantActionable</span></span>|<span data-ttu-id="bb04e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb04e-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="bb04e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb04e-116">JSON representation</span></span>

<span data-ttu-id="bb04e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb04e-117">The following is a JSON representation of the resource.</span></span>

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


