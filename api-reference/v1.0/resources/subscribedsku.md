---
title: Tipo de recurso subscribedSku
description: Contém informações sobre um serviço SKU assinado por uma empresa.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3343661f6c72a057c73b70f91a284f3168a9c72
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639063"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="43d77-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="43d77-103">subscribedSku resource type</span></span>

<span data-ttu-id="43d77-104">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="43d77-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="43d77-105">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="43d77-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="43d77-106">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="43d77-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="43d77-107">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="43d77-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="43d77-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="43d77-108">Methods</span></span>
| <span data-ttu-id="43d77-109">Método</span><span class="sxs-lookup"><span data-stu-id="43d77-109">Method</span></span>           | <span data-ttu-id="43d77-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43d77-110">Return Type</span></span>    |<span data-ttu-id="43d77-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="43d77-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43d77-112">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="43d77-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="43d77-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="43d77-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="43d77-114">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="43d77-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="43d77-115">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="43d77-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="43d77-116">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="43d77-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="43d77-117">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="43d77-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="43d77-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43d77-118">Properties</span></span>
| <span data-ttu-id="43d77-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43d77-119">Property</span></span>     | <span data-ttu-id="43d77-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="43d77-120">Type</span></span>   |<span data-ttu-id="43d77-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="43d77-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43d77-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="43d77-122">appliesTo</span></span>|<span data-ttu-id="43d77-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d77-123">String</span></span>| <span data-ttu-id="43d77-124">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="43d77-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="43d77-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="43d77-125">capabilityStatus</span></span>|<span data-ttu-id="43d77-126">String</span><span class="sxs-lookup"><span data-stu-id="43d77-126">String</span></span>| <span data-ttu-id="43d77-127">Por exemplo, "habilitado".</span><span class="sxs-lookup"><span data-stu-id="43d77-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="43d77-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="43d77-128">consumedUnits</span></span>|<span data-ttu-id="43d77-129">Int32</span><span class="sxs-lookup"><span data-stu-id="43d77-129">Int32</span></span>| <span data-ttu-id="43d77-130">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="43d77-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="43d77-131">id</span><span class="sxs-lookup"><span data-stu-id="43d77-131">id</span></span>|<span data-ttu-id="43d77-132">String</span><span class="sxs-lookup"><span data-stu-id="43d77-132">String</span></span>| <span data-ttu-id="43d77-133">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="43d77-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="43d77-134">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="43d77-134">Key, not nullable.</span></span> |
|<span data-ttu-id="43d77-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="43d77-135">prepaidUnits</span></span>|[<span data-ttu-id="43d77-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="43d77-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="43d77-137">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="43d77-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="43d77-138">onplans</span><span class="sxs-lookup"><span data-stu-id="43d77-138">servicePlans</span></span>|<span data-ttu-id="43d77-139">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="43d77-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="43d77-140">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="43d77-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="43d77-141">Não anulável</span><span class="sxs-lookup"><span data-stu-id="43d77-141">Not nullable</span></span> |
|<span data-ttu-id="43d77-142">skuId</span><span class="sxs-lookup"><span data-stu-id="43d77-142">skuId</span></span>|<span data-ttu-id="43d77-143">Guid</span><span class="sxs-lookup"><span data-stu-id="43d77-143">Guid</span></span>| <span data-ttu-id="43d77-144">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="43d77-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="43d77-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="43d77-145">skuPartNumber</span></span>|<span data-ttu-id="43d77-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d77-146">String</span></span>| <span data-ttu-id="43d77-147">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="43d77-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="43d77-148">Relações</span><span class="sxs-lookup"><span data-stu-id="43d77-148">Relationships</span></span>
<span data-ttu-id="43d77-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43d77-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43d77-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43d77-150">JSON representation</span></span>

<span data-ttu-id="43d77-151">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="43d77-151">Here is a JSON representation of the resource</span></span>

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
