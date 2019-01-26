---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575615"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="6ec57-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="6ec57-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="6ec57-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ec57-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6ec57-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ec57-105">JSON representation</span></span>

<span data-ttu-id="6ec57-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6ec57-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="6ec57-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ec57-107">Properties</span></span>

| <span data-ttu-id="6ec57-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ec57-108">Property</span></span> | <span data-ttu-id="6ec57-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ec57-109">Type</span></span>  | <span data-ttu-id="6ec57-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ec57-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="6ec57-111">id</span><span class="sxs-lookup"><span data-stu-id="6ec57-111">id</span></span>  | <span data-ttu-id="6ec57-112">string</span><span class="sxs-lookup"><span data-stu-id="6ec57-112">string</span></span> | <span data-ttu-id="6ec57-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ec57-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="6ec57-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="6ec57-114">persistChanges</span></span> | <span data-ttu-id="6ec57-115">booliano</span><span class="sxs-lookup"><span data-stu-id="6ec57-115">boolean</span></span> |  <span data-ttu-id="6ec57-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="6ec57-116">`true` for persistent session.</span></span> <span data-ttu-id="6ec57-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="6ec57-117">`false` for non-persistent session (view mode)</span></span> |

