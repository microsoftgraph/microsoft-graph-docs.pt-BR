---
title: tipo de recurso mentionsPreview
description: Representa informações sobre objetos de menção em uma instância de recurso.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 721cd2b82e972f98c36252b6cef9c18623390c93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971599"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="28e36-103">tipo de recurso mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="28e36-103">mentionsPreview resource type</span></span>

<span data-ttu-id="28e36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e36-105">Representa informações sobre objetos de [menção](../resources/mention.md) em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="28e36-105">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="28e36-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e36-106">Properties</span></span>
| <span data-ttu-id="28e36-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e36-107">Property</span></span>     | <span data-ttu-id="28e36-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e36-108">Type</span></span>   |<span data-ttu-id="28e36-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e36-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28e36-110">ismencionado</span><span class="sxs-lookup"><span data-stu-id="28e36-110">isMentioned</span></span> | <span data-ttu-id="28e36-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="28e36-111">Boolean</span></span> | <span data-ttu-id="28e36-112">True se o usuário conectado é mencionado na instância de recurso pai.</span><span class="sxs-lookup"><span data-stu-id="28e36-112">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="28e36-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="28e36-113">Read-only.</span></span> <span data-ttu-id="28e36-114">Oferece suporte a filtro.</span><span class="sxs-lookup"><span data-stu-id="28e36-114">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28e36-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e36-115">JSON representation</span></span>

<span data-ttu-id="28e36-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e36-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


