---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3856a8ae5d73eefaa1c7700f16bc5fd9c2f46bda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046164"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="37484-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="37484-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="37484-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37484-105">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="37484-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="37484-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37484-106">JSON representation</span></span>

<span data-ttu-id="37484-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="37484-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="37484-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37484-108">Properties</span></span>

| <span data-ttu-id="37484-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37484-109">Property</span></span> | <span data-ttu-id="37484-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37484-110">Type</span></span>  | <span data-ttu-id="37484-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37484-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="37484-112">id</span><span class="sxs-lookup"><span data-stu-id="37484-112">id</span></span>  | <span data-ttu-id="37484-113">string</span><span class="sxs-lookup"><span data-stu-id="37484-113">string</span></span> | <span data-ttu-id="37484-114">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="37484-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="37484-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="37484-115">persistChanges</span></span> | <span data-ttu-id="37484-116">string</span><span class="sxs-lookup"><span data-stu-id="37484-116">string</span></span> |  <span data-ttu-id="37484-117">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="37484-117">`true` for persistent session.</span></span> <span data-ttu-id="37484-118">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="37484-118">`false` for non-persistent session (view mode)</span></span> |

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


