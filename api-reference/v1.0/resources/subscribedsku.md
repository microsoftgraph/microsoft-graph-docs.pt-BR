---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0dbb255bced328b6b3d40e675ee53e6cf3fbece
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094152"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="ed413-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ed413-103">subscribedSku resource type</span></span>

<span data-ttu-id="ed413-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed413-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed413-105">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="ed413-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="ed413-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="ed413-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="ed413-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="ed413-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="ed413-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="ed413-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ed413-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed413-109">Methods</span></span>
| <span data-ttu-id="ed413-110">Método</span><span class="sxs-lookup"><span data-stu-id="ed413-110">Method</span></span>           | <span data-ttu-id="ed413-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed413-111">Return Type</span></span>    |<span data-ttu-id="ed413-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed413-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed413-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ed413-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="ed413-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="ed413-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="ed413-115">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="ed413-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="ed413-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="ed413-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="ed413-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="ed413-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="ed413-118">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="ed413-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed413-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed413-119">Properties</span></span>
| <span data-ttu-id="ed413-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed413-120">Property</span></span>     | <span data-ttu-id="ed413-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed413-121">Type</span></span>   |<span data-ttu-id="ed413-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed413-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed413-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ed413-123">appliesTo</span></span>|<span data-ttu-id="ed413-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed413-124">String</span></span>| <span data-ttu-id="ed413-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="ed413-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="ed413-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="ed413-126">capabilityStatus</span></span>|<span data-ttu-id="ed413-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed413-127">String</span></span>|  <span data-ttu-id="ed413-128">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="ed413-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="ed413-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="ed413-129">consumedUnits</span></span>|<span data-ttu-id="ed413-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ed413-130">Int32</span></span>| <span data-ttu-id="ed413-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="ed413-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="ed413-132">id</span><span class="sxs-lookup"><span data-stu-id="ed413-132">id</span></span>|<span data-ttu-id="ed413-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed413-133">String</span></span>| <span data-ttu-id="ed413-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="ed413-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="ed413-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed413-135">Key, not nullable.</span></span> |
|<span data-ttu-id="ed413-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="ed413-136">prepaidUnits</span></span>|[<span data-ttu-id="ed413-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="ed413-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="ed413-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="ed413-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="ed413-139">onplans</span><span class="sxs-lookup"><span data-stu-id="ed413-139">servicePlans</span></span>|<span data-ttu-id="ed413-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="ed413-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="ed413-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="ed413-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="ed413-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="ed413-142">Not nullable</span></span> |
|<span data-ttu-id="ed413-143">skuId</span><span class="sxs-lookup"><span data-stu-id="ed413-143">skuId</span></span>|<span data-ttu-id="ed413-144">Guid</span><span class="sxs-lookup"><span data-stu-id="ed413-144">Guid</span></span>| <span data-ttu-id="ed413-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="ed413-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="ed413-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="ed413-146">skuPartNumber</span></span>|<span data-ttu-id="ed413-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed413-147">String</span></span>| <span data-ttu-id="ed413-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="ed413-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="ed413-149">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [list subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="ed413-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed413-150">Relações</span><span class="sxs-lookup"><span data-stu-id="ed413-150">Relationships</span></span>
<span data-ttu-id="ed413-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed413-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed413-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed413-152">JSON representation</span></span>

<span data-ttu-id="ed413-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ed413-153">Here is a JSON representation of the resource</span></span>

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

