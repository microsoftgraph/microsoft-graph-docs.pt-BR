---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819180"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="d70e0-103">tipo de recurso de office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d70e0-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d70e0-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d70e0-104">Properties</span></span>

| <span data-ttu-id="d70e0-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d70e0-105">Property</span></span>          | <span data-ttu-id="d70e0-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d70e0-106">Type</span></span>   | <span data-ttu-id="d70e0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d70e0-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d70e0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d70e0-108">reportRefreshDate</span></span> | <span data-ttu-id="d70e0-109">Data</span><span class="sxs-lookup"><span data-stu-id="d70e0-109">Date</span></span>   | <span data-ttu-id="d70e0-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d70e0-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d70e0-111">total</span><span class="sxs-lookup"><span data-stu-id="d70e0-111">total</span></span>             | <span data-ttu-id="d70e0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d70e0-112">Int64</span></span>  | <span data-ttu-id="d70e0-113">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="d70e0-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d70e0-114">ativo</span><span class="sxs-lookup"><span data-stu-id="d70e0-114">active</span></span>            | <span data-ttu-id="d70e0-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d70e0-115">Int64</span></span>  | <span data-ttu-id="d70e0-116">O número de arquivos que foram exibidos, editado, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="d70e0-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d70e0-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="d70e0-117">reportDate</span></span>        | <span data-ttu-id="d70e0-118">Data</span><span class="sxs-lookup"><span data-stu-id="d70e0-118">Date</span></span>   | <span data-ttu-id="d70e0-119">A data em que um número de arquivos foram ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="d70e0-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="d70e0-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d70e0-120">reportPeriod</span></span>      | <span data-ttu-id="d70e0-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70e0-121">String</span></span> | <span data-ttu-id="d70e0-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="d70e0-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d70e0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d70e0-123">JSON representation</span></span>

<span data-ttu-id="d70e0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d70e0-124">The following is a JSON representation of the resource.</span></span>

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
