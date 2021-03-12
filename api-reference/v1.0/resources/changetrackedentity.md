---
title: Tipo de recurso changeTrackedEntity
description: Representa uma entidade para controlar as alterações feitas em qualquer recurso Shifts com suporte
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6037e8ff07c79834dd8929ec93997c2a26282d28
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719791"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="3e4a8-103">Tipo de recurso changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="3e4a8-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="3e4a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e4a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e4a8-105">Representa uma entidade para controlar as alterações feitas em qualquer agenda [com](schedule.md) suporte e recurso associado.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3e4a8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e4a8-106">Properties</span></span>

| <span data-ttu-id="3e4a8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e4a8-107">Property</span></span>     | <span data-ttu-id="3e4a8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e4a8-108">Type</span></span>        | <span data-ttu-id="3e4a8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e4a8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e4a8-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4a8-110">createdDateTime</span></span>|<span data-ttu-id="3e4a8-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4a8-111">DateTimeOffset</span></span>|<span data-ttu-id="3e4a8-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e4a8-113">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="3e4a8-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="3e4a8-114">id</span><span class="sxs-lookup"><span data-stu-id="3e4a8-114">id</span></span>|<span data-ttu-id="3e4a8-115">String</span><span class="sxs-lookup"><span data-stu-id="3e4a8-115">String</span></span>| <span data-ttu-id="3e4a8-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-116">Read-only.</span></span>|
|<span data-ttu-id="3e4a8-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3e4a8-117">lastModifiedBy</span></span>|[<span data-ttu-id="3e4a8-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="3e4a8-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="3e4a8-119">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="3e4a8-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4a8-120">lastModifiedDateTime</span></span>|<span data-ttu-id="3e4a8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4a8-121">DateTimeOffset</span></span>|<span data-ttu-id="3e4a8-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e4a8-123">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="3e4a8-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e4a8-124">Relações</span><span class="sxs-lookup"><span data-stu-id="3e4a8-124">Relationships</span></span>

<span data-ttu-id="3e4a8-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e4a8-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e4a8-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e4a8-126">JSON representation</span></span>

<span data-ttu-id="3e4a8-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e4a8-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "changeTrackedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

