---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
ms.openlocfilehash: 17290890ff27fded1aaf5d7fdb2c0cdacee09b0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873714"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="0297f-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0297f-103">subscribedSku resource type</span></span>

<span data-ttu-id="0297f-104">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="0297f-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="0297f-p101">Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="0297f-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0297f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0297f-108">Methods</span></span>
| <span data-ttu-id="0297f-109">Método</span><span class="sxs-lookup"><span data-stu-id="0297f-109">Method</span></span>           | <span data-ttu-id="0297f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0297f-110">Return Type</span></span>    |<span data-ttu-id="0297f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0297f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0297f-112">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0297f-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="0297f-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="0297f-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="0297f-114">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="0297f-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="0297f-115">Lista subscribedsku</span><span class="sxs-lookup"><span data-stu-id="0297f-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="0297f-116">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="0297f-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="0297f-117">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="0297f-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="0297f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0297f-118">Properties</span></span>
| <span data-ttu-id="0297f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0297f-119">Property</span></span>     | <span data-ttu-id="0297f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0297f-120">Type</span></span>   |<span data-ttu-id="0297f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0297f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0297f-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0297f-122">appliesTo</span></span>|<span data-ttu-id="0297f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0297f-123">String</span></span>| <span data-ttu-id="0297f-124">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="0297f-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="0297f-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="0297f-125">capabilityStatus</span></span>|<span data-ttu-id="0297f-126">String</span><span class="sxs-lookup"><span data-stu-id="0297f-126">String</span></span>| <span data-ttu-id="0297f-127">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="0297f-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="0297f-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="0297f-128">consumedUnits</span></span>|<span data-ttu-id="0297f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0297f-129">Int32</span></span>| <span data-ttu-id="0297f-130">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="0297f-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="0297f-131">id</span><span class="sxs-lookup"><span data-stu-id="0297f-131">id</span></span>|<span data-ttu-id="0297f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0297f-132">String</span></span>| <span data-ttu-id="0297f-p102">O identificador exclusivo do objeto SKU assinado. Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="0297f-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="0297f-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="0297f-135">prepaidUnits</span></span>|[<span data-ttu-id="0297f-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="0297f-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="0297f-137">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="0297f-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="0297f-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="0297f-138">servicePlans</span></span>|<span data-ttu-id="0297f-139">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="0297f-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="0297f-p103">Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável</span><span class="sxs-lookup"><span data-stu-id="0297f-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="0297f-142">skuId</span><span class="sxs-lookup"><span data-stu-id="0297f-142">skuId</span></span>|<span data-ttu-id="0297f-143">Guid</span><span class="sxs-lookup"><span data-stu-id="0297f-143">Guid</span></span>| <span data-ttu-id="0297f-144">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="0297f-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="0297f-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="0297f-145">skuPartNumber</span></span>|<span data-ttu-id="0297f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0297f-146">String</span></span>| <span data-ttu-id="0297f-147">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="0297f-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="0297f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="0297f-148">Relationships</span></span>
<span data-ttu-id="0297f-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0297f-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0297f-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0297f-150">JSON representation</span></span>

<span data-ttu-id="0297f-151">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0297f-151">Here is a JSON representation of the resource</span></span>

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
