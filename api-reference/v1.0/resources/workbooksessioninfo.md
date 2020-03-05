---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1e9746f27a23b12a3bfdf3168cd271c7f2cbc0d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446689"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="63d0f-103">Tipo de recurso workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="63d0f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="63d0f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="63d0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63d0f-105">Fornece informações sobre a sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="63d0f-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="63d0f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63d0f-106">JSON representation</span></span>

<span data-ttu-id="63d0f-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="63d0f-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="63d0f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63d0f-108">Properties</span></span>

| <span data-ttu-id="63d0f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63d0f-109">Property</span></span> | <span data-ttu-id="63d0f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d0f-110">Type</span></span>  | <span data-ttu-id="63d0f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63d0f-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="63d0f-112">id</span><span class="sxs-lookup"><span data-stu-id="63d0f-112">id</span></span>  | <span data-ttu-id="63d0f-113">string</span><span class="sxs-lookup"><span data-stu-id="63d0f-113">string</span></span> | <span data-ttu-id="63d0f-114">ID da sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="63d0f-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="63d0f-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="63d0f-115">persistChanges</span></span> | <span data-ttu-id="63d0f-116">booliano</span><span class="sxs-lookup"><span data-stu-id="63d0f-116">boolean</span></span> |  <span data-ttu-id="63d0f-117">`true` para sessão persistente.</span><span class="sxs-lookup"><span data-stu-id="63d0f-117">`true` for persistent session.</span></span> <span data-ttu-id="63d0f-118">`false` para sessão não persistente (modo de exibição)</span><span class="sxs-lookup"><span data-stu-id="63d0f-118">`false` for non-persistent session (view mode)</span></span> |

