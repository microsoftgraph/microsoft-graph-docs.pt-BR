---
title: Tipo de recurso printTaskTrigger
description: Determina as condições em que um novo printTask será executado com base na printTaskDefinition associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766319"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="cd999-103">Tipo de recurso printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="cd999-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="cd999-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd999-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd999-105">Determina a condição na qual um [novo printTask](printtask.md) será acionado com base na [impressão associadaTaskDefinition](printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cd999-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="cd999-106">Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="cd999-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="cd999-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd999-107">Methods</span></span>

| <span data-ttu-id="cd999-108">Método</span><span class="sxs-lookup"><span data-stu-id="cd999-108">Method</span></span>       | <span data-ttu-id="cd999-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd999-109">Return Type</span></span> | <span data-ttu-id="cd999-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd999-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cd999-111">List</span><span class="sxs-lookup"><span data-stu-id="cd999-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="cd999-112">[Coleção printTaskTrigger](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="cd999-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="cd999-113">Obter uma lista de printTaskTriggers associados a uma impressora [específica.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="cd999-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="cd999-114">Get</span><span class="sxs-lookup"><span data-stu-id="cd999-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="cd999-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="cd999-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="cd999-116">Obter uma determinada printTaskTrigger associada a uma impressora [específica.](printer.md)</span><span class="sxs-lookup"><span data-stu-id="cd999-116">Get a particular printTaskTrigger associated with a particular [printer](printer.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="cd999-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd999-117">Properties</span></span>
| <span data-ttu-id="cd999-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd999-118">Property</span></span>     | <span data-ttu-id="cd999-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd999-119">Type</span></span>        | <span data-ttu-id="cd999-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd999-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd999-121">id</span><span class="sxs-lookup"><span data-stu-id="cd999-121">id</span></span>|<span data-ttu-id="cd999-122">String</span><span class="sxs-lookup"><span data-stu-id="cd999-122">String</span></span>|<span data-ttu-id="cd999-123">O identificador printTaskTrigger.</span><span class="sxs-lookup"><span data-stu-id="cd999-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="cd999-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd999-124">Read-only.</span></span>|
|<span data-ttu-id="cd999-125">event</span><span class="sxs-lookup"><span data-stu-id="cd999-125">event</span></span>|<span data-ttu-id="cd999-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="cd999-126">printEvent</span></span>|<span data-ttu-id="cd999-127">O evento Impressão Universal que fará com que um [novo printTask](printtask.md) seja acionado.</span><span class="sxs-lookup"><span data-stu-id="cd999-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="cd999-128">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cd999-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="cd999-129">valores printEvent</span><span class="sxs-lookup"><span data-stu-id="cd999-129">printEvent values</span></span>

|<span data-ttu-id="cd999-130">Membro</span><span class="sxs-lookup"><span data-stu-id="cd999-130">Member</span></span>|<span data-ttu-id="cd999-131">Valor</span><span class="sxs-lookup"><span data-stu-id="cd999-131">Value</span></span>|<span data-ttu-id="cd999-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd999-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd999-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="cd999-133">jobStarted</span></span>|<span data-ttu-id="cd999-134">0</span><span class="sxs-lookup"><span data-stu-id="cd999-134">0</span></span>|<span data-ttu-id="cd999-135">Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.</span><span class="sxs-lookup"><span data-stu-id="cd999-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="cd999-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="cd999-136">unknownFutureValue</span></span>|<span data-ttu-id="cd999-137">1</span><span class="sxs-lookup"><span data-stu-id="cd999-137">1</span></span>|<span data-ttu-id="cd999-138">Valor de sentinela de enumeração evolvável.</span><span class="sxs-lookup"><span data-stu-id="cd999-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="cd999-139">Não usar.</span><span class="sxs-lookup"><span data-stu-id="cd999-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd999-140">Relações</span><span class="sxs-lookup"><span data-stu-id="cd999-140">Relationships</span></span>
| <span data-ttu-id="cd999-141">Relação</span><span class="sxs-lookup"><span data-stu-id="cd999-141">Relationship</span></span> | <span data-ttu-id="cd999-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd999-142">Type</span></span>        | <span data-ttu-id="cd999-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd999-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd999-144">definition</span><span class="sxs-lookup"><span data-stu-id="cd999-144">definition</span></span>|[<span data-ttu-id="cd999-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="cd999-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="cd999-146">Uma definição abstrata que será usada para criar [uma printTask](printtask.md) quando disparada por um evento de impressão.</span><span class="sxs-lookup"><span data-stu-id="cd999-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="cd999-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd999-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd999-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd999-148">JSON representation</span></span>

<span data-ttu-id="cd999-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd999-149">The following is a JSON representation of the resource.</span></span>

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


