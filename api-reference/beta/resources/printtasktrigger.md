---
title: tipo de recurso printTaskTrigger
description: Determina as condições sob as quais uma nova multitarefa será executada com base no printTaskDefinition associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0a9ca4d06f43c9dd0964f0bb4c9614bfb4a78c1e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091545"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="a8e21-103">tipo de recurso printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="a8e21-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="a8e21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8e21-105">Determina a condição sob a qual uma nova [multitarefa](printtask.md) será disparada com base no [printTaskDefinition](printtaskdefinition.md)associado.</span><span class="sxs-lookup"><span data-stu-id="a8e21-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="a8e21-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="a8e21-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="a8e21-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a8e21-107">Methods</span></span>

| <span data-ttu-id="a8e21-108">Método</span><span class="sxs-lookup"><span data-stu-id="a8e21-108">Method</span></span>       | <span data-ttu-id="a8e21-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a8e21-109">Return Type</span></span> | <span data-ttu-id="a8e21-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e21-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a8e21-111">Listar</span><span class="sxs-lookup"><span data-stu-id="a8e21-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="a8e21-112">coleção [printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="a8e21-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="a8e21-113">Obtenha uma lista de printTaskTriggers associados a uma [impressora](printer.md)específica.</span><span class="sxs-lookup"><span data-stu-id="a8e21-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="a8e21-114">Get</span><span class="sxs-lookup"><span data-stu-id="a8e21-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="a8e21-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="a8e21-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="a8e21-116">Obter o printTaskTrigger associado a uma [multitarefa](printtask.md)em particular.</span><span class="sxs-lookup"><span data-stu-id="a8e21-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |


## <a name="properties"></a><span data-ttu-id="a8e21-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8e21-117">Properties</span></span>
| <span data-ttu-id="a8e21-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8e21-118">Property</span></span>     | <span data-ttu-id="a8e21-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e21-119">Type</span></span>        | <span data-ttu-id="a8e21-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e21-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8e21-121">id</span><span class="sxs-lookup"><span data-stu-id="a8e21-121">id</span></span>|<span data-ttu-id="a8e21-122">String</span><span class="sxs-lookup"><span data-stu-id="a8e21-122">String</span></span>|<span data-ttu-id="a8e21-123">O identificador do printTaskTrigger.</span><span class="sxs-lookup"><span data-stu-id="a8e21-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="a8e21-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8e21-124">Read-only.</span></span>|
|<span data-ttu-id="a8e21-125">event</span><span class="sxs-lookup"><span data-stu-id="a8e21-125">event</span></span>|<span data-ttu-id="a8e21-126">MyEvent</span><span class="sxs-lookup"><span data-stu-id="a8e21-126">printEvent</span></span>|<span data-ttu-id="a8e21-127">O evento de impressão universal que fará com que [uma nova impressão seja disparada](printtask.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e21-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="a8e21-128">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8e21-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="a8e21-129">valores de MyEvent</span><span class="sxs-lookup"><span data-stu-id="a8e21-129">printEvent values</span></span>

|<span data-ttu-id="a8e21-130">Membro</span><span class="sxs-lookup"><span data-stu-id="a8e21-130">Member</span></span>|<span data-ttu-id="a8e21-131">Valor</span><span class="sxs-lookup"><span data-stu-id="a8e21-131">Value</span></span>|<span data-ttu-id="a8e21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e21-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="a8e21-133">jobStarted</span></span>|<span data-ttu-id="a8e21-134">,0</span><span class="sxs-lookup"><span data-stu-id="a8e21-134">0</span></span>|<span data-ttu-id="a8e21-135">Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.</span><span class="sxs-lookup"><span data-stu-id="a8e21-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="a8e21-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="a8e21-136">unknownFutureValue</span></span>|<span data-ttu-id="a8e21-137">1 </span><span class="sxs-lookup"><span data-stu-id="a8e21-137">1</span></span>|<span data-ttu-id="a8e21-138">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="a8e21-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="a8e21-139">Não usar.</span><span class="sxs-lookup"><span data-stu-id="a8e21-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e21-140">Relações</span><span class="sxs-lookup"><span data-stu-id="a8e21-140">Relationships</span></span>
| <span data-ttu-id="a8e21-141">Relação</span><span class="sxs-lookup"><span data-stu-id="a8e21-141">Relationship</span></span> | <span data-ttu-id="a8e21-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e21-142">Type</span></span>        | <span data-ttu-id="a8e21-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e21-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8e21-144">definir</span><span class="sxs-lookup"><span data-stu-id="a8e21-144">definition</span></span>|[<span data-ttu-id="a8e21-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="a8e21-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="a8e21-146">Uma definição abstrata que será usada para criar uma [multitarefa](printtask.md) quando disparado por um evento Print.</span><span class="sxs-lookup"><span data-stu-id="a8e21-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="a8e21-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8e21-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8e21-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8e21-148">JSON representation</span></span>

<span data-ttu-id="a8e21-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8e21-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
