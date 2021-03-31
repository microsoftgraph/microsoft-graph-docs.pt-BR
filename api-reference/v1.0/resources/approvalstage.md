---
title: Tipo de recurso approvalStage
description: O objeto approvalStage associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6212553d9364c4352bf1d6796156a4020854bf1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469497"
---
# <a name="approvalstage-resource-type"></a><span data-ttu-id="1dcc5-103">Tipo de recurso approvalStage</span><span class="sxs-lookup"><span data-stu-id="1dcc5-103">approvalStage resource type</span></span>

<span data-ttu-id="1dcc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dcc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1dcc5-105">Especifica estágios de decisão na aprovação.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-105">Specifies decision stages in the approval.</span></span>

## <a name="properties"></a><span data-ttu-id="1dcc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dcc5-106">Properties</span></span>

|<span data-ttu-id="1dcc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dcc5-107">Property</span></span>|<span data-ttu-id="1dcc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dcc5-108">Type</span></span>|<span data-ttu-id="1dcc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcc5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dcc5-110">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="1dcc5-110">assignedToMe</span></span>|<span data-ttu-id="1dcc5-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="1dcc5-111">Boolean</span></span>|<span data-ttu-id="1dcc5-112">Indica se o estágio é atribuído ao usuário chamador para revisar.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-112">Indicates whether the stage is assigned to the calling user to review.</span></span> <span data-ttu-id="1dcc5-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-113">Read-only.</span></span>|
|<span data-ttu-id="1dcc5-114">displayName</span><span class="sxs-lookup"><span data-stu-id="1dcc5-114">displayName</span></span>|<span data-ttu-id="1dcc5-115">String</span><span class="sxs-lookup"><span data-stu-id="1dcc5-115">String</span></span>|<span data-ttu-id="1dcc5-116">O rótulo fornecido pelo criador da política para identificar um estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-116">The label provided by the policy creator to identify an approval stage.</span></span> <span data-ttu-id="1dcc5-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-117">Read-only.</span></span>|
|<span data-ttu-id="1dcc5-118">id</span><span class="sxs-lookup"><span data-stu-id="1dcc5-118">id</span></span>|<span data-ttu-id="1dcc5-119">String</span><span class="sxs-lookup"><span data-stu-id="1dcc5-119">String</span></span>|<span data-ttu-id="1dcc5-120">O identificador do estágio associado a um objeto de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-120">The identifier of the stage associated with an approval object.</span></span> <span data-ttu-id="1dcc5-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-121">Read-only.</span></span>|
|<span data-ttu-id="1dcc5-122">justification</span><span class="sxs-lookup"><span data-stu-id="1dcc5-122">justification</span></span>|<span data-ttu-id="1dcc5-123">String</span><span class="sxs-lookup"><span data-stu-id="1dcc5-123">String</span></span>|<span data-ttu-id="1dcc5-124">A justificativa associada à decisão do estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-124">The justification associated with the approval stage decision.</span></span>|
|<span data-ttu-id="1dcc5-125">reviewResult</span><span class="sxs-lookup"><span data-stu-id="1dcc5-125">reviewResult</span></span>|<span data-ttu-id="1dcc5-126">String</span><span class="sxs-lookup"><span data-stu-id="1dcc5-126">String</span></span>|<span data-ttu-id="1dcc5-127">O resultado desse registro de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-127">The result of this approval record.</span></span> <span data-ttu-id="1dcc5-128">Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="1dcc5-128">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="1dcc5-129">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="1dcc5-129">reviewedBy</span></span>|[<span data-ttu-id="1dcc5-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1dcc5-130">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1dcc5-131">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-131">The identifier of the reviewer.</span></span> <span data-ttu-id="1dcc5-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-132">Read-only.</span></span>|
|<span data-ttu-id="1dcc5-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcc5-133">reviewedDateTime</span></span>|<span data-ttu-id="1dcc5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dcc5-134">DateTimeOffset</span></span>|<span data-ttu-id="1dcc5-135">A data e a hora em que uma decisão foi registrada.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-135">The date and time when a decision was recorded.</span></span> <span data-ttu-id="1dcc5-136">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-136">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1dcc5-137">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1dcc5-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-138">Read-only.</span></span>|
|<span data-ttu-id="1dcc5-139">status</span><span class="sxs-lookup"><span data-stu-id="1dcc5-139">status</span></span>|<span data-ttu-id="1dcc5-140">String</span><span class="sxs-lookup"><span data-stu-id="1dcc5-140">String</span></span>|<span data-ttu-id="1dcc5-141">O status do estágio.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-141">The stage status.</span></span> <span data-ttu-id="1dcc5-142">Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` .</span><span class="sxs-lookup"><span data-stu-id="1dcc5-142">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="1dcc5-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-143">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dcc5-144">Relações</span><span class="sxs-lookup"><span data-stu-id="1dcc5-144">Relationships</span></span>

<span data-ttu-id="1dcc5-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dcc5-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dcc5-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dcc5-146">JSON representation</span></span>

<span data-ttu-id="1dcc5-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dcc5-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
