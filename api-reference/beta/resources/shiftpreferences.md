---
title: tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuída a turnos no cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d35f77e7d048adb0b0bb49604423bbe2ff53031c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058024"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="52ef7-103">tipo de recurso shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="52ef7-103">shiftPreferences resource type</span></span>

<span data-ttu-id="52ef7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52ef7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ef7-105">Representa a disponibilidade de um usuário a ser atribuída a turnos no [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="52ef7-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="52ef7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52ef7-106">Methods</span></span>

| <span data-ttu-id="52ef7-107">Método</span><span class="sxs-lookup"><span data-stu-id="52ef7-107">Method</span></span>       | <span data-ttu-id="52ef7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52ef7-108">Return Type</span></span> | <span data-ttu-id="52ef7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ef7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52ef7-110">Get</span><span class="sxs-lookup"><span data-stu-id="52ef7-110">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="52ef7-111">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="52ef7-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="52ef7-112">Leia as propriedades e os relacionamentos de um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="52ef7-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="52ef7-113">Update</span><span class="sxs-lookup"><span data-stu-id="52ef7-113">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="52ef7-114">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="52ef7-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="52ef7-115">Atualizar um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="52ef7-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52ef7-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52ef7-116">Properties</span></span>

|<span data-ttu-id="52ef7-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52ef7-117">Property</span></span>          |<span data-ttu-id="52ef7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ef7-118">Type</span></span>           |<span data-ttu-id="52ef7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ef7-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="52ef7-120">id</span><span class="sxs-lookup"><span data-stu-id="52ef7-120">id</span></span> | `Edm.String` | <span data-ttu-id="52ef7-121">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="52ef7-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="52ef7-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="52ef7-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="52ef7-123">A chave de alteração da entidade.</span><span class="sxs-lookup"><span data-stu-id="52ef7-123">The change key for the entity.</span></span> |
| <span data-ttu-id="52ef7-124">availability</span><span class="sxs-lookup"><span data-stu-id="52ef7-124">availability</span></span> | <span data-ttu-id="52ef7-125">coleção [shiftAvailability](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="52ef7-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="52ef7-126">Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="52ef7-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="52ef7-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52ef7-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="52ef7-128">Carimbo de data/hora correspondente a quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="52ef7-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="52ef7-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52ef7-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="52ef7-130">Carimbo de data/hora correspondente a quando a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="52ef7-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="52ef7-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="52ef7-131">lastModifiedBy</span></span> | [<span data-ttu-id="52ef7-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="52ef7-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="52ef7-133">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="52ef7-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="52ef7-134">Relações</span><span class="sxs-lookup"><span data-stu-id="52ef7-134">Relationships</span></span>

<span data-ttu-id="52ef7-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52ef7-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52ef7-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52ef7-136">JSON representation</span></span>

<span data-ttu-id="52ef7-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52ef7-137">The following is a JSON representation of the resource.</span></span>

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


