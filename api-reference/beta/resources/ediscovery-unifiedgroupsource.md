---
title: Tipo de recurso unifiedGroupSource
description: O contêiner do grupo de um custodiado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445942"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="5490f-103">Tipo de recurso unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="5490f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5490f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5490f-105">O contêiner do [grupo de um custodiado.](ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="5490f-105">The container for a [custodian's](ediscovery-custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="5490f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="5490f-106">Methods</span></span>

|<span data-ttu-id="5490f-107">Método</span><span class="sxs-lookup"><span data-stu-id="5490f-107">Method</span></span>|<span data-ttu-id="5490f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5490f-108">Return type</span></span>|<span data-ttu-id="5490f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5490f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5490f-110">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="5490f-110">List unifiedGroupSources</span></span>](../api/ediscovery-custodian-list-unifiedgroupsources.md)|<span data-ttu-id="5490f-111">[coleção microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="5490f-111">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="5490f-112">Obter uma lista dos **objetos unifiedGroupSource** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="5490f-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="5490f-113">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-113">Create unifiedGroupSource</span></span>](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="5490f-114">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-114">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="5490f-115">Crie um novo **objeto unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="5490f-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="5490f-116">Obter unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-116">Get unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-get.md)|[<span data-ttu-id="5490f-117">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-117">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="5490f-118">Leia as propriedades e as relações de um **objeto unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="5490f-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="5490f-119">Excluir unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="5490f-119">Delete unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-delete.md)|<span data-ttu-id="5490f-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="5490f-120">None</span></span>|<span data-ttu-id="5490f-121">Exclua **um objeto unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="5490f-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5490f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5490f-122">Properties</span></span>

|<span data-ttu-id="5490f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5490f-123">Property</span></span>|<span data-ttu-id="5490f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5490f-124">Type</span></span>|<span data-ttu-id="5490f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5490f-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5490f-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="5490f-126">createdBy</span></span>|[<span data-ttu-id="5490f-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="5490f-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5490f-128">O usuário que criou **o unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="5490f-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="5490f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5490f-129">createdDateTime</span></span>|<span data-ttu-id="5490f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5490f-130">DateTimeOffset</span></span>|<span data-ttu-id="5490f-131">A data e a hora em **que o unifiedGroupSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="5490f-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="5490f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5490f-132">displayName</span></span>|<span data-ttu-id="5490f-133">String</span><span class="sxs-lookup"><span data-stu-id="5490f-133">String</span></span>|<span data-ttu-id="5490f-134">O nome de exibição do grupo unificado - Esse é o nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="5490f-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="5490f-135">id</span><span class="sxs-lookup"><span data-stu-id="5490f-135">id</span></span>|<span data-ttu-id="5490f-136">String</span><span class="sxs-lookup"><span data-stu-id="5490f-136">String</span></span>|<span data-ttu-id="5490f-137">A ID do **unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="5490f-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="5490f-138">Essa não é a ID do grupo real.</span><span class="sxs-lookup"><span data-stu-id="5490f-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="5490f-139">includedSources</span><span class="sxs-lookup"><span data-stu-id="5490f-139">includedSources</span></span>|<span data-ttu-id="5490f-140">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="5490f-140">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="5490f-141">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="5490f-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="5490f-142">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="5490f-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="5490f-143">valores sourceType</span><span class="sxs-lookup"><span data-stu-id="5490f-143">sourceType values</span></span>

<span data-ttu-id="5490f-144">Tipos de fonte relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5490f-144">Types of source related to the user.</span></span> <span data-ttu-id="5490f-145">Inclui caixa de correio e site por padrão.</span><span class="sxs-lookup"><span data-stu-id="5490f-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="5490f-146">Member</span><span class="sxs-lookup"><span data-stu-id="5490f-146">Member</span></span>|<span data-ttu-id="5490f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="5490f-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="5490f-148">mailbox</span><span class="sxs-lookup"><span data-stu-id="5490f-148">mailbox</span></span>|<span data-ttu-id="5490f-149">Representa uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5490f-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="5490f-150">site</span><span class="sxs-lookup"><span data-stu-id="5490f-150">site</span></span>|<span data-ttu-id="5490f-151">Representa um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5490f-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5490f-152">Relações</span><span class="sxs-lookup"><span data-stu-id="5490f-152">Relationships</span></span>

|<span data-ttu-id="5490f-153">Relação</span><span class="sxs-lookup"><span data-stu-id="5490f-153">Relationship</span></span>|<span data-ttu-id="5490f-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="5490f-154">Type</span></span>|<span data-ttu-id="5490f-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="5490f-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5490f-156">group</span><span class="sxs-lookup"><span data-stu-id="5490f-156">group</span></span>|[<span data-ttu-id="5490f-157">group</span><span class="sxs-lookup"><span data-stu-id="5490f-157">group</span></span>](../resources/group.md)|<span data-ttu-id="5490f-158">O grupo associado ao **unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="5490f-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5490f-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5490f-159">JSON representation</span></span>

<span data-ttu-id="5490f-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5490f-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
