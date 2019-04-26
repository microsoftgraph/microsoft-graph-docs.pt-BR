---
title: tipo de recurso historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade. À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c43a4f0515f8d61625e11abe8bbdbe2464c729f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344050"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="dffed-106">tipo de recurso historyItem</span><span class="sxs-lookup"><span data-stu-id="dffed-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dffed-107">Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dffed-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="dffed-108">As atividades do usuário representam um único destino dentro de seu aplicativo, por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="dffed-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="dffed-109">Quando um usuário participa dessa atividade, o contrato é capturado como um item de histórico que indica a hora de início e término da atividade.</span><span class="sxs-lookup"><span data-stu-id="dffed-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="dffed-110">À medida que o usuário se reencaixa com essa atividade ao longo do tempo, vários itens de histórico são registrados para uma única atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="dffed-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="dffed-111">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **Activity** para refletir o período do contrato do usuário.</span><span class="sxs-lookup"><span data-stu-id="dffed-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="dffed-112">Cada vez que um usuário reparticipa de uma atividade, um novo **historyItem** é adicionado à atividade para acumular o envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="dffed-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="dffed-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="dffed-113">Methods</span></span>

|<span data-ttu-id="dffed-114">Método</span><span class="sxs-lookup"><span data-stu-id="dffed-114">Method</span></span> | <span data-ttu-id="dffed-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dffed-115">Return Type</span></span> | <span data-ttu-id="dffed-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="dffed-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="dffed-117">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="dffed-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="dffed-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="dffed-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="dffed-119">Cria ou substitui um **historyItem** existente para aquela atividade (Upsert).</span><span class="sxs-lookup"><span data-stu-id="dffed-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="dffed-120">A ID precisa ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="dffed-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="dffed-121">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="dffed-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="dffed-122">Sem conteúdo</span><span class="sxs-lookup"><span data-stu-id="dffed-122">No Content</span></span> | <span data-ttu-id="dffed-123">Exclui o **historyItem** especificado para essa atividade.</span><span class="sxs-lookup"><span data-stu-id="dffed-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="dffed-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dffed-124">Properties</span></span>

|<span data-ttu-id="dffed-125">Nome</span><span class="sxs-lookup"><span data-stu-id="dffed-125">Name</span></span> | <span data-ttu-id="dffed-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="dffed-126">Type</span></span> | <span data-ttu-id="dffed-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dffed-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="dffed-128">status</span><span class="sxs-lookup"><span data-stu-id="dffed-128">status</span></span> | <span data-ttu-id="dffed-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dffed-129">string</span></span> | <span data-ttu-id="dffed-130">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="dffed-130">Set by the server.</span></span> <span data-ttu-id="dffed-131">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="dffed-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="dffed-132">Valores: ativo, atualizado, excluído, ignorado.</span><span class="sxs-lookup"><span data-stu-id="dffed-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="dffed-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="dffed-133">userTimezone</span></span> | <span data-ttu-id="dffed-134">String</span><span class="sxs-lookup"><span data-stu-id="dffed-134">String</span></span> | <span data-ttu-id="dffed-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffed-135">Optional.</span></span> <span data-ttu-id="dffed-136">O fuso horário em que o dispositivo do usuário usado para gerar a atividade estava localizado no momento da criação da atividade.</span><span class="sxs-lookup"><span data-stu-id="dffed-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="dffed-137">Valores fornecidos como IDs de Olson para oferecer suporte à representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="dffed-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="dffed-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dffed-138">createdDateTime</span></span> | <span data-ttu-id="dffed-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffed-139">DateTimeOffset</span></span> | <span data-ttu-id="dffed-140">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="dffed-140">Set by the server.</span></span> <span data-ttu-id="dffed-141">DateTime em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="dffed-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="dffed-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dffed-142">lastModifiedDateTime</span></span> | <span data-ttu-id="dffed-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffed-143">DateTimeOffset</span></span> | <span data-ttu-id="dffed-144">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="dffed-144">Set by the server.</span></span> <span data-ttu-id="dffed-145">DateTime em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="dffed-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="dffed-146">id</span><span class="sxs-lookup"><span data-stu-id="dffed-146">id</span></span> | <span data-ttu-id="dffed-147">String</span><span class="sxs-lookup"><span data-stu-id="dffed-147">String</span></span> | <span data-ttu-id="dffed-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dffed-148">Required.</span></span> <span data-ttu-id="dffed-149">Client-set GUID para o objeto **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="dffed-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="dffed-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="dffed-150">startedDateTime</span></span> | <span data-ttu-id="dffed-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffed-151">DateTimeOffset</span></span> | <span data-ttu-id="dffed-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dffed-152">Required.</span></span> <span data-ttu-id="dffed-153">DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="dffed-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="dffed-154">Obrigatório para histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="dffed-154">Required for timeline history.</span></span>|
|<span data-ttu-id="dffed-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="dffed-155">lastActiveDateTime</span></span> | <span data-ttu-id="dffed-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffed-156">DateTimeOffset</span></span> | <span data-ttu-id="dffed-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffed-157">Optional.</span></span> <span data-ttu-id="dffed-158">DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido pela última vez como ativo ou concluído-se nulo, o status do **HistoryItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="dffed-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="dffed-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dffed-159">expirationDateTime</span></span> | <span data-ttu-id="dffed-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffed-160">DateTimeOffset</span></span> | <span data-ttu-id="dffed-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffed-161">Optional.</span></span> <span data-ttu-id="dffed-162">DateTime UTC quando o **historyItem** passará pela exclusão permanente.</span><span class="sxs-lookup"><span data-stu-id="dffed-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="dffed-163">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dffed-163">Can be set by the client.</span></span>|
|<span data-ttu-id="dffed-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="dffed-164">activeDurationSeconds</span></span> | <span data-ttu-id="dffed-165">int</span><span class="sxs-lookup"><span data-stu-id="dffed-165">int</span></span> | <span data-ttu-id="dffed-166">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffed-166">Optional.</span></span> <span data-ttu-id="dffed-167">A duração do contrato de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="dffed-167">The duration of active user engagement.</span></span> <span data-ttu-id="dffed-168">Se não for fornecido, isso será calculado a partir do **startedDateTime** e do **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="dffed-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dffed-169">Relações</span><span class="sxs-lookup"><span data-stu-id="dffed-169">Relationships</span></span>

|<span data-ttu-id="dffed-170">Relação</span><span class="sxs-lookup"><span data-stu-id="dffed-170">Relationship</span></span> | <span data-ttu-id="dffed-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="dffed-171">Type</span></span> | <span data-ttu-id="dffed-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="dffed-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="dffed-173">atividade</span><span class="sxs-lookup"><span data-stu-id="dffed-173">activity</span></span>| [<span data-ttu-id="dffed-174">atividade</span><span class="sxs-lookup"><span data-stu-id="dffed-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="dffed-175">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dffed-175">Optional.</span></span> <span data-ttu-id="dffed-176">NavigationProperty/conFinamento; Propriedade de navegação para a atividade associada.</span><span class="sxs-lookup"><span data-stu-id="dffed-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dffed-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dffed-177">JSON representation</span></span>

<span data-ttu-id="dffed-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dffed-178">Here is a JSON representation of the resource.</span></span>

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
