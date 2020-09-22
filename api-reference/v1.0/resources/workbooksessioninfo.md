---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d5b75d3062b087848f804c0f89726c67783c540
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015103"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="22a89-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="22a89-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="22a89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22a89-105">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="22a89-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22a89-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22a89-106">JSON representation</span></span>

<span data-ttu-id="22a89-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="22a89-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="22a89-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22a89-108">Properties</span></span>

| <span data-ttu-id="22a89-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a89-109">Property</span></span> | <span data-ttu-id="22a89-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a89-110">Type</span></span>  | <span data-ttu-id="22a89-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a89-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="22a89-112">id</span><span class="sxs-lookup"><span data-stu-id="22a89-112">id</span></span>  | <span data-ttu-id="22a89-113">string</span><span class="sxs-lookup"><span data-stu-id="22a89-113">string</span></span> | <span data-ttu-id="22a89-114">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="22a89-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="22a89-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="22a89-115">persistChanges</span></span> | <span data-ttu-id="22a89-116">booliano</span><span class="sxs-lookup"><span data-stu-id="22a89-116">boolean</span></span> |  <span data-ttu-id="22a89-117">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="22a89-117">`true` for persistent session.</span></span> <span data-ttu-id="22a89-118">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="22a89-118">`false` for non-persistent session (view mode)</span></span> |


