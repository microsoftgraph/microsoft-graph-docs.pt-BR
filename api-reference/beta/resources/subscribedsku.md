---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda do directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528ec916edf049ef48b057afabad943bbb2182cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520293"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="c59a1-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c59a1-105">subscribedSku resource type</span></span>

<span data-ttu-id="c59a1-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c59a1-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c59a1-107">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="c59a1-107">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="c59a1-108">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="c59a1-108">Query filter expressions are not supported.</span></span> <span data-ttu-id="c59a1-109">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="c59a1-109">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="c59a1-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="c59a1-110">Methods</span></span>
| <span data-ttu-id="c59a1-111">Método</span><span class="sxs-lookup"><span data-stu-id="c59a1-111">Method</span></span>           | <span data-ttu-id="c59a1-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c59a1-112">Return Type</span></span>    |<span data-ttu-id="c59a1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c59a1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c59a1-114">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c59a1-114">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="c59a1-115">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c59a1-115">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="c59a1-116">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="c59a1-116">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="c59a1-117">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="c59a1-117">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="c59a1-118">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="c59a1-118">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="c59a1-119">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="c59a1-119">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="c59a1-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c59a1-120">Properties</span></span>
| <span data-ttu-id="c59a1-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c59a1-121">Property</span></span>     | <span data-ttu-id="c59a1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c59a1-122">Type</span></span>   |<span data-ttu-id="c59a1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c59a1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c59a1-124">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c59a1-124">appliesTo</span></span>|<span data-ttu-id="c59a1-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c59a1-125">String</span></span>| <span data-ttu-id="c59a1-126">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="c59a1-126">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="c59a1-127">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="c59a1-127">capabilityStatus</span></span>|<span data-ttu-id="c59a1-128">String</span><span class="sxs-lookup"><span data-stu-id="c59a1-128">String</span></span>| <span data-ttu-id="c59a1-129">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c59a1-129">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="c59a1-130">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="c59a1-130">consumedUnits</span></span>|<span data-ttu-id="c59a1-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c59a1-131">Int32</span></span>| <span data-ttu-id="c59a1-132">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="c59a1-132">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="c59a1-133">id</span><span class="sxs-lookup"><span data-stu-id="c59a1-133">id</span></span>|<span data-ttu-id="c59a1-134">String</span><span class="sxs-lookup"><span data-stu-id="c59a1-134">String</span></span>| <span data-ttu-id="c59a1-135">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="c59a1-135">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="c59a1-136">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="c59a1-136">Key, not nullable.</span></span> |
|<span data-ttu-id="c59a1-137">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="c59a1-137">prepaidUnits</span></span>|[<span data-ttu-id="c59a1-138">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="c59a1-138">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="c59a1-139">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="c59a1-139">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="c59a1-140">onplans</span><span class="sxs-lookup"><span data-stu-id="c59a1-140">servicePlans</span></span>|<span data-ttu-id="c59a1-141">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c59a1-141">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c59a1-142">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="c59a1-142">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="c59a1-143">Não anulável</span><span class="sxs-lookup"><span data-stu-id="c59a1-143">Not nullable</span></span> |
|<span data-ttu-id="c59a1-144">skuId</span><span class="sxs-lookup"><span data-stu-id="c59a1-144">skuId</span></span>|<span data-ttu-id="c59a1-145">Guid</span><span class="sxs-lookup"><span data-stu-id="c59a1-145">Guid</span></span>| <span data-ttu-id="c59a1-146">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="c59a1-146">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="c59a1-147">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="c59a1-147">skuPartNumber</span></span>|<span data-ttu-id="c59a1-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c59a1-148">String</span></span>| <span data-ttu-id="c59a1-149">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="c59a1-149">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="c59a1-150">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [list subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="c59a1-150">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c59a1-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c59a1-151">Relationships</span></span>
<span data-ttu-id="c59a1-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c59a1-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c59a1-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c59a1-153">JSON representation</span></span>

<span data-ttu-id="c59a1-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c59a1-154">Here is a JSON representation of the resource</span></span>

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
