---
title: tipo de recurso de email
description: tipo de recurso de email
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a8a69ae484afab6b558890fbd186a4850235ead
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809422"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="adcf1-103">tipo de recurso de email</span><span class="sxs-lookup"><span data-stu-id="adcf1-103">itemEmail resource type</span></span>

<span data-ttu-id="adcf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adcf1-105">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="adcf1-105">Represents detailed information about email addresses associated with the user.</span></span>

<span data-ttu-id="adcf1-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="adcf1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="adcf1-107">Methods</span></span>
|<span data-ttu-id="adcf1-108">Método</span><span class="sxs-lookup"><span data-stu-id="adcf1-108">Method</span></span>|<span data-ttu-id="adcf1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="adcf1-109">Return type</span></span>|<span data-ttu-id="adcf1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="adcf1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="adcf1-111">Listar emails</span><span class="sxs-lookup"><span data-stu-id="adcf1-111">List emails</span></span>](../api/profile-list-emails.md)|<span data-ttu-id="adcf1-112">coleção [email](../resources/itememail.md)</span><span class="sxs-lookup"><span data-stu-id="adcf1-112">[itemEmail](../resources/itememail.md) collection</span></span>|<span data-ttu-id="adcf1-113">Obtenha os recursos de email da propriedade de navegação emails.</span><span class="sxs-lookup"><span data-stu-id="adcf1-113">Get the itemEmail resources from the emails navigation property.</span></span>|
|[<span data-ttu-id="adcf1-114">Criar email</span><span class="sxs-lookup"><span data-stu-id="adcf1-114">Create itemEmail</span></span>](../api/profile-post-emails.md)|[<span data-ttu-id="adcf1-115">Email</span><span class="sxs-lookup"><span data-stu-id="adcf1-115">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="adcf1-116">Criar um novo objeto de email.</span><span class="sxs-lookup"><span data-stu-id="adcf1-116">Create a new itemEmail object.</span></span>|
|[<span data-ttu-id="adcf1-117">Obter email</span><span class="sxs-lookup"><span data-stu-id="adcf1-117">Get itemEmail</span></span>](../api/itememail-get.md)|[<span data-ttu-id="adcf1-118">Email</span><span class="sxs-lookup"><span data-stu-id="adcf1-118">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="adcf1-119">Leia as propriedades e os relacionamentos de um objeto item de [email](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="adcf1-119">Read the properties and relationships of an [itemEmail](../resources/itememail.md) object.</span></span>|
|[<span data-ttu-id="adcf1-120">Atualizar email</span><span class="sxs-lookup"><span data-stu-id="adcf1-120">Update itemEmail</span></span>](../api/itememail-update.md)|[<span data-ttu-id="adcf1-121">Email</span><span class="sxs-lookup"><span data-stu-id="adcf1-121">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="adcf1-122">Atualiza as propriedades de um objeto item de [email](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="adcf1-122">Update the properties of an [itemEmail](../resources/itememail.md) object.</span></span>|
|[<span data-ttu-id="adcf1-123">Excluir email</span><span class="sxs-lookup"><span data-stu-id="adcf1-123">Delete itemEmail</span></span>](../api/itememail-delete.md)|<span data-ttu-id="adcf1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="adcf1-124">None</span></span>|<span data-ttu-id="adcf1-125">Exclui um objeto [MyEmail](../resources/itememail.md) .</span><span class="sxs-lookup"><span data-stu-id="adcf1-125">Deletes an [itemEmail](../resources/itememail.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="adcf1-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adcf1-126">Properties</span></span>
|<span data-ttu-id="adcf1-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adcf1-127">Property</span></span>|<span data-ttu-id="adcf1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="adcf1-128">Type</span></span>|<span data-ttu-id="adcf1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="adcf1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adcf1-130">address</span><span class="sxs-lookup"><span data-stu-id="adcf1-130">address</span></span>|<span data-ttu-id="adcf1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adcf1-131">String</span></span>|<span data-ttu-id="adcf1-132">O próprio endereço de email.</span><span class="sxs-lookup"><span data-stu-id="adcf1-132">The email address itself.</span></span>|
|<span data-ttu-id="adcf1-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="adcf1-133">allowedAudiences</span></span>|<span data-ttu-id="adcf1-134">String</span><span class="sxs-lookup"><span data-stu-id="adcf1-134">String</span></span>|<span data-ttu-id="adcf1-135">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="adcf1-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="adcf1-136">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="adcf1-137">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="adcf1-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="adcf1-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="adcf1-138">createdBy</span></span>|[<span data-ttu-id="adcf1-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="adcf1-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="adcf1-140">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="adcf1-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="adcf1-141">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adcf1-142">createdDateTime</span></span>|<span data-ttu-id="adcf1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adcf1-143">DateTimeOffset</span></span>|<span data-ttu-id="adcf1-144">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="adcf1-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="adcf1-145">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-146">displayName</span><span class="sxs-lookup"><span data-stu-id="adcf1-146">displayName</span></span>|<span data-ttu-id="adcf1-147">String</span><span class="sxs-lookup"><span data-stu-id="adcf1-147">String</span></span>|<span data-ttu-id="adcf1-148">O nome ou rótulo que um usuário associou a um endereço de email específico.</span><span class="sxs-lookup"><span data-stu-id="adcf1-148">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="adcf1-149">id</span><span class="sxs-lookup"><span data-stu-id="adcf1-149">id</span></span>|<span data-ttu-id="adcf1-150">String</span><span class="sxs-lookup"><span data-stu-id="adcf1-150">String</span></span>|<span data-ttu-id="adcf1-151">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="adcf1-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="adcf1-152">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="adcf1-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="adcf1-153">fracassa</span><span class="sxs-lookup"><span data-stu-id="adcf1-153">inference</span></span>|[<span data-ttu-id="adcf1-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="adcf1-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="adcf1-155">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="adcf1-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="adcf1-156">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="adcf1-157">lastModifiedBy</span></span>|[<span data-ttu-id="adcf1-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="adcf1-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="adcf1-159">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="adcf1-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="adcf1-160">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adcf1-161">lastModifiedDateTime</span></span>|<span data-ttu-id="adcf1-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adcf1-162">DateTimeOffset</span></span>|<span data-ttu-id="adcf1-163">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="adcf1-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="adcf1-164">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-165">source</span><span class="sxs-lookup"><span data-stu-id="adcf1-165">source</span></span>|[<span data-ttu-id="adcf1-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="adcf1-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="adcf1-167">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="adcf1-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="adcf1-168">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="adcf1-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="adcf1-169">type</span><span class="sxs-lookup"><span data-stu-id="adcf1-169">type</span></span>|<span data-ttu-id="adcf1-170">emailtype</span><span class="sxs-lookup"><span data-stu-id="adcf1-170">emailType</span></span>|<span data-ttu-id="adcf1-171">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="adcf1-171">The type of email address.</span></span> <span data-ttu-id="adcf1-172">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="adcf1-172">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adcf1-173">Relações</span><span class="sxs-lookup"><span data-stu-id="adcf1-173">Relationships</span></span>
<span data-ttu-id="adcf1-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="adcf1-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adcf1-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adcf1-175">JSON representation</span></span>
<span data-ttu-id="adcf1-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="adcf1-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "0f30bf5d-bf5d-0f30-5dbf-300f5dbf300f",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```
