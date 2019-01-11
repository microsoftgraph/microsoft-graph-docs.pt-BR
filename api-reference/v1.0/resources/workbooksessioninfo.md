---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 900ebdcefbdfa83e7b72b1c926a441f1c497626a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826926"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="bb419-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="bb419-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="bb419-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bb419-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb419-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb419-105">JSON representation</span></span>

<span data-ttu-id="bb419-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bb419-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bb419-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb419-107">Properties</span></span>

| <span data-ttu-id="bb419-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb419-108">Property</span></span> | <span data-ttu-id="bb419-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb419-109">Type</span></span>  | <span data-ttu-id="bb419-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb419-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="bb419-111">id</span><span class="sxs-lookup"><span data-stu-id="bb419-111">id</span></span>  | <span data-ttu-id="bb419-112">string</span><span class="sxs-lookup"><span data-stu-id="bb419-112">string</span></span> | <span data-ttu-id="bb419-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bb419-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="bb419-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="bb419-114">persistChanges</span></span> | <span data-ttu-id="bb419-115">booliano</span><span class="sxs-lookup"><span data-stu-id="bb419-115">boolean</span></span> |  <span data-ttu-id="bb419-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="bb419-116">`true` for persistent session.</span></span> <span data-ttu-id="bb419-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="bb419-117">`false` for non-persistent session (view mode)</span></span> |

