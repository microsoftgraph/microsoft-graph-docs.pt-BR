---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Expressões de filtro de consulta não são suportadas. Herda de directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522697"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="5e43f-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5e43f-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e43f-p102">Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="5e43f-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="5e43f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e43f-109">Methods</span></span>
| <span data-ttu-id="5e43f-110">Método</span><span class="sxs-lookup"><span data-stu-id="5e43f-110">Method</span></span>           | <span data-ttu-id="5e43f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e43f-111">Return Type</span></span>    |<span data-ttu-id="5e43f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e43f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e43f-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5e43f-113">[Get subscribedSku](../api/subscribedsku-get.md)</span></span> | [<span data-ttu-id="5e43f-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5e43f-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="5e43f-115">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="5e43f-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="5e43f-116">List subscribedSku</span><span class="sxs-lookup"><span data-stu-id="5e43f-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="5e43f-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="5e43f-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="5e43f-118">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="5e43f-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e43f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e43f-119">Properties</span></span>
| <span data-ttu-id="5e43f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e43f-120">Property</span></span>     | <span data-ttu-id="5e43f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e43f-121">Type</span></span>   |<span data-ttu-id="5e43f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e43f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e43f-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="5e43f-123">appliesTo</span></span>|<span data-ttu-id="5e43f-124">String</span><span class="sxs-lookup"><span data-stu-id="5e43f-124">String</span></span>| <span data-ttu-id="5e43f-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="5e43f-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="5e43f-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="5e43f-126">capabilityStatus</span></span>|<span data-ttu-id="5e43f-127">String</span><span class="sxs-lookup"><span data-stu-id="5e43f-127">String</span></span>| <span data-ttu-id="5e43f-128">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="5e43f-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="5e43f-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="5e43f-129">consumedUnits</span></span>|<span data-ttu-id="5e43f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="5e43f-130">Int32</span></span>| <span data-ttu-id="5e43f-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="5e43f-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="5e43f-132">id</span><span class="sxs-lookup"><span data-stu-id="5e43f-132">id</span></span>|<span data-ttu-id="5e43f-133">String</span><span class="sxs-lookup"><span data-stu-id="5e43f-133">String</span></span>| <span data-ttu-id="5e43f-p103">O identificador exclusivo do objeto SKU assinado. Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="5e43f-p103">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="5e43f-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="5e43f-136">prepaidUnits</span></span>|[<span data-ttu-id="5e43f-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="5e43f-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="5e43f-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="5e43f-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="5e43f-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="5e43f-139">servicePlans</span></span>|<span data-ttu-id="5e43f-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="5e43f-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="5e43f-p104">Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável</span><span class="sxs-lookup"><span data-stu-id="5e43f-p104">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="5e43f-143">skuId</span><span class="sxs-lookup"><span data-stu-id="5e43f-143">skuId</span></span>|<span data-ttu-id="5e43f-144">Guid</span><span class="sxs-lookup"><span data-stu-id="5e43f-144">Guid</span></span>| <span data-ttu-id="5e43f-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="5e43f-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="5e43f-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="5e43f-146">skuPartNumber</span></span>|<span data-ttu-id="5e43f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e43f-147">String</span></span>| <span data-ttu-id="5e43f-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="5e43f-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e43f-149">Relações</span><span class="sxs-lookup"><span data-stu-id="5e43f-149">Relationships</span></span>
<span data-ttu-id="5e43f-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e43f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e43f-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e43f-151">JSON representation</span></span>

<span data-ttu-id="5e43f-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5e43f-152">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/subscribedsku.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
