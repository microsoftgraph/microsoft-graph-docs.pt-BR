---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ae6bdc7dc16b072090a04773de93324385401f81
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809072"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="76c08-103">tipo de recurso webaccount</span><span class="sxs-lookup"><span data-stu-id="76c08-103">webAccount resource type</span></span>

<span data-ttu-id="76c08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76c08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c08-105">Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="76c08-105">Represents web accounts the user has indicated they use or have added to their user [profile](profile.md).</span></span>

<span data-ttu-id="76c08-106">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="76c08-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="76c08-107">Methods</span></span>

|<span data-ttu-id="76c08-108">Método</span><span class="sxs-lookup"><span data-stu-id="76c08-108">Method</span></span>|<span data-ttu-id="76c08-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76c08-109">Return type</span></span>|<span data-ttu-id="76c08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76c08-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76c08-111">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="76c08-111">List webAccounts</span></span>](../api/profile-list-webaccounts.md)|<span data-ttu-id="76c08-112">coleção [Webaccount](../resources/webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="76c08-112">[webAccount](../resources/webaccount.md) collection</span></span>|<span data-ttu-id="76c08-113">Obtenha os recursos da conta da webaccount da propriedade de navegação webaccounts.</span><span class="sxs-lookup"><span data-stu-id="76c08-113">Get the webAccount resources from the webAccounts navigation property.</span></span>|
|[<span data-ttu-id="76c08-114">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="76c08-114">Create webAccount</span></span>](../api/profile-post-webaccounts.md)|[<span data-ttu-id="76c08-115">conta da</span><span class="sxs-lookup"><span data-stu-id="76c08-115">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="76c08-116">Criar um novo objeto webaccount.</span><span class="sxs-lookup"><span data-stu-id="76c08-116">Create a new webAccount object.</span></span>|
|[<span data-ttu-id="76c08-117">Obter webaccount</span><span class="sxs-lookup"><span data-stu-id="76c08-117">Get webAccount</span></span>](../api/webaccount-get.md)|[<span data-ttu-id="76c08-118">conta da</span><span class="sxs-lookup"><span data-stu-id="76c08-118">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="76c08-119">Leia as propriedades e os relacionamentos de um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="76c08-119">Read the properties and relationships of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="76c08-120">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="76c08-120">Update webAccount</span></span>](../api/webaccount-update.md)|[<span data-ttu-id="76c08-121">conta da</span><span class="sxs-lookup"><span data-stu-id="76c08-121">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="76c08-122">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="76c08-122">Update the properties of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="76c08-123">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="76c08-123">Delete webAccount</span></span>](../api/webaccount-delete.md)|<span data-ttu-id="76c08-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76c08-124">None</span></span>|<span data-ttu-id="76c08-125">Exclui um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="76c08-125">Deletes a [webAccount](../resources/webaccount.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76c08-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76c08-126">Properties</span></span>

|<span data-ttu-id="76c08-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76c08-127">Property</span></span>|<span data-ttu-id="76c08-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="76c08-128">Type</span></span>|<span data-ttu-id="76c08-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="76c08-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c08-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="76c08-130">allowedAudiences</span></span>|<span data-ttu-id="76c08-131">String</span><span class="sxs-lookup"><span data-stu-id="76c08-131">String</span></span>|<span data-ttu-id="76c08-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="76c08-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="76c08-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="76c08-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="76c08-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="76c08-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="76c08-135">createdBy</span></span>|[<span data-ttu-id="76c08-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="76c08-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="76c08-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="76c08-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="76c08-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76c08-139">createdDateTime</span></span>|<span data-ttu-id="76c08-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76c08-140">DateTimeOffset</span></span>|<span data-ttu-id="76c08-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="76c08-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="76c08-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-143">description</span><span class="sxs-lookup"><span data-stu-id="76c08-143">description</span></span>|<span data-ttu-id="76c08-144">String</span><span class="sxs-lookup"><span data-stu-id="76c08-144">String</span></span>|<span data-ttu-id="76c08-145">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="76c08-145">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="76c08-146">id</span><span class="sxs-lookup"><span data-stu-id="76c08-146">id</span></span>|<span data-ttu-id="76c08-147">String</span><span class="sxs-lookup"><span data-stu-id="76c08-147">String</span></span>|<span data-ttu-id="76c08-148">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="76c08-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="76c08-149">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="76c08-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="76c08-150">fracassa</span><span class="sxs-lookup"><span data-stu-id="76c08-150">inference</span></span>|[<span data-ttu-id="76c08-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="76c08-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="76c08-152">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="76c08-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="76c08-153">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="76c08-154">lastModifiedBy</span></span>|[<span data-ttu-id="76c08-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="76c08-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="76c08-156">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="76c08-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="76c08-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76c08-158">lastModifiedDateTime</span></span>|<span data-ttu-id="76c08-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76c08-159">DateTimeOffset</span></span>|<span data-ttu-id="76c08-160">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="76c08-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="76c08-161">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-162">service</span><span class="sxs-lookup"><span data-stu-id="76c08-162">service</span></span>|[<span data-ttu-id="76c08-163">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="76c08-163">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="76c08-164">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="76c08-164">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="76c08-165">source</span><span class="sxs-lookup"><span data-stu-id="76c08-165">source</span></span>|[<span data-ttu-id="76c08-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="76c08-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="76c08-167">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="76c08-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="76c08-168">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="76c08-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="76c08-169">statusMessage</span><span class="sxs-lookup"><span data-stu-id="76c08-169">statusMessage</span></span>|<span data-ttu-id="76c08-170">String</span><span class="sxs-lookup"><span data-stu-id="76c08-170">String</span></span>|<span data-ttu-id="76c08-171">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="76c08-171">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="76c08-172">userId</span><span class="sxs-lookup"><span data-stu-id="76c08-172">userId</span></span>|<span data-ttu-id="76c08-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76c08-173">String</span></span>|<span data-ttu-id="76c08-174">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="76c08-174">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="76c08-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="76c08-175">webUrl</span></span>|<span data-ttu-id="76c08-176">String</span><span class="sxs-lookup"><span data-stu-id="76c08-176">String</span></span>|<span data-ttu-id="76c08-177">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="76c08-177">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76c08-178">Relações</span><span class="sxs-lookup"><span data-stu-id="76c08-178">Relationships</span></span>
<span data-ttu-id="76c08-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76c08-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76c08-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76c08-180">JSON representation</span></span>
<span data-ttu-id="76c08-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76c08-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webAccount",
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
  "description": "String",
  "userId": "String",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation"
  },
  "statusMessage": "String",
  "webUrl": "String"
}
```
