---
title: Tipo de recurso serviceAnnouncementBase
description: Esse é um tipo de base abstrato para serviceHealthIssue e serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 46e1e6428d1371683a8ad1febae990146a9fe898
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109068"
---
# <a name="serviceannouncementbase-resource-type"></a><span data-ttu-id="4307f-103">Tipo de recurso serviceAnnouncementBase</span><span class="sxs-lookup"><span data-stu-id="4307f-103">serviceAnnouncementBase resource type</span></span>

<span data-ttu-id="4307f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4307f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4307f-105">Este é um tipo de base abstrato [para serviceHealthIssue](../resources/servicehealthissue.md) e [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span><span class="sxs-lookup"><span data-stu-id="4307f-105">This is an abstract base type for [serviceHealthIssue](../resources/servicehealthissue.md) and [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

<span data-ttu-id="4307f-106">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="4307f-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4307f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4307f-107">Methods</span></span>
<span data-ttu-id="4307f-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4307f-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="4307f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4307f-109">Properties</span></span>
|<span data-ttu-id="4307f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4307f-110">Property</span></span>|<span data-ttu-id="4307f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4307f-111">Type</span></span>|<span data-ttu-id="4307f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4307f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4307f-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="4307f-113">details</span></span>|<span data-ttu-id="4307f-114">Coleção([keyValuePair](../resources/keyvaluepair.md))</span><span class="sxs-lookup"><span data-stu-id="4307f-114">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="4307f-115">Detalhes adicionais sobre o evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-115">Additional details about service event.</span></span> <span data-ttu-id="4307f-116">Essa propriedade não dá suporte a filtros.</span><span class="sxs-lookup"><span data-stu-id="4307f-116">This property doesn't support filters.</span></span>|
|<span data-ttu-id="4307f-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4307f-117">endDateTime</span></span>|<span data-ttu-id="4307f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4307f-118">DateTimeOffset</span></span>|<span data-ttu-id="4307f-119">A hora de término do evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-119">The end time of the service event.</span></span>|
|<span data-ttu-id="4307f-120">id</span><span class="sxs-lookup"><span data-stu-id="4307f-120">id</span></span>|<span data-ttu-id="4307f-121">String</span><span class="sxs-lookup"><span data-stu-id="4307f-121">String</span></span>|<span data-ttu-id="4307f-122">A id do evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-122">The id of the service event.</span></span>|
|<span data-ttu-id="4307f-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4307f-123">lastModifiedDateTime</span></span>|<span data-ttu-id="4307f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4307f-124">DateTimeOffset</span></span>|<span data-ttu-id="4307f-125">A última hora modificada do evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-125">The last modified time of the service event.</span></span>|
|<span data-ttu-id="4307f-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4307f-126">startDateTime</span></span>|<span data-ttu-id="4307f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4307f-127">DateTimeOffset</span></span>|<span data-ttu-id="4307f-128">A hora de início do evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-128">The start time of the service event.</span></span>|
|<span data-ttu-id="4307f-129">title</span><span class="sxs-lookup"><span data-stu-id="4307f-129">title</span></span>|<span data-ttu-id="4307f-130">String</span><span class="sxs-lookup"><span data-stu-id="4307f-130">String</span></span>|<span data-ttu-id="4307f-131">O título do evento de serviço.</span><span class="sxs-lookup"><span data-stu-id="4307f-131">The title of the service event.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4307f-132">Relações</span><span class="sxs-lookup"><span data-stu-id="4307f-132">Relationships</span></span>
<span data-ttu-id="4307f-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4307f-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4307f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4307f-134">JSON representation</span></span>
<span data-ttu-id="4307f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4307f-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```