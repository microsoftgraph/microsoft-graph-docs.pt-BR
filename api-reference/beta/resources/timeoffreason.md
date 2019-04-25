---
title: tipo de recurso timeOffReason
description: Uma razão válida para ser demorada no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582852"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="ec268-103">tipo de recurso timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec268-104">Uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="ec268-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ec268-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec268-105">Methods</span></span>

| <span data-ttu-id="ec268-106">Método</span><span class="sxs-lookup"><span data-stu-id="ec268-106">Method</span></span>       | <span data-ttu-id="ec268-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec268-107">Return Type</span></span>  |<span data-ttu-id="ec268-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec268-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec268-109">Criar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="ec268-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ec268-111">Criar uma página `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ec268-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="ec268-112">Listar timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="ec268-113">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="ec268-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="ec268-114">Obter uma lista dos `timeOffReasons` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="ec268-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="ec268-115">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="ec268-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ec268-117">Obter um `timeOffReason` por ID.</span><span class="sxs-lookup"><span data-stu-id="ec268-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="ec268-118">Substituir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="ec268-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="ec268-120">Substituir um `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ec268-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="ec268-121">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ec268-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="ec268-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec268-122">None</span></span> | <span data-ttu-id="ec268-123">Marcar `timeOffReason` como inativa.</span><span class="sxs-lookup"><span data-stu-id="ec268-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec268-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec268-124">Properties</span></span>
|<span data-ttu-id="ec268-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ec268-125">Name</span></span>          |<span data-ttu-id="ec268-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec268-126">Type</span></span>           |<span data-ttu-id="ec268-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec268-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="ec268-128">id</span><span class="sxs-lookup"><span data-stu-id="ec268-128">id</span></span>            |`string`      |<span data-ttu-id="ec268-129">A ID da tarefa `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ec268-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="ec268-130">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="ec268-130">displayName</span></span>               | `string`                  | <span data-ttu-id="ec268-131">O nome do `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ec268-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="ec268-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec268-132">Required.</span></span> |
| <span data-ttu-id="ec268-133">icontype</span><span class="sxs-lookup"><span data-stu-id="ec268-133">iconType</span></span> | `enum`   | <span data-ttu-id="ec268-134">Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado.</span><span class="sxs-lookup"><span data-stu-id="ec268-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="ec268-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec268-135">Required.</span></span> |
| <span data-ttu-id="ec268-136">isActive</span><span class="sxs-lookup"><span data-stu-id="ec268-136">isActive</span></span>          |`bool`      | <span data-ttu-id="ec268-137">Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="ec268-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="ec268-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec268-138">Required.</span></span> |
| <span data-ttu-id="ec268-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec268-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="ec268-140">O carimbo de data/hora `timeOffReason` em que foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="ec268-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="ec268-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ec268-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ec268-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="ec268-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ec268-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec268-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="ec268-144">O carimbo de data/hora `timeOffReason` em que foi atualizado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ec268-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="ec268-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ec268-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ec268-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="ec268-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="ec268-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ec268-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="ec268-148">A identidade da última atualização `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="ec268-148">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec268-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec268-149">JSON representation</span></span>

<span data-ttu-id="ec268-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec268-150">Here is a JSON representation of the resource.</span></span>

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
