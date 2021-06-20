---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 291a30b0d8d4aa9181114cf392b5c466fc395925
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030793"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="0cf63-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0cf63-103">subscribedSku resource type</span></span>

<span data-ttu-id="0cf63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf63-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cf63-105">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="0cf63-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="0cf63-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="0cf63-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="0cf63-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="0cf63-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="0cf63-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="0cf63-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0cf63-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0cf63-109">Methods</span></span>
| <span data-ttu-id="0cf63-110">Método</span><span class="sxs-lookup"><span data-stu-id="0cf63-110">Method</span></span>           | <span data-ttu-id="0cf63-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0cf63-111">Return Type</span></span>    |<span data-ttu-id="0cf63-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf63-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cf63-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0cf63-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="0cf63-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0cf63-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="0cf63-115">Obter uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="0cf63-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="0cf63-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="0cf63-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="0cf63-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="0cf63-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="0cf63-118">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="0cf63-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cf63-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cf63-119">Properties</span></span>
| <span data-ttu-id="0cf63-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cf63-120">Property</span></span>     | <span data-ttu-id="0cf63-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf63-121">Type</span></span>   |<span data-ttu-id="0cf63-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf63-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cf63-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0cf63-123">appliesTo</span></span>|<span data-ttu-id="0cf63-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf63-124">String</span></span>| <span data-ttu-id="0cf63-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="0cf63-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="0cf63-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="0cf63-126">capabilityStatus</span></span>|<span data-ttu-id="0cf63-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf63-127">String</span></span>|  <span data-ttu-id="0cf63-128">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="0cf63-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="0cf63-129">O capabilityStatus é se a propriedade `Enabled` **prepaidUnits** tiver pelo menos uma unidade habilitada e se o cliente `LockedOut` cancelar sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="0cf63-129">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled**, and `LockedOut` if the customer cancelled their subscription.</span></span> |
|<span data-ttu-id="0cf63-130">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="0cf63-130">consumedUnits</span></span>|<span data-ttu-id="0cf63-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf63-131">Int32</span></span>| <span data-ttu-id="0cf63-132">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="0cf63-132">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="0cf63-133">id</span><span class="sxs-lookup"><span data-stu-id="0cf63-133">id</span></span>|<span data-ttu-id="0cf63-134">String</span><span class="sxs-lookup"><span data-stu-id="0cf63-134">String</span></span>| <span data-ttu-id="0cf63-135">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="0cf63-135">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="0cf63-136">Chave, não anulada.</span><span class="sxs-lookup"><span data-stu-id="0cf63-136">Key, not nullable.</span></span> |
|<span data-ttu-id="0cf63-137">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="0cf63-137">prepaidUnits</span></span>|[<span data-ttu-id="0cf63-138">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="0cf63-138">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="0cf63-139">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="0cf63-139">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="0cf63-140">servicePlans</span><span class="sxs-lookup"><span data-stu-id="0cf63-140">servicePlans</span></span>|<span data-ttu-id="0cf63-141">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="0cf63-141">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="0cf63-142">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="0cf63-142">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="0cf63-143">Não anulada</span><span class="sxs-lookup"><span data-stu-id="0cf63-143">Not nullable</span></span> |
|<span data-ttu-id="0cf63-144">skuId</span><span class="sxs-lookup"><span data-stu-id="0cf63-144">skuId</span></span>|<span data-ttu-id="0cf63-145">Guid</span><span class="sxs-lookup"><span data-stu-id="0cf63-145">Guid</span></span>| <span data-ttu-id="0cf63-146">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="0cf63-146">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="0cf63-147">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="0cf63-147">skuPartNumber</span></span>|<span data-ttu-id="0cf63-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf63-148">String</span></span>| <span data-ttu-id="0cf63-149">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="0cf63-149">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="0cf63-150">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [List subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="0cf63-150">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cf63-151">Relações</span><span class="sxs-lookup"><span data-stu-id="0cf63-151">Relationships</span></span>
<span data-ttu-id="0cf63-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cf63-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cf63-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cf63-153">JSON representation</span></span>

<span data-ttu-id="0cf63-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0cf63-154">Here is a JSON representation of the resource</span></span>

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

