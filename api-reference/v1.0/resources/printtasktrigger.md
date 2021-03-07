---
title: Tipo de recurso printTaskTrigger
description: Determina as condições em que um novo printTask será executado com base na printTaskDefinition associada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c0871f936b0935e6a599e79d6fb1a75f7e28f7ed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517013"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="0d492-103">Tipo de recurso printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="0d492-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="0d492-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d492-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0d492-105">Determina a condição na qual um [novo printTask](printtask.md) será acionado com base na [impressão associadaTaskDefinition](printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0d492-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="0d492-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="0d492-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="0d492-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0d492-107">Methods</span></span>
|<span data-ttu-id="0d492-108">Método</span><span class="sxs-lookup"><span data-stu-id="0d492-108">Method</span></span>|<span data-ttu-id="0d492-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0d492-109">Return type</span></span>|<span data-ttu-id="0d492-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d492-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="0d492-111">List</span><span class="sxs-lookup"><span data-stu-id="0d492-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="0d492-112">[Coleção printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="0d492-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="0d492-113">Obter uma lista de printTaskTriggers associados a uma impressora [específica.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="0d492-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="0d492-114">Get</span><span class="sxs-lookup"><span data-stu-id="0d492-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="0d492-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="0d492-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="0d492-116">Obter o printTaskTrigger associado a um [printTask específico.](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="0d492-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="0d492-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d492-117">Properties</span></span>
|<span data-ttu-id="0d492-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d492-118">Property</span></span>|<span data-ttu-id="0d492-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d492-119">Type</span></span>|<span data-ttu-id="0d492-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d492-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d492-121">id</span><span class="sxs-lookup"><span data-stu-id="0d492-121">id</span></span>|<span data-ttu-id="0d492-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d492-122">String</span></span>|<span data-ttu-id="0d492-123">O identificador printTaskTrigger.</span><span class="sxs-lookup"><span data-stu-id="0d492-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="0d492-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d492-124">Read-only.</span></span>|
|<span data-ttu-id="0d492-125">event</span><span class="sxs-lookup"><span data-stu-id="0d492-125">event</span></span>|<span data-ttu-id="0d492-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="0d492-126">printEvent</span></span>|<span data-ttu-id="0d492-127">O evento Impressão Universal que fará com que um [novo printTask](printtask.md) seja acionado.</span><span class="sxs-lookup"><span data-stu-id="0d492-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="0d492-128">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0d492-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="0d492-129">valores printEvent</span><span class="sxs-lookup"><span data-stu-id="0d492-129">printEvent values</span></span>

|<span data-ttu-id="0d492-130">Membro</span><span class="sxs-lookup"><span data-stu-id="0d492-130">Member</span></span>|<span data-ttu-id="0d492-131">Valor</span><span class="sxs-lookup"><span data-stu-id="0d492-131">Value</span></span>|<span data-ttu-id="0d492-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d492-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d492-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="0d492-133">jobStarted</span></span>|<span data-ttu-id="0d492-134">0</span><span class="sxs-lookup"><span data-stu-id="0d492-134">0</span></span>|<span data-ttu-id="0d492-135">Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.</span><span class="sxs-lookup"><span data-stu-id="0d492-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="0d492-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="0d492-136">unknownFutureValue</span></span>|<span data-ttu-id="0d492-137">1 </span><span class="sxs-lookup"><span data-stu-id="0d492-137">1</span></span>|<span data-ttu-id="0d492-138">Valor de sentinela de enumeração evolvável.</span><span class="sxs-lookup"><span data-stu-id="0d492-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="0d492-139">Não usar.</span><span class="sxs-lookup"><span data-stu-id="0d492-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d492-140">Relações</span><span class="sxs-lookup"><span data-stu-id="0d492-140">Relationships</span></span>
|<span data-ttu-id="0d492-141">Relação</span><span class="sxs-lookup"><span data-stu-id="0d492-141">Relationship</span></span>|<span data-ttu-id="0d492-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d492-142">Type</span></span>|<span data-ttu-id="0d492-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d492-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d492-144">definition</span><span class="sxs-lookup"><span data-stu-id="0d492-144">definition</span></span>|[<span data-ttu-id="0d492-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0d492-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="0d492-146">Uma definição abstrata que será usada para criar [uma printTask](printtask.md) quando disparada por um evento de impressão.</span><span class="sxs-lookup"><span data-stu-id="0d492-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="0d492-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d492-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d492-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d492-148">JSON representation</span></span>
<span data-ttu-id="0d492-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d492-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

