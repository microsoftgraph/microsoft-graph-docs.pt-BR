---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda de directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e57ff1e59c7caf5b29e582b7381492a7eee5b4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964814"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="37d73-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="37d73-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37d73-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="37d73-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="37d73-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="37d73-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="37d73-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="37d73-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="37d73-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="37d73-109">Methods</span></span>
| <span data-ttu-id="37d73-110">Método</span><span class="sxs-lookup"><span data-stu-id="37d73-110">Method</span></span>           | <span data-ttu-id="37d73-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37d73-111">Return Type</span></span>    |<span data-ttu-id="37d73-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d73-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37d73-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="37d73-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="37d73-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="37d73-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="37d73-115">Obtenha uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="37d73-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="37d73-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="37d73-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="37d73-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="37d73-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="37d73-118">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="37d73-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="37d73-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37d73-119">Properties</span></span>
| <span data-ttu-id="37d73-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37d73-120">Property</span></span>     | <span data-ttu-id="37d73-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="37d73-121">Type</span></span>   |<span data-ttu-id="37d73-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d73-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37d73-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="37d73-123">appliesTo</span></span>|<span data-ttu-id="37d73-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37d73-124">String</span></span>| <span data-ttu-id="37d73-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="37d73-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="37d73-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="37d73-126">capabilityStatus</span></span>|<span data-ttu-id="37d73-127">String</span><span class="sxs-lookup"><span data-stu-id="37d73-127">String</span></span>| <span data-ttu-id="37d73-128">Por exemplo, "habilitado".</span><span class="sxs-lookup"><span data-stu-id="37d73-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="37d73-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="37d73-129">consumedUnits</span></span>|<span data-ttu-id="37d73-130">Int32</span><span class="sxs-lookup"><span data-stu-id="37d73-130">Int32</span></span>| <span data-ttu-id="37d73-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="37d73-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="37d73-132">id</span><span class="sxs-lookup"><span data-stu-id="37d73-132">id</span></span>|<span data-ttu-id="37d73-133">String</span><span class="sxs-lookup"><span data-stu-id="37d73-133">String</span></span>| <span data-ttu-id="37d73-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="37d73-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="37d73-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="37d73-135">Key, not nullable.</span></span> |
|<span data-ttu-id="37d73-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="37d73-136">prepaidUnits</span></span>|[<span data-ttu-id="37d73-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="37d73-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="37d73-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="37d73-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="37d73-139">onplans</span><span class="sxs-lookup"><span data-stu-id="37d73-139">servicePlans</span></span>|<span data-ttu-id="37d73-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="37d73-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="37d73-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="37d73-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="37d73-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="37d73-142">Not nullable</span></span> |
|<span data-ttu-id="37d73-143">skuId</span><span class="sxs-lookup"><span data-stu-id="37d73-143">skuId</span></span>|<span data-ttu-id="37d73-144">Guid</span><span class="sxs-lookup"><span data-stu-id="37d73-144">Guid</span></span>| <span data-ttu-id="37d73-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="37d73-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="37d73-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="37d73-146">skuPartNumber</span></span>|<span data-ttu-id="37d73-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37d73-147">String</span></span>| <span data-ttu-id="37d73-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="37d73-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="37d73-149">Relações</span><span class="sxs-lookup"><span data-stu-id="37d73-149">Relationships</span></span>
<span data-ttu-id="37d73-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37d73-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37d73-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37d73-151">JSON representation</span></span>

<span data-ttu-id="37d73-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="37d73-152">Here is a JSON representation of the resource</span></span>

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
