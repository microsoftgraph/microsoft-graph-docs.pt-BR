---
title: tipo de recurso de historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 029c17e09348977752f3ce5632740b2bdac64e46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977434"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="164e9-106">tipo de recurso de historyItem</span><span class="sxs-lookup"><span data-stu-id="164e9-106">historyItem resource type</span></span>

<span data-ttu-id="164e9-107">Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="164e9-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="164e9-108">As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="164e9-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="164e9-109">Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade.</span><span class="sxs-lookup"><span data-stu-id="164e9-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="164e9-110">À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="164e9-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="164e9-111">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **atividade** para refletir o período de participação do usuário.</span><span class="sxs-lookup"><span data-stu-id="164e9-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="164e9-112">Cada vez que um usuário emprega-se novamente com uma atividade, um novo **historyItem** é adicionado à atividade acumular compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="164e9-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="164e9-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="164e9-113">Methods</span></span>

|<span data-ttu-id="164e9-114">Método</span><span class="sxs-lookup"><span data-stu-id="164e9-114">Method</span></span> | <span data-ttu-id="164e9-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="164e9-115">Return Type</span></span> | <span data-ttu-id="164e9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="164e9-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="164e9-117">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="164e9-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="164e9-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="164e9-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="164e9-119">Cria ou substitui um existente **historyItem** para a atividade (upsert).</span><span class="sxs-lookup"><span data-stu-id="164e9-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="164e9-120">A ID deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="164e9-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="164e9-121">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="164e9-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="164e9-122">Nenhum conteúdo</span><span class="sxs-lookup"><span data-stu-id="164e9-122">No Content</span></span> | <span data-ttu-id="164e9-123">Exclui o **historyItem** especificado para a atividade.</span><span class="sxs-lookup"><span data-stu-id="164e9-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="164e9-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="164e9-124">Properties</span></span>

|<span data-ttu-id="164e9-125">Nome</span><span class="sxs-lookup"><span data-stu-id="164e9-125">Name</span></span> | <span data-ttu-id="164e9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="164e9-126">Type</span></span> | <span data-ttu-id="164e9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="164e9-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="164e9-128">status</span><span class="sxs-lookup"><span data-stu-id="164e9-128">status</span></span> | <span data-ttu-id="164e9-129">status</span><span class="sxs-lookup"><span data-stu-id="164e9-129">status</span></span> | <span data-ttu-id="164e9-130">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="164e9-130">Set by the server.</span></span> <span data-ttu-id="164e9-131">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="164e9-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="164e9-132">Valores: ativo, atualizado, excluídos, ignorado.</span><span class="sxs-lookup"><span data-stu-id="164e9-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="164e9-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="164e9-133">userTimezone</span></span> | <span data-ttu-id="164e9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="164e9-134">String</span></span> | <span data-ttu-id="164e9-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="164e9-135">Optional.</span></span> <span data-ttu-id="164e9-136">O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade.</span><span class="sxs-lookup"><span data-stu-id="164e9-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="164e9-137">Valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="164e9-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="164e9-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="164e9-138">createdDateTime</span></span> | <span data-ttu-id="164e9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164e9-139">DateTimeOffset</span></span> | <span data-ttu-id="164e9-140">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="164e9-140">Set by the server.</span></span> <span data-ttu-id="164e9-141">Data e hora em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="164e9-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="164e9-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="164e9-142">lastModifiedDateTime</span></span> | <span data-ttu-id="164e9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164e9-143">DateTimeOffset</span></span> | <span data-ttu-id="164e9-144">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="164e9-144">Set by the server.</span></span> <span data-ttu-id="164e9-145">Data e hora em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="164e9-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="164e9-146">id</span><span class="sxs-lookup"><span data-stu-id="164e9-146">id</span></span> | <span data-ttu-id="164e9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="164e9-147">String</span></span> | <span data-ttu-id="164e9-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="164e9-148">Required.</span></span> <span data-ttu-id="164e9-149">GUID do conjunto de cliente para o objeto **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="164e9-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="164e9-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="164e9-150">startedDateTime</span></span> | <span data-ttu-id="164e9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164e9-151">DateTimeOffset</span></span> | <span data-ttu-id="164e9-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="164e9-152">Required.</span></span> <span data-ttu-id="164e9-153">DateTime UTC quando **historyItem** (sessão atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="164e9-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="164e9-154">Necessário para o histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="164e9-154">Required for timeline history.</span></span>|
|<span data-ttu-id="164e9-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="164e9-155">lastActiveDateTime</span></span> | <span data-ttu-id="164e9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164e9-156">DateTimeOffset</span></span> | <span data-ttu-id="164e9-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="164e9-157">Optional.</span></span> <span data-ttu-id="164e9-158">DateTime UTC quando **historyItem** (sessão atividade) foi compreendido última como status ativo ou terminar - se for null, **historyItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="164e9-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="164e9-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="164e9-159">expirationDateTime</span></span> | <span data-ttu-id="164e9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164e9-160">DateTimeOffset</span></span> | <span data-ttu-id="164e9-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="164e9-161">Optional.</span></span> <span data-ttu-id="164e9-162">DateTime UTC quando os **historyItem** passará rígido-delete.</span><span class="sxs-lookup"><span data-stu-id="164e9-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="164e9-163">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="164e9-163">Can be set by the client.</span></span>|
|<span data-ttu-id="164e9-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="164e9-164">activeDurationSeconds</span></span> | <span data-ttu-id="164e9-165">int</span><span class="sxs-lookup"><span data-stu-id="164e9-165">int</span></span> | <span data-ttu-id="164e9-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="164e9-166">Optional.</span></span> <span data-ttu-id="164e9-167">A duração de participação de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="164e9-167">The duration of active user engagement.</span></span> <span data-ttu-id="164e9-168">Se não fornecido, isso é calculado do **startedDateTime** e **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="164e9-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="164e9-169">Relações</span><span class="sxs-lookup"><span data-stu-id="164e9-169">Relationships</span></span>

|<span data-ttu-id="164e9-170">Relação</span><span class="sxs-lookup"><span data-stu-id="164e9-170">Relationship</span></span> | <span data-ttu-id="164e9-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="164e9-171">Type</span></span> | <span data-ttu-id="164e9-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="164e9-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="164e9-173">atividade</span><span class="sxs-lookup"><span data-stu-id="164e9-173">activity</span></span>| [<span data-ttu-id="164e9-174">userActivity</span><span class="sxs-lookup"><span data-stu-id="164e9-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="164e9-175">Opcional.</span><span class="sxs-lookup"><span data-stu-id="164e9-175">Optional.</span></span> <span data-ttu-id="164e9-176">NavigationProperty/contenção; propriedade de navegação à atividade associada.</span><span class="sxs-lookup"><span data-stu-id="164e9-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="164e9-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="164e9-177">JSON representation</span></span>

<span data-ttu-id="164e9-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="164e9-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
