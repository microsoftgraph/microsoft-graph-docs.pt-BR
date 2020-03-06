---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b7f1d532c88b3b289e0d337236843fada7c0dd2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533608"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="36aa8-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="36aa8-103">subscribedSku resource type</span></span>

<span data-ttu-id="36aa8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36aa8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36aa8-105">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="36aa8-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="36aa8-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="36aa8-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="36aa8-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="36aa8-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="36aa8-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="36aa8-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="36aa8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="36aa8-109">Methods</span></span>
| <span data-ttu-id="36aa8-110">Método</span><span class="sxs-lookup"><span data-stu-id="36aa8-110">Method</span></span>           | <span data-ttu-id="36aa8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36aa8-111">Return Type</span></span>    |<span data-ttu-id="36aa8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="36aa8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36aa8-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="36aa8-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="36aa8-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="36aa8-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="36aa8-115">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="36aa8-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="36aa8-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="36aa8-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="36aa8-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="36aa8-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="36aa8-118">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="36aa8-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="36aa8-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36aa8-119">Properties</span></span>
| <span data-ttu-id="36aa8-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36aa8-120">Property</span></span>     | <span data-ttu-id="36aa8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="36aa8-121">Type</span></span>   |<span data-ttu-id="36aa8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="36aa8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36aa8-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="36aa8-123">appliesTo</span></span>|<span data-ttu-id="36aa8-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36aa8-124">String</span></span>| <span data-ttu-id="36aa8-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="36aa8-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="36aa8-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="36aa8-126">capabilityStatus</span></span>|<span data-ttu-id="36aa8-127">String</span><span class="sxs-lookup"><span data-stu-id="36aa8-127">String</span></span>|  <span data-ttu-id="36aa8-128">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="36aa8-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="36aa8-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="36aa8-129">consumedUnits</span></span>|<span data-ttu-id="36aa8-130">Int32</span><span class="sxs-lookup"><span data-stu-id="36aa8-130">Int32</span></span>| <span data-ttu-id="36aa8-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="36aa8-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="36aa8-132">id</span><span class="sxs-lookup"><span data-stu-id="36aa8-132">id</span></span>|<span data-ttu-id="36aa8-133">String</span><span class="sxs-lookup"><span data-stu-id="36aa8-133">String</span></span>| <span data-ttu-id="36aa8-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="36aa8-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="36aa8-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="36aa8-135">Key, not nullable.</span></span> |
|<span data-ttu-id="36aa8-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="36aa8-136">prepaidUnits</span></span>|[<span data-ttu-id="36aa8-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="36aa8-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="36aa8-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="36aa8-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="36aa8-139">onplans</span><span class="sxs-lookup"><span data-stu-id="36aa8-139">servicePlans</span></span>|<span data-ttu-id="36aa8-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="36aa8-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="36aa8-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="36aa8-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="36aa8-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="36aa8-142">Not nullable</span></span> |
|<span data-ttu-id="36aa8-143">skuId</span><span class="sxs-lookup"><span data-stu-id="36aa8-143">skuId</span></span>|<span data-ttu-id="36aa8-144">Guid</span><span class="sxs-lookup"><span data-stu-id="36aa8-144">Guid</span></span>| <span data-ttu-id="36aa8-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="36aa8-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="36aa8-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="36aa8-146">skuPartNumber</span></span>|<span data-ttu-id="36aa8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36aa8-147">String</span></span>| <span data-ttu-id="36aa8-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="36aa8-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="36aa8-149">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [list subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="36aa8-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="36aa8-150">Relações</span><span class="sxs-lookup"><span data-stu-id="36aa8-150">Relationships</span></span>
<span data-ttu-id="36aa8-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36aa8-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36aa8-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36aa8-152">JSON representation</span></span>

<span data-ttu-id="36aa8-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="36aa8-153">Here is a JSON representation of the resource</span></span>

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
