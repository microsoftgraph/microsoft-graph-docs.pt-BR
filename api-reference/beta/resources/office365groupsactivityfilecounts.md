---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034332"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="64750-103">tipo de recurso de office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="64750-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="64750-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64750-104">Properties</span></span>

| <span data-ttu-id="64750-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64750-105">Property</span></span>          | <span data-ttu-id="64750-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="64750-106">Type</span></span>   | <span data-ttu-id="64750-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="64750-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="64750-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="64750-108">reportRefreshDate</span></span> | <span data-ttu-id="64750-109">Data</span><span class="sxs-lookup"><span data-stu-id="64750-109">Date</span></span>   | <span data-ttu-id="64750-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="64750-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="64750-111">total</span><span class="sxs-lookup"><span data-stu-id="64750-111">total</span></span>             | <span data-ttu-id="64750-112">Int64</span><span class="sxs-lookup"><span data-stu-id="64750-112">Int64</span></span>  | <span data-ttu-id="64750-113">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="64750-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="64750-114">ativo</span><span class="sxs-lookup"><span data-stu-id="64750-114">active</span></span>            | <span data-ttu-id="64750-115">Int64</span><span class="sxs-lookup"><span data-stu-id="64750-115">Int64</span></span>  | <span data-ttu-id="64750-116">O número de arquivos que foram exibidos, editado, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="64750-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="64750-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="64750-117">reportDate</span></span>        | <span data-ttu-id="64750-118">Data</span><span class="sxs-lookup"><span data-stu-id="64750-118">Date</span></span>   | <span data-ttu-id="64750-119">A data em que um número de arquivos foram ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="64750-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="64750-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="64750-120">reportPeriod</span></span>      | <span data-ttu-id="64750-121">String</span><span class="sxs-lookup"><span data-stu-id="64750-121">String</span></span> | <span data-ttu-id="64750-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="64750-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="64750-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64750-123">JSON representation</span></span>

<span data-ttu-id="64750-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64750-124">The following is a JSON representation of the resource.</span></span>

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
