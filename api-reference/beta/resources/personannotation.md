---
title: tipo de recurso personAnnotation
description: tipo de recurso personAnnotation
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 757797a8a252f934050cb8425f49042707734ed5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812896"
---
# <a name="personannotation-resource-type"></a><span data-ttu-id="8815f-103">tipo de recurso personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-103">personAnnotation resource type</span></span>

<span data-ttu-id="8815f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8815f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8815f-105">Fornece informações sobre as anotações que o usuário já associou em vários serviços e compartilhou com outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="8815f-105">Provides information within notes that the user has associated with themselves in various services and shared with others.</span></span>

<span data-ttu-id="8815f-106">Herda de [Myfacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8815f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8815f-107">Methods</span></span>
|<span data-ttu-id="8815f-108">Método</span><span class="sxs-lookup"><span data-stu-id="8815f-108">Method</span></span>|<span data-ttu-id="8815f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8815f-109">Return type</span></span>|<span data-ttu-id="8815f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8815f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8815f-111">Listar anotações</span><span class="sxs-lookup"><span data-stu-id="8815f-111">List notes</span></span>](../api/profile-list-notes.md)|<span data-ttu-id="8815f-112">coleção [personAnnotation](../resources/personannotation.md)</span><span class="sxs-lookup"><span data-stu-id="8815f-112">[personAnnotation](../resources/personannotation.md) collection</span></span>|<span data-ttu-id="8815f-113">Obtenha os recursos personAnnotation da propriedade de navegação Notes.</span><span class="sxs-lookup"><span data-stu-id="8815f-113">Get the personAnnotation resources from the notes navigation property.</span></span>|
|[<span data-ttu-id="8815f-114">Criar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-114">Create personAnnotation</span></span>](../api/profile-post-notes.md)|[<span data-ttu-id="8815f-115">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-115">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="8815f-116">Criar um novo objeto personAnnotation.</span><span class="sxs-lookup"><span data-stu-id="8815f-116">Create a new personAnnotation object.</span></span>|
|[<span data-ttu-id="8815f-117">Obter personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-117">Get personAnnotation</span></span>](../api/personannotation-get.md)|[<span data-ttu-id="8815f-118">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-118">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="8815f-119">Leia as propriedades e os relacionamentos de um objeto [personAnnotation](../resources/personannotation.md) .</span><span class="sxs-lookup"><span data-stu-id="8815f-119">Read the properties and relationships of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="8815f-120">Atualizar personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-120">Update personAnnotation</span></span>](../api/personannotation-update.md)|[<span data-ttu-id="8815f-121">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-121">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="8815f-122">Atualiza as propriedades de um objeto [personAnnotation](../resources/personannotation.md) .</span><span class="sxs-lookup"><span data-stu-id="8815f-122">Update the properties of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="8815f-123">Excluir personAnnotation</span><span class="sxs-lookup"><span data-stu-id="8815f-123">Delete personAnnotation</span></span>](../api/personannotation-delete.md)|<span data-ttu-id="8815f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8815f-124">None</span></span>|<span data-ttu-id="8815f-125">Exclui um objeto [personAnnotation](../resources/personannotation.md) .</span><span class="sxs-lookup"><span data-stu-id="8815f-125">Deletes a [personAnnotation](../resources/personannotation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8815f-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8815f-126">Properties</span></span>
|<span data-ttu-id="8815f-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8815f-127">Property</span></span>|<span data-ttu-id="8815f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8815f-128">Type</span></span>|<span data-ttu-id="8815f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8815f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8815f-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8815f-130">allowedAudiences</span></span>|<span data-ttu-id="8815f-131">String</span><span class="sxs-lookup"><span data-stu-id="8815f-131">String</span></span>|<span data-ttu-id="8815f-132">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="8815f-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8815f-133">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8815f-134">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8815f-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8815f-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="8815f-135">createdBy</span></span>|[<span data-ttu-id="8815f-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="8815f-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8815f-137">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="8815f-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="8815f-138">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8815f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8815f-139">createdDateTime</span></span>|<span data-ttu-id="8815f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8815f-140">DateTimeOffset</span></span>|<span data-ttu-id="8815f-141">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="8815f-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="8815f-142">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8815f-143">detalhada</span><span class="sxs-lookup"><span data-stu-id="8815f-143">detail</span></span>|[<span data-ttu-id="8815f-144">itemBody</span><span class="sxs-lookup"><span data-stu-id="8815f-144">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="8815f-145">Contém os detalhes da anotação propriamente dita.</span><span class="sxs-lookup"><span data-stu-id="8815f-145">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="8815f-146">displayName</span><span class="sxs-lookup"><span data-stu-id="8815f-146">displayName</span></span>|<span data-ttu-id="8815f-147">String</span><span class="sxs-lookup"><span data-stu-id="8815f-147">String</span></span>|<span data-ttu-id="8815f-148">Contém um nome amigável para a anotação.</span><span class="sxs-lookup"><span data-stu-id="8815f-148">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="8815f-149">id</span><span class="sxs-lookup"><span data-stu-id="8815f-149">id</span></span>|<span data-ttu-id="8815f-150">String</span><span class="sxs-lookup"><span data-stu-id="8815f-150">String</span></span>|<span data-ttu-id="8815f-151">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="8815f-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="8815f-152">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="8815f-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="8815f-153">fracassa</span><span class="sxs-lookup"><span data-stu-id="8815f-153">inference</span></span>|[<span data-ttu-id="8815f-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8815f-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8815f-155">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="8815f-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8815f-156">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8815f-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8815f-157">lastModifiedBy</span></span>|[<span data-ttu-id="8815f-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="8815f-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8815f-159">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8815f-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="8815f-160">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8815f-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8815f-161">lastModifiedDateTime</span></span>|<span data-ttu-id="8815f-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8815f-162">DateTimeOffset</span></span>|<span data-ttu-id="8815f-163">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="8815f-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="8815f-164">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8815f-165">source</span><span class="sxs-lookup"><span data-stu-id="8815f-165">source</span></span>|[<span data-ttu-id="8815f-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8815f-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8815f-167">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="8815f-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8815f-168">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8815f-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8815f-169">Relações</span><span class="sxs-lookup"><span data-stu-id="8815f-169">Relationships</span></span>
<span data-ttu-id="8815f-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8815f-170">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8815f-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8815f-171">JSON representation</span></span>
<span data-ttu-id="8815f-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8815f-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```