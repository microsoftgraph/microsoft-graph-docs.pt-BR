---
title: tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dff3266aa268f2d26ca15492c72fa25a5f562a29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522439"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="8e6b8-103">tipo de recurso office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="8e6b8-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="8e6b8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8e6b8-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8e6b8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e6b8-105">Properties</span></span>

| <span data-ttu-id="8e6b8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e6b8-106">Property</span></span>          | <span data-ttu-id="8e6b8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6b8-107">Type</span></span>   | <span data-ttu-id="8e6b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6b8-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="8e6b8-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8e6b8-109">reportRefreshDate</span></span> | <span data-ttu-id="8e6b8-110">Data</span><span class="sxs-lookup"><span data-stu-id="8e6b8-110">Date</span></span>   | <span data-ttu-id="8e6b8-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="8e6b8-112">total</span><span class="sxs-lookup"><span data-stu-id="8e6b8-112">total</span></span>             | <span data-ttu-id="8e6b8-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8e6b8-113">Int64</span></span>  | <span data-ttu-id="8e6b8-114">O número total de arquivos na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="8e6b8-115">active</span><span class="sxs-lookup"><span data-stu-id="8e6b8-115">active</span></span>            | <span data-ttu-id="8e6b8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8e6b8-116">Int64</span></span>  | <span data-ttu-id="8e6b8-117">O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="8e6b8-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="8e6b8-118">reportDate</span></span>        | <span data-ttu-id="8e6b8-119">Data</span><span class="sxs-lookup"><span data-stu-id="8e6b8-119">Date</span></span>   | <span data-ttu-id="8e6b8-120">A data em que um número de arquivos estava ativo no site do SharePoint do grupo.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="8e6b8-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8e6b8-121">reportPeriod</span></span>      | <span data-ttu-id="8e6b8-122">String</span><span class="sxs-lookup"><span data-stu-id="8e6b8-122">String</span></span> | <span data-ttu-id="8e6b8-123">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8e6b8-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e6b8-124">JSON representation</span></span>

<span data-ttu-id="8e6b8-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6b8-125">The following is a JSON representation of the resource.</span></span>

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
