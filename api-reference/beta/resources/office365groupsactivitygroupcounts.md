---
title: tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c249123a01cde2fe952f5111affe645415ddc6cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092381"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="f1b34-103">tipo de recurso office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="f1b34-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="f1b34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b34-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f1b34-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1b34-105">Properties</span></span>

| <span data-ttu-id="f1b34-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1b34-106">Property</span></span>          | <span data-ttu-id="f1b34-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b34-107">Type</span></span>   | <span data-ttu-id="f1b34-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b34-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f1b34-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f1b34-109">reportRefreshDate</span></span> | <span data-ttu-id="f1b34-110">Data</span><span class="sxs-lookup"><span data-stu-id="f1b34-110">Date</span></span>   | <span data-ttu-id="f1b34-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f1b34-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="f1b34-112">total</span><span class="sxs-lookup"><span data-stu-id="f1b34-112">total</span></span>             | <span data-ttu-id="f1b34-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b34-113">Int64</span></span>  | <span data-ttu-id="f1b34-114">O número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="f1b34-114">The total number of groups.</span></span>              |
| <span data-ttu-id="f1b34-115">active</span><span class="sxs-lookup"><span data-stu-id="f1b34-115">active</span></span>            | <span data-ttu-id="f1b34-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b34-116">Int64</span></span>  | <span data-ttu-id="f1b34-117">O número de grupos ativos.</span><span class="sxs-lookup"><span data-stu-id="f1b34-117">The number of active groups.</span></span> <span data-ttu-id="f1b34-118">Um grupo é considerado ativo se qualquer um dos seguintes ocorrerem: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="f1b34-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="f1b34-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="f1b34-119">reportDate</span></span>        | <span data-ttu-id="f1b34-120">Data</span><span class="sxs-lookup"><span data-stu-id="f1b34-120">Date</span></span>   | <span data-ttu-id="f1b34-121">A data em que um número de grupos estava ativo.</span><span class="sxs-lookup"><span data-stu-id="f1b34-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="f1b34-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f1b34-122">reportPeriod</span></span>      | <span data-ttu-id="f1b34-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b34-123">String</span></span> | <span data-ttu-id="f1b34-124">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="f1b34-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f1b34-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1b34-125">JSON representation</span></span>

<span data-ttu-id="f1b34-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1b34-126">The following is a JSON representation of the resource.</span></span>

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


