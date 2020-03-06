---
title: tipo de recurso historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 4053811f1f44621b05830bf40b17d02e0112b455
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533944"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="18a27-106">tipo de recurso historyItem</span><span class="sxs-lookup"><span data-stu-id="18a27-106">historyItem resource type</span></span>

<span data-ttu-id="18a27-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a27-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18a27-108">Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a27-108">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="18a27-109">As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="18a27-109">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="18a27-110">Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade.</span><span class="sxs-lookup"><span data-stu-id="18a27-110">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="18a27-111">À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="18a27-111">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="18a27-112">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **Activity** para refletir o período do contrato do usuário.</span><span class="sxs-lookup"><span data-stu-id="18a27-112">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="18a27-113">Cada vez que um usuário reparticipa de uma atividade, um novo **historyItem** é adicionado à atividade para acumular o envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="18a27-113">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="18a27-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="18a27-114">Methods</span></span>

|<span data-ttu-id="18a27-115">Método</span><span class="sxs-lookup"><span data-stu-id="18a27-115">Method</span></span> | <span data-ttu-id="18a27-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18a27-116">Return Type</span></span> | <span data-ttu-id="18a27-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a27-117">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="18a27-118">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="18a27-118">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="18a27-119">historyItem</span><span class="sxs-lookup"><span data-stu-id="18a27-119">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="18a27-120">Cria ou substitui um **historyItem** existente para aquela atividade (Upsert).</span><span class="sxs-lookup"><span data-stu-id="18a27-120">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="18a27-121">A ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="18a27-121">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="18a27-122">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="18a27-122">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="18a27-123">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="18a27-123">No Content</span></span> | <span data-ttu-id="18a27-124">Exclui o **historyItem** especificado para essa atividade.</span><span class="sxs-lookup"><span data-stu-id="18a27-124">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="18a27-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18a27-125">Properties</span></span>

|<span data-ttu-id="18a27-126">Nome</span><span class="sxs-lookup"><span data-stu-id="18a27-126">Name</span></span> | <span data-ttu-id="18a27-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a27-127">Type</span></span> | <span data-ttu-id="18a27-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a27-128">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="18a27-129">status</span><span class="sxs-lookup"><span data-stu-id="18a27-129">status</span></span> | <span data-ttu-id="18a27-130">status</span><span class="sxs-lookup"><span data-stu-id="18a27-130">status</span></span> | <span data-ttu-id="18a27-131">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="18a27-131">Set by the server.</span></span> <span data-ttu-id="18a27-132">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="18a27-132">A status code used to identify valid objects.</span></span> <span data-ttu-id="18a27-133">Valores: ativo, atualizado, excluído, ignorado.</span><span class="sxs-lookup"><span data-stu-id="18a27-133">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="18a27-134">usertimezone</span><span class="sxs-lookup"><span data-stu-id="18a27-134">userTimezone</span></span> | <span data-ttu-id="18a27-135">String</span><span class="sxs-lookup"><span data-stu-id="18a27-135">String</span></span> | <span data-ttu-id="18a27-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18a27-136">Optional.</span></span> <span data-ttu-id="18a27-137">O fuso horário em que o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade.</span><span class="sxs-lookup"><span data-stu-id="18a27-137">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="18a27-138">Valores fornecidos como IDs de Olson para oferecer suporte à representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="18a27-138">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="18a27-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18a27-139">createdDateTime</span></span> | <span data-ttu-id="18a27-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a27-140">DateTimeOffset</span></span> | <span data-ttu-id="18a27-141">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="18a27-141">Set by the server.</span></span> <span data-ttu-id="18a27-142">DateTime em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="18a27-142">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="18a27-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a27-143">lastModifiedDateTime</span></span> | <span data-ttu-id="18a27-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a27-144">DateTimeOffset</span></span> | <span data-ttu-id="18a27-145">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="18a27-145">Set by the server.</span></span> <span data-ttu-id="18a27-146">DateTime em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="18a27-146">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="18a27-147">id</span><span class="sxs-lookup"><span data-stu-id="18a27-147">id</span></span> | <span data-ttu-id="18a27-148">String</span><span class="sxs-lookup"><span data-stu-id="18a27-148">String</span></span> | <span data-ttu-id="18a27-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a27-149">Required.</span></span> <span data-ttu-id="18a27-150">Client-set GUID para o objeto **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="18a27-150">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="18a27-151">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a27-151">startedDateTime</span></span> | <span data-ttu-id="18a27-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a27-152">DateTimeOffset</span></span> | <span data-ttu-id="18a27-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a27-153">Required.</span></span> <span data-ttu-id="18a27-154">DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="18a27-154">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="18a27-155">Obrigatório para histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="18a27-155">Required for timeline history.</span></span>|
|<span data-ttu-id="18a27-156">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="18a27-156">lastActiveDateTime</span></span> | <span data-ttu-id="18a27-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a27-157">DateTimeOffset</span></span> | <span data-ttu-id="18a27-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18a27-158">Optional.</span></span> <span data-ttu-id="18a27-159">DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido pela última vez como ativo ou concluído-se nulo, o status do **HistoryItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="18a27-159">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="18a27-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18a27-160">expirationDateTime</span></span> | <span data-ttu-id="18a27-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a27-161">DateTimeOffset</span></span> | <span data-ttu-id="18a27-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18a27-162">Optional.</span></span> <span data-ttu-id="18a27-163">DateTime UTC quando o **historyItem** passará pela exclusão permanente.</span><span class="sxs-lookup"><span data-stu-id="18a27-163">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="18a27-164">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18a27-164">Can be set by the client.</span></span>|
|<span data-ttu-id="18a27-165">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="18a27-165">activeDurationSeconds</span></span> | <span data-ttu-id="18a27-166">int</span><span class="sxs-lookup"><span data-stu-id="18a27-166">int</span></span> | <span data-ttu-id="18a27-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18a27-167">Optional.</span></span> <span data-ttu-id="18a27-168">A duração do contrato de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="18a27-168">The duration of active user engagement.</span></span> <span data-ttu-id="18a27-169">Se não for fornecido, isso será calculado a partir do **startedDateTime** e do **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="18a27-169">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a27-170">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="18a27-170">Relationships</span></span>

|<span data-ttu-id="18a27-171">Relação</span><span class="sxs-lookup"><span data-stu-id="18a27-171">Relationship</span></span> | <span data-ttu-id="18a27-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a27-172">Type</span></span> | <span data-ttu-id="18a27-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a27-173">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="18a27-174">atividade</span><span class="sxs-lookup"><span data-stu-id="18a27-174">activity</span></span>| [<span data-ttu-id="18a27-175">userActivity</span><span class="sxs-lookup"><span data-stu-id="18a27-175">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="18a27-176">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18a27-176">Optional.</span></span> <span data-ttu-id="18a27-177">NavigationProperty/confinamento; Propriedade de navegação para a atividade associada.</span><span class="sxs-lookup"><span data-stu-id="18a27-177">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18a27-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18a27-178">JSON representation</span></span>

<span data-ttu-id="18a27-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18a27-179">Here is a JSON representation of the resource.</span></span>

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
