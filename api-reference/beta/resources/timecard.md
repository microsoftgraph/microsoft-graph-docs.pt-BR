---
title: tipo de recurso do cartão de tempo
description: Uma entrada de cartão de ponto na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786370"
---
# <a name="timecard-resource-type"></a><span data-ttu-id="bad88-103">tipo de recurso do cartão de tempo</span><span class="sxs-lookup"><span data-stu-id="bad88-103">timecard resource type</span></span>

<span data-ttu-id="bad88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bad88-105">Representa uma entrada de cartão de ponto na agenda.</span><span class="sxs-lookup"><span data-stu-id="bad88-105">Represents a timecard entry in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="bad88-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bad88-106">Methods</span></span>

| <span data-ttu-id="bad88-107">Método</span><span class="sxs-lookup"><span data-stu-id="bad88-107">Method</span></span>       | <span data-ttu-id="bad88-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bad88-108">Return type</span></span>  |<span data-ttu-id="bad88-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad88-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bad88-110">List</span><span class="sxs-lookup"><span data-stu-id="bad88-110">List</span></span>](../api/timecard-list.md) | <span data-ttu-id="bad88-111">[coleção timeCard](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="bad88-111">[timeCard](timecard.md) collection</span></span> | <span data-ttu-id="bad88-112">Obter a lista de **objetos de cartão de** ponto nesta agenda.</span><span class="sxs-lookup"><span data-stu-id="bad88-112">Get the list of **timecard** objects in this schedule.</span></span>|
|[<span data-ttu-id="bad88-113">Create</span><span class="sxs-lookup"><span data-stu-id="bad88-113">Create</span></span>](../api/timecard-post.md) | [<span data-ttu-id="bad88-114">timeCard</span><span class="sxs-lookup"><span data-stu-id="bad88-114">timeCard</span></span>](timecard.md) | <span data-ttu-id="bad88-115">Crie um novo **objeto de cartão de** ponto.</span><span class="sxs-lookup"><span data-stu-id="bad88-115">Create a new **timecard** object.</span></span>|
|[<span data-ttu-id="bad88-116">Get</span><span class="sxs-lookup"><span data-stu-id="bad88-116">Get</span></span>](../api/timecard-get.md) | [<span data-ttu-id="bad88-117">timeCard</span><span class="sxs-lookup"><span data-stu-id="bad88-117">timeCard</span></span>](timecard.md) | <span data-ttu-id="bad88-118">Obter um **objeto de cartão** de ponto por ID.</span><span class="sxs-lookup"><span data-stu-id="bad88-118">Get a **timecard** object by ID.</span></span>|
|[<span data-ttu-id="bad88-119">Replace</span><span class="sxs-lookup"><span data-stu-id="bad88-119">Replace</span></span>](../api/timecard-replace.md) | <span data-ttu-id="bad88-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-120">None</span></span> | <span data-ttu-id="bad88-121">Substitua um **objeto de cartão de** ponto.</span><span class="sxs-lookup"><span data-stu-id="bad88-121">Replace a **timecard** object.</span></span>|
|[<span data-ttu-id="bad88-122">Delete</span><span class="sxs-lookup"><span data-stu-id="bad88-122">Delete</span></span>](../api/timecard-delete.md) | <span data-ttu-id="bad88-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-123">None</span></span> | <span data-ttu-id="bad88-124">**Exclua um objeto de** cartão de ponto da agenda.</span><span class="sxs-lookup"><span data-stu-id="bad88-124">Delete a **timecard** object from the schedule.</span></span>|
|[<span data-ttu-id="bad88-125">clockIn</span><span class="sxs-lookup"><span data-stu-id="bad88-125">clockIn</span></span>](../api/timecard-clockin.md) | [<span data-ttu-id="bad88-126">timeCard</span><span class="sxs-lookup"><span data-stu-id="bad88-126">timeCard</span></span>](timecard.md) | <span data-ttu-id="bad88-127">Entre para iniciar um **cartão de ponto**.</span><span class="sxs-lookup"><span data-stu-id="bad88-127">Clock in to start a **timecard**.</span></span>|
|[<span data-ttu-id="bad88-128">clockOut</span><span class="sxs-lookup"><span data-stu-id="bad88-128">clockOut</span></span>](../api/timecard-clockout.md) | <span data-ttu-id="bad88-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-129">None</span></span> | <span data-ttu-id="bad88-130">Clock out to end a open **timecard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-130">Clock out to end an open **timecard**.</span></span>|
|[<span data-ttu-id="bad88-131">startBreak</span><span class="sxs-lookup"><span data-stu-id="bad88-131">startBreak</span></span>](../api/timecard-startbreak.md) | <span data-ttu-id="bad88-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-132">None</span></span> | <span data-ttu-id="bad88-133">Inicie um **timeCardBreak** em um cartão **de ponto específico.**</span><span class="sxs-lookup"><span data-stu-id="bad88-133">Start a **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="bad88-134">endBreak</span><span class="sxs-lookup"><span data-stu-id="bad88-134">endBreak</span></span>](../api/timecard-endbreak.md) | <span data-ttu-id="bad88-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-135">None</span></span> | <span data-ttu-id="bad88-136">Termine o tempo **de aberturaCardBreak** em um **cartão de ponto específico.**</span><span class="sxs-lookup"><span data-stu-id="bad88-136">End the open **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="bad88-137">confirmTimeCard</span><span class="sxs-lookup"><span data-stu-id="bad88-137">confirmTimeCard</span></span>](../api/timecard-confirm.md) | <span data-ttu-id="bad88-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bad88-138">None</span></span> | <span data-ttu-id="bad88-139">Confirme **um registro de cartão de** ponto.</span><span class="sxs-lookup"><span data-stu-id="bad88-139">Confirm a **timecard** record.</span></span>|

## <a name="properties"></a><span data-ttu-id="bad88-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bad88-140">Properties</span></span>
|<span data-ttu-id="bad88-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bad88-141">Property</span></span>               |<span data-ttu-id="bad88-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad88-142">Type</span></span>           |<span data-ttu-id="bad88-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad88-143">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="bad88-144">id</span><span class="sxs-lookup"><span data-stu-id="bad88-144">id</span></span>                    |`string`  |<span data-ttu-id="bad88-145">ID do **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-145">ID of the **timeCard**.</span></span>|
| <span data-ttu-id="bad88-146">userId</span><span class="sxs-lookup"><span data-stu-id="bad88-146">userId</span></span>                    |`string` |<span data-ttu-id="bad88-147">ID do usuário à qual o **cartão de** usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="bad88-147">User ID to which  the **timeCard** belongs.</span></span> |
| <span data-ttu-id="bad88-148">estado</span><span class="sxs-lookup"><span data-stu-id="bad88-148">state</span></span>                 |`timeCardState`  | <span data-ttu-id="bad88-149">O estado atual do **timeCard durante** seu ciclo de vida. Os valores possíveis são: `clockedIn` `onBreak` , , , `clockedOut` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="bad88-149">The current state of the **timeCard** during its life cycle.Possible values are: `clockedIn`, `onBreak`, `clockedOut`, `unknownFutureValue`.</span></span>|
| <span data-ttu-id="bad88-150">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="bad88-150">clockInEvent</span></span>       |[<span data-ttu-id="bad88-151">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="bad88-151">timeCardEvent</span></span>](../resources/timecardevent.md)    | <span data-ttu-id="bad88-152">O evento de clock-in do **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-152">The clock-in event of the **timeCard**.</span></span> |
| <span data-ttu-id="bad88-153">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="bad88-153">clockOutEvent</span></span>                 |[<span data-ttu-id="bad88-154">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="bad88-154">timeCardEvent</span></span>](../resources/timecardevent.md)  |<span data-ttu-id="bad88-155">O evento de saída do **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-155">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="bad88-156">notes</span><span class="sxs-lookup"><span data-stu-id="bad88-156">notes</span></span>                 | [<span data-ttu-id="bad88-157">itemBody</span><span class="sxs-lookup"><span data-stu-id="bad88-157">itemBody</span></span>](itembody.md)  |<span data-ttu-id="bad88-158">Observações sobre **o timeCard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-158">Notes about the **timeCard**.</span></span> |
| <span data-ttu-id="bad88-159">quebras</span><span class="sxs-lookup"><span data-stu-id="bad88-159">breaks</span></span>    |<span data-ttu-id="bad88-160">[Coleção timeCardBreak](timecardbreak.md)</span><span class="sxs-lookup"><span data-stu-id="bad88-160">[timeCardBreak](timecardbreak.md) collection</span></span>  |<span data-ttu-id="bad88-161">A lista de quebras associada ao **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="bad88-161">The list of breaks associated with the **timeCard**.</span></span>|
| <span data-ttu-id="bad88-162">originalEntry</span><span class="sxs-lookup"><span data-stu-id="bad88-162">originalEntry</span></span>| [<span data-ttu-id="bad88-163">timeCardEntry</span><span class="sxs-lookup"><span data-stu-id="bad88-163">timeCardEntry</span></span>](../resources/timecardentry.md) | <span data-ttu-id="bad88-164">O **timeCardEntry** original do **timeCard**, antes das edições do usuário.</span><span class="sxs-lookup"><span data-stu-id="bad88-164">The original **timeCardEntry** of the **timeCard**, before user edits.</span></span> |
| <span data-ttu-id="bad88-165">confirmedBy</span><span class="sxs-lookup"><span data-stu-id="bad88-165">confirmedBy</span></span> |`confirmedBy`    | <span data-ttu-id="bad88-166">Indique se essa **entrada timeCard** está confirmada.</span><span class="sxs-lookup"><span data-stu-id="bad88-166">Indicate if this **timeCard** entry is confirmed.</span></span> <span data-ttu-id="bad88-167">Os valores possíveis são `none`, `user`, `manager`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bad88-167">Possible values are `none`, `user`, `manager`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bad88-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bad88-168">createdDateTime</span></span>|`Edm.dateTimeOffset`| <span data-ttu-id="bad88-169">O timestamp no qual o **timeCard** foi criado.</span><span class="sxs-lookup"><span data-stu-id="bad88-169">The timestamp in which the **timeCard** was created.</span></span> |
|<span data-ttu-id="bad88-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="bad88-170">createdBy</span></span>|`IdentitySet`| <span data-ttu-id="bad88-171">Identidade da pessoa que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="bad88-171">Identity of the person who created the entity.</span></span> |
|<span data-ttu-id="bad88-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bad88-172">lastModifiedDateTime</span></span>|`dateTimeOffset`| <span data-ttu-id="bad88-173">O timestamp no qual **o timeCard** foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bad88-173">The timestamp in which the **timeCard** was last modified.</span></span>|
|<span data-ttu-id="bad88-174">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bad88-174">lastModifiedBy</span></span>| `IdentitySet`| <span data-ttu-id="bad88-175">Identidade da pessoa que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bad88-175">Identity of the person who last modified the entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bad88-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bad88-176">JSON representation</span></span>

<span data-ttu-id="bad88-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bad88-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
