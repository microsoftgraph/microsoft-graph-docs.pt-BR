---
title: tipo de recurso changeTrackedEntity
description: Representa uma entidade para controlar as alterações feitas em qualquer recurso de turnos com suporte
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c420274f6ff8e0521f9fd5baca193e95334f3de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042687"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="5820d-103">tipo de recurso changeTrackedEntity</span><span class="sxs-lookup"><span data-stu-id="5820d-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="5820d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5820d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5820d-105">Representa uma entidade para rastrear as alterações feitas em qualquer [cronograma](schedule.md) compatível e recurso associado.</span><span class="sxs-lookup"><span data-stu-id="5820d-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5820d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5820d-106">Properties</span></span>

| <span data-ttu-id="5820d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5820d-107">Property</span></span>     | <span data-ttu-id="5820d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5820d-108">Type</span></span>        | <span data-ttu-id="5820d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5820d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5820d-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5820d-110">createdDateTime</span></span>|<span data-ttu-id="5820d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5820d-111">DateTimeOffset</span></span>|<span data-ttu-id="5820d-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5820d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5820d-114">id</span><span class="sxs-lookup"><span data-stu-id="5820d-114">id</span></span>|<span data-ttu-id="5820d-115">String</span><span class="sxs-lookup"><span data-stu-id="5820d-115">String</span></span>| <span data-ttu-id="5820d-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5820d-116">Read-only.</span></span>|
|<span data-ttu-id="5820d-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5820d-117">lastModifiedBy</span></span>|[<span data-ttu-id="5820d-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="5820d-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="5820d-119">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5820d-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="5820d-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5820d-120">lastModifiedDateTime</span></span>|<span data-ttu-id="5820d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5820d-121">DateTimeOffset</span></span>|<span data-ttu-id="5820d-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5820d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="5820d-124">Relações</span><span class="sxs-lookup"><span data-stu-id="5820d-124">Relationships</span></span>

<span data-ttu-id="5820d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5820d-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5820d-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5820d-126">JSON representation</span></span>

<span data-ttu-id="5820d-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5820d-127">The following is a JSON representation of the resource.</span></span>

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


