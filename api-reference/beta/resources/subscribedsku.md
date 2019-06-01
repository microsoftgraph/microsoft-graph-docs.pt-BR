---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda de directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9763592ee444cbf0ae73ffbad81288bb5fdd76c2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655114"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="fb486-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="fb486-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb486-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="fb486-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="fb486-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="fb486-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="fb486-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="fb486-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fb486-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb486-109">Methods</span></span>
| <span data-ttu-id="fb486-110">Método</span><span class="sxs-lookup"><span data-stu-id="fb486-110">Method</span></span>           | <span data-ttu-id="fb486-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb486-111">Return Type</span></span>    |<span data-ttu-id="fb486-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb486-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb486-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="fb486-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="fb486-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="fb486-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="fb486-115">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="fb486-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="fb486-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="fb486-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="fb486-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="fb486-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="fb486-118">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="fb486-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb486-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb486-119">Properties</span></span>
| <span data-ttu-id="fb486-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb486-120">Property</span></span>     | <span data-ttu-id="fb486-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb486-121">Type</span></span>   |<span data-ttu-id="fb486-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb486-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb486-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="fb486-123">appliesTo</span></span>|<span data-ttu-id="fb486-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb486-124">String</span></span>| <span data-ttu-id="fb486-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="fb486-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="fb486-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="fb486-126">capabilityStatus</span></span>|<span data-ttu-id="fb486-127">String</span><span class="sxs-lookup"><span data-stu-id="fb486-127">String</span></span>| <span data-ttu-id="fb486-128">Por exemplo, "habilitado".</span><span class="sxs-lookup"><span data-stu-id="fb486-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="fb486-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="fb486-129">consumedUnits</span></span>|<span data-ttu-id="fb486-130">Int32</span><span class="sxs-lookup"><span data-stu-id="fb486-130">Int32</span></span>| <span data-ttu-id="fb486-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="fb486-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="fb486-132">id</span><span class="sxs-lookup"><span data-stu-id="fb486-132">id</span></span>|<span data-ttu-id="fb486-133">String</span><span class="sxs-lookup"><span data-stu-id="fb486-133">String</span></span>| <span data-ttu-id="fb486-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="fb486-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="fb486-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="fb486-135">Key, not nullable.</span></span> |
|<span data-ttu-id="fb486-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="fb486-136">prepaidUnits</span></span>|[<span data-ttu-id="fb486-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="fb486-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="fb486-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="fb486-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="fb486-139">onplans</span><span class="sxs-lookup"><span data-stu-id="fb486-139">servicePlans</span></span>|<span data-ttu-id="fb486-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="fb486-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="fb486-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="fb486-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="fb486-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="fb486-142">Not nullable</span></span> |
|<span data-ttu-id="fb486-143">skuId</span><span class="sxs-lookup"><span data-stu-id="fb486-143">skuId</span></span>|<span data-ttu-id="fb486-144">Guid</span><span class="sxs-lookup"><span data-stu-id="fb486-144">Guid</span></span>| <span data-ttu-id="fb486-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="fb486-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="fb486-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="fb486-146">skuPartNumber</span></span>|<span data-ttu-id="fb486-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb486-147">String</span></span>| <span data-ttu-id="fb486-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="fb486-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb486-149">Relações</span><span class="sxs-lookup"><span data-stu-id="fb486-149">Relationships</span></span>
<span data-ttu-id="fb486-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb486-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb486-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb486-151">JSON representation</span></span>

<span data-ttu-id="fb486-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fb486-152">Here is a JSON representation of the resource</span></span>

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
