---
title: tipo de recurso unifiedGroupSource
description: O contêiner para o grupo de um dos responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597525"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="6e0d6-103">tipo de recurso unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="6e0d6-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6e0d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e0d6-105">O contêiner para o grupo de um [dos responsáveis](custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="6e0d6-105">The container for a [custodian's](custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="6e0d6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="6e0d6-106">Methods</span></span>

|<span data-ttu-id="6e0d6-107">Método</span><span class="sxs-lookup"><span data-stu-id="6e0d6-107">Method</span></span>|<span data-ttu-id="6e0d6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e0d6-108">Return type</span></span>|<span data-ttu-id="6e0d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0d6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e0d6-110">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="6e0d6-110">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="6e0d6-111">coleção [unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="6e0d6-111">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="6e0d6-112">Obtenha uma lista dos objetos **unifiedGroupSource** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="6e0d6-113">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-113">Create unifiedGroupSource</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="6e0d6-114">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-114">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="6e0d6-115">Criar um novo objeto **unifiedGroupSource** .</span><span class="sxs-lookup"><span data-stu-id="6e0d6-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="6e0d6-116">Obter unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-116">Get unifiedGroupSource</span></span>](../api/unifiedgroupsource-get.md)|[<span data-ttu-id="6e0d6-117">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-117">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="6e0d6-118">Leia as propriedades e os relacionamentos de um objeto **unifiedGroupSource** .</span><span class="sxs-lookup"><span data-stu-id="6e0d6-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="6e0d6-119">Excluir unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="6e0d6-119">Delete unifiedGroupSource</span></span>](../api/unifiedgroupsource-delete.md)|<span data-ttu-id="6e0d6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e0d6-120">None</span></span>|<span data-ttu-id="6e0d6-121">Excluir um objeto **unifiedGroupSource** .</span><span class="sxs-lookup"><span data-stu-id="6e0d6-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e0d6-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e0d6-122">Properties</span></span>

|<span data-ttu-id="6e0d6-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e0d6-123">Property</span></span>|<span data-ttu-id="6e0d6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e0d6-124">Type</span></span>|<span data-ttu-id="6e0d6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0d6-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0d6-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="6e0d6-126">createdBy</span></span>|[<span data-ttu-id="6e0d6-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="6e0d6-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="6e0d6-128">O usuário que criou o **unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="6e0d6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e0d6-129">createdDateTime</span></span>|<span data-ttu-id="6e0d6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e0d6-130">DateTimeOffset</span></span>|<span data-ttu-id="6e0d6-131">A data e a hora em que o **unifiedGroupSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="6e0d6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6e0d6-132">displayName</span></span>|<span data-ttu-id="6e0d6-133">String</span><span class="sxs-lookup"><span data-stu-id="6e0d6-133">String</span></span>|<span data-ttu-id="6e0d6-134">O nome de exibição do grupo unificado-este é o nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="6e0d6-135">id</span><span class="sxs-lookup"><span data-stu-id="6e0d6-135">id</span></span>|<span data-ttu-id="6e0d6-136">String</span><span class="sxs-lookup"><span data-stu-id="6e0d6-136">String</span></span>|<span data-ttu-id="6e0d6-137">A ID do **unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="6e0d6-138">Essa não é a ID do grupo real.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="6e0d6-139">includedSources</span><span class="sxs-lookup"><span data-stu-id="6e0d6-139">includedSources</span></span>|<span data-ttu-id="6e0d6-140">sourceType</span><span class="sxs-lookup"><span data-stu-id="6e0d6-140">sourceType</span></span>|<span data-ttu-id="6e0d6-141">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="6e0d6-142">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="6e0d6-143">valores de sourceType</span><span class="sxs-lookup"><span data-stu-id="6e0d6-143">sourceType values</span></span>

<span data-ttu-id="6e0d6-144">Tipos de fonte relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-144">Types of source related to the user.</span></span> <span data-ttu-id="6e0d6-145">Inclui a caixa de correio e o site por padrão.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="6e0d6-146">Member</span><span class="sxs-lookup"><span data-stu-id="6e0d6-146">Member</span></span>|<span data-ttu-id="6e0d6-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0d6-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="6e0d6-148">mailbox</span><span class="sxs-lookup"><span data-stu-id="6e0d6-148">mailbox</span></span>|<span data-ttu-id="6e0d6-149">Representa uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="6e0d6-150">site</span><span class="sxs-lookup"><span data-stu-id="6e0d6-150">site</span></span>|<span data-ttu-id="6e0d6-151">Representa um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e0d6-152">Relações</span><span class="sxs-lookup"><span data-stu-id="6e0d6-152">Relationships</span></span>

|<span data-ttu-id="6e0d6-153">Relação</span><span class="sxs-lookup"><span data-stu-id="6e0d6-153">Relationship</span></span>|<span data-ttu-id="6e0d6-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e0d6-154">Type</span></span>|<span data-ttu-id="6e0d6-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e0d6-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0d6-156">group</span><span class="sxs-lookup"><span data-stu-id="6e0d6-156">group</span></span>|[<span data-ttu-id="6e0d6-157">group</span><span class="sxs-lookup"><span data-stu-id="6e0d6-157">group</span></span>](../resources/group.md)|<span data-ttu-id="6e0d6-158">O grupo associado ao **unifiedGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e0d6-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e0d6-159">JSON representation</span></span>

<span data-ttu-id="6e0d6-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e0d6-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
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
