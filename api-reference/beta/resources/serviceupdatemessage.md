---
title: Tipo de recurso serviceUpdateMessage
description: Representa os comunicados de alterações em um serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e8bea9b3c44f99d5be0d87b01d47db4505873681
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109063"
---
# <a name="serviceupdatemessage-resource-type"></a><span data-ttu-id="dc54b-103">Tipo de recurso serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="dc54b-103">serviceUpdateMessage resource type</span></span>

<span data-ttu-id="dc54b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc54b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc54b-105">Representa os comunicados sobre alterações em um serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-105">Represents the announcements about changes in a service.</span></span>

<span data-ttu-id="dc54b-106">Representa comunicados como atualizações principais, novos recursos em um produto; por exemplo, a publicação de um novo recurso Windows.</span><span class="sxs-lookup"><span data-stu-id="dc54b-106">Represents announcements such as major updates, new features in a product; for example, the publication of a new Windows feature.</span></span>

<span data-ttu-id="dc54b-107">Herda [de serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-107">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc54b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc54b-108">Methods</span></span>
|<span data-ttu-id="dc54b-109">Método</span><span class="sxs-lookup"><span data-stu-id="dc54b-109">Method</span></span>|<span data-ttu-id="dc54b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc54b-110">Return type</span></span>|<span data-ttu-id="dc54b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc54b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc54b-112">Obter serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="dc54b-112">Get serviceUpdateMessage</span></span>](../api/serviceupdatemessage-get.md)|[<span data-ttu-id="dc54b-113">serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="dc54b-113">serviceUpdateMessage</span></span>](../resources/serviceupdatemessage.md)|<span data-ttu-id="dc54b-114">Recupere as propriedades e as relações de um [objeto serviceUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="dc54b-114">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span> |
|[<span data-ttu-id="dc54b-115">markRead</span><span class="sxs-lookup"><span data-stu-id="dc54b-115">markRead</span></span>](../api/serviceupdatemessage-markread.md)|<span data-ttu-id="dc54b-116">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-116">Boolean</span></span>|<span data-ttu-id="dc54b-117">Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **lido** para o usuário que está assinado.</span><span class="sxs-lookup"><span data-stu-id="dc54b-117">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **read** for the signed in user.</span></span>|
|[<span data-ttu-id="dc54b-118">markUnread</span><span class="sxs-lookup"><span data-stu-id="dc54b-118">markUnread</span></span>](../api/serviceupdatemessage-markunread.md)|<span data-ttu-id="dc54b-119">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-119">Boolean</span></span>|<span data-ttu-id="dc54b-120">Marque uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como **não** lido para o usuário insinuável.</span><span class="sxs-lookup"><span data-stu-id="dc54b-120">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **unread** for the signed in user.</span></span>|
|[<span data-ttu-id="dc54b-121">archive</span><span class="sxs-lookup"><span data-stu-id="dc54b-121">archive</span></span>](../api/serviceupdatemessage-archive.md)|<span data-ttu-id="dc54b-122">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-122">Boolean</span></span>|<span data-ttu-id="dc54b-123">Arquivar uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário inscrevedo.</span><span class="sxs-lookup"><span data-stu-id="dc54b-123">Archive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="dc54b-124">unarchive</span><span class="sxs-lookup"><span data-stu-id="dc54b-124">unarchive</span></span>](../api/serviceupdatemessage-unarchive.md)|<span data-ttu-id="dc54b-125">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-125">Boolean</span></span>|<span data-ttu-id="dc54b-126">Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="dc54b-126">Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="dc54b-127">favorite</span><span class="sxs-lookup"><span data-stu-id="dc54b-127">favorite</span></span>](../api/serviceupdatemessage-favorite.md)|<span data-ttu-id="dc54b-128">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-128">Boolean</span></span>|<span data-ttu-id="dc54b-129">Altere o status de uma lista [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s como favorito para o usuário que está assinado.</span><span class="sxs-lookup"><span data-stu-id="dc54b-129">Change the status of a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s to favorite for the signed in user.</span></span>|
|[<span data-ttu-id="dc54b-130">unfavorite</span><span class="sxs-lookup"><span data-stu-id="dc54b-130">unfavorite</span></span>](../api/serviceupdatemessage-unfavorite.md)|<span data-ttu-id="dc54b-131">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-131">Boolean</span></span>|<span data-ttu-id="dc54b-132">Remova o status favorito [de serviceUpdateMessage](../resources/serviceupdatemessage.md)s para o usuário instituto.</span><span class="sxs-lookup"><span data-stu-id="dc54b-132">Remove the favorite status of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc54b-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc54b-133">Properties</span></span>
|<span data-ttu-id="dc54b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc54b-134">Property</span></span>|<span data-ttu-id="dc54b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc54b-135">Type</span></span>|<span data-ttu-id="dc54b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc54b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc54b-137">actionRequiredByDateTime</span><span class="sxs-lookup"><span data-stu-id="dc54b-137">actionRequiredByDateTime</span></span>|<span data-ttu-id="dc54b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc54b-138">DateTimeOffset</span></span>|<span data-ttu-id="dc54b-139">O prazo esperado da ação para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="dc54b-139">The expected deadline of the action for the message.</span></span>|
|<span data-ttu-id="dc54b-140">corpo</span><span class="sxs-lookup"><span data-stu-id="dc54b-140">body</span></span>|[<span data-ttu-id="dc54b-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="dc54b-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="dc54b-142">O tipo de conteúdo e o conteúdo do corpo da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-142">The content type and content of the service message body.</span></span>|
|<span data-ttu-id="dc54b-143">category</span><span class="sxs-lookup"><span data-stu-id="dc54b-143">category</span></span>|<span data-ttu-id="dc54b-144">serviceUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="dc54b-144">serviceUpdateCategory</span></span>|<span data-ttu-id="dc54b-145">A categoria de mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-145">The service message category.</span></span> <span data-ttu-id="dc54b-146">Os valores possíveis são: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dc54b-146">Possible values are: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dc54b-147">detalhes</span><span class="sxs-lookup"><span data-stu-id="dc54b-147">details</span></span>|<span data-ttu-id="dc54b-148">Coleção([keyValuePair](../resources/keyvaluepair.md))</span><span class="sxs-lookup"><span data-stu-id="dc54b-148">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="dc54b-149">Detalhes adicionais sobre a mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-149">Additional details about service message.</span></span> <span data-ttu-id="dc54b-150">Essa propriedade não dá suporte a filtros.</span><span class="sxs-lookup"><span data-stu-id="dc54b-150">This property doesn't support filters.</span></span> <span data-ttu-id="dc54b-151">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-151">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dc54b-152">endDateTime</span></span>|<span data-ttu-id="dc54b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc54b-153">DateTimeOffset</span></span>|<span data-ttu-id="dc54b-154">A hora de término da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-154">The end time of the service message.</span></span> <span data-ttu-id="dc54b-155">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-155">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-156">id</span><span class="sxs-lookup"><span data-stu-id="dc54b-156">id</span></span>|<span data-ttu-id="dc54b-157">String</span><span class="sxs-lookup"><span data-stu-id="dc54b-157">String</span></span>|<span data-ttu-id="dc54b-158">A id da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-158">The id of the service message.</span></span> <span data-ttu-id="dc54b-159">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-159">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-160">isMajorChange</span><span class="sxs-lookup"><span data-stu-id="dc54b-160">isMajorChange</span></span>|<span data-ttu-id="dc54b-161">Booleano</span><span class="sxs-lookup"><span data-stu-id="dc54b-161">Boolean</span></span>|<span data-ttu-id="dc54b-162">Indica se a mensagem descreve uma atualização importante para o serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-162">Indicates whether the message describes a major update for the service.</span></span>|
|<span data-ttu-id="dc54b-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc54b-163">lastModifiedDateTime</span></span>|<span data-ttu-id="dc54b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc54b-164">DateTimeOffset</span></span>|<span data-ttu-id="dc54b-165">A última hora modificada da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-165">The last modified time of the service message.</span></span> <span data-ttu-id="dc54b-166">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-166">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-167">services</span><span class="sxs-lookup"><span data-stu-id="dc54b-167">services</span></span>|<span data-ttu-id="dc54b-168">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="dc54b-168">Collection(string)</span></span>|<span data-ttu-id="dc54b-169">Os serviços afetados pela mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-169">The affected services by the service message.</span></span>|
|<span data-ttu-id="dc54b-170">severity</span><span class="sxs-lookup"><span data-stu-id="dc54b-170">severity</span></span>|<span data-ttu-id="dc54b-171">serviceUpdateSeverity</span><span class="sxs-lookup"><span data-stu-id="dc54b-171">serviceUpdateSeverity</span></span>|<span data-ttu-id="dc54b-172">A gravidade da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-172">The severity of the service message.</span></span> <span data-ttu-id="dc54b-173">Os valores possíveis são: `normal`, `high`, `critical`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dc54b-173">Possible values are: `normal`, `high`, `critical`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dc54b-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc54b-174">startDateTime</span></span>|<span data-ttu-id="dc54b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc54b-175">DateTimeOffset</span></span>|<span data-ttu-id="dc54b-176">A hora de início da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-176">The start time of the service message.</span></span> <span data-ttu-id="dc54b-177">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-177">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-178">tags</span><span class="sxs-lookup"><span data-stu-id="dc54b-178">tags</span></span>|<span data-ttu-id="dc54b-179">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="dc54b-179">Collection(string)</span></span>|<span data-ttu-id="dc54b-180">Uma coleção de marcas para a mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-180">A collection of tags for the service message.</span></span>|
|<span data-ttu-id="dc54b-181">title</span><span class="sxs-lookup"><span data-stu-id="dc54b-181">title</span></span>|<span data-ttu-id="dc54b-182">String</span><span class="sxs-lookup"><span data-stu-id="dc54b-182">String</span></span>|<span data-ttu-id="dc54b-183">O título da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-183">The title of the service message.</span></span> <span data-ttu-id="dc54b-184">Herdado [do serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="dc54b-184">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="dc54b-185">viewPoint</span><span class="sxs-lookup"><span data-stu-id="dc54b-185">viewPoint</span></span>|[<span data-ttu-id="dc54b-186">serviceUpdateMessageViewpoint</span><span class="sxs-lookup"><span data-stu-id="dc54b-186">serviceUpdateMessageViewpoint</span></span>](../resources/serviceupdatemessageviewpoint.md)|<span data-ttu-id="dc54b-187">Representa os dados de pontos de exibição do usuário da mensagem de serviço.</span><span class="sxs-lookup"><span data-stu-id="dc54b-187">Represents user view points data of the service message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc54b-188">Relações</span><span class="sxs-lookup"><span data-stu-id="dc54b-188">Relationships</span></span>
<span data-ttu-id="dc54b-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc54b-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc54b-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc54b-190">JSON representation</span></span>
<span data-ttu-id="dc54b-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc54b-191">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  }
}
```

