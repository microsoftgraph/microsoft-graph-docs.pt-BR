---
title: tipo de recurso synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 936201202a36d85f8b7a0caa5cfb1cebb002bbb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520020"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="4469a-103">tipo de recurso synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="4469a-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="4469a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4469a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4469a-105">Resume os resultados da execução do trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4469a-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="4469a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4469a-106">Properties</span></span>
| <span data-ttu-id="4469a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4469a-107">Property</span></span>     | <span data-ttu-id="4469a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4469a-108">Type</span></span>   |<span data-ttu-id="4469a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4469a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4469a-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4469a-110">activityIdentifier</span></span>           |<span data-ttu-id="4469a-111">String</span><span class="sxs-lookup"><span data-stu-id="4469a-111">String</span></span> |<span data-ttu-id="4469a-112">Identificador do trabalho executado.</span><span class="sxs-lookup"><span data-stu-id="4469a-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="4469a-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="4469a-113">countEntitled</span></span>                |<span data-ttu-id="4469a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-114">Int64</span></span>  |<span data-ttu-id="4469a-115">Contagem de entradas processadas que foram atribuídas para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4469a-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="4469a-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="4469a-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="4469a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-117">Int64</span></span>  |<span data-ttu-id="4469a-118">Contagem de entradas processadas que foram atribuídas para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4469a-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="4469a-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="4469a-119">countEscrowed</span></span>                |<span data-ttu-id="4469a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-120">Int64</span></span>  |<span data-ttu-id="4469a-121">Contagem de entradas que foram caução (erros).</span><span class="sxs-lookup"><span data-stu-id="4469a-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="4469a-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="4469a-122">countEscrowedRaw</span></span>             |<span data-ttu-id="4469a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-123">Int64</span></span>  |<span data-ttu-id="4469a-124">Contagem de entradas que foram caução, incluindo caução geradas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="4469a-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="4469a-125">countExported</span><span class="sxs-lookup"><span data-stu-id="4469a-125">countExported</span></span>                |<span data-ttu-id="4469a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-126">Int64</span></span>  |<span data-ttu-id="4469a-127">Contagem de entradas exportadas.</span><span class="sxs-lookup"><span data-stu-id="4469a-127">Count of exported entries.</span></span>|
|<span data-ttu-id="4469a-128">countExports</span><span class="sxs-lookup"><span data-stu-id="4469a-128">countExports</span></span>                 |<span data-ttu-id="4469a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-129">Int64</span></span>  |<span data-ttu-id="4469a-130">Contagem de entradas que devem ser exportadas.</span><span class="sxs-lookup"><span data-stu-id="4469a-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="4469a-131">countImported</span><span class="sxs-lookup"><span data-stu-id="4469a-131">countImported</span></span>                |<span data-ttu-id="4469a-132">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-132">Int64</span></span>  |<span data-ttu-id="4469a-133">Contagem de entradas importadas.</span><span class="sxs-lookup"><span data-stu-id="4469a-133">Count of imported entries.</span></span>|
|<span data-ttu-id="4469a-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="4469a-134">countImportedDeltas</span></span>          |<span data-ttu-id="4469a-135">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-135">Int64</span></span>  |<span data-ttu-id="4469a-136">Contagem de alterações delta importadas.</span><span class="sxs-lookup"><span data-stu-id="4469a-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="4469a-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="4469a-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="4469a-138">Int64</span><span class="sxs-lookup"><span data-stu-id="4469a-138">Int64</span></span>  |<span data-ttu-id="4469a-139">Contagem de alterações delta importadas referentes a alterações de referência.</span><span class="sxs-lookup"><span data-stu-id="4469a-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="4469a-140">erro</span><span class="sxs-lookup"><span data-stu-id="4469a-140">error</span></span>                        |[<span data-ttu-id="4469a-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="4469a-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="4469a-142">Se for encontrado um erro, conterá um objeto **synchronizationError** com detalhes.</span><span class="sxs-lookup"><span data-stu-id="4469a-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="4469a-143">state</span><span class="sxs-lookup"><span data-stu-id="4469a-143">state</span></span>                        |<span data-ttu-id="4469a-144">String</span><span class="sxs-lookup"><span data-stu-id="4469a-144">String</span></span> |<span data-ttu-id="4469a-145">Código que resume o resultado desta execução.</span><span class="sxs-lookup"><span data-stu-id="4469a-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="4469a-146">Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="4469a-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="4469a-147">timecomeçou</span><span class="sxs-lookup"><span data-stu-id="4469a-147">timeBegan</span></span>                    |<span data-ttu-id="4469a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4469a-148">DateTimeOffset</span></span>|<span data-ttu-id="4469a-149">Hora em que esta execução de trabalho começou.</span><span class="sxs-lookup"><span data-stu-id="4469a-149">Time when this job run began.</span></span> <span data-ttu-id="4469a-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4469a-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4469a-151">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4469a-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4469a-152">timeterminou</span><span class="sxs-lookup"><span data-stu-id="4469a-152">timeEnded</span></span>                    |<span data-ttu-id="4469a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4469a-153">DateTimeOffset</span></span>|<span data-ttu-id="4469a-154">Hora em que esse trabalho foi executado.</span><span class="sxs-lookup"><span data-stu-id="4469a-154">Time when this job run ended.</span></span> <span data-ttu-id="4469a-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4469a-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4469a-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4469a-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4469a-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4469a-157">JSON representation</span></span>

<span data-ttu-id="4469a-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4469a-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
