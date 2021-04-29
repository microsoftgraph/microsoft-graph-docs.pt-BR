---
title: Tipo de recurso siteSource
description: O contêiner de um site associado a um custodiado.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c178565b628728fcf6124ea3058e979f8423ce90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080474"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="54aab-103">Tipo de recurso siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-103">siteSource resource type</span></span>

<span data-ttu-id="54aab-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="54aab-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54aab-105">O contêiner de um site associado a um [custodiado](ediscovery-custodian.md).</span><span class="sxs-lookup"><span data-stu-id="54aab-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="54aab-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="54aab-106">Methods</span></span>

|<span data-ttu-id="54aab-107">Método</span><span class="sxs-lookup"><span data-stu-id="54aab-107">Method</span></span>|<span data-ttu-id="54aab-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="54aab-108">Return type</span></span>|<span data-ttu-id="54aab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="54aab-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54aab-110">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="54aab-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="54aab-111">[coleção microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="54aab-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="54aab-112">Obter uma lista de **objetos siteSource** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="54aab-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="54aab-113">Criar siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="54aab-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="54aab-115">Crie um novo **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="54aab-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="54aab-116">Obter siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="54aab-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="54aab-118">Leia as propriedades e as relações de um **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="54aab-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="54aab-119">Excluir siteSource</span><span class="sxs-lookup"><span data-stu-id="54aab-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="54aab-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54aab-120">None</span></span>|<span data-ttu-id="54aab-121">Excluir um **objeto siteSource.**</span><span class="sxs-lookup"><span data-stu-id="54aab-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54aab-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54aab-122">Properties</span></span>

|<span data-ttu-id="54aab-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54aab-123">Property</span></span>|<span data-ttu-id="54aab-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="54aab-124">Type</span></span>|<span data-ttu-id="54aab-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="54aab-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54aab-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="54aab-126">createdBy</span></span>|[<span data-ttu-id="54aab-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="54aab-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="54aab-128">O usuário que criou **o siteSource**.</span><span class="sxs-lookup"><span data-stu-id="54aab-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="54aab-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54aab-129">createdDateTime</span></span>|<span data-ttu-id="54aab-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54aab-130">DateTimeOffset</span></span>|<span data-ttu-id="54aab-131">A data e a hora **em que o siteSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="54aab-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="54aab-132">displayName</span><span class="sxs-lookup"><span data-stu-id="54aab-132">displayName</span></span>|<span data-ttu-id="54aab-133">String</span><span class="sxs-lookup"><span data-stu-id="54aab-133">String</span></span>|<span data-ttu-id="54aab-134">O nome de exibição **do siteSource**.</span><span class="sxs-lookup"><span data-stu-id="54aab-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="54aab-135">Esse será o nome do SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="54aab-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="54aab-136">id</span><span class="sxs-lookup"><span data-stu-id="54aab-136">id</span></span>|<span data-ttu-id="54aab-137">String</span><span class="sxs-lookup"><span data-stu-id="54aab-137">String</span></span>| <span data-ttu-id="54aab-138">A ID do **siteSource**.</span><span class="sxs-lookup"><span data-stu-id="54aab-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="54aab-139">A origem do site pode ser recuperada a qualquer momento com [Get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span><span class="sxs-lookup"><span data-stu-id="54aab-139">The site source can be retrieved at any time with [Get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span></span>|

## <a name="relationships"></a><span data-ttu-id="54aab-140">Relações</span><span class="sxs-lookup"><span data-stu-id="54aab-140">Relationships</span></span>

|<span data-ttu-id="54aab-141">Relação</span><span class="sxs-lookup"><span data-stu-id="54aab-141">Relationship</span></span>|<span data-ttu-id="54aab-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="54aab-142">Type</span></span>|<span data-ttu-id="54aab-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="54aab-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54aab-144">site</span><span class="sxs-lookup"><span data-stu-id="54aab-144">site</span></span>|[<span data-ttu-id="54aab-145">site</span><span class="sxs-lookup"><span data-stu-id="54aab-145">site</span></span>](../resources/site.md)|<span data-ttu-id="54aab-146">O SharePoint site associado ao **siteSource**.</span><span class="sxs-lookup"><span data-stu-id="54aab-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54aab-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54aab-147">JSON representation</span></span>

<span data-ttu-id="54aab-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54aab-148">The following is a JSON representation of the resource.</span></span>
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
