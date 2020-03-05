---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: eadd5947a03fce69f790e2e9f0a4d738078002cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522064"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="ece22-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="ece22-103">outlookUser resource type</span></span>

<span data-ttu-id="ece22-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ece22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ece22-105">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="ece22-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ece22-106">Methods</span></span>

| <span data-ttu-id="ece22-107">Método</span><span class="sxs-lookup"><span data-stu-id="ece22-107">Method</span></span>           | <span data-ttu-id="ece22-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ece22-108">Return Type</span></span>    |<span data-ttu-id="ece22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece22-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ece22-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="ece22-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="ece22-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ece22-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="ece22-112">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="ece22-113">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="ece22-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="ece22-114">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="ece22-115">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="ece22-116">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ece22-116">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="ece22-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ece22-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="ece22-118">Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-118">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-119">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="ece22-119">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="ece22-120">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="ece22-121">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-121">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-122">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="ece22-122">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="ece22-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="ece22-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="ece22-124">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-124">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-125">Listar taskGroups</span><span class="sxs-lookup"><span data-stu-id="ece22-125">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="ece22-126">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-126">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="ece22-127">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-127">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-128">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="ece22-128">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="ece22-129">outlookTask</span><span class="sxs-lookup"><span data-stu-id="ece22-129">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="ece22-130">Crie uma tarefa do Outlook no grupo de tarefas padrão`My Tasks`() e na pasta de`Tasks`tarefas padrão () na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-130">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-131">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="ece22-131">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="ece22-132">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-132">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="ece22-133">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-133">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="ece22-134">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="ece22-134">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="ece22-135">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-135">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="ece22-136">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-136">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="ece22-137">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="ece22-137">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="ece22-138">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-138">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="ece22-139">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-139">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="ece22-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ece22-140">Properties</span></span>
<span data-ttu-id="ece22-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ece22-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ece22-142">Relações</span><span class="sxs-lookup"><span data-stu-id="ece22-142">Relationships</span></span>
| <span data-ttu-id="ece22-143">Relação</span><span class="sxs-lookup"><span data-stu-id="ece22-143">Relationship</span></span> | <span data-ttu-id="ece22-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece22-144">Type</span></span>   |<span data-ttu-id="ece22-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece22-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece22-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="ece22-146">masterCategories</span></span>|<span data-ttu-id="ece22-147">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="ece22-148">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="ece22-149">taskFolders</span><span class="sxs-lookup"><span data-stu-id="ece22-149">taskFolders</span></span>|<span data-ttu-id="ece22-150">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="ece22-151">As pastas de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-151">The user's Outlook task folders.</span></span> <span data-ttu-id="ece22-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ece22-152">Read-only.</span></span> <span data-ttu-id="ece22-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ece22-153">Nullable.</span></span>|
|<span data-ttu-id="ece22-154">taskGroups</span><span class="sxs-lookup"><span data-stu-id="ece22-154">taskGroups</span></span>|<span data-ttu-id="ece22-155">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="ece22-156">Grupos de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-156">The user's Outlook task groups.</span></span> <span data-ttu-id="ece22-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ece22-157">Read-only.</span></span> <span data-ttu-id="ece22-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ece22-158">Nullable.</span></span>|
|<span data-ttu-id="ece22-159">tarefas</span><span class="sxs-lookup"><span data-stu-id="ece22-159">tasks</span></span>|<span data-ttu-id="ece22-160">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="ece22-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="ece22-161">As tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="ece22-161">The user's Outlook tasks.</span></span> <span data-ttu-id="ece22-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ece22-162">Read-only.</span></span> <span data-ttu-id="ece22-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ece22-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ece22-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ece22-164">JSON representation</span></span>

<span data-ttu-id="ece22-165">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ece22-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
