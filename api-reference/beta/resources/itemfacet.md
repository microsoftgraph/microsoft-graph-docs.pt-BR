---
title: tipo de recurso de Multiface
description: tipo de recurso de Multiface
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: bb89037b3d5b88e57ec12b2b02a5e2ed37cb2601
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939324"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="efa5b-103">tipo de recurso de Multiface</span><span class="sxs-lookup"><span data-stu-id="efa5b-103">itemFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efa5b-104">Representa o tipo de base abstrato que todos os tipos de recurso no EntitySet de [perfil](profile.md) herdam de.</span><span class="sxs-lookup"><span data-stu-id="efa5b-104">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="efa5b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efa5b-105">Properties</span></span>

| <span data-ttu-id="efa5b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa5b-106">Property</span></span>             | <span data-ttu-id="efa5b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa5b-107">Type</span></span>                            | <span data-ttu-id="efa5b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa5b-108">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="efa5b-109">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="efa5b-109">allowedAudiences</span></span>      |<span data-ttu-id="efa5b-110">string</span><span class="sxs-lookup"><span data-stu-id="efa5b-110">string</span></span>                           | <span data-ttu-id="efa5b-111">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="efa5b-111">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="efa5b-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="efa5b-112">createdBy</span></span>             |[<span data-ttu-id="efa5b-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="efa5b-113">identitySet</span></span>](identityset.md)    | <span data-ttu-id="efa5b-114">Quando a entidade foi originalmente criada.</span><span class="sxs-lookup"><span data-stu-id="efa5b-114">When the entity was originally created.</span></span>   |
|<span data-ttu-id="efa5b-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efa5b-115">createdDateTime</span></span>       |<span data-ttu-id="efa5b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa5b-116">DateTimeOffset</span></span>                   |<span data-ttu-id="efa5b-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="efa5b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="efa5b-119">id</span><span class="sxs-lookup"><span data-stu-id="efa5b-119">id</span></span>                    |<span data-ttu-id="efa5b-120">String</span><span class="sxs-lookup"><span data-stu-id="efa5b-120">String</span></span>                           | <span data-ttu-id="efa5b-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa5b-121">Read-only.</span></span>|
|<span data-ttu-id="efa5b-122">fracassa</span><span class="sxs-lookup"><span data-stu-id="efa5b-122">inference</span></span>             |[<span data-ttu-id="efa5b-123">inferenceData</span><span class="sxs-lookup"><span data-stu-id="efa5b-123">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="efa5b-124">Contém detalhes de inferência se a entidade for inferida.</span><span class="sxs-lookup"><span data-stu-id="efa5b-124">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="efa5b-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="efa5b-125">lastModifiedBy</span></span>        |[<span data-ttu-id="efa5b-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="efa5b-126">identitySet</span></span>](identityset.md)    | <span data-ttu-id="efa5b-127">Identificador do parceiro ou usuário que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="efa5b-127">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="efa5b-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efa5b-128">lastModifiedDateTime</span></span>  |<span data-ttu-id="efa5b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa5b-129">DateTimeOffset</span></span>                   |<span data-ttu-id="efa5b-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="efa5b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="efa5b-132">Relações</span><span class="sxs-lookup"><span data-stu-id="efa5b-132">Relationships</span></span>

<span data-ttu-id="efa5b-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efa5b-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa5b-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efa5b-134">JSON representation</span></span>

<span data-ttu-id="efa5b-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efa5b-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "allowedAudiences": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "inference": {"@odata.type": "microsoft.graph.inferenceData"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemFacet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->