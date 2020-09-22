---
title: tipo de recurso de patente
description: tipo de recurso de patente
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7e6732a53f841902422348f90dada22174813b39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089287"
---
# <a name="itempatent-resource-type"></a><span data-ttu-id="cb986-103">tipo de recurso de patente</span><span class="sxs-lookup"><span data-stu-id="cb986-103">itemPatent resource type</span></span>
 
<span data-ttu-id="cb986-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb986-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb986-105">Representa uma patente concedida ou em um campo que foi adicionada ao [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cb986-105">Represents a granted or filed patent which has been added to a user's [profile](../resources/profile.md).</span></span>

<span data-ttu-id="cb986-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb986-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb986-107">Methods</span></span>
|<span data-ttu-id="cb986-108">Método</span><span class="sxs-lookup"><span data-stu-id="cb986-108">Method</span></span>|<span data-ttu-id="cb986-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb986-109">Return type</span></span>|<span data-ttu-id="cb986-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb986-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb986-111">Listar patentes</span><span class="sxs-lookup"><span data-stu-id="cb986-111">List patents</span></span>](../api/profile-list-patents.md)|<span data-ttu-id="cb986-112">coleção [Ispatenteado](../resources/itempatent.md)</span><span class="sxs-lookup"><span data-stu-id="cb986-112">[itemPatent](../resources/itempatent.md) collection</span></span>|<span data-ttu-id="cb986-113">Obtenha os recursos de patente da propriedade de navegação patentes.</span><span class="sxs-lookup"><span data-stu-id="cb986-113">Get the itemPatent resources from the patents navigation property.</span></span>|
|[<span data-ttu-id="cb986-114">Criar ispatente</span><span class="sxs-lookup"><span data-stu-id="cb986-114">Create itemPatent</span></span>](../api/profile-post-patents.md)|[<span data-ttu-id="cb986-115">Patente</span><span class="sxs-lookup"><span data-stu-id="cb986-115">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="cb986-116">Criar um novo objeto de patente.</span><span class="sxs-lookup"><span data-stu-id="cb986-116">Create a new itemPatent object.</span></span>|
|[<span data-ttu-id="cb986-117">Obter ispatente</span><span class="sxs-lookup"><span data-stu-id="cb986-117">Get itemPatent</span></span>](../api/itempatent-get.md)|[<span data-ttu-id="cb986-118">Patente</span><span class="sxs-lookup"><span data-stu-id="cb986-118">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="cb986-119">Leia as propriedades e os relacionamentos de um objeto de [patente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="cb986-119">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>|
|[<span data-ttu-id="cb986-120">Atualizar a ispatente</span><span class="sxs-lookup"><span data-stu-id="cb986-120">Update itemPatent</span></span>](../api/itempatent-update.md)|[<span data-ttu-id="cb986-121">Patente</span><span class="sxs-lookup"><span data-stu-id="cb986-121">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="cb986-122">Atualiza as propriedades de um objeto [dopatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="cb986-122">Update the properties of an [itemPatent](../resources/itempatent.md) object.</span></span>|
|[<span data-ttu-id="cb986-123">Excluir a ispatente</span><span class="sxs-lookup"><span data-stu-id="cb986-123">Delete itemPatent</span></span>](../api/itempatent-delete.md)|<span data-ttu-id="cb986-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb986-124">None</span></span>|<span data-ttu-id="cb986-125">Exclui um objeto [ispatente](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="cb986-125">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb986-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb986-126">Properties</span></span>
|<span data-ttu-id="cb986-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb986-127">Property</span></span>|<span data-ttu-id="cb986-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb986-128">Type</span></span>|<span data-ttu-id="cb986-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb986-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb986-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="cb986-130">allowedAudiences</span></span>|<span data-ttu-id="cb986-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-131">String</span></span>|<span data-ttu-id="cb986-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="cb986-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="cb986-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="cb986-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cb986-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cb986-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="cb986-135">createdBy</span></span>|[<span data-ttu-id="cb986-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="cb986-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="cb986-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="cb986-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="cb986-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb986-139">createdDateTime</span></span>|<span data-ttu-id="cb986-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb986-140">DateTimeOffset</span></span>|<span data-ttu-id="cb986-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="cb986-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="cb986-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-143">description</span><span class="sxs-lookup"><span data-stu-id="cb986-143">description</span></span>|<span data-ttu-id="cb986-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-144">String</span></span>|<span data-ttu-id="cb986-145">Descpription da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="cb986-145">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="cb986-146">displayName</span><span class="sxs-lookup"><span data-stu-id="cb986-146">displayName</span></span>|<span data-ttu-id="cb986-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-147">String</span></span>|<span data-ttu-id="cb986-148">Título da patente ou do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="cb986-148">Title of the patent or filing.</span></span> |
|<span data-ttu-id="cb986-149">id</span><span class="sxs-lookup"><span data-stu-id="cb986-149">id</span></span>|<span data-ttu-id="cb986-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-150">String</span></span>|<span data-ttu-id="cb986-151">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="cb986-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="cb986-152">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="cb986-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="cb986-153">fracassa</span><span class="sxs-lookup"><span data-stu-id="cb986-153">inference</span></span>|[<span data-ttu-id="cb986-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="cb986-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="cb986-155">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="cb986-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="cb986-156">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-157">ispending</span><span class="sxs-lookup"><span data-stu-id="cb986-157">isPending</span></span>        |<span data-ttu-id="cb986-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb986-158">Boolean</span></span>     |<span data-ttu-id="cb986-159">Indica que a patente está pendente.</span><span class="sxs-lookup"><span data-stu-id="cb986-159">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="cb986-160">issuedDate</span><span class="sxs-lookup"><span data-stu-id="cb986-160">issuedDate</span></span>       |<span data-ttu-id="cb986-161">Data</span><span class="sxs-lookup"><span data-stu-id="cb986-161">Date</span></span>        |<span data-ttu-id="cb986-162">A data em que a patente foi concedida.</span><span class="sxs-lookup"><span data-stu-id="cb986-162">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="cb986-163">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="cb986-163">issuingAuthority</span></span> |<span data-ttu-id="cb986-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-164">String</span></span>      |<span data-ttu-id="cb986-165">Autoridade que concedeu a patente.</span><span class="sxs-lookup"><span data-stu-id="cb986-165">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="cb986-166">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cb986-166">lastModifiedBy</span></span>|[<span data-ttu-id="cb986-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="cb986-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="cb986-168">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cb986-168">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="cb986-169">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-169">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb986-170">lastModifiedDateTime</span></span>|<span data-ttu-id="cb986-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb986-171">DateTimeOffset</span></span>|<span data-ttu-id="cb986-172">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="cb986-172">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="cb986-173">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-173">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-174">number</span><span class="sxs-lookup"><span data-stu-id="cb986-174">number</span></span>           |<span data-ttu-id="cb986-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb986-175">String</span></span>      |<span data-ttu-id="cb986-176">O número de patente.</span><span class="sxs-lookup"><span data-stu-id="cb986-176">The patent number.</span></span>                      |
|<span data-ttu-id="cb986-177">source</span><span class="sxs-lookup"><span data-stu-id="cb986-177">source</span></span>|[<span data-ttu-id="cb986-178">personDataSource</span><span class="sxs-lookup"><span data-stu-id="cb986-178">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="cb986-179">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="cb986-179">Where the values originated if synced from another service.</span></span> <span data-ttu-id="cb986-180">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="cb986-180">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cb986-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="cb986-181">webUrl</span></span>           |<span data-ttu-id="cb986-182">String</span><span class="sxs-lookup"><span data-stu-id="cb986-182">String</span></span>      |<span data-ttu-id="cb986-183">URL que faz referência à patente ou ao arquivamento.</span><span class="sxs-lookup"><span data-stu-id="cb986-183">URL referencing the patent or filing.</span></span> |


## <a name="relationships"></a><span data-ttu-id="cb986-184">Relações</span><span class="sxs-lookup"><span data-stu-id="cb986-184">Relationships</span></span>
<span data-ttu-id="cb986-185">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb986-185">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb986-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb986-186">JSON representation</span></span>
<span data-ttu-id="cb986-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb986-187">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
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
  "displayName": "String",
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```


