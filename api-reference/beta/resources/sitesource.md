---
title: tipo de recurso de site da filial
description: O contêiner de um site associado a um responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597529"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="1888f-103">tipo de recurso de site da filial</span><span class="sxs-lookup"><span data-stu-id="1888f-103">siteSource resource type</span></span>

<span data-ttu-id="1888f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1888f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1888f-105">O contêiner de um site associado a um [responsáveis](custodian.md).</span><span class="sxs-lookup"><span data-stu-id="1888f-105">The container for a site associated with a [custodian](custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1888f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1888f-106">Methods</span></span>

|<span data-ttu-id="1888f-107">Método</span><span class="sxs-lookup"><span data-stu-id="1888f-107">Method</span></span>|<span data-ttu-id="1888f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1888f-108">Return type</span></span>|<span data-ttu-id="1888f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1888f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1888f-110">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="1888f-110">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="1888f-111">coleção de [sites de site](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="1888f-111">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="1888f-112">Obter uma lista de objetos de **site de site** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1888f-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="1888f-113">Criar site local</span><span class="sxs-lookup"><span data-stu-id="1888f-113">Create siteSource</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="1888f-114">site da site</span><span class="sxs-lookup"><span data-stu-id="1888f-114">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="1888f-115">Criar um novo objeto **sitery** .</span><span class="sxs-lookup"><span data-stu-id="1888f-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="1888f-116">Obter local de site</span><span class="sxs-lookup"><span data-stu-id="1888f-116">Get siteSource</span></span>](../api/sitesource-get.md)|[<span data-ttu-id="1888f-117">site da site</span><span class="sxs-lookup"><span data-stu-id="1888f-117">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="1888f-118">Leia as propriedades e os relacionamentos de um objeto de **site** .</span><span class="sxs-lookup"><span data-stu-id="1888f-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="1888f-119">Excluir site local</span><span class="sxs-lookup"><span data-stu-id="1888f-119">Delete siteSource</span></span>](../api/sitesource-delete.md)|<span data-ttu-id="1888f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1888f-120">None</span></span>|<span data-ttu-id="1888f-121">Excluir um objeto de **site** .</span><span class="sxs-lookup"><span data-stu-id="1888f-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1888f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1888f-122">Properties</span></span>

|<span data-ttu-id="1888f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1888f-123">Property</span></span>|<span data-ttu-id="1888f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1888f-124">Type</span></span>|<span data-ttu-id="1888f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1888f-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1888f-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="1888f-126">createdBy</span></span>|[<span data-ttu-id="1888f-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="1888f-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1888f-128">O usuário que criou a **site**.</span><span class="sxs-lookup"><span data-stu-id="1888f-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="1888f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1888f-129">createdDateTime</span></span>|<span data-ttu-id="1888f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1888f-130">DateTimeOffset</span></span>|<span data-ttu-id="1888f-131">A data e a hora em que o **site local** foi criado.</span><span class="sxs-lookup"><span data-stu-id="1888f-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="1888f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1888f-132">displayName</span></span>|<span data-ttu-id="1888f-133">String</span><span class="sxs-lookup"><span data-stu-id="1888f-133">String</span></span>|<span data-ttu-id="1888f-134">O nome de exibição do **site**.</span><span class="sxs-lookup"><span data-stu-id="1888f-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="1888f-135">Este será o nome do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1888f-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="1888f-136">id</span><span class="sxs-lookup"><span data-stu-id="1888f-136">id</span></span>|<span data-ttu-id="1888f-137">String</span><span class="sxs-lookup"><span data-stu-id="1888f-137">String</span></span>| <span data-ttu-id="1888f-138">A ID da sessão de **site**.</span><span class="sxs-lookup"><span data-stu-id="1888f-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="1888f-139">Esta não é a ID do site real.</span><span class="sxs-lookup"><span data-stu-id="1888f-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1888f-140">Relações</span><span class="sxs-lookup"><span data-stu-id="1888f-140">Relationships</span></span>

|<span data-ttu-id="1888f-141">Relação</span><span class="sxs-lookup"><span data-stu-id="1888f-141">Relationship</span></span>|<span data-ttu-id="1888f-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="1888f-142">Type</span></span>|<span data-ttu-id="1888f-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="1888f-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1888f-144">site</span><span class="sxs-lookup"><span data-stu-id="1888f-144">site</span></span>|[<span data-ttu-id="1888f-145">site</span><span class="sxs-lookup"><span data-stu-id="1888f-145">site</span></span>](../resources/site.md)|<span data-ttu-id="1888f-146">O site do SharePoint associado ao **site**.</span><span class="sxs-lookup"><span data-stu-id="1888f-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1888f-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1888f-147">JSON representation</span></span>

<span data-ttu-id="1888f-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1888f-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
