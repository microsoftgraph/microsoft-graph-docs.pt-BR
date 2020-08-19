---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0c36ea4d861738316a3ce6593c12a79a59d97c68
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809401"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="5e6e7-103">tipo de recurso de Tel.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-103">itemPhone resource type</span></span>

<span data-ttu-id="5e6e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e6e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e6e7-105">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

<span data-ttu-id="5e6e7-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5e6e7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e6e7-107">Methods</span></span>

|<span data-ttu-id="5e6e7-108">Método</span><span class="sxs-lookup"><span data-stu-id="5e6e7-108">Method</span></span>|<span data-ttu-id="5e6e7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e6e7-109">Return type</span></span>|<span data-ttu-id="5e6e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6e7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e6e7-111">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="5e6e7-111">List phones</span></span>](../api/profile-list-phones.md)|<span data-ttu-id="5e6e7-112">coleção [Multiphone](../resources/itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="5e6e7-112">[itemPhone](../resources/itemphone.md) collection</span></span>|<span data-ttu-id="5e6e7-113">Obtenha os recursos de telefonia da propriedade de navegação phones.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-113">Get the itemPhone resources from the phones navigation property.</span></span>|
|[<span data-ttu-id="5e6e7-114">Criar um número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-114">Create itemPhone</span></span>](../api/profile-post-phones.md)|[<span data-ttu-id="5e6e7-115">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-115">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="5e6e7-116">Criar um novo objeto MyPhone.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-116">Create a new itemPhone object.</span></span>|
|[<span data-ttu-id="5e6e7-117">Obter o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-117">Get itemPhone</span></span>](../api/itemphone-get.md)|[<span data-ttu-id="5e6e7-118">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-118">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="5e6e7-119">Leia as propriedades e os relacionamentos de um objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="5e6e7-119">Read the properties and relationships of an [itemPhone](../resources/itemphone.md) object.</span></span>|
|[<span data-ttu-id="5e6e7-120">Atualizar o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-120">Update itemPhone</span></span>](../api/itemphone-update.md)|[<span data-ttu-id="5e6e7-121">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-121">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="5e6e7-122">Atualiza as propriedades de um objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="5e6e7-122">Update the properties of an [itemPhone](../resources/itemphone.md) object.</span></span>|
|[<span data-ttu-id="5e6e7-123">Excluir o número de telefone</span><span class="sxs-lookup"><span data-stu-id="5e6e7-123">Delete itemPhone</span></span>](../api/itemphone-delete.md)|<span data-ttu-id="5e6e7-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e6e7-124">None</span></span>|<span data-ttu-id="5e6e7-125">Exclui um objeto [MyPhone](../resources/itemphone.md) .</span><span class="sxs-lookup"><span data-stu-id="5e6e7-125">Deletes an [itemPhone](../resources/itemphone.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e6e7-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e6e7-126">Properties</span></span>

|<span data-ttu-id="5e6e7-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e6e7-127">Property</span></span>|<span data-ttu-id="5e6e7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e6e7-128">Type</span></span>|<span data-ttu-id="5e6e7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e6e7-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e6e7-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5e6e7-130">allowedAudiences</span></span>|<span data-ttu-id="5e6e7-131">String</span><span class="sxs-lookup"><span data-stu-id="5e6e7-131">String</span></span>|<span data-ttu-id="5e6e7-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5e6e7-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5e6e7-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5e6e7-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e6e7-135">createdBy</span></span>|[<span data-ttu-id="5e6e7-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e6e7-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5e6e7-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="5e6e7-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6e7-139">createdDateTime</span></span>|<span data-ttu-id="5e6e7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6e7-140">DateTimeOffset</span></span>|<span data-ttu-id="5e6e7-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="5e6e7-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5e6e7-143">displayName</span></span>|<span data-ttu-id="5e6e7-144">String</span><span class="sxs-lookup"><span data-stu-id="5e6e7-144">String</span></span>|<span data-ttu-id="5e6e7-145">Nome amigável o usuário atribuiu este número de telefone.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-145">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="5e6e7-146">id</span><span class="sxs-lookup"><span data-stu-id="5e6e7-146">id</span></span>|<span data-ttu-id="5e6e7-147">String</span><span class="sxs-lookup"><span data-stu-id="5e6e7-147">String</span></span>|<span data-ttu-id="5e6e7-148">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="5e6e7-149">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5e6e7-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="5e6e7-150">fracassa</span><span class="sxs-lookup"><span data-stu-id="5e6e7-150">inference</span></span>|[<span data-ttu-id="5e6e7-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5e6e7-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5e6e7-152">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5e6e7-153">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5e6e7-154">lastModifiedBy</span></span>|[<span data-ttu-id="5e6e7-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e6e7-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5e6e7-156">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="5e6e7-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e6e7-158">lastModifiedDateTime</span></span>|<span data-ttu-id="5e6e7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e6e7-159">DateTimeOffset</span></span>|<span data-ttu-id="5e6e7-160">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="5e6e7-161">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-162">number</span><span class="sxs-lookup"><span data-stu-id="5e6e7-162">number</span></span>|<span data-ttu-id="5e6e7-163">String</span><span class="sxs-lookup"><span data-stu-id="5e6e7-163">String</span></span>|<span data-ttu-id="5e6e7-164">Número de telefone fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-164">Phone number provided by the user.</span></span>|
|<span data-ttu-id="5e6e7-165">source</span><span class="sxs-lookup"><span data-stu-id="5e6e7-165">source</span></span>|[<span data-ttu-id="5e6e7-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5e6e7-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5e6e7-167">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5e6e7-168">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e7-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e6e7-169">type</span><span class="sxs-lookup"><span data-stu-id="5e6e7-169">type</span></span>|<span data-ttu-id="5e6e7-170">PhoneType</span><span class="sxs-lookup"><span data-stu-id="5e6e7-170">phoneType</span></span>|<span data-ttu-id="5e6e7-171">O tipo de número de telefone dentro do objeto.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-171">The type of phone number within the object.</span></span> <span data-ttu-id="5e6e7-172">Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-172">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e6e7-173">Relações</span><span class="sxs-lookup"><span data-stu-id="5e6e7-173">Relationships</span></span>

<span data-ttu-id="5e6e7-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e6e7-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e6e7-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e6e7-175">JSON representation</span></span>

<span data-ttu-id="5e6e7-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e6e7-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.itemPhone",
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
  "displayName": "String",
  "type": "String",
  "number": "String"
}
```
