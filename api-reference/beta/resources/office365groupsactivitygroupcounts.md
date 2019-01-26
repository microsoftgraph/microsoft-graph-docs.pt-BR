---
title: tipo de recurso de office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572483"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="fb4ec-103">tipo de recurso de office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="fb4ec-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fb4ec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb4ec-104">Properties</span></span>

| <span data-ttu-id="fb4ec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb4ec-105">Property</span></span>          | <span data-ttu-id="fb4ec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb4ec-106">Type</span></span>   | <span data-ttu-id="fb4ec-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb4ec-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fb4ec-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fb4ec-108">reportRefreshDate</span></span> | <span data-ttu-id="fb4ec-109">Data</span><span class="sxs-lookup"><span data-stu-id="fb4ec-109">Date</span></span>   | <span data-ttu-id="fb4ec-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fb4ec-111">total</span><span class="sxs-lookup"><span data-stu-id="fb4ec-111">total</span></span>             | <span data-ttu-id="fb4ec-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fb4ec-112">Int64</span></span>  | <span data-ttu-id="fb4ec-113">O número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-113">The total number of groups.</span></span>              |
| <span data-ttu-id="fb4ec-114">ativo</span><span class="sxs-lookup"><span data-stu-id="fb4ec-114">active</span></span>            | <span data-ttu-id="fb4ec-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fb4ec-115">Int64</span></span>  | <span data-ttu-id="fb4ec-116">O número de grupos do active.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-116">The number of active groups.</span></span> <span data-ttu-id="fb4ec-117">Um grupo será considerado ativo se qualquer um dos seguintes ocorreu: email da caixa de correio recebida; de grupo usuário exibido, editado, compartilhados ou sincronizados arquivos na biblioteca de documentos do SharePoint; usuário exibir páginas do SharePoint; usuário postados, ler ou curtidas mensagens no Yammer grupos.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="fb4ec-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="fb4ec-118">reportDate</span></span>        | <span data-ttu-id="fb4ec-119">Data</span><span class="sxs-lookup"><span data-stu-id="fb4ec-119">Date</span></span>   | <span data-ttu-id="fb4ec-120">A data em que um número de grupos estava ativo.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="fb4ec-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fb4ec-121">reportPeriod</span></span>      | <span data-ttu-id="fb4ec-122">String</span><span class="sxs-lookup"><span data-stu-id="fb4ec-122">String</span></span> | <span data-ttu-id="fb4ec-123">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fb4ec-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb4ec-124">JSON representation</span></span>

<span data-ttu-id="fb4ec-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb4ec-125">The following is a JSON representation of the resource.</span></span>

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
