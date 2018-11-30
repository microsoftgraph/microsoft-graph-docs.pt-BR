---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036492"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="52f59-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="52f59-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="52f59-104">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="52f59-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="52f59-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52f59-105">JSON representation</span></span>

<span data-ttu-id="52f59-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="52f59-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="52f59-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52f59-107">Properties</span></span>

| <span data-ttu-id="52f59-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52f59-108">Property</span></span> | <span data-ttu-id="52f59-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="52f59-109">Type</span></span>  | <span data-ttu-id="52f59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f59-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="52f59-111">id</span><span class="sxs-lookup"><span data-stu-id="52f59-111">id</span></span>  | <span data-ttu-id="52f59-112">string</span><span class="sxs-lookup"><span data-stu-id="52f59-112">string</span></span> | <span data-ttu-id="52f59-113">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="52f59-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="52f59-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="52f59-114">persistChanges</span></span> | <span data-ttu-id="52f59-115">string</span><span class="sxs-lookup"><span data-stu-id="52f59-115">string</span></span> |  <span data-ttu-id="52f59-116">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="52f59-116">`true` for persistent session.</span></span> <span data-ttu-id="52f59-117">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="52f59-117">`false` for non-persistent session (view mode)</span></span> |

