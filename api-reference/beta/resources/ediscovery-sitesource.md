---
title: Tipo de recurso siteSource
description: O contêiner de um site associado a um custodiado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa4b8d0ccbe80ef0f65d27fa8ef648d1ea07b63
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445896"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="2089a-103">Tipo de recurso siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-103">siteSource resource type</span></span>

<span data-ttu-id="2089a-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2089a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2089a-105">O contêiner de um site associado a um [custodiado](ediscovery-custodian.md).</span><span class="sxs-lookup"><span data-stu-id="2089a-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2089a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2089a-106">Methods</span></span>

|<span data-ttu-id="2089a-107">Método</span><span class="sxs-lookup"><span data-stu-id="2089a-107">Method</span></span>|<span data-ttu-id="2089a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2089a-108">Return type</span></span>|<span data-ttu-id="2089a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2089a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2089a-110">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="2089a-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="2089a-111">[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="2089a-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="2089a-112">Obter uma lista de **objetos siteSource** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2089a-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="2089a-113">Criar siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="2089a-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="2089a-115">Crie um novo **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="2089a-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="2089a-116">Obter siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="2089a-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="2089a-118">Leia as propriedades e as relações de um **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="2089a-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="2089a-119">Excluir siteSource</span><span class="sxs-lookup"><span data-stu-id="2089a-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="2089a-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2089a-120">None</span></span>|<span data-ttu-id="2089a-121">Excluir um **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="2089a-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2089a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2089a-122">Properties</span></span>

|<span data-ttu-id="2089a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2089a-123">Property</span></span>|<span data-ttu-id="2089a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2089a-124">Type</span></span>|<span data-ttu-id="2089a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2089a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2089a-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="2089a-126">createdBy</span></span>|[<span data-ttu-id="2089a-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="2089a-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="2089a-128">O usuário que criou **o siteSource**.</span><span class="sxs-lookup"><span data-stu-id="2089a-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="2089a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2089a-129">createdDateTime</span></span>|<span data-ttu-id="2089a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2089a-130">DateTimeOffset</span></span>|<span data-ttu-id="2089a-131">A data e a hora **em que o siteSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="2089a-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="2089a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2089a-132">displayName</span></span>|<span data-ttu-id="2089a-133">String</span><span class="sxs-lookup"><span data-stu-id="2089a-133">String</span></span>|<span data-ttu-id="2089a-134">O nome de exibição **do siteSource**.</span><span class="sxs-lookup"><span data-stu-id="2089a-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="2089a-135">Esse será o nome do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2089a-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="2089a-136">id</span><span class="sxs-lookup"><span data-stu-id="2089a-136">id</span></span>|<span data-ttu-id="2089a-137">String</span><span class="sxs-lookup"><span data-stu-id="2089a-137">String</span></span>| <span data-ttu-id="2089a-138">A ID do **siteSource**.</span><span class="sxs-lookup"><span data-stu-id="2089a-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="2089a-139">Essa não é a ID do site real.</span><span class="sxs-lookup"><span data-stu-id="2089a-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2089a-140">Relações</span><span class="sxs-lookup"><span data-stu-id="2089a-140">Relationships</span></span>

|<span data-ttu-id="2089a-141">Relação</span><span class="sxs-lookup"><span data-stu-id="2089a-141">Relationship</span></span>|<span data-ttu-id="2089a-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="2089a-142">Type</span></span>|<span data-ttu-id="2089a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="2089a-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2089a-144">site</span><span class="sxs-lookup"><span data-stu-id="2089a-144">site</span></span>|[<span data-ttu-id="2089a-145">site</span><span class="sxs-lookup"><span data-stu-id="2089a-145">site</span></span>](../resources/site.md)|<span data-ttu-id="2089a-146">O site do SharePoint associado ao **siteSource**.</span><span class="sxs-lookup"><span data-stu-id="2089a-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2089a-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2089a-147">JSON representation</span></span>

<span data-ttu-id="2089a-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2089a-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
