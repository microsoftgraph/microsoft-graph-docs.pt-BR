---
title: Tipo de recurso subscribedSku
description: Representa o tipo SKU inscrito.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3d41247ebb88e4941556408fe6fbebbabc54ff8d
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030898"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="382fb-103">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="382fb-103">subscribedSku resource type</span></span>

<span data-ttu-id="382fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="382fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="382fb-105">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="382fb-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="382fb-106">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="382fb-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="382fb-107">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="382fb-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="382fb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="382fb-108">Methods</span></span>
| <span data-ttu-id="382fb-109">Método</span><span class="sxs-lookup"><span data-stu-id="382fb-109">Method</span></span>           | <span data-ttu-id="382fb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="382fb-110">Return Type</span></span>    |<span data-ttu-id="382fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="382fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="382fb-112">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="382fb-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="382fb-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="382fb-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="382fb-114">Obter uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="382fb-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="382fb-115">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="382fb-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="382fb-116">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="382fb-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="382fb-117">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="382fb-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="382fb-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="382fb-118">Properties</span></span>
| <span data-ttu-id="382fb-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="382fb-119">Property</span></span>     | <span data-ttu-id="382fb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="382fb-120">Type</span></span>   |<span data-ttu-id="382fb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="382fb-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="382fb-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="382fb-122">appliesTo</span></span>|<span data-ttu-id="382fb-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="382fb-123">String</span></span>| <span data-ttu-id="382fb-124">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="382fb-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="382fb-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="382fb-125">capabilityStatus</span></span>|<span data-ttu-id="382fb-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="382fb-126">String</span></span>| <span data-ttu-id="382fb-127">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="382fb-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="382fb-128">O capabilityStatus é se a propriedade `Enabled` **prepaidUnits** tiver pelo menos uma unidade habilitada e se o cliente `LockedOut` cancelar sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="382fb-128">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled**, and `LockedOut` if the customer cancelled their subscription.</span></span> |
|<span data-ttu-id="382fb-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="382fb-129">consumedUnits</span></span>|<span data-ttu-id="382fb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="382fb-130">Int32</span></span>| <span data-ttu-id="382fb-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="382fb-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="382fb-132">id</span><span class="sxs-lookup"><span data-stu-id="382fb-132">id</span></span>|<span data-ttu-id="382fb-133">String</span><span class="sxs-lookup"><span data-stu-id="382fb-133">String</span></span>| <span data-ttu-id="382fb-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="382fb-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="382fb-135">Chave, não anulada.</span><span class="sxs-lookup"><span data-stu-id="382fb-135">Key, not nullable.</span></span> |
|<span data-ttu-id="382fb-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="382fb-136">prepaidUnits</span></span>|[<span data-ttu-id="382fb-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="382fb-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="382fb-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="382fb-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="382fb-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="382fb-139">servicePlans</span></span>|<span data-ttu-id="382fb-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="382fb-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="382fb-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="382fb-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="382fb-142">Não anulada</span><span class="sxs-lookup"><span data-stu-id="382fb-142">Not nullable</span></span> |
|<span data-ttu-id="382fb-143">skuId</span><span class="sxs-lookup"><span data-stu-id="382fb-143">skuId</span></span>|<span data-ttu-id="382fb-144">Guid</span><span class="sxs-lookup"><span data-stu-id="382fb-144">Guid</span></span>| <span data-ttu-id="382fb-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="382fb-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="382fb-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="382fb-146">skuPartNumber</span></span>|<span data-ttu-id="382fb-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="382fb-147">String</span></span>| <span data-ttu-id="382fb-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="382fb-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="382fb-149">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [List subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="382fb-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="382fb-150">Relações</span><span class="sxs-lookup"><span data-stu-id="382fb-150">Relationships</span></span>
<span data-ttu-id="382fb-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="382fb-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="382fb-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="382fb-152">JSON representation</span></span>

<span data-ttu-id="382fb-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="382fb-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


