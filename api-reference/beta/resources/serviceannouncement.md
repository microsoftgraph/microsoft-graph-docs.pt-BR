---
title: Tipo de recurso serviceAnnouncement
description: Um contêiner de nível superior para recursos de comunicações de serviço
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c22cbcd9fd8e67137e649cc099ff7980468c246f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109069"
---
# <a name="serviceannouncement-resource-type"></a><span data-ttu-id="9d21f-103">Tipo de recurso serviceAnnouncement</span><span class="sxs-lookup"><span data-stu-id="9d21f-103">serviceAnnouncement resource type</span></span>

<span data-ttu-id="9d21f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d21f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d21f-105">Um contêiner de nível superior para recursos de comunicações de serviço.</span><span class="sxs-lookup"><span data-stu-id="9d21f-105">A top-level container for service communications resources.</span></span>

## <a name="methods"></a><span data-ttu-id="9d21f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9d21f-106">Methods</span></span>
|<span data-ttu-id="9d21f-107">Método</span><span class="sxs-lookup"><span data-stu-id="9d21f-107">Method</span></span>|<span data-ttu-id="9d21f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d21f-108">Return type</span></span>|<span data-ttu-id="9d21f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d21f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d21f-110">Listar healthOverviews</span><span class="sxs-lookup"><span data-stu-id="9d21f-110">List healthOverviews</span></span>](../api/serviceannouncement-list-healthoverviews.md)|<span data-ttu-id="9d21f-111">[Coleção serviceHealth](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="9d21f-111">[serviceHealth](../resources/servicehealth.md) collection</span></span>|<span data-ttu-id="9d21f-112">Obter os recursos serviceHealth da propriedade de navegação healthOverviews.</span><span class="sxs-lookup"><span data-stu-id="9d21f-112">Get the serviceHealth resources from the healthOverviews navigation property.</span></span>|
|[<span data-ttu-id="9d21f-113">Listar problemas</span><span class="sxs-lookup"><span data-stu-id="9d21f-113">List issues</span></span>](../api/serviceannouncement-list-issues.md)|<span data-ttu-id="9d21f-114">[Coleção serviceHealthIssue](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="9d21f-114">[serviceHealthIssue](../resources/servicehealthissue.md) collection</span></span>|<span data-ttu-id="9d21f-115">Obter os recursos serviceHealthIssue da propriedade de navegação de problemas.</span><span class="sxs-lookup"><span data-stu-id="9d21f-115">Get the serviceHealthIssue resources from the issues navigation property.</span></span>|
|[<span data-ttu-id="9d21f-116">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="9d21f-116">List messages</span></span>](../api/serviceannouncement-list-messages.md)|<span data-ttu-id="9d21f-117">[Coleção serviceUpdateMessage](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="9d21f-117">[serviceUpdateMessage](../resources/serviceupdatemessage.md) collection</span></span>|<span data-ttu-id="9d21f-118">Obter os recursos serviceUpdateMessage da propriedade de navegação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="9d21f-118">Get the serviceUpdateMessage resources from the messages navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d21f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d21f-119">Properties</span></span>
<span data-ttu-id="9d21f-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d21f-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="9d21f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9d21f-121">Relationships</span></span>
|<span data-ttu-id="9d21f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d21f-122">Property</span></span>|<span data-ttu-id="9d21f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d21f-123">Type</span></span>|<span data-ttu-id="9d21f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d21f-124">Description</span></span>|
|-|-|-|
|<span data-ttu-id="9d21f-125">messages</span><span class="sxs-lookup"><span data-stu-id="9d21f-125">messages</span></span>|<span data-ttu-id="9d21f-126">Coleção([serviceUpdateMessage](serviceupdatemessage.md))</span><span class="sxs-lookup"><span data-stu-id="9d21f-126">Collection([serviceUpdateMessage](serviceupdatemessage.md))</span></span>|<span data-ttu-id="9d21f-127">Uma coleção de mensagens de serviço para locatário.</span><span class="sxs-lookup"><span data-stu-id="9d21f-127">A collection of service messages for tenant.</span></span> <span data-ttu-id="9d21f-128">Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.</span><span class="sxs-lookup"><span data-stu-id="9d21f-128">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="9d21f-129">healthOverviews</span><span class="sxs-lookup"><span data-stu-id="9d21f-129">healthOverviews</span></span>|<span data-ttu-id="9d21f-130">Collection([serviceHealth](servicehealth.md))</span><span class="sxs-lookup"><span data-stu-id="9d21f-130">Collection([serviceHealth](servicehealth.md))</span></span>|<span data-ttu-id="9d21f-131">Uma coleção de informações de saúde do serviço para locatário.</span><span class="sxs-lookup"><span data-stu-id="9d21f-131">A collection of service health information for tenant.</span></span> <span data-ttu-id="9d21f-132">Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.</span><span class="sxs-lookup"><span data-stu-id="9d21f-132">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="9d21f-133">issues</span><span class="sxs-lookup"><span data-stu-id="9d21f-133">issues</span></span>|<span data-ttu-id="9d21f-134">Collection([serviceHealthIssue](servicehealthissue.md))</span><span class="sxs-lookup"><span data-stu-id="9d21f-134">Collection([serviceHealthIssue](servicehealthissue.md))</span></span>|<span data-ttu-id="9d21f-135">Uma coleção de problemas de serviço para locatário.</span><span class="sxs-lookup"><span data-stu-id="9d21f-135">A collection of service issues for tenant.</span></span> <span data-ttu-id="9d21f-136">Essa propriedade é uma propriedade de navegação contida, ela é anulada e readonly.</span><span class="sxs-lookup"><span data-stu-id="9d21f-136">This property is a contained navigation property, it is nullable and readonly.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d21f-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d21f-137">JSON representation</span></span>
<span data-ttu-id="9d21f-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d21f-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```