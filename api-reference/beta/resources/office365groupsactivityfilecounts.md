---
title: tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457071"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="fdc3e-103">tipo de recurso office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="fdc3e-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fdc3e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdc3e-104">Properties</span></span>

| <span data-ttu-id="fdc3e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc3e-105">Property</span></span>          | <span data-ttu-id="fdc3e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdc3e-106">Type</span></span>   | <span data-ttu-id="fdc3e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdc3e-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fdc3e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fdc3e-108">reportRefreshDate</span></span> | <span data-ttu-id="fdc3e-109">Data</span><span class="sxs-lookup"><span data-stu-id="fdc3e-109">Date</span></span>   | <span data-ttu-id="fdc3e-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fdc3e-111">total</span><span class="sxs-lookup"><span data-stu-id="fdc3e-111">total</span></span>             | <span data-ttu-id="fdc3e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fdc3e-112">Int64</span></span>  | <span data-ttu-id="fdc3e-113">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="fdc3e-114">active</span><span class="sxs-lookup"><span data-stu-id="fdc3e-114">active</span></span>            | <span data-ttu-id="fdc3e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fdc3e-115">Int64</span></span>  | <span data-ttu-id="fdc3e-116">O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="fdc3e-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="fdc3e-117">reportDate</span></span>        | <span data-ttu-id="fdc3e-118">Data</span><span class="sxs-lookup"><span data-stu-id="fdc3e-118">Date</span></span>   | <span data-ttu-id="fdc3e-119">A data em que um número de arquivos estava ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="fdc3e-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fdc3e-120">reportPeriod</span></span>      | <span data-ttu-id="fdc3e-121">String</span><span class="sxs-lookup"><span data-stu-id="fdc3e-121">String</span></span> | <span data-ttu-id="fdc3e-122">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fdc3e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdc3e-123">JSON representation</span></span>

<span data-ttu-id="fdc3e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdc3e-124">The following is a JSON representation of the resource.</span></span>

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
