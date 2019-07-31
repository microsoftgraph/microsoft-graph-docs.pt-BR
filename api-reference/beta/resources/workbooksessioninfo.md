---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3b2d52b6389c6fc00eb0bf3b3b6d81774f6f882a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963910"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="13471-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="13471-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13471-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="13471-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="13471-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13471-105">JSON representation</span></span>

<span data-ttu-id="13471-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="13471-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="13471-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13471-107">Properties</span></span>

| <span data-ttu-id="13471-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13471-108">Property</span></span> | <span data-ttu-id="13471-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="13471-109">Type</span></span>  | <span data-ttu-id="13471-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13471-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="13471-111">id</span><span class="sxs-lookup"><span data-stu-id="13471-111">id</span></span>  | <span data-ttu-id="13471-112">string</span><span class="sxs-lookup"><span data-stu-id="13471-112">string</span></span> | <span data-ttu-id="13471-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="13471-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="13471-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="13471-114">persistChanges</span></span> | <span data-ttu-id="13471-115">string</span><span class="sxs-lookup"><span data-stu-id="13471-115">string</span></span> |  <span data-ttu-id="13471-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="13471-116">`true` for persistent session.</span></span> <span data-ttu-id="13471-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="13471-117">`false` for non-persistent session (view mode)</span></span> |

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
