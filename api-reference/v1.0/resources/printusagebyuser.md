---
title: Tipo de recurso printUsageByUser
description: Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c478a4f9827de96d4db0da5d8533628bd8468d98
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517011"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="8dc9b-103">Tipo de recurso printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="8dc9b-103">printUsageByUser resource type</span></span>

<span data-ttu-id="8dc9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8dc9b-105">Descreve a atividade de impressão de um usuário durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="8dc9b-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="8dc9b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8dc9b-106">Methods</span></span>
|<span data-ttu-id="8dc9b-107">Método</span><span class="sxs-lookup"><span data-stu-id="8dc9b-107">Method</span></span>|<span data-ttu-id="8dc9b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8dc9b-108">Return type</span></span>|<span data-ttu-id="8dc9b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc9b-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="8dc9b-110">Lista (diariamente)</span><span class="sxs-lookup"><span data-stu-id="8dc9b-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="8dc9b-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="8dc9b-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="8dc9b-112">Obter uma lista de resumos de uso diário de impressão, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="8dc9b-113">Lista (mensal)</span><span class="sxs-lookup"><span data-stu-id="8dc9b-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="8dc9b-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="8dc9b-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="8dc9b-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="8dc9b-116">Get</span><span class="sxs-lookup"><span data-stu-id="8dc9b-116">Get</span></span>](../api/printusagebyuser-get.md) | [<span data-ttu-id="8dc9b-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="8dc9b-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="8dc9b-118">Ler propriedades e relações de um objeto printUsageByUser.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8dc9b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dc9b-119">Properties</span></span>
|<span data-ttu-id="8dc9b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dc9b-120">Property</span></span>|<span data-ttu-id="8dc9b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc9b-121">Type</span></span>|<span data-ttu-id="8dc9b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc9b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc9b-123">id</span><span class="sxs-lookup"><span data-stu-id="8dc9b-123">id</span></span>|<span data-ttu-id="8dc9b-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc9b-124">String</span></span>|<span data-ttu-id="8dc9b-125">A ID deste resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="8dc9b-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8dc9b-126">userPrincipalName</span></span>|<span data-ttu-id="8dc9b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc9b-127">String</span></span>|<span data-ttu-id="8dc9b-128">O UPN do usuário representado por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="8dc9b-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="8dc9b-129">usageDate</span></span>|<span data-ttu-id="8dc9b-130">Data</span><span class="sxs-lookup"><span data-stu-id="8dc9b-130">Date</span></span>|<span data-ttu-id="8dc9b-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="8dc9b-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="8dc9b-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="8dc9b-133">Int64</span><span class="sxs-lookup"><span data-stu-id="8dc9b-133">Int64</span></span>|<span data-ttu-id="8dc9b-134">O número de trabalhos de impressão em preto e branco concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="8dc9b-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="8dc9b-135">completedColorJobCount</span></span>|<span data-ttu-id="8dc9b-136">Int64</span><span class="sxs-lookup"><span data-stu-id="8dc9b-136">Int64</span></span>|<span data-ttu-id="8dc9b-137">O número de trabalhos de impressão de cores concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="8dc9b-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="8dc9b-138">incompleteJobCount</span></span>|<span data-ttu-id="8dc9b-139">Int64</span><span class="sxs-lookup"><span data-stu-id="8dc9b-139">Int64</span></span>|<span data-ttu-id="8dc9b-140">O número de trabalhos de impressão que foram enraizadas em nome do usuário, mas não concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dc9b-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dc9b-141">JSON representation</span></span>
<span data-ttu-id="8dc9b-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dc9b-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

