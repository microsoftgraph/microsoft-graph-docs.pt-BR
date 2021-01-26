---
title: Tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1f4f26e141dc25e1e5e249ad116bc9a988274f18
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981498"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="e4880-103">Tipo de recurso office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e4880-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="e4880-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4880-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e4880-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4880-105">Properties</span></span>

| <span data-ttu-id="e4880-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4880-106">Property</span></span>          | <span data-ttu-id="e4880-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4880-107">Type</span></span>   | <span data-ttu-id="e4880-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4880-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e4880-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e4880-109">reportRefreshDate</span></span> | <span data-ttu-id="e4880-110">Data</span><span class="sxs-lookup"><span data-stu-id="e4880-110">Date</span></span>   | <span data-ttu-id="e4880-111">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e4880-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="e4880-112">total</span><span class="sxs-lookup"><span data-stu-id="e4880-112">total</span></span>             | <span data-ttu-id="e4880-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e4880-113">Int64</span></span>  | <span data-ttu-id="e4880-114">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e4880-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="e4880-115">ativo</span><span class="sxs-lookup"><span data-stu-id="e4880-115">active</span></span>            | <span data-ttu-id="e4880-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e4880-116">Int64</span></span>  | <span data-ttu-id="e4880-117">O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e4880-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="e4880-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="e4880-118">reportDate</span></span>        | <span data-ttu-id="e4880-119">Data</span><span class="sxs-lookup"><span data-stu-id="e4880-119">Date</span></span>   | <span data-ttu-id="e4880-120">A data em que vários arquivos estavam ativos no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e4880-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="e4880-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e4880-121">reportPeriod</span></span>      | <span data-ttu-id="e4880-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4880-122">String</span></span> | <span data-ttu-id="e4880-123">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="e4880-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e4880-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4880-124">JSON representation</span></span>

<span data-ttu-id="e4880-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4880-125">The following is a JSON representation of the resource.</span></span>

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


