---
title: Tipo de recurso subscribedSku
description: " criar, atualizar e excluir não são suportados. Expressões de filtro de consulta não são suportadas. Herda de directoryObject."
localization_priority: Normal
ms.openlocfilehash: 07f40c766d7f46974cf99b9954f63a61c2c0c621
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829600"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="72439-105">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="72439-105">subscribedSku resource type</span></span>

> <span data-ttu-id="72439-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72439-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72439-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72439-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72439-p103">Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="72439-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="72439-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="72439-111">Methods</span></span>
| <span data-ttu-id="72439-112">Método</span><span class="sxs-lookup"><span data-stu-id="72439-112">Method</span></span>           | <span data-ttu-id="72439-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="72439-113">Return Type</span></span>    |<span data-ttu-id="72439-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="72439-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72439-115">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="72439-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="72439-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="72439-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="72439-117">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="72439-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="72439-118">Lista subscribedsku</span><span class="sxs-lookup"><span data-stu-id="72439-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="72439-119">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="72439-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="72439-120">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="72439-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="72439-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72439-121">Properties</span></span>
| <span data-ttu-id="72439-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72439-122">Property</span></span>     | <span data-ttu-id="72439-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="72439-123">Type</span></span>   |<span data-ttu-id="72439-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="72439-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72439-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="72439-125">appliesTo</span></span>|<span data-ttu-id="72439-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72439-126">String</span></span>| <span data-ttu-id="72439-127">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="72439-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="72439-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="72439-128">capabilityStatus</span></span>|<span data-ttu-id="72439-129">String</span><span class="sxs-lookup"><span data-stu-id="72439-129">String</span></span>| <span data-ttu-id="72439-130">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="72439-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="72439-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="72439-131">consumedUnits</span></span>|<span data-ttu-id="72439-132">Int32</span><span class="sxs-lookup"><span data-stu-id="72439-132">Int32</span></span>| <span data-ttu-id="72439-133">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="72439-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="72439-134">id</span><span class="sxs-lookup"><span data-stu-id="72439-134">id</span></span>|<span data-ttu-id="72439-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72439-135">String</span></span>| <span data-ttu-id="72439-p104">O identificador exclusivo do objeto SKU assinado. Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="72439-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="72439-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="72439-138">prepaidUnits</span></span>|[<span data-ttu-id="72439-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="72439-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="72439-140">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="72439-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="72439-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="72439-141">servicePlans</span></span>|<span data-ttu-id="72439-142">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="72439-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="72439-p105">Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável</span><span class="sxs-lookup"><span data-stu-id="72439-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="72439-145">skuId</span><span class="sxs-lookup"><span data-stu-id="72439-145">skuId</span></span>|<span data-ttu-id="72439-146">Guid</span><span class="sxs-lookup"><span data-stu-id="72439-146">Guid</span></span>| <span data-ttu-id="72439-147">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="72439-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="72439-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="72439-148">skuPartNumber</span></span>|<span data-ttu-id="72439-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72439-149">String</span></span>| <span data-ttu-id="72439-150">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="72439-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="72439-151">Relações</span><span class="sxs-lookup"><span data-stu-id="72439-151">Relationships</span></span>
<span data-ttu-id="72439-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72439-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72439-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72439-153">JSON representation</span></span>

<span data-ttu-id="72439-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="72439-154">Here is a JSON representation of the resource</span></span>

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
