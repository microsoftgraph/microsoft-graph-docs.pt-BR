---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860960"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="7a8e6-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="7a8e6-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="7a8e6-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a8e6-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7a8e6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8e6-105">JSON representation</span></span>

<span data-ttu-id="7a8e6-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a8e6-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7a8e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8e6-107">Properties</span></span>

| <span data-ttu-id="7a8e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8e6-108">Property</span></span> | <span data-ttu-id="7a8e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8e6-109">Type</span></span>  | <span data-ttu-id="7a8e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8e6-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="7a8e6-111">id</span><span class="sxs-lookup"><span data-stu-id="7a8e6-111">id</span></span>  | <span data-ttu-id="7a8e6-112">string</span><span class="sxs-lookup"><span data-stu-id="7a8e6-112">string</span></span> | <span data-ttu-id="7a8e6-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a8e6-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="7a8e6-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="7a8e6-114">persistChanges</span></span> | <span data-ttu-id="7a8e6-115">string</span><span class="sxs-lookup"><span data-stu-id="7a8e6-115">string</span></span> |  <span data-ttu-id="7a8e6-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="7a8e6-116">`true` for persistent session.</span></span> <span data-ttu-id="7a8e6-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="7a8e6-117">`false` for non-persistent session (view mode)</span></span> |

