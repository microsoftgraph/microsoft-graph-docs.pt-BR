---
title: tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuída a turnos no cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 083b0ad81ffee25d8a03bf5ff38815d2ca0155a8
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952269"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="fa728-103">tipo de recurso shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="fa728-103">shiftPreferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa728-104">Representa a disponibilidade de um usuário a ser atribuída a turnos no [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="fa728-104">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fa728-105">Methods</span><span class="sxs-lookup"><span data-stu-id="fa728-105">Methods</span></span>

| <span data-ttu-id="fa728-106">Método</span><span class="sxs-lookup"><span data-stu-id="fa728-106">Method</span></span>       | <span data-ttu-id="fa728-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fa728-107">Return Type</span></span> | <span data-ttu-id="fa728-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa728-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fa728-109">Get</span><span class="sxs-lookup"><span data-stu-id="fa728-109">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="fa728-110">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="fa728-110">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="fa728-111">Leia as propriedades e os relacionamentos de um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="fa728-111">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="fa728-112">Update</span><span class="sxs-lookup"><span data-stu-id="fa728-112">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="fa728-113">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="fa728-113">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="fa728-114">Atualizar um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="fa728-114">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fa728-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa728-115">Properties</span></span>

|<span data-ttu-id="fa728-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa728-116">Property</span></span>          |<span data-ttu-id="fa728-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa728-117">Type</span></span>           |<span data-ttu-id="fa728-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa728-118">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fa728-119">id</span><span class="sxs-lookup"><span data-stu-id="fa728-119">id</span></span> | `Edm.String` | <span data-ttu-id="fa728-120">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="fa728-120">The identifier of the entity.</span></span> |
| <span data-ttu-id="fa728-121">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="fa728-121">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="fa728-122">A chave de alteração da entidade.</span><span class="sxs-lookup"><span data-stu-id="fa728-122">The change key for the entity.</span></span> |
| <span data-ttu-id="fa728-123">availability</span><span class="sxs-lookup"><span data-stu-id="fa728-123">availability</span></span> | <span data-ttu-id="fa728-124">coleção [shiftAvailability](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="fa728-124">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="fa728-125">Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="fa728-125">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="fa728-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa728-126">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="fa728-127">Carimbo de data/hora correspondente a quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="fa728-127">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="fa728-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa728-128">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="fa728-129">Carimbo de data/hora correspondente a quando a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fa728-129">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="fa728-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fa728-130">lastModifiedBy</span></span> | [<span data-ttu-id="fa728-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa728-131">identitySet</span></span>](identityset.md) | <span data-ttu-id="fa728-132">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fa728-132">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fa728-133">Relações</span><span class="sxs-lookup"><span data-stu-id="fa728-133">Relationships</span></span>

<span data-ttu-id="fa728-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa728-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa728-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa728-135">JSON representation</span></span>

<span data-ttu-id="fa728-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa728-136">The following is a JSON representation of the resource.</span></span>

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
