---
title: tipo de recurso de historyItem
description: Representa um item de histórico de uma atividade em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade. À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.
localization_priority: Normal
ms.openlocfilehash: 7eb6d72b55530d1938c9c092dd5b80f54929a3e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825771"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="a93a8-106">tipo de recurso de historyItem</span><span class="sxs-lookup"><span data-stu-id="a93a8-106">historyItem resource type</span></span>

> <span data-ttu-id="a93a8-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a93a8-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a93a8-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a93a8-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a93a8-109">Representa um item de histórico de uma [atividade](projectrome-activity.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a93a8-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="a93a8-110">As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo.</span><span class="sxs-lookup"><span data-stu-id="a93a8-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="a93a8-111">Quando um usuário emprega com que a atividade, o compromisso é capturado como um item de histórico que indica a hora de início e término para a atividade.</span><span class="sxs-lookup"><span data-stu-id="a93a8-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="a93a8-112">À medida que o usuário emprega novamente com que a atividade ao longo do tempo, vários itens de histórico são registrados para atividade de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="a93a8-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="a93a8-113">Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **atividade** para refletir o período de participação do usuário.</span><span class="sxs-lookup"><span data-stu-id="a93a8-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="a93a8-114">Cada vez que um usuário emprega-se novamente com uma atividade, um novo **historyItem** é adicionado à atividade acumular compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="a93a8-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="a93a8-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="a93a8-115">Methods</span></span>

|<span data-ttu-id="a93a8-116">Método</span><span class="sxs-lookup"><span data-stu-id="a93a8-116">Method</span></span> | <span data-ttu-id="a93a8-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a93a8-117">Return Type</span></span> | <span data-ttu-id="a93a8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93a8-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="a93a8-119">Criar ou substituir historyItem</span><span class="sxs-lookup"><span data-stu-id="a93a8-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="a93a8-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="a93a8-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="a93a8-121">Cria ou substitui um existente **historyItem** para a atividade (upsert).</span><span class="sxs-lookup"><span data-stu-id="a93a8-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="a93a8-122">A ID deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="a93a8-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="a93a8-123">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="a93a8-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="a93a8-124">Nenhum conteúdo</span><span class="sxs-lookup"><span data-stu-id="a93a8-124">No Content</span></span> | <span data-ttu-id="a93a8-125">Exclui o **historyItem** especificado para a atividade.</span><span class="sxs-lookup"><span data-stu-id="a93a8-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="a93a8-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a93a8-126">Properties</span></span>

|<span data-ttu-id="a93a8-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a93a8-127">Name</span></span> | <span data-ttu-id="a93a8-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a93a8-128">Type</span></span> | <span data-ttu-id="a93a8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93a8-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a93a8-130">status</span><span class="sxs-lookup"><span data-stu-id="a93a8-130">status</span></span> | <span data-ttu-id="a93a8-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="a93a8-131">EnumType</span></span> | <span data-ttu-id="a93a8-132">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="a93a8-132">Set by the server.</span></span> <span data-ttu-id="a93a8-133">Um código de status usado para identificar objetos válidos.</span><span class="sxs-lookup"><span data-stu-id="a93a8-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="a93a8-134">Valores: ativo, atualizado, excluídos, ignorado.</span><span class="sxs-lookup"><span data-stu-id="a93a8-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="a93a8-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="a93a8-135">userTimezone</span></span> | <span data-ttu-id="a93a8-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a93a8-136">String</span></span> | <span data-ttu-id="a93a8-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a93a8-137">Optional.</span></span> <span data-ttu-id="a93a8-138">O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade.</span><span class="sxs-lookup"><span data-stu-id="a93a8-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="a93a8-139">Valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.</span><span class="sxs-lookup"><span data-stu-id="a93a8-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="a93a8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a93a8-140">createdDateTime</span></span> | <span data-ttu-id="a93a8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a93a8-141">DateTimeOffset</span></span> | <span data-ttu-id="a93a8-142">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="a93a8-142">Set by the server.</span></span> <span data-ttu-id="a93a8-143">Data e hora em UTC quando o objeto foi criado no servidor.</span><span class="sxs-lookup"><span data-stu-id="a93a8-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="a93a8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a93a8-144">lastModifiedDateTime</span></span> | <span data-ttu-id="a93a8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a93a8-145">DateTimeOffset</span></span> | <span data-ttu-id="a93a8-146">Definido pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="a93a8-146">Set by the server.</span></span> <span data-ttu-id="a93a8-147">Data e hora em UTC quando o objeto foi modificado no servidor.</span><span class="sxs-lookup"><span data-stu-id="a93a8-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="a93a8-148">id</span><span class="sxs-lookup"><span data-stu-id="a93a8-148">id</span></span> | <span data-ttu-id="a93a8-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a93a8-149">String</span></span> | <span data-ttu-id="a93a8-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a93a8-150">Required.</span></span> <span data-ttu-id="a93a8-151">GUID do conjunto de cliente para o objeto **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="a93a8-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="a93a8-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="a93a8-152">startedDateTime</span></span> | <span data-ttu-id="a93a8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a93a8-153">DateTimeOffset</span></span> | <span data-ttu-id="a93a8-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a93a8-154">Required.</span></span> <span data-ttu-id="a93a8-155">DateTime UTC quando **historyItem** (sessão atividade) foi iniciado.</span><span class="sxs-lookup"><span data-stu-id="a93a8-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="a93a8-156">Necessário para o histórico de linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="a93a8-156">Required for timeline history.</span></span>|
|<span data-ttu-id="a93a8-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="a93a8-157">lastActiveDateTime</span></span> | <span data-ttu-id="a93a8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a93a8-158">DateTimeOffset</span></span> | <span data-ttu-id="a93a8-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a93a8-159">Optional.</span></span> <span data-ttu-id="a93a8-160">DateTime UTC quando **historyItem** (sessão atividade) foi compreendido última como status ativo ou terminar - se for null, **historyItem** deve ser contínuo.</span><span class="sxs-lookup"><span data-stu-id="a93a8-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="a93a8-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a93a8-161">expirationDateTime</span></span> | <span data-ttu-id="a93a8-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a93a8-162">DateTimeOffset</span></span> | <span data-ttu-id="a93a8-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a93a8-163">Optional.</span></span> <span data-ttu-id="a93a8-164">DateTime UTC quando os **historyItem** passará rígido-delete.</span><span class="sxs-lookup"><span data-stu-id="a93a8-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="a93a8-165">Pode ser definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a93a8-165">Can be set by the client.</span></span>|
|<span data-ttu-id="a93a8-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="a93a8-166">activeDurationSeconds</span></span> | <span data-ttu-id="a93a8-167">int</span><span class="sxs-lookup"><span data-stu-id="a93a8-167">int</span></span> | <span data-ttu-id="a93a8-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a93a8-168">Optional.</span></span> <span data-ttu-id="a93a8-169">A duração de participação de usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a93a8-169">The duration of active user engagement.</span></span> <span data-ttu-id="a93a8-170">Se não fornecido, isso é calculado do **startedDateTime** e **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a93a8-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a93a8-171">Relações</span><span class="sxs-lookup"><span data-stu-id="a93a8-171">Relationships</span></span>

|<span data-ttu-id="a93a8-172">Relação</span><span class="sxs-lookup"><span data-stu-id="a93a8-172">Relationship</span></span> | <span data-ttu-id="a93a8-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="a93a8-173">Type</span></span> | <span data-ttu-id="a93a8-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93a8-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="a93a8-175">atividade</span><span class="sxs-lookup"><span data-stu-id="a93a8-175">activity</span></span>| [<span data-ttu-id="a93a8-176">atividade</span><span class="sxs-lookup"><span data-stu-id="a93a8-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="a93a8-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a93a8-177">Optional.</span></span> <span data-ttu-id="a93a8-178">NavigationProperty/contenção; propriedade de navegação à atividade associada.</span><span class="sxs-lookup"><span data-stu-id="a93a8-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a93a8-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a93a8-179">JSON representation</span></span>

<span data-ttu-id="a93a8-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a93a8-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
