---
title: tipo de recurso de endereço
description: tipo de recurso de endereço
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ea99085ca04ea85b78a2fee1b80525ef934856a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809606"
---
# <a name="itemaddress-resource-type"></a><span data-ttu-id="697fd-103">tipo de recurso de endereço</span><span class="sxs-lookup"><span data-stu-id="697fd-103">itemAddress resource type</span></span>

<span data-ttu-id="697fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="697fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="697fd-105">Representa um endereço físico e detalhes do local onde o endereço é encontrado.</span><span class="sxs-lookup"><span data-stu-id="697fd-105">Represents a physical address and details of the location where the address is found.</span></span>

<span data-ttu-id="697fd-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="697fd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="697fd-107">Methods</span></span>
|<span data-ttu-id="697fd-108">Método</span><span class="sxs-lookup"><span data-stu-id="697fd-108">Method</span></span>|<span data-ttu-id="697fd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="697fd-109">Return type</span></span>|<span data-ttu-id="697fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="697fd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="697fd-111">Listar endereços</span><span class="sxs-lookup"><span data-stu-id="697fd-111">List addresses</span></span>](../api/profile-list-addresses.md)|<span data-ttu-id="697fd-112">coleção [myAddress](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="697fd-112">[itemAddress](../resources/itemaddress.md) collection</span></span>|<span data-ttu-id="697fd-113">Obtenha os recursos de endereço da propriedade de navegação addresses.</span><span class="sxs-lookup"><span data-stu-id="697fd-113">Get the itemAddress resources from the addresses navigation property.</span></span>|
|[<span data-ttu-id="697fd-114">Criar endereço</span><span class="sxs-lookup"><span data-stu-id="697fd-114">Create itemAddress</span></span>](../api/profile-post-addresses.md)|[<span data-ttu-id="697fd-115">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="697fd-115">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="697fd-116">Criar um novo objeto de endereço.</span><span class="sxs-lookup"><span data-stu-id="697fd-116">Create a new itemAddress object.</span></span>|
|[<span data-ttu-id="697fd-117">Get endereço</span><span class="sxs-lookup"><span data-stu-id="697fd-117">Get itemAddress</span></span>](../api/itemaddress-get.md)|[<span data-ttu-id="697fd-118">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="697fd-118">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="697fd-119">Leia as propriedades e os relacionamentos de [um objeto](../resources/itemaddress.md) item.</span><span class="sxs-lookup"><span data-stu-id="697fd-119">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="697fd-120">Atualizar endereço</span><span class="sxs-lookup"><span data-stu-id="697fd-120">Update itemAddress</span></span>](../api/itemaddress-update.md)|[<span data-ttu-id="697fd-121">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="697fd-121">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="697fd-122">Atualizar as propriedades [de um objeto](../resources/itemaddress.md) item.</span><span class="sxs-lookup"><span data-stu-id="697fd-122">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="697fd-123">Excluir endereço</span><span class="sxs-lookup"><span data-stu-id="697fd-123">Delete itemAddress</span></span>](../api/itemaddress-delete.md)|<span data-ttu-id="697fd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="697fd-124">None</span></span>|<span data-ttu-id="697fd-125">Exclui um objeto [myAddress](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="697fd-125">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="697fd-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="697fd-126">Properties</span></span>
|<span data-ttu-id="697fd-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="697fd-127">Property</span></span>|<span data-ttu-id="697fd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="697fd-128">Type</span></span>|<span data-ttu-id="697fd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="697fd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="697fd-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="697fd-130">allowedAudiences</span></span>|<span data-ttu-id="697fd-131">String</span><span class="sxs-lookup"><span data-stu-id="697fd-131">String</span></span>|<span data-ttu-id="697fd-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="697fd-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="697fd-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="697fd-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="697fd-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="697fd-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="697fd-135">createdBy</span></span>|[<span data-ttu-id="697fd-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="697fd-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="697fd-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="697fd-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="697fd-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="697fd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="697fd-139">createdDateTime</span></span>|<span data-ttu-id="697fd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="697fd-140">DateTimeOffset</span></span>|<span data-ttu-id="697fd-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="697fd-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="697fd-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="697fd-143">detalhada</span><span class="sxs-lookup"><span data-stu-id="697fd-143">detail</span></span>|[<span data-ttu-id="697fd-144">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="697fd-144">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="697fd-145">Detalhes sobre o próprio endereço.</span><span class="sxs-lookup"><span data-stu-id="697fd-145">Details about the address itself.</span></span>|
|<span data-ttu-id="697fd-146">displayName</span><span class="sxs-lookup"><span data-stu-id="697fd-146">displayName</span></span>|<span data-ttu-id="697fd-147">String</span><span class="sxs-lookup"><span data-stu-id="697fd-147">String</span></span>|<span data-ttu-id="697fd-148">Nome amigável que o usuário atribuiu a este endereço.</span><span class="sxs-lookup"><span data-stu-id="697fd-148">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="697fd-149">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="697fd-149">geoCoordinates</span></span>|[<span data-ttu-id="697fd-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="697fd-150">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="697fd-151">As geocoordenas do endereço.</span><span class="sxs-lookup"><span data-stu-id="697fd-151">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="697fd-152">id</span><span class="sxs-lookup"><span data-stu-id="697fd-152">id</span></span>|<span data-ttu-id="697fd-153">String</span><span class="sxs-lookup"><span data-stu-id="697fd-153">String</span></span>|<span data-ttu-id="697fd-154">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="697fd-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="697fd-155">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="697fd-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="697fd-156">fracassa</span><span class="sxs-lookup"><span data-stu-id="697fd-156">inference</span></span>|[<span data-ttu-id="697fd-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="697fd-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="697fd-158">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="697fd-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="697fd-159">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="697fd-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="697fd-160">lastModifiedBy</span></span>|[<span data-ttu-id="697fd-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="697fd-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="697fd-162">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="697fd-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="697fd-163">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="697fd-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="697fd-164">lastModifiedDateTime</span></span>|<span data-ttu-id="697fd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="697fd-165">DateTimeOffset</span></span>|<span data-ttu-id="697fd-166">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="697fd-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="697fd-167">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="697fd-168">source</span><span class="sxs-lookup"><span data-stu-id="697fd-168">source</span></span>|[<span data-ttu-id="697fd-169">personDataSource</span><span class="sxs-lookup"><span data-stu-id="697fd-169">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="697fd-170">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="697fd-170">Where the values originated if synced from another service.</span></span> <span data-ttu-id="697fd-171">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="697fd-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="697fd-172">Relações</span><span class="sxs-lookup"><span data-stu-id="697fd-172">Relationships</span></span>
<span data-ttu-id="697fd-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="697fd-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="697fd-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="697fd-174">JSON representation</span></span>
<span data-ttu-id="697fd-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="697fd-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
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
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```
