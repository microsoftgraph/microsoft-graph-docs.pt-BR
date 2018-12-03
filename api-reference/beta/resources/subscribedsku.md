---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Expressões de filtro de consulta não são suportadas. Herda de directoryObject."
ms.openlocfilehash: ab9b64d8de67379aa002ffeec78edd327b15b222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039765"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="d8b69-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d8b69-105">subscribedSku resource type</span></span>

> <span data-ttu-id="d8b69-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8b69-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8b69-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8b69-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8b69-p103">Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d8b69-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d8b69-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8b69-111">Methods</span></span>
| <span data-ttu-id="d8b69-112">Método</span><span class="sxs-lookup"><span data-stu-id="d8b69-112">Method</span></span>           | <span data-ttu-id="d8b69-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8b69-113">Return Type</span></span>    |<span data-ttu-id="d8b69-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b69-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8b69-115">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d8b69-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="d8b69-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d8b69-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="d8b69-117">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="d8b69-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="d8b69-118">Lista subscribedsku</span><span class="sxs-lookup"><span data-stu-id="d8b69-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="d8b69-119">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="d8b69-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="d8b69-120">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="d8b69-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8b69-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8b69-121">Properties</span></span>
| <span data-ttu-id="d8b69-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8b69-122">Property</span></span>     | <span data-ttu-id="d8b69-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8b69-123">Type</span></span>   |<span data-ttu-id="d8b69-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b69-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8b69-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d8b69-125">appliesTo</span></span>|<span data-ttu-id="d8b69-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b69-126">String</span></span>| <span data-ttu-id="d8b69-127">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="d8b69-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="d8b69-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d8b69-128">capabilityStatus</span></span>|<span data-ttu-id="d8b69-129">String</span><span class="sxs-lookup"><span data-stu-id="d8b69-129">String</span></span>| <span data-ttu-id="d8b69-130">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="d8b69-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="d8b69-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="d8b69-131">consumedUnits</span></span>|<span data-ttu-id="d8b69-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b69-132">Int32</span></span>| <span data-ttu-id="d8b69-133">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="d8b69-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="d8b69-134">id</span><span class="sxs-lookup"><span data-stu-id="d8b69-134">id</span></span>|<span data-ttu-id="d8b69-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b69-135">String</span></span>| <span data-ttu-id="d8b69-p104">O identificador exclusivo do objeto SKU assinado. Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="d8b69-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="d8b69-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="d8b69-138">prepaidUnits</span></span>|[<span data-ttu-id="d8b69-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="d8b69-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="d8b69-140">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="d8b69-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="d8b69-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="d8b69-141">servicePlans</span></span>|<span data-ttu-id="d8b69-142">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="d8b69-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="d8b69-p105">Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável</span><span class="sxs-lookup"><span data-stu-id="d8b69-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="d8b69-145">skuId</span><span class="sxs-lookup"><span data-stu-id="d8b69-145">skuId</span></span>|<span data-ttu-id="d8b69-146">Guid</span><span class="sxs-lookup"><span data-stu-id="d8b69-146">Guid</span></span>| <span data-ttu-id="d8b69-147">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="d8b69-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="d8b69-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="d8b69-148">skuPartNumber</span></span>|<span data-ttu-id="d8b69-149">String</span><span class="sxs-lookup"><span data-stu-id="d8b69-149">String</span></span>| <span data-ttu-id="d8b69-150">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="d8b69-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8b69-151">Relações</span><span class="sxs-lookup"><span data-stu-id="d8b69-151">Relationships</span></span>
<span data-ttu-id="d8b69-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8b69-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b69-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8b69-153">JSON representation</span></span>

<span data-ttu-id="d8b69-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d8b69-154">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
