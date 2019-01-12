---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972555"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="e8031-103">tipo de recurso de office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e8031-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e8031-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8031-104">Properties</span></span>

| <span data-ttu-id="e8031-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8031-105">Property</span></span>          | <span data-ttu-id="e8031-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8031-106">Type</span></span>   | <span data-ttu-id="e8031-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8031-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e8031-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e8031-108">reportRefreshDate</span></span> | <span data-ttu-id="e8031-109">Data</span><span class="sxs-lookup"><span data-stu-id="e8031-109">Date</span></span>   | <span data-ttu-id="e8031-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e8031-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="e8031-111">total</span><span class="sxs-lookup"><span data-stu-id="e8031-111">total</span></span>             | <span data-ttu-id="e8031-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e8031-112">Int64</span></span>  | <span data-ttu-id="e8031-113">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e8031-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="e8031-114">ativo</span><span class="sxs-lookup"><span data-stu-id="e8031-114">active</span></span>            | <span data-ttu-id="e8031-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e8031-115">Int64</span></span>  | <span data-ttu-id="e8031-116">O número de arquivos que foram exibidos, editado, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e8031-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="e8031-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="e8031-117">reportDate</span></span>        | <span data-ttu-id="e8031-118">Data</span><span class="sxs-lookup"><span data-stu-id="e8031-118">Date</span></span>   | <span data-ttu-id="e8031-119">A data em que um número de arquivos foram ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="e8031-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="e8031-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e8031-120">reportPeriod</span></span>      | <span data-ttu-id="e8031-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8031-121">String</span></span> | <span data-ttu-id="e8031-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="e8031-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e8031-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8031-123">JSON representation</span></span>

<span data-ttu-id="e8031-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8031-124">The following is a JSON representation of the resource.</span></span>

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
