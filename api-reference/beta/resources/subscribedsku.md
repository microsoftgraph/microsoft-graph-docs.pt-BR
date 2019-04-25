---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Não há suporte para expressões de filtro de consulta. Herda de directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582072"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="f1eef-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="f1eef-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1eef-106">Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="f1eef-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="f1eef-107">Não há suporte para expressões de filtro de consulta.</span><span class="sxs-lookup"><span data-stu-id="f1eef-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="f1eef-108">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f1eef-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="f1eef-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1eef-109">Methods</span></span>
| <span data-ttu-id="f1eef-110">Método</span><span class="sxs-lookup"><span data-stu-id="f1eef-110">Method</span></span>           | <span data-ttu-id="f1eef-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1eef-111">Return Type</span></span>    |<span data-ttu-id="f1eef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1eef-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1eef-113">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="f1eef-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="f1eef-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="f1eef-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="f1eef-115">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="f1eef-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="f1eef-116">Listar subscribedsku</span><span class="sxs-lookup"><span data-stu-id="f1eef-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="f1eef-117">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="f1eef-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="f1eef-118">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="f1eef-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1eef-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1eef-119">Properties</span></span>
| <span data-ttu-id="f1eef-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1eef-120">Property</span></span>     | <span data-ttu-id="f1eef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1eef-121">Type</span></span>   |<span data-ttu-id="f1eef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1eef-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1eef-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f1eef-123">appliesTo</span></span>|<span data-ttu-id="f1eef-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1eef-124">String</span></span>| <span data-ttu-id="f1eef-125">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="f1eef-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="f1eef-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f1eef-126">capabilityStatus</span></span>|<span data-ttu-id="f1eef-127">String</span><span class="sxs-lookup"><span data-stu-id="f1eef-127">String</span></span>| <span data-ttu-id="f1eef-128">Por exemplo, "habilitado".</span><span class="sxs-lookup"><span data-stu-id="f1eef-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="f1eef-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="f1eef-129">consumedUnits</span></span>|<span data-ttu-id="f1eef-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f1eef-130">Int32</span></span>| <span data-ttu-id="f1eef-131">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="f1eef-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="f1eef-132">id</span><span class="sxs-lookup"><span data-stu-id="f1eef-132">id</span></span>|<span data-ttu-id="f1eef-133">String</span><span class="sxs-lookup"><span data-stu-id="f1eef-133">String</span></span>| <span data-ttu-id="f1eef-134">O identificador exclusivo do objeto SKU assinado.</span><span class="sxs-lookup"><span data-stu-id="f1eef-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="f1eef-135">Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="f1eef-135">Key, not nullable.</span></span> |
|<span data-ttu-id="f1eef-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="f1eef-136">prepaidUnits</span></span>|[<span data-ttu-id="f1eef-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="f1eef-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="f1eef-138">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="f1eef-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="f1eef-139">onPlans</span><span class="sxs-lookup"><span data-stu-id="f1eef-139">servicePlans</span></span>|<span data-ttu-id="f1eef-140">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="f1eef-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="f1eef-141">Informações sobre os planos do serviço que estão disponíveis com o SKU.</span><span class="sxs-lookup"><span data-stu-id="f1eef-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="f1eef-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="f1eef-142">Not nullable</span></span> |
|<span data-ttu-id="f1eef-143">skuId</span><span class="sxs-lookup"><span data-stu-id="f1eef-143">skuId</span></span>|<span data-ttu-id="f1eef-144">Guid</span><span class="sxs-lookup"><span data-stu-id="f1eef-144">Guid</span></span>| <span data-ttu-id="f1eef-145">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="f1eef-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="f1eef-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="f1eef-146">skuPartNumber</span></span>|<span data-ttu-id="f1eef-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1eef-147">String</span></span>| <span data-ttu-id="f1eef-148">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="f1eef-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1eef-149">Relações</span><span class="sxs-lookup"><span data-stu-id="f1eef-149">Relationships</span></span>
<span data-ttu-id="f1eef-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1eef-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1eef-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1eef-151">JSON representation</span></span>

<span data-ttu-id="f1eef-152">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f1eef-152">Here is a JSON representation of the resource</span></span>

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
