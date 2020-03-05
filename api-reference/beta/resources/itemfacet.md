---
title: tipo de recurso de Multiface
description: tipo de recurso de Multiface
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: efd4977872dfefc5a0e5be9b10ad1fa196fa20a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523069"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="c7186-103">tipo de recurso de Multiface</span><span class="sxs-lookup"><span data-stu-id="c7186-103">itemFacet resource type</span></span>

<span data-ttu-id="c7186-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7186-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7186-105">Representa o tipo de base abstrato que todos os tipos de recurso no EntitySet de [perfil](profile.md) herdam de.</span><span class="sxs-lookup"><span data-stu-id="c7186-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="c7186-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7186-106">Properties</span></span>

| <span data-ttu-id="c7186-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7186-107">Property</span></span>             | <span data-ttu-id="c7186-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7186-108">Type</span></span>                            | <span data-ttu-id="c7186-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7186-109">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="c7186-110">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c7186-110">allowedAudiences</span></span>      |<span data-ttu-id="c7186-111">string</span><span class="sxs-lookup"><span data-stu-id="c7186-111">string</span></span>                           | <span data-ttu-id="c7186-112">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c7186-112">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="c7186-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c7186-113">createdBy</span></span>             |[<span data-ttu-id="c7186-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c7186-114">identitySet</span></span>](identityset.md)    | <span data-ttu-id="c7186-115">Quando a entidade foi originalmente criada.</span><span class="sxs-lookup"><span data-stu-id="c7186-115">When the entity was originally created.</span></span>   |
|<span data-ttu-id="c7186-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7186-116">createdDateTime</span></span>       |<span data-ttu-id="c7186-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7186-117">DateTimeOffset</span></span>                   |<span data-ttu-id="c7186-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c7186-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c7186-120">id</span><span class="sxs-lookup"><span data-stu-id="c7186-120">id</span></span>                    |<span data-ttu-id="c7186-121">String</span><span class="sxs-lookup"><span data-stu-id="c7186-121">String</span></span>                           | <span data-ttu-id="c7186-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7186-122">Read-only.</span></span>|
|<span data-ttu-id="c7186-123">fracassa</span><span class="sxs-lookup"><span data-stu-id="c7186-123">inference</span></span>             |[<span data-ttu-id="c7186-124">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c7186-124">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="c7186-125">Contém detalhes de inferência se a entidade for inferida.</span><span class="sxs-lookup"><span data-stu-id="c7186-125">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="c7186-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c7186-126">lastModifiedBy</span></span>        |[<span data-ttu-id="c7186-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="c7186-127">identitySet</span></span>](identityset.md)    | <span data-ttu-id="c7186-128">Identificador do parceiro ou usuário que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c7186-128">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="c7186-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7186-129">lastModifiedDateTime</span></span>  |<span data-ttu-id="c7186-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7186-130">DateTimeOffset</span></span>                   |<span data-ttu-id="c7186-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c7186-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7186-133">Relações</span><span class="sxs-lookup"><span data-stu-id="c7186-133">Relationships</span></span>

<span data-ttu-id="c7186-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7186-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7186-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7186-135">JSON representation</span></span>

<span data-ttu-id="c7186-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7186-136">The following is a JSON representation of the resource.</span></span>

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