---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
ms.openlocfilehash: 1e097cad70a6058aab28ad85d7cf6b3c3b52ac75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305982"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="a0b69-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="a0b69-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="a0b69-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a0b69-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a0b69-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0b69-105">JSON representation</span></span>

<span data-ttu-id="a0b69-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a0b69-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a0b69-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0b69-107">Properties</span></span>

| <span data-ttu-id="a0b69-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0b69-108">Property</span></span> | <span data-ttu-id="a0b69-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0b69-109">Type</span></span>  | <span data-ttu-id="a0b69-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0b69-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="a0b69-111">id</span><span class="sxs-lookup"><span data-stu-id="a0b69-111">id</span></span>  | <span data-ttu-id="a0b69-112">string</span><span class="sxs-lookup"><span data-stu-id="a0b69-112">string</span></span> | <span data-ttu-id="a0b69-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a0b69-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="a0b69-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="a0b69-114">persistChanges</span></span> | <span data-ttu-id="a0b69-115">booliano</span><span class="sxs-lookup"><span data-stu-id="a0b69-115">boolean</span></span> |  <span data-ttu-id="a0b69-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="a0b69-116">`true` for persistent session.</span></span> <span data-ttu-id="a0b69-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="a0b69-117">`false` for non-persistent session (view mode)</span></span> |

