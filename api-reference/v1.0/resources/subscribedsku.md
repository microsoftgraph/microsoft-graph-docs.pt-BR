---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcd9e9b9cf32b3bfc35c5c10cb43a2a748b32041
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394614"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="5fc86-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5fc86-103">subscribedSku resource type</span></span>

<span data-ttu-id="5fc86-104">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="5fc86-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="5fc86-105">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="5fc86-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="5fc86-106">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="5fc86-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="5fc86-107">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="5fc86-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5fc86-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5fc86-108">Methods</span></span>
| <span data-ttu-id="5fc86-109">Método</span><span class="sxs-lookup"><span data-stu-id="5fc86-109">Method</span></span>           | <span data-ttu-id="5fc86-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5fc86-110">Return Type</span></span>    |<span data-ttu-id="5fc86-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fc86-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fc86-112">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5fc86-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="5fc86-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5fc86-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="5fc86-114">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="5fc86-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="5fc86-115">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="5fc86-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="5fc86-116">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="5fc86-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="5fc86-117">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="5fc86-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fc86-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fc86-118">Properties</span></span>
| <span data-ttu-id="5fc86-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fc86-119">Property</span></span>     | <span data-ttu-id="5fc86-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fc86-120">Type</span></span>   |<span data-ttu-id="5fc86-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fc86-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fc86-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="5fc86-122">appliesTo</span></span>|<span data-ttu-id="5fc86-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fc86-123">String</span></span>| <span data-ttu-id="5fc86-124">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="5fc86-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="5fc86-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="5fc86-125">capabilityStatus</span></span>|<span data-ttu-id="5fc86-126">String</span><span class="sxs-lookup"><span data-stu-id="5fc86-126">String</span></span>|  <span data-ttu-id="5fc86-127">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="5fc86-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="5fc86-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="5fc86-128">consumedUnits</span></span>|<span data-ttu-id="5fc86-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5fc86-129">Int32</span></span>| <span data-ttu-id="5fc86-130">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="5fc86-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="5fc86-131">id</span><span class="sxs-lookup"><span data-stu-id="5fc86-131">id</span></span>|<span data-ttu-id="5fc86-132">String</span><span class="sxs-lookup"><span data-stu-id="5fc86-132">String</span></span>| <span data-ttu-id="5fc86-133">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="5fc86-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="5fc86-134">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="5fc86-134">Key, not nullable.</span></span> |
|<span data-ttu-id="5fc86-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="5fc86-135">prepaidUnits</span></span>|[<span data-ttu-id="5fc86-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="5fc86-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="5fc86-137">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="5fc86-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="5fc86-138">onplans</span><span class="sxs-lookup"><span data-stu-id="5fc86-138">servicePlans</span></span>|<span data-ttu-id="5fc86-139">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="5fc86-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="5fc86-140">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="5fc86-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="5fc86-141">Não anulável</span><span class="sxs-lookup"><span data-stu-id="5fc86-141">Not nullable</span></span> |
|<span data-ttu-id="5fc86-142">skuId</span><span class="sxs-lookup"><span data-stu-id="5fc86-142">skuId</span></span>|<span data-ttu-id="5fc86-143">Guid</span><span class="sxs-lookup"><span data-stu-id="5fc86-143">Guid</span></span>| <span data-ttu-id="5fc86-144">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="5fc86-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="5fc86-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="5fc86-145">skuPartNumber</span></span>|<span data-ttu-id="5fc86-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fc86-146">String</span></span>| <span data-ttu-id="5fc86-147">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="5fc86-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="5fc86-148">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [list subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="5fc86-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fc86-149">Relações</span><span class="sxs-lookup"><span data-stu-id="5fc86-149">Relationships</span></span>
<span data-ttu-id="5fc86-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fc86-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fc86-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fc86-151">JSON representation</span></span>

<span data-ttu-id="5fc86-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5fc86-152">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
