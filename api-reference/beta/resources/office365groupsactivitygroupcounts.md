---
title: tipo de recurso de office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d3c1272f9bd99c3e7ee0f29a4c303e1c8ca95525
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975880"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="a00b2-103">tipo de recurso de office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="a00b2-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a00b2-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a00b2-104">Properties</span></span>

| <span data-ttu-id="a00b2-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00b2-105">Property</span></span>          | <span data-ttu-id="a00b2-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00b2-106">Type</span></span>   | <span data-ttu-id="a00b2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00b2-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a00b2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a00b2-108">reportRefreshDate</span></span> | <span data-ttu-id="a00b2-109">Data</span><span class="sxs-lookup"><span data-stu-id="a00b2-109">Date</span></span>   | <span data-ttu-id="a00b2-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a00b2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="a00b2-111">total</span><span class="sxs-lookup"><span data-stu-id="a00b2-111">total</span></span>             | <span data-ttu-id="a00b2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a00b2-112">Int64</span></span>  | <span data-ttu-id="a00b2-113">O número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="a00b2-113">The total number of groups.</span></span>              |
| <span data-ttu-id="a00b2-114">ativo</span><span class="sxs-lookup"><span data-stu-id="a00b2-114">active</span></span>            | <span data-ttu-id="a00b2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a00b2-115">Int64</span></span>  | <span data-ttu-id="a00b2-116">O número de grupos do active.</span><span class="sxs-lookup"><span data-stu-id="a00b2-116">The number of active groups.</span></span> <span data-ttu-id="a00b2-117">Um grupo será considerado ativo se qualquer um dos seguintes ocorreu: email da caixa de correio recebida; de grupo usuário exibido, editado, compartilhados ou sincronizados arquivos na biblioteca de documentos do SharePoint; usuário exibir páginas do SharePoint; usuário postados, ler ou curtidas mensagens no Yammer grupos.</span><span class="sxs-lookup"><span data-stu-id="a00b2-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="a00b2-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="a00b2-118">reportDate</span></span>        | <span data-ttu-id="a00b2-119">Data</span><span class="sxs-lookup"><span data-stu-id="a00b2-119">Date</span></span>   | <span data-ttu-id="a00b2-120">A data em que um número de grupos estava ativo.</span><span class="sxs-lookup"><span data-stu-id="a00b2-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="a00b2-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a00b2-121">reportPeriod</span></span>      | <span data-ttu-id="a00b2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a00b2-122">String</span></span> | <span data-ttu-id="a00b2-123">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="a00b2-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a00b2-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a00b2-124">JSON representation</span></span>

<span data-ttu-id="a00b2-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a00b2-125">The following is a JSON representation of the resource.</span></span>

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
