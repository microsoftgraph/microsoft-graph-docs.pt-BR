---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962447"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="aedf0-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="aedf0-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="aedf0-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="aedf0-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="aedf0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aedf0-105">JSON representation</span></span>

<span data-ttu-id="aedf0-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="aedf0-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="aedf0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aedf0-107">Properties</span></span>

| <span data-ttu-id="aedf0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aedf0-108">Property</span></span> | <span data-ttu-id="aedf0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="aedf0-109">Type</span></span>  | <span data-ttu-id="aedf0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aedf0-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="aedf0-111">id</span><span class="sxs-lookup"><span data-stu-id="aedf0-111">id</span></span>  | <span data-ttu-id="aedf0-112">string</span><span class="sxs-lookup"><span data-stu-id="aedf0-112">string</span></span> | <span data-ttu-id="aedf0-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="aedf0-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="aedf0-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="aedf0-114">persistChanges</span></span> | <span data-ttu-id="aedf0-115">string</span><span class="sxs-lookup"><span data-stu-id="aedf0-115">string</span></span> |  <span data-ttu-id="aedf0-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="aedf0-116">`true` for persistent session.</span></span> <span data-ttu-id="aedf0-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="aedf0-117">`false` for non-persistent session (view mode)</span></span> |

