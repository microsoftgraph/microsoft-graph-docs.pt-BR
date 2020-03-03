---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda do directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c88ac94d35b93a76ec2ea4f096b69facb7f26435
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394502"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="a3005-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a3005-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3005-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="a3005-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="a3005-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="a3005-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="a3005-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a3005-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="a3005-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a3005-109">Methods</span></span>
| <span data-ttu-id="a3005-110">Método</span><span class="sxs-lookup"><span data-stu-id="a3005-110">Method</span></span>           | <span data-ttu-id="a3005-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a3005-111">Return Type</span></span>    |<span data-ttu-id="a3005-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3005-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3005-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a3005-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="a3005-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a3005-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="a3005-115">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="a3005-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="a3005-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="a3005-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="a3005-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="a3005-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="a3005-118">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="a3005-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3005-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3005-119">Properties</span></span>
| <span data-ttu-id="a3005-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3005-120">Property</span></span>     | <span data-ttu-id="a3005-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3005-121">Type</span></span>   |<span data-ttu-id="a3005-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3005-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3005-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="a3005-123">appliesTo</span></span>|<span data-ttu-id="a3005-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3005-124">String</span></span>| <span data-ttu-id="a3005-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="a3005-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="a3005-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="a3005-126">capabilityStatus</span></span>|<span data-ttu-id="a3005-127">String</span><span class="sxs-lookup"><span data-stu-id="a3005-127">String</span></span>| <span data-ttu-id="a3005-128">Os valores possíveis são: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="a3005-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="a3005-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="a3005-129">consumedUnits</span></span>|<span data-ttu-id="a3005-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a3005-130">Int32</span></span>| <span data-ttu-id="a3005-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="a3005-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="a3005-132">id</span><span class="sxs-lookup"><span data-stu-id="a3005-132">id</span></span>|<span data-ttu-id="a3005-133">String</span><span class="sxs-lookup"><span data-stu-id="a3005-133">String</span></span>| <span data-ttu-id="a3005-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="a3005-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="a3005-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="a3005-135">Key, not nullable.</span></span> |
|<span data-ttu-id="a3005-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="a3005-136">prepaidUnits</span></span>|[<span data-ttu-id="a3005-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="a3005-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="a3005-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="a3005-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="a3005-139">onplans</span><span class="sxs-lookup"><span data-stu-id="a3005-139">servicePlans</span></span>|<span data-ttu-id="a3005-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="a3005-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="a3005-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="a3005-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="a3005-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="a3005-142">Not nullable</span></span> |
|<span data-ttu-id="a3005-143">skuId</span><span class="sxs-lookup"><span data-stu-id="a3005-143">skuId</span></span>|<span data-ttu-id="a3005-144">Guid</span><span class="sxs-lookup"><span data-stu-id="a3005-144">Guid</span></span>| <span data-ttu-id="a3005-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="a3005-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="a3005-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="a3005-146">skuPartNumber</span></span>|<span data-ttu-id="a3005-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3005-147">String</span></span>| <span data-ttu-id="a3005-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="a3005-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="a3005-149">Para obter uma lista de assinaturas comerciais que uma organização adquiriu, consulte [list subscribedSkus](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="a3005-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3005-150">Relações</span><span class="sxs-lookup"><span data-stu-id="a3005-150">Relationships</span></span>
<span data-ttu-id="a3005-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3005-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3005-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3005-152">JSON representation</span></span>

<span data-ttu-id="a3005-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a3005-153">Here is a JSON representation of the resource</span></span>

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
