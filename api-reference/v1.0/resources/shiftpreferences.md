---
title: tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuída a turnos no cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c1f2b4acdc61fcf7889ea0b9dd1046aff112c9e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970660"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="f03d6-103">tipo de recurso shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f03d6-103">shiftPreferences resource type</span></span>

<span data-ttu-id="f03d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f03d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f03d6-105">Representa a disponibilidade de um usuário a ser atribuída a turnos no [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f03d6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="f03d6-106">Methods</span></span>

| <span data-ttu-id="f03d6-107">Método</span><span class="sxs-lookup"><span data-stu-id="f03d6-107">Method</span></span>       | <span data-ttu-id="f03d6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f03d6-108">Return Type</span></span> | <span data-ttu-id="f03d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f03d6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f03d6-110">Get</span><span class="sxs-lookup"><span data-stu-id="f03d6-110">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="f03d6-111">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f03d6-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="f03d6-112">Leia as propriedades e os relacionamentos de um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="f03d6-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="f03d6-113">Atualização</span><span class="sxs-lookup"><span data-stu-id="f03d6-113">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="f03d6-114">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f03d6-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="f03d6-115">Atualizar um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="f03d6-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f03d6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f03d6-116">Properties</span></span>

|<span data-ttu-id="f03d6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f03d6-117">Property</span></span>          |<span data-ttu-id="f03d6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f03d6-118">Type</span></span>           |<span data-ttu-id="f03d6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f03d6-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f03d6-120">id</span><span class="sxs-lookup"><span data-stu-id="f03d6-120">id</span></span> | `Edm.String` | <span data-ttu-id="f03d6-121">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="f03d6-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="f03d6-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="f03d6-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="f03d6-123">A chave de alteração da entidade.</span><span class="sxs-lookup"><span data-stu-id="f03d6-123">The change key for the entity.</span></span> |
| <span data-ttu-id="f03d6-124">availability</span><span class="sxs-lookup"><span data-stu-id="f03d6-124">availability</span></span> | <span data-ttu-id="f03d6-125">coleção [shiftAvailability](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="f03d6-126">Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="f03d6-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="f03d6-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f03d6-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="f03d6-128">Carimbo de data/hora correspondente a quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="f03d6-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="f03d6-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f03d6-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="f03d6-130">Carimbo de data/hora correspondente a quando a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f03d6-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="f03d6-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f03d6-131">lastModifiedBy</span></span> | [<span data-ttu-id="f03d6-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="f03d6-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="f03d6-133">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f03d6-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f03d6-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f03d6-134">Relationships</span></span>

<span data-ttu-id="f03d6-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f03d6-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f03d6-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f03d6-136">JSON representation</span></span>

<span data-ttu-id="f03d6-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f03d6-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "availability": [{"@odata.type": "microsoft.graph.shiftAvailability"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

