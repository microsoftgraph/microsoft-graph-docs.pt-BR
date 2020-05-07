---
title: tipo de recurso shiftPreferences
description: Representa a disponibilidade de um usuário a ser atribuída a turnos no cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 91a6093ad66d906fe9917ae7a22d2297ded4b4d7
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154854"
---
# <a name="shiftpreferences-resource-type"></a><span data-ttu-id="f1671-103">tipo de recurso shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f1671-103">shiftPreferences resource type</span></span>

<span data-ttu-id="f1671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1671-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1671-105">Representa a disponibilidade de um usuário a ser atribuída a turnos no [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f1671-105">Represents a user's availability to be assigned shifts in the [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f1671-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1671-106">Methods</span></span>

| <span data-ttu-id="f1671-107">Método</span><span class="sxs-lookup"><span data-stu-id="f1671-107">Method</span></span>       | <span data-ttu-id="f1671-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1671-108">Return Type</span></span> | <span data-ttu-id="f1671-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1671-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f1671-110">Get</span><span class="sxs-lookup"><span data-stu-id="f1671-110">Get</span></span>](../api/shiftpreferences-get.md) | [<span data-ttu-id="f1671-111">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f1671-111">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="f1671-112">Leia as propriedades e os relacionamentos de um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="f1671-112">Read the properties and relationships of a **shiftPreferences** object.</span></span> |
| [<span data-ttu-id="f1671-113">Update</span><span class="sxs-lookup"><span data-stu-id="f1671-113">Update</span></span>](../api/shiftpreferences-put.md) | [<span data-ttu-id="f1671-114">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f1671-114">shiftPreferences</span></span>](shiftpreferences.md) | <span data-ttu-id="f1671-115">Atualizar um objeto **shiftPreferences** .</span><span class="sxs-lookup"><span data-stu-id="f1671-115">Update a **shiftPreferences** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f1671-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1671-116">Properties</span></span>

|<span data-ttu-id="f1671-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1671-117">Property</span></span>          |<span data-ttu-id="f1671-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1671-118">Type</span></span>           |<span data-ttu-id="f1671-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1671-119">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f1671-120">id</span><span class="sxs-lookup"><span data-stu-id="f1671-120">id</span></span> | `Edm.String` | <span data-ttu-id="f1671-121">O identificador da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1671-121">The identifier of the entity.</span></span> |
| <span data-ttu-id="f1671-122">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="f1671-122">@odata.etag</span></span> | `Edm.String` | <span data-ttu-id="f1671-123">A chave de alteração da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1671-123">The change key for the entity.</span></span> |
| <span data-ttu-id="f1671-124">availability</span><span class="sxs-lookup"><span data-stu-id="f1671-124">availability</span></span> | <span data-ttu-id="f1671-125">coleção [shiftAvailability](shiftavailability.md)</span><span class="sxs-lookup"><span data-stu-id="f1671-125">[shiftAvailability](shiftavailability.md) collection</span></span> | <span data-ttu-id="f1671-126">Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="f1671-126">Availability of the user to be scheduled for work and its recurrence pattern.</span></span> |
| <span data-ttu-id="f1671-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1671-127">createdDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="f1671-128">Carimbo de data/hora correspondente a quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="f1671-128">Timestamp corresponding to when the entity was created.</span></span> |
| <span data-ttu-id="f1671-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1671-129">lastModifiedDateTime</span></span> | `Edm.DateTimeOffset` | <span data-ttu-id="f1671-130">Carimbo de data/hora correspondente a quando a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f1671-130">Timestamp corresponding to when the entity was last modified.</span></span> |
| <span data-ttu-id="f1671-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f1671-131">lastModifiedBy</span></span> | [<span data-ttu-id="f1671-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="f1671-132">identitySet</span></span>](identityset.md) | <span data-ttu-id="f1671-133">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f1671-133">Identity of the person who last modified the entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1671-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f1671-134">Relationships</span></span>

<span data-ttu-id="f1671-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1671-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1671-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1671-136">JSON representation</span></span>

<span data-ttu-id="f1671-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1671-137">The following is a JSON representation of the resource.</span></span>

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
