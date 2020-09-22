---
title: tipo de recurso changeTrackedEntity
description: Representa uma entidade para controlar as alterações feitas em qualquer recurso de turnos com suporte
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2b4e569df025277d1b9a39e9e10110631bbb6537
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009356"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="f57b5-103">tipo de recurso changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="f57b5-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="f57b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f57b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f57b5-105">Representa uma entidade para rastrear as alterações feitas em qualquer [cronograma](schedule.md) compatível e recurso associado.</span><span class="sxs-lookup"><span data-stu-id="f57b5-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f57b5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f57b5-106">Properties</span></span>

| <span data-ttu-id="f57b5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f57b5-107">Property</span></span>     | <span data-ttu-id="f57b5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f57b5-108">Type</span></span>        | <span data-ttu-id="f57b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f57b5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f57b5-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f57b5-110">createdDateTime</span></span>|<span data-ttu-id="f57b5-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f57b5-111">DateTimeOffset</span></span>|<span data-ttu-id="f57b5-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f57b5-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f57b5-114">id</span><span class="sxs-lookup"><span data-stu-id="f57b5-114">id</span></span>|<span data-ttu-id="f57b5-115">String</span><span class="sxs-lookup"><span data-stu-id="f57b5-115">String</span></span>| <span data-ttu-id="f57b5-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f57b5-116">Read-only.</span></span>|
|<span data-ttu-id="f57b5-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f57b5-117">lastModifiedBy</span></span>|[<span data-ttu-id="f57b5-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="f57b5-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="f57b5-119">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f57b5-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="f57b5-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f57b5-120">lastModifiedDateTime</span></span>|<span data-ttu-id="f57b5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f57b5-121">DateTimeOffset</span></span>|<span data-ttu-id="f57b5-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f57b5-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="f57b5-124">Relações</span><span class="sxs-lookup"><span data-stu-id="f57b5-124">Relationships</span></span>

<span data-ttu-id="f57b5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f57b5-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f57b5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f57b5-126">JSON representation</span></span>

<span data-ttu-id="f57b5-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f57b5-127">The following is a JSON representation of the resource.</span></span>

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

