---
title: tipo de recurso personWebsite
description: tipo de recurso personWebsite
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e3f41b352af77073d6338888c8349e38145daff9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811081"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="560da-103">tipo de recurso personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-103">personWebsite resource type</span></span>

<span data-ttu-id="560da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="560da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="560da-105">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="560da-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="560da-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="560da-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="560da-107">Methods</span></span>
|<span data-ttu-id="560da-108">Método</span><span class="sxs-lookup"><span data-stu-id="560da-108">Method</span></span>|<span data-ttu-id="560da-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="560da-109">Return type</span></span>|<span data-ttu-id="560da-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="560da-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="560da-111">Listar sites</span><span class="sxs-lookup"><span data-stu-id="560da-111">List websites</span></span>](../api/profile-list-websites.md)|<span data-ttu-id="560da-112">coleção [personWebsite](../resources/personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="560da-112">[personWebsite](../resources/personwebsite.md) collection</span></span>|<span data-ttu-id="560da-113">Obtenha os recursos personWebsite da propriedade de navegação sites.</span><span class="sxs-lookup"><span data-stu-id="560da-113">Get the personWebsite resources from the websites navigation property.</span></span>|
|[<span data-ttu-id="560da-114">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-114">Create personWebsite</span></span>](../api/profile-post-websites.md)|[<span data-ttu-id="560da-115">personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-115">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="560da-116">Criar um novo objeto personWebsite.</span><span class="sxs-lookup"><span data-stu-id="560da-116">Create a new personWebsite object.</span></span>|
|[<span data-ttu-id="560da-117">Obter personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-117">Get personWebsite</span></span>](../api/personwebsite-get.md)|[<span data-ttu-id="560da-118">personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-118">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="560da-119">Leia as propriedades e os relacionamentos de um objeto [personWebsite](../resources/personwebsite.md) .</span><span class="sxs-lookup"><span data-stu-id="560da-119">Read the properties and relationships of a [personWebsite](../resources/personwebsite.md) object.</span></span>|
|[<span data-ttu-id="560da-120">Atualizar personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-120">Update personWebsite</span></span>](../api/personwebsite-update.md)|[<span data-ttu-id="560da-121">personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-121">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="560da-122">Atualiza as propriedades de um objeto [personWebsite](../resources/personwebsite.md) .</span><span class="sxs-lookup"><span data-stu-id="560da-122">Update the properties of a [personWebsite](../resources/personwebsite.md) object.</span></span>|
|[<span data-ttu-id="560da-123">Excluir personWebsite</span><span class="sxs-lookup"><span data-stu-id="560da-123">Delete personWebsite</span></span>](../api/personwebsite-delete.md)|<span data-ttu-id="560da-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="560da-124">None</span></span>|<span data-ttu-id="560da-125">Exclui um objeto [personWebsite](../resources/personwebsite.md) .</span><span class="sxs-lookup"><span data-stu-id="560da-125">Deletes a [personWebsite](../resources/personwebsite.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="560da-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="560da-126">Properties</span></span>

| <span data-ttu-id="560da-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="560da-127">Property</span></span>     | <span data-ttu-id="560da-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="560da-128">Type</span></span>              | <span data-ttu-id="560da-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="560da-129">Description</span></span>                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|<span data-ttu-id="560da-130">categories</span><span class="sxs-lookup"><span data-stu-id="560da-130">categories</span></span>    |<span data-ttu-id="560da-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="560da-131">String collection</span></span>  | <span data-ttu-id="560da-132">Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).</span><span class="sxs-lookup"><span data-stu-id="560da-132">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="560da-133">description</span><span class="sxs-lookup"><span data-stu-id="560da-133">description</span></span>   |<span data-ttu-id="560da-134">String</span><span class="sxs-lookup"><span data-stu-id="560da-134">String</span></span>             | <span data-ttu-id="560da-135">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="560da-135">Contains a description of the website.</span></span>                                                        |
|<span data-ttu-id="560da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="560da-136">displayName</span></span>   |<span data-ttu-id="560da-137">String</span><span class="sxs-lookup"><span data-stu-id="560da-137">String</span></span>             | <span data-ttu-id="560da-138">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="560da-138">Contains a friendly name for the website.</span></span>                                                     |
|<span data-ttu-id="560da-139">webUrl</span><span class="sxs-lookup"><span data-stu-id="560da-139">webUrl</span></span>        |<span data-ttu-id="560da-140">String</span><span class="sxs-lookup"><span data-stu-id="560da-140">String</span></span>             | <span data-ttu-id="560da-141">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="560da-141">Contains a link to the website itself.</span></span>                                                        |

## <a name="properties"></a><span data-ttu-id="560da-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="560da-142">Properties</span></span>
|<span data-ttu-id="560da-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="560da-143">Property</span></span>|<span data-ttu-id="560da-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="560da-144">Type</span></span>|<span data-ttu-id="560da-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="560da-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="560da-146">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="560da-146">allowedAudiences</span></span>|<span data-ttu-id="560da-147">String</span><span class="sxs-lookup"><span data-stu-id="560da-147">String</span></span>|<span data-ttu-id="560da-148">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="560da-148">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="560da-149">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="560da-150">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="560da-150">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="560da-151">categories</span><span class="sxs-lookup"><span data-stu-id="560da-151">categories</span></span>|<span data-ttu-id="560da-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="560da-152">String collection</span></span>|<span data-ttu-id="560da-153">Contém categorias que um usuário associou ao site (por exemplo, pessoal, receitas).</span><span class="sxs-lookup"><span data-stu-id="560da-153">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="560da-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="560da-154">createdBy</span></span>|[<span data-ttu-id="560da-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="560da-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="560da-156">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="560da-156">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="560da-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="560da-158">createdDateTime</span></span>|<span data-ttu-id="560da-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="560da-159">DateTimeOffset</span></span>|<span data-ttu-id="560da-160">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="560da-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="560da-161">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-162">description</span><span class="sxs-lookup"><span data-stu-id="560da-162">description</span></span>|<span data-ttu-id="560da-163">String</span><span class="sxs-lookup"><span data-stu-id="560da-163">String</span></span>|<span data-ttu-id="560da-164">Contém uma descrição do site.</span><span class="sxs-lookup"><span data-stu-id="560da-164">Contains a description of the website.</span></span>|
|<span data-ttu-id="560da-165">displayName</span><span class="sxs-lookup"><span data-stu-id="560da-165">displayName</span></span>|<span data-ttu-id="560da-166">String</span><span class="sxs-lookup"><span data-stu-id="560da-166">String</span></span>|<span data-ttu-id="560da-167">Contém um nome amigável para o site.</span><span class="sxs-lookup"><span data-stu-id="560da-167">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="560da-168">id</span><span class="sxs-lookup"><span data-stu-id="560da-168">id</span></span>|<span data-ttu-id="560da-169">String</span><span class="sxs-lookup"><span data-stu-id="560da-169">String</span></span>|<span data-ttu-id="560da-170">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="560da-170">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="560da-171">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="560da-171">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="560da-172">fracassa</span><span class="sxs-lookup"><span data-stu-id="560da-172">inference</span></span>|[<span data-ttu-id="560da-173">inferenceData</span><span class="sxs-lookup"><span data-stu-id="560da-173">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="560da-174">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="560da-174">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="560da-175">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-175">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="560da-176">lastModifiedBy</span></span>|[<span data-ttu-id="560da-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="560da-177">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="560da-178">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="560da-178">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="560da-179">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-179">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="560da-180">lastModifiedDateTime</span></span>|<span data-ttu-id="560da-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="560da-181">DateTimeOffset</span></span>|<span data-ttu-id="560da-182">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="560da-182">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="560da-183">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-183">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-184">source</span><span class="sxs-lookup"><span data-stu-id="560da-184">source</span></span>|[<span data-ttu-id="560da-185">personDataSource</span><span class="sxs-lookup"><span data-stu-id="560da-185">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="560da-186">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="560da-186">Where the values originated if synced from another service.</span></span> <span data-ttu-id="560da-187">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="560da-187">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="560da-188">webUrl</span><span class="sxs-lookup"><span data-stu-id="560da-188">webUrl</span></span>|<span data-ttu-id="560da-189">String</span><span class="sxs-lookup"><span data-stu-id="560da-189">String</span></span>|<span data-ttu-id="560da-190">Contém um link para o próprio site.</span><span class="sxs-lookup"><span data-stu-id="560da-190">Contains a link to the website itself.</span></span>|

## <a name="relationships"></a><span data-ttu-id="560da-191">Relações</span><span class="sxs-lookup"><span data-stu-id="560da-191">Relationships</span></span>
<span data-ttu-id="560da-192">Nenhum</span><span class="sxs-lookup"><span data-stu-id="560da-192">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="560da-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="560da-193">JSON representation</span></span>
<span data-ttu-id="560da-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="560da-194">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```
