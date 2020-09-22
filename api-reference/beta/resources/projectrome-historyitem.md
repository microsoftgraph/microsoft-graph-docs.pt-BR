---
title: tipo de recurso historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: 8d5c3d303944dffc27e9996302ac31de671565b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993153"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="1acb5-106">tipo de recurso historyItem</span><span class="sxs-lookup"><span data-stu-id="1acb5-106">historyItem resource type</span></span>

<span data-ttu-id="1acb5-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1acb5-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1acb5-108">Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1acb5-108">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="1acb5-109">As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1acb5-109">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="1acb5-110">Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade.</span><span class="sxs-lookup"><span data-stu-id="1acb5-110">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="1acb5-111">À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="1acb5-111">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="1acb5-112">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **Activity** para refletir o período do contrato do usuário.</span><span class="sxs-lookup"><span data-stu-id="1acb5-112">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="1acb5-113">Cada vez que um usuário reparticipa de uma atividade, um novo **historyItem** é adicionado à atividade para acumular o envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="1acb5-113">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="1acb5-114">Methods</span><span class="sxs-lookup"><span data-stu-id="1acb5-114">Methods</span></span>

|<span data-ttu-id="1acb5-115">Método</span><span class="sxs-lookup"><span data-stu-id="1acb5-115">Method</span></span> | <span data-ttu-id="1acb5-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1acb5-116">Return Type</span></span> | <span data-ttu-id="1acb5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1acb5-117">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="1acb5-118">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="1acb5-118">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="1acb5-119">historyItem</span><span class="sxs-lookup"><span data-stu-id="1acb5-119">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="1acb5-120">Cria ou substitui um **historyItem** existente para aquela atividade (Upsert).</span><span class="sxs-lookup"><span data-stu-id="1acb5-120">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="1acb5-121">A ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="1acb5-121">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="1acb5-122">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="1acb5-122">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="1acb5-123">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="1acb5-123">No Content</span></span> | <span data-ttu-id="1acb5-124">Exclui o **historyItem** especificado para essa atividade.</span><span class="sxs-lookup"><span data-stu-id="1acb5-124">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="1acb5-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1acb5-125">Properties</span></span>

|<span data-ttu-id="1acb5-126">Nome</span><span class="sxs-lookup"><span data-stu-id="1acb5-126">Name</span></span> | <span data-ttu-id="1acb5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1acb5-127">Type</span></span> | <span data-ttu-id="1acb5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1acb5-128">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1acb5-129">status</span><span class="sxs-lookup"><span data-stu-id="1acb5-129">status</span></span> | <span data-ttu-id="1acb5-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1acb5-130">string</span></span> | <span data-ttu-id="1acb5-131">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="1acb5-131">Set by the server.</span></span> <span data-ttu-id="1acb5-132">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="1acb5-132">A status code used to identify valid objects.</span></span> <span data-ttu-id="1acb5-133">Valores: ativo, atualizado, excluído, ignorado.</span><span class="sxs-lookup"><span data-stu-id="1acb5-133">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="1acb5-134">usertimezone</span><span class="sxs-lookup"><span data-stu-id="1acb5-134">userTimezone</span></span> | <span data-ttu-id="1acb5-135">String</span><span class="sxs-lookup"><span data-stu-id="1acb5-135">String</span></span> | <span data-ttu-id="1acb5-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1acb5-136">Optional.</span></span> <span data-ttu-id="1acb5-137">O fuso horário em que o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade.</span><span class="sxs-lookup"><span data-stu-id="1acb5-137">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="1acb5-138">Valores fornecidos como IDs de Olson para oferecer suporte à representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="1acb5-138">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="1acb5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1acb5-139">createdDateTime</span></span> | <span data-ttu-id="1acb5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acb5-140">DateTimeOffset</span></span> | <span data-ttu-id="1acb5-141">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="1acb5-141">Set by the server.</span></span> <span data-ttu-id="1acb5-142">DateTime em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="1acb5-142">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="1acb5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1acb5-143">lastModifiedDateTime</span></span> | <span data-ttu-id="1acb5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acb5-144">DateTimeOffset</span></span> | <span data-ttu-id="1acb5-145">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="1acb5-145">Set by the server.</span></span> <span data-ttu-id="1acb5-146">DateTime em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="1acb5-146">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="1acb5-147">id</span><span class="sxs-lookup"><span data-stu-id="1acb5-147">id</span></span> | <span data-ttu-id="1acb5-148">String</span><span class="sxs-lookup"><span data-stu-id="1acb5-148">String</span></span> | <span data-ttu-id="1acb5-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1acb5-149">Required.</span></span> <span data-ttu-id="1acb5-150">Client-set GUID para o objeto **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="1acb5-150">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="1acb5-151">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="1acb5-151">startedDateTime</span></span> | <span data-ttu-id="1acb5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acb5-152">DateTimeOffset</span></span> | <span data-ttu-id="1acb5-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1acb5-153">Required.</span></span> <span data-ttu-id="1acb5-154">DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="1acb5-154">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="1acb5-155">Obrigatório para histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="1acb5-155">Required for timeline history.</span></span>|
|<span data-ttu-id="1acb5-156">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="1acb5-156">lastActiveDateTime</span></span> | <span data-ttu-id="1acb5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acb5-157">DateTimeOffset</span></span> | <span data-ttu-id="1acb5-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1acb5-158">Optional.</span></span> <span data-ttu-id="1acb5-159">DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido pela última vez como ativo ou concluído-se nulo, o status do **HistoryItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="1acb5-159">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="1acb5-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1acb5-160">expirationDateTime</span></span> | <span data-ttu-id="1acb5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1acb5-161">DateTimeOffset</span></span> | <span data-ttu-id="1acb5-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1acb5-162">Optional.</span></span> <span data-ttu-id="1acb5-163">DateTime UTC quando o **historyItem** passará pela exclusão permanente.</span><span class="sxs-lookup"><span data-stu-id="1acb5-163">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="1acb5-164">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1acb5-164">Can be set by the client.</span></span>|
|<span data-ttu-id="1acb5-165">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="1acb5-165">activeDurationSeconds</span></span> | <span data-ttu-id="1acb5-166">int</span><span class="sxs-lookup"><span data-stu-id="1acb5-166">int</span></span> | <span data-ttu-id="1acb5-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1acb5-167">Optional.</span></span> <span data-ttu-id="1acb5-168">A duração do contrato de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="1acb5-168">The duration of active user engagement.</span></span> <span data-ttu-id="1acb5-169">Se não for fornecido, isso será calculado a partir do **startedDateTime** e do **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="1acb5-169">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1acb5-170">Relações</span><span class="sxs-lookup"><span data-stu-id="1acb5-170">Relationships</span></span>

|<span data-ttu-id="1acb5-171">Relação</span><span class="sxs-lookup"><span data-stu-id="1acb5-171">Relationship</span></span> | <span data-ttu-id="1acb5-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="1acb5-172">Type</span></span> | <span data-ttu-id="1acb5-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="1acb5-173">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="1acb5-174">atividade</span><span class="sxs-lookup"><span data-stu-id="1acb5-174">activity</span></span>| [<span data-ttu-id="1acb5-175">atividade</span><span class="sxs-lookup"><span data-stu-id="1acb5-175">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="1acb5-176">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1acb5-176">Optional.</span></span> <span data-ttu-id="1acb5-177">NavigationProperty/confinamento; Propriedade de navegação para a atividade associada.</span><span class="sxs-lookup"><span data-stu-id="1acb5-177">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1acb5-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1acb5-178">JSON representation</span></span>

<span data-ttu-id="1acb5-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1acb5-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


