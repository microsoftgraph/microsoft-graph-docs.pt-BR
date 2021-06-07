---
title: Tipo de recurso printUsageByUser
description: Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b4809f77e7ceeba79ea5b7e75737fb0750cc4dc
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781213"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="65cb7-103">Tipo de recurso printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="65cb7-103">printUsageByUser resource type</span></span>

<span data-ttu-id="65cb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65cb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65cb7-105">Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="65cb7-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="65cb7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="65cb7-106">Methods</span></span>

| <span data-ttu-id="65cb7-107">Método</span><span class="sxs-lookup"><span data-stu-id="65cb7-107">Method</span></span>       | <span data-ttu-id="65cb7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65cb7-108">Return Type</span></span> | <span data-ttu-id="65cb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="65cb7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="65cb7-110">Lista (diariamente)</span><span class="sxs-lookup"><span data-stu-id="65cb7-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="65cb7-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="65cb7-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="65cb7-112">Obter uma lista de resumos de uso diário de impressão, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="65cb7-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="65cb7-113">Lista (mensal)</span><span class="sxs-lookup"><span data-stu-id="65cb7-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="65cb7-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="65cb7-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="65cb7-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="65cb7-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="65cb7-116">Get</span><span class="sxs-lookup"><span data-stu-id="65cb7-116">Get</span></span>](../api/printusagebyuser-get.md) | [<span data-ttu-id="65cb7-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="65cb7-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="65cb7-118">Ler propriedades e relações de um objeto printUsageByUser.</span><span class="sxs-lookup"><span data-stu-id="65cb7-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="65cb7-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65cb7-119">Properties</span></span>
| <span data-ttu-id="65cb7-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65cb7-120">Property</span></span>     | <span data-ttu-id="65cb7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="65cb7-121">Type</span></span>        | <span data-ttu-id="65cb7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="65cb7-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65cb7-123">id</span><span class="sxs-lookup"><span data-stu-id="65cb7-123">id</span></span>|<span data-ttu-id="65cb7-124">String</span><span class="sxs-lookup"><span data-stu-id="65cb7-124">String</span></span>|<span data-ttu-id="65cb7-125">A ID deste resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="65cb7-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="65cb7-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65cb7-126">userPrincipalName</span></span>|<span data-ttu-id="65cb7-127">String</span><span class="sxs-lookup"><span data-stu-id="65cb7-127">String</span></span>|<span data-ttu-id="65cb7-128">O UPN do usuário representado por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="65cb7-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="65cb7-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="65cb7-129">usageDate</span></span>|<span data-ttu-id="65cb7-130">Data</span><span class="sxs-lookup"><span data-stu-id="65cb7-130">Date</span></span>|<span data-ttu-id="65cb7-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="65cb7-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="65cb7-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="65cb7-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="65cb7-133">Int64</span><span class="sxs-lookup"><span data-stu-id="65cb7-133">Int64</span></span>|<span data-ttu-id="65cb7-134">O número de trabalhos de impressão em preto e branco concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="65cb7-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="65cb7-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="65cb7-135">completedColorJobCount</span></span>|<span data-ttu-id="65cb7-136">Int64</span><span class="sxs-lookup"><span data-stu-id="65cb7-136">Int64</span></span>|<span data-ttu-id="65cb7-137">O número de trabalhos de impressão de cores concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="65cb7-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="65cb7-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="65cb7-138">incompleteJobCount</span></span>|<span data-ttu-id="65cb7-139">Int64</span><span class="sxs-lookup"><span data-stu-id="65cb7-139">Int64</span></span>|<span data-ttu-id="65cb7-140">O número de trabalhos de impressão que foram enraizadas em nome do usuário, mas não concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="65cb7-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65cb7-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65cb7-141">JSON representation</span></span>

<span data-ttu-id="65cb7-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65cb7-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

