---
title: Tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: ad2610f5cbd3aae56651a0a5651e4ee4319b3bb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981491"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="6053e-103">Tipo de recurso office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="6053e-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="6053e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6053e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="6053e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6053e-105">Properties</span></span>

| <span data-ttu-id="6053e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6053e-106">Property</span></span>          | <span data-ttu-id="6053e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6053e-107">Type</span></span>   | <span data-ttu-id="6053e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6053e-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6053e-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6053e-109">reportRefreshDate</span></span> | <span data-ttu-id="6053e-110">Data</span><span class="sxs-lookup"><span data-stu-id="6053e-110">Date</span></span>   | <span data-ttu-id="6053e-111">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6053e-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="6053e-112">total</span><span class="sxs-lookup"><span data-stu-id="6053e-112">total</span></span>             | <span data-ttu-id="6053e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6053e-113">Int64</span></span>  | <span data-ttu-id="6053e-114">O número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="6053e-114">The total number of groups.</span></span>              |
| <span data-ttu-id="6053e-115">ativo</span><span class="sxs-lookup"><span data-stu-id="6053e-115">active</span></span>            | <span data-ttu-id="6053e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6053e-116">Int64</span></span>  | <span data-ttu-id="6053e-117">O número de grupos ativos.</span><span class="sxs-lookup"><span data-stu-id="6053e-117">The number of active groups.</span></span> <span data-ttu-id="6053e-118">Um grupo será considerado ativo se ocorrer um dos seguintes: email recebido da caixa de correio do grupo; usuário visualizado, editado, compartilhado ou sincronizado arquivos na biblioteca de documentos do SharePoint; usuário visualizou páginas do SharePoint; usuário postou, leu ou curtiu mensagens em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="6053e-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="6053e-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6053e-119">reportDate</span></span>        | <span data-ttu-id="6053e-120">Data</span><span class="sxs-lookup"><span data-stu-id="6053e-120">Date</span></span>   | <span data-ttu-id="6053e-121">A data em que vários grupos estavam ativos.</span><span class="sxs-lookup"><span data-stu-id="6053e-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="6053e-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6053e-122">reportPeriod</span></span>      | <span data-ttu-id="6053e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6053e-123">String</span></span> | <span data-ttu-id="6053e-124">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="6053e-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6053e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6053e-125">JSON representation</span></span>

<span data-ttu-id="6053e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6053e-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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


