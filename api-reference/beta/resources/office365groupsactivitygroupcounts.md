---
title: tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 3f49ddaf6f62367c5e8ebbffae669bf3cc1d86f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009479"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="38780-103">tipo de recurso office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="38780-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="38780-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38780-104">Properties</span></span>

| <span data-ttu-id="38780-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38780-105">Property</span></span>          | <span data-ttu-id="38780-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="38780-106">Type</span></span>   | <span data-ttu-id="38780-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="38780-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="38780-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="38780-108">reportRefreshDate</span></span> | <span data-ttu-id="38780-109">Data</span><span class="sxs-lookup"><span data-stu-id="38780-109">Date</span></span>   | <span data-ttu-id="38780-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="38780-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="38780-111">total</span><span class="sxs-lookup"><span data-stu-id="38780-111">total</span></span>             | <span data-ttu-id="38780-112">Int64</span><span class="sxs-lookup"><span data-stu-id="38780-112">Int64</span></span>  | <span data-ttu-id="38780-113">O número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="38780-113">The total number of groups.</span></span>              |
| <span data-ttu-id="38780-114">active</span><span class="sxs-lookup"><span data-stu-id="38780-114">active</span></span>            | <span data-ttu-id="38780-115">Int64</span><span class="sxs-lookup"><span data-stu-id="38780-115">Int64</span></span>  | <span data-ttu-id="38780-116">O número de grupos ativos.</span><span class="sxs-lookup"><span data-stu-id="38780-116">The number of active groups.</span></span> <span data-ttu-id="38780-117">Um grupo é considerado ativo se qualquer um dos seguintes ocorrerem: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="38780-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="38780-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="38780-118">reportDate</span></span>        | <span data-ttu-id="38780-119">Data</span><span class="sxs-lookup"><span data-stu-id="38780-119">Date</span></span>   | <span data-ttu-id="38780-120">A data em que um número de grupos estava ativo.</span><span class="sxs-lookup"><span data-stu-id="38780-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="38780-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="38780-121">reportPeriod</span></span>      | <span data-ttu-id="38780-122">String</span><span class="sxs-lookup"><span data-stu-id="38780-122">String</span></span> | <span data-ttu-id="38780-123">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="38780-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="38780-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38780-124">JSON representation</span></span>

<span data-ttu-id="38780-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38780-125">The following is a JSON representation of the resource.</span></span>

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
