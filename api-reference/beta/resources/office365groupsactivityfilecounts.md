---
title: tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c887ecb526d9c4215c1d8586bcbcb799c9e2c476
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092402"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="80b4b-103">tipo de recurso office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="80b4b-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="80b4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80b4b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="80b4b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80b4b-105">Properties</span></span>

| <span data-ttu-id="80b4b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80b4b-106">Property</span></span>          | <span data-ttu-id="80b4b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="80b4b-107">Type</span></span>   | <span data-ttu-id="80b4b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="80b4b-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="80b4b-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80b4b-109">reportRefreshDate</span></span> | <span data-ttu-id="80b4b-110">Data</span><span class="sxs-lookup"><span data-stu-id="80b4b-110">Date</span></span>   | <span data-ttu-id="80b4b-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="80b4b-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="80b4b-112">total</span><span class="sxs-lookup"><span data-stu-id="80b4b-112">total</span></span>             | <span data-ttu-id="80b4b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="80b4b-113">Int64</span></span>  | <span data-ttu-id="80b4b-114">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="80b4b-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="80b4b-115">active</span><span class="sxs-lookup"><span data-stu-id="80b4b-115">active</span></span>            | <span data-ttu-id="80b4b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="80b4b-116">Int64</span></span>  | <span data-ttu-id="80b4b-117">O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="80b4b-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="80b4b-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="80b4b-118">reportDate</span></span>        | <span data-ttu-id="80b4b-119">Data</span><span class="sxs-lookup"><span data-stu-id="80b4b-119">Date</span></span>   | <span data-ttu-id="80b4b-120">A data em que um número de arquivos estava ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="80b4b-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="80b4b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80b4b-121">reportPeriod</span></span>      | <span data-ttu-id="80b4b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80b4b-122">String</span></span> | <span data-ttu-id="80b4b-123">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="80b4b-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="80b4b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80b4b-124">JSON representation</span></span>

<span data-ttu-id="80b4b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80b4b-125">The following is a JSON representation of the resource.</span></span>

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


