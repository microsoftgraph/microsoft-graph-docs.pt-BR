---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3035574b92dfa703b926a81163efbb7f6eff764b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345770"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="3036d-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="3036d-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3036d-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3036d-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3036d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3036d-105">JSON representation</span></span>

<span data-ttu-id="3036d-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3036d-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="3036d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3036d-107">Properties</span></span>

| <span data-ttu-id="3036d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3036d-108">Property</span></span> | <span data-ttu-id="3036d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3036d-109">Type</span></span>  | <span data-ttu-id="3036d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3036d-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="3036d-111">id</span><span class="sxs-lookup"><span data-stu-id="3036d-111">id</span></span>  | <span data-ttu-id="3036d-112">string</span><span class="sxs-lookup"><span data-stu-id="3036d-112">string</span></span> | <span data-ttu-id="3036d-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3036d-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="3036d-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="3036d-114">persistChanges</span></span> | <span data-ttu-id="3036d-115">string</span><span class="sxs-lookup"><span data-stu-id="3036d-115">string</span></span> |  <span data-ttu-id="3036d-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="3036d-116">`true` for persistent session.</span></span> <span data-ttu-id="3036d-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="3036d-117">`false` for non-persistent session (view mode)</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
