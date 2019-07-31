---
title: tipo de recurso mentionsPreview
description: Representa informações sobre objetos de menção em uma instância de recurso.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c4604657e18498a85aa8646b5d69db7d74299bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009699"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="4f84d-103">tipo de recurso mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="4f84d-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f84d-104">Representa informações sobre objetos de [menção](../resources/mention.md) em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="4f84d-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="4f84d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f84d-105">Properties</span></span>
| <span data-ttu-id="4f84d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f84d-106">Property</span></span>     | <span data-ttu-id="4f84d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f84d-107">Type</span></span>   |<span data-ttu-id="4f84d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f84d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f84d-109">ismencionado</span><span class="sxs-lookup"><span data-stu-id="4f84d-109">isMentioned</span></span> | <span data-ttu-id="4f84d-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="4f84d-110">Boolean</span></span> | <span data-ttu-id="4f84d-111">True se o usuário conectado é mencionado na instância de recurso pai.</span><span class="sxs-lookup"><span data-stu-id="4f84d-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="4f84d-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f84d-112">Read-only.</span></span> <span data-ttu-id="4f84d-113">Oferece suporte a filtro.</span><span class="sxs-lookup"><span data-stu-id="4f84d-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f84d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f84d-114">JSON representation</span></span>

<span data-ttu-id="4f84d-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f84d-115">Here is a JSON representation of the resource.</span></span>

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
