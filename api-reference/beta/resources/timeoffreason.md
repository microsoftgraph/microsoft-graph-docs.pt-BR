---
title: tipo de recurso timeOffReason
description: Uma razão válida para ser demorada no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657529"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="04259-103">tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04259-104">Uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="04259-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="04259-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="04259-105">Methods</span></span>

| <span data-ttu-id="04259-106">Método</span><span class="sxs-lookup"><span data-stu-id="04259-106">Method</span></span>       | <span data-ttu-id="04259-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04259-107">Return Type</span></span>  |<span data-ttu-id="04259-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="04259-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04259-109">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="04259-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04259-111">Criar um novo `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="04259-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="04259-112">Listar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="04259-113">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="04259-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="04259-114">Obtenha a lista `timeOffReasons` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="04259-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="04259-115">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="04259-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04259-117">Obter a `timeOffReason` por ID.</span><span class="sxs-lookup"><span data-stu-id="04259-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="04259-118">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="04259-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="04259-120">Substitua um `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="04259-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="04259-121">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="04259-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="04259-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04259-122">None</span></span> | <span data-ttu-id="04259-123">Marcar `timeOffReason` como inativa.</span><span class="sxs-lookup"><span data-stu-id="04259-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="04259-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04259-124">Properties</span></span>
|<span data-ttu-id="04259-125">Nome</span><span class="sxs-lookup"><span data-stu-id="04259-125">Name</span></span>          |<span data-ttu-id="04259-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="04259-126">Type</span></span>           |<span data-ttu-id="04259-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="04259-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="04259-128">id</span><span class="sxs-lookup"><span data-stu-id="04259-128">id</span></span>            |`string`      |<span data-ttu-id="04259-129">ID do `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="04259-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="04259-130">displayName</span><span class="sxs-lookup"><span data-stu-id="04259-130">displayName</span></span>               | `string`                  | <span data-ttu-id="04259-131">O nome do `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="04259-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="04259-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04259-132">Required.</span></span> |
| <span data-ttu-id="04259-133">icontype</span><span class="sxs-lookup"><span data-stu-id="04259-133">iconType</span></span> | `enum`   | <span data-ttu-id="04259-134">Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado.</span><span class="sxs-lookup"><span data-stu-id="04259-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="04259-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04259-135">Required.</span></span> |
| <span data-ttu-id="04259-136">IsActive</span><span class="sxs-lookup"><span data-stu-id="04259-136">isActive</span></span>          |`bool`      | <span data-ttu-id="04259-137">Indica se o `timeOffReason` pode ser usado ao criar novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="04259-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="04259-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04259-138">Required.</span></span> |
| <span data-ttu-id="04259-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04259-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="04259-140">O carimbo de data/hora `timeOffReason` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="04259-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="04259-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="04259-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04259-142">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="04259-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="04259-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04259-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="04259-144">O carimbo de data/hora `timeOffReason` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="04259-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="04259-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="04259-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04259-146">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="04259-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="04259-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="04259-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="04259-148">A identidade que foi atualizada pela `timeOffReason`última vez.</span><span class="sxs-lookup"><span data-stu-id="04259-148">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04259-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04259-149">JSON representation</span></span>

<span data-ttu-id="04259-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04259-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
