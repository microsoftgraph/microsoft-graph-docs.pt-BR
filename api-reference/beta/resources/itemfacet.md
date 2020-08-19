---
title: tipo de recurso de Multiface
description: tipo de recurso de Multiface
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b32baed9dd6bad45f37b7be24b67308e0624b42c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809394"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="6b042-103">tipo de recurso de Multiface</span><span class="sxs-lookup"><span data-stu-id="6b042-103">itemFacet resource type</span></span>

<span data-ttu-id="6b042-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b042-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b042-105">Representa o tipo de base abstrato que todos os tipos de recurso no EntitySet de [perfil](profile.md) herdam de.</span><span class="sxs-lookup"><span data-stu-id="6b042-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="6b042-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b042-106">Properties</span></span>
|<span data-ttu-id="6b042-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b042-107">Property</span></span>|<span data-ttu-id="6b042-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b042-108">Type</span></span>|<span data-ttu-id="6b042-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b042-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b042-110">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="6b042-110">allowedAudiences</span></span>|<span data-ttu-id="6b042-111">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="6b042-111">allowedAudiences</span></span>|<span data-ttu-id="6b042-112">As audiências que podem ver os valores contidos na entidade associada.</span><span class="sxs-lookup"><span data-stu-id="6b042-112">The audiences that are able to see the values contained within the associated entity.</span></span> <span data-ttu-id="6b042-113">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6b042-113">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6b042-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="6b042-114">createdBy</span></span>|[<span data-ttu-id="6b042-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b042-115">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="6b042-116">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="6b042-116">Provides the identifier of the user and/or application that created the entity.</span></span>|
|<span data-ttu-id="6b042-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b042-117">createdDateTime</span></span>|<span data-ttu-id="6b042-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b042-118">DateTimeOffset</span></span>|<span data-ttu-id="6b042-119">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="6b042-119">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="6b042-120">id</span><span class="sxs-lookup"><span data-stu-id="6b042-120">id</span></span>|<span data-ttu-id="6b042-121">String</span><span class="sxs-lookup"><span data-stu-id="6b042-121">String</span></span>|<span data-ttu-id="6b042-122">Identificador usado para endereçamento individual de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="6b042-122">Identifier used for individually addressing an entity.</span></span> <span data-ttu-id="6b042-123">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="6b042-123">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="6b042-124">fracassa</span><span class="sxs-lookup"><span data-stu-id="6b042-124">inference</span></span>|[<span data-ttu-id="6b042-125">inferenceData</span><span class="sxs-lookup"><span data-stu-id="6b042-125">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="6b042-126">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="6b042-126">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span>|
|<span data-ttu-id="6b042-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6b042-127">lastModifiedBy</span></span>|[<span data-ttu-id="6b042-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b042-128">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="6b042-129">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6b042-129">Provides the identifier of the user and/or application that last modified the entity.</span></span>|
|<span data-ttu-id="6b042-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b042-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6b042-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b042-131">DateTimeOffset</span></span>|<span data-ttu-id="6b042-132">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="6b042-132">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="6b042-133">source</span><span class="sxs-lookup"><span data-stu-id="6b042-133">source</span></span>|[<span data-ttu-id="6b042-134">personDataSource</span><span class="sxs-lookup"><span data-stu-id="6b042-134">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="6b042-135">Onde os valores de uma entidade se originaram se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="6b042-135">Where the values within an entity originated if synced from another service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b042-136">Relações</span><span class="sxs-lookup"><span data-stu-id="6b042-136">Relationships</span></span>
<span data-ttu-id="6b042-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b042-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b042-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b042-138">JSON representation</span></span>
<span data-ttu-id="6b042-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b042-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemFacet",
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
  }
}
```

