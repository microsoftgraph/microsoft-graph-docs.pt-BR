---
title: tipo de recurso de endereço
description: tipo de recurso de endereço
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ca6848b6b5ac60d419e56914a59e2470d5970ed9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075634"
---
# <a name="itemaddress-resource-type"></a><span data-ttu-id="8a6ee-103">tipo de recurso de endereço</span><span class="sxs-lookup"><span data-stu-id="8a6ee-103">itemAddress resource type</span></span>

<span data-ttu-id="8a6ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a6ee-105">Representa um endereço físico e detalhes do local onde o endereço é encontrado.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-105">Represents a physical address and details of the location where the address is found.</span></span>

<span data-ttu-id="8a6ee-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8a6ee-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8a6ee-107">Methods</span></span>
|<span data-ttu-id="8a6ee-108">Método</span><span class="sxs-lookup"><span data-stu-id="8a6ee-108">Method</span></span>|<span data-ttu-id="8a6ee-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8a6ee-109">Return type</span></span>|<span data-ttu-id="8a6ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a6ee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a6ee-111">Listar endereços</span><span class="sxs-lookup"><span data-stu-id="8a6ee-111">List addresses</span></span>](../api/profile-list-addresses.md)|<span data-ttu-id="8a6ee-112">coleção [myAddress](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="8a6ee-112">[itemAddress](../resources/itemaddress.md) collection</span></span>|<span data-ttu-id="8a6ee-113">Obtenha os recursos de endereço da propriedade de navegação addresses.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-113">Get the itemAddress resources from the addresses navigation property.</span></span>|
|[<span data-ttu-id="8a6ee-114">Criar endereço</span><span class="sxs-lookup"><span data-stu-id="8a6ee-114">Create itemAddress</span></span>](../api/profile-post-addresses.md)|[<span data-ttu-id="8a6ee-115">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="8a6ee-115">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="8a6ee-116">Criar um novo objeto de endereço.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-116">Create a new itemAddress object.</span></span>|
|[<span data-ttu-id="8a6ee-117">Get endereço</span><span class="sxs-lookup"><span data-stu-id="8a6ee-117">Get itemAddress</span></span>](../api/itemaddress-get.md)|[<span data-ttu-id="8a6ee-118">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="8a6ee-118">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="8a6ee-119">Leia as propriedades e os relacionamentos de [um objeto](../resources/itemaddress.md) item.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-119">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="8a6ee-120">Atualizar endereço</span><span class="sxs-lookup"><span data-stu-id="8a6ee-120">Update itemAddress</span></span>](../api/itemaddress-update.md)|[<span data-ttu-id="8a6ee-121">Endereço do destinatário</span><span class="sxs-lookup"><span data-stu-id="8a6ee-121">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="8a6ee-122">Atualizar as propriedades [de um objeto](../resources/itemaddress.md) item.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-122">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="8a6ee-123">Excluir endereço</span><span class="sxs-lookup"><span data-stu-id="8a6ee-123">Delete itemAddress</span></span>](../api/itemaddress-delete.md)|<span data-ttu-id="8a6ee-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a6ee-124">None</span></span>|<span data-ttu-id="8a6ee-125">Exclui um objeto [myAddress](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="8a6ee-125">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a6ee-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a6ee-126">Properties</span></span>
|<span data-ttu-id="8a6ee-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a6ee-127">Property</span></span>|<span data-ttu-id="8a6ee-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a6ee-128">Type</span></span>|<span data-ttu-id="8a6ee-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a6ee-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6ee-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8a6ee-130">allowedAudiences</span></span>|<span data-ttu-id="8a6ee-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a6ee-131">String</span></span>|<span data-ttu-id="8a6ee-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8a6ee-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8a6ee-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8a6ee-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="8a6ee-135">createdBy</span></span>|[<span data-ttu-id="8a6ee-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a6ee-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8a6ee-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="8a6ee-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a6ee-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a6ee-139">createdDateTime</span></span>|<span data-ttu-id="8a6ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a6ee-140">DateTimeOffset</span></span>|<span data-ttu-id="8a6ee-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="8a6ee-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a6ee-143">detalhada</span><span class="sxs-lookup"><span data-stu-id="8a6ee-143">detail</span></span>|[<span data-ttu-id="8a6ee-144">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8a6ee-144">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8a6ee-145">Detalhes sobre o próprio endereço.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-145">Details about the address itself.</span></span>|
|<span data-ttu-id="8a6ee-146">displayName</span><span class="sxs-lookup"><span data-stu-id="8a6ee-146">displayName</span></span>|<span data-ttu-id="8a6ee-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a6ee-147">String</span></span>|<span data-ttu-id="8a6ee-148">Nome amigável que o usuário atribuiu a este endereço.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-148">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="8a6ee-149">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8a6ee-149">geoCoordinates</span></span>|[<span data-ttu-id="8a6ee-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8a6ee-150">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="8a6ee-151">As geocoordenas do endereço.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-151">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="8a6ee-152">id</span><span class="sxs-lookup"><span data-stu-id="8a6ee-152">id</span></span>|<span data-ttu-id="8a6ee-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a6ee-153">String</span></span>|<span data-ttu-id="8a6ee-154">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="8a6ee-155">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="8a6ee-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="8a6ee-156">fracassa</span><span class="sxs-lookup"><span data-stu-id="8a6ee-156">inference</span></span>|[<span data-ttu-id="8a6ee-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8a6ee-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8a6ee-158">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8a6ee-159">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a6ee-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8a6ee-160">lastModifiedBy</span></span>|[<span data-ttu-id="8a6ee-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a6ee-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8a6ee-162">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="8a6ee-163">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a6ee-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a6ee-164">lastModifiedDateTime</span></span>|<span data-ttu-id="8a6ee-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a6ee-165">DateTimeOffset</span></span>|<span data-ttu-id="8a6ee-166">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="8a6ee-167">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a6ee-168">source</span><span class="sxs-lookup"><span data-stu-id="8a6ee-168">source</span></span>|[<span data-ttu-id="8a6ee-169">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8a6ee-169">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8a6ee-170">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-170">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8a6ee-171">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a6ee-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a6ee-172">Relações</span><span class="sxs-lookup"><span data-stu-id="8a6ee-172">Relationships</span></span>
<span data-ttu-id="8a6ee-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a6ee-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6ee-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a6ee-174">JSON representation</span></span>
<span data-ttu-id="8a6ee-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a6ee-175">The following is a JSON representation of the resource.</span></span>
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


