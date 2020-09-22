---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 29d66809d14cfc72d43286aef801490cef20cb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057673"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="13b7c-103">tipo de recurso webaccount</span><span class="sxs-lookup"><span data-stu-id="13b7c-103">webAccount resource type</span></span>

<span data-ttu-id="13b7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13b7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13b7c-105">Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="13b7c-105">Represents web accounts the user has indicated they use or have added to their user [profile](profile.md).</span></span>

<span data-ttu-id="13b7c-106">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13b7c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="13b7c-107">Methods</span></span>

|<span data-ttu-id="13b7c-108">Método</span><span class="sxs-lookup"><span data-stu-id="13b7c-108">Method</span></span>|<span data-ttu-id="13b7c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13b7c-109">Return type</span></span>|<span data-ttu-id="13b7c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13b7c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13b7c-111">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="13b7c-111">List webAccounts</span></span>](../api/profile-list-webaccounts.md)|<span data-ttu-id="13b7c-112">coleção [Webaccount](../resources/webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="13b7c-112">[webAccount](../resources/webaccount.md) collection</span></span>|<span data-ttu-id="13b7c-113">Obtenha os recursos da conta da webaccount da propriedade de navegação webaccounts.</span><span class="sxs-lookup"><span data-stu-id="13b7c-113">Get the webAccount resources from the webAccounts navigation property.</span></span>|
|[<span data-ttu-id="13b7c-114">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="13b7c-114">Create webAccount</span></span>](../api/profile-post-webaccounts.md)|[<span data-ttu-id="13b7c-115">conta da</span><span class="sxs-lookup"><span data-stu-id="13b7c-115">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="13b7c-116">Criar um novo objeto webaccount.</span><span class="sxs-lookup"><span data-stu-id="13b7c-116">Create a new webAccount object.</span></span>|
|[<span data-ttu-id="13b7c-117">Obter webaccount</span><span class="sxs-lookup"><span data-stu-id="13b7c-117">Get webAccount</span></span>](../api/webaccount-get.md)|[<span data-ttu-id="13b7c-118">conta da</span><span class="sxs-lookup"><span data-stu-id="13b7c-118">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="13b7c-119">Leia as propriedades e os relacionamentos de um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="13b7c-119">Read the properties and relationships of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="13b7c-120">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="13b7c-120">Update webAccount</span></span>](../api/webaccount-update.md)|[<span data-ttu-id="13b7c-121">conta da</span><span class="sxs-lookup"><span data-stu-id="13b7c-121">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="13b7c-122">Atualizar as propriedades de um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="13b7c-122">Update the properties of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="13b7c-123">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="13b7c-123">Delete webAccount</span></span>](../api/webaccount-delete.md)|<span data-ttu-id="13b7c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13b7c-124">None</span></span>|<span data-ttu-id="13b7c-125">Exclui um objeto [webaccount](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="13b7c-125">Deletes a [webAccount](../resources/webaccount.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13b7c-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13b7c-126">Properties</span></span>

|<span data-ttu-id="13b7c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13b7c-127">Property</span></span>|<span data-ttu-id="13b7c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="13b7c-128">Type</span></span>|<span data-ttu-id="13b7c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="13b7c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b7c-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="13b7c-130">allowedAudiences</span></span>|<span data-ttu-id="13b7c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13b7c-131">String</span></span>|<span data-ttu-id="13b7c-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="13b7c-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="13b7c-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="13b7c-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="13b7c-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="13b7c-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="13b7c-135">createdBy</span></span>|[<span data-ttu-id="13b7c-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="13b7c-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="13b7c-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="13b7c-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="13b7c-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13b7c-139">createdDateTime</span></span>|<span data-ttu-id="13b7c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13b7c-140">DateTimeOffset</span></span>|<span data-ttu-id="13b7c-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="13b7c-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="13b7c-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-143">description</span><span class="sxs-lookup"><span data-stu-id="13b7c-143">description</span></span>|<span data-ttu-id="13b7c-144">String</span><span class="sxs-lookup"><span data-stu-id="13b7c-144">String</span></span>|<span data-ttu-id="13b7c-145">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="13b7c-145">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="13b7c-146">id</span><span class="sxs-lookup"><span data-stu-id="13b7c-146">id</span></span>|<span data-ttu-id="13b7c-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13b7c-147">String</span></span>|<span data-ttu-id="13b7c-148">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="13b7c-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="13b7c-149">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="13b7c-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="13b7c-150">fracassa</span><span class="sxs-lookup"><span data-stu-id="13b7c-150">inference</span></span>|[<span data-ttu-id="13b7c-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="13b7c-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="13b7c-152">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="13b7c-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="13b7c-153">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="13b7c-154">lastModifiedBy</span></span>|[<span data-ttu-id="13b7c-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="13b7c-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="13b7c-156">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="13b7c-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="13b7c-157">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13b7c-158">lastModifiedDateTime</span></span>|<span data-ttu-id="13b7c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13b7c-159">DateTimeOffset</span></span>|<span data-ttu-id="13b7c-160">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="13b7c-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="13b7c-161">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-162">service</span><span class="sxs-lookup"><span data-stu-id="13b7c-162">service</span></span>|[<span data-ttu-id="13b7c-163">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="13b7c-163">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="13b7c-164">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="13b7c-164">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="13b7c-165">source</span><span class="sxs-lookup"><span data-stu-id="13b7c-165">source</span></span>|[<span data-ttu-id="13b7c-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="13b7c-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="13b7c-167">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="13b7c-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="13b7c-168">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="13b7c-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="13b7c-169">statusMessage</span><span class="sxs-lookup"><span data-stu-id="13b7c-169">statusMessage</span></span>|<span data-ttu-id="13b7c-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13b7c-170">String</span></span>|<span data-ttu-id="13b7c-171">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="13b7c-171">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="13b7c-172">userId</span><span class="sxs-lookup"><span data-stu-id="13b7c-172">userId</span></span>|<span data-ttu-id="13b7c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13b7c-173">String</span></span>|<span data-ttu-id="13b7c-174">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="13b7c-174">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="13b7c-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="13b7c-175">webUrl</span></span>|<span data-ttu-id="13b7c-176">String</span><span class="sxs-lookup"><span data-stu-id="13b7c-176">String</span></span>|<span data-ttu-id="13b7c-177">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="13b7c-177">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b7c-178">Relações</span><span class="sxs-lookup"><span data-stu-id="13b7c-178">Relationships</span></span>
<span data-ttu-id="13b7c-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13b7c-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13b7c-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13b7c-180">JSON representation</span></span>
<span data-ttu-id="13b7c-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13b7c-181">The following is a JSON representation of the resource.</span></span>
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


