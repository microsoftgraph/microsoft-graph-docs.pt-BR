---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c23cccabcea33b8cdaacba6ae9abede456c5c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009262"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="76cea-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="76cea-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76cea-104">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="76cea-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="76cea-105">Methods</span></span>

| <span data-ttu-id="76cea-106">Método</span><span class="sxs-lookup"><span data-stu-id="76cea-106">Method</span></span>           | <span data-ttu-id="76cea-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76cea-107">Return Type</span></span>    |<span data-ttu-id="76cea-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="76cea-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="76cea-109">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="76cea-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="76cea-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="76cea-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="76cea-111">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="76cea-112">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="76cea-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="76cea-113">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="76cea-114">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="76cea-115">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="76cea-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="76cea-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="76cea-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="76cea-117">Crie uma pasta de tarefas no grupo de tarefas padrão`My Tasks`() da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-118">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="76cea-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="76cea-119">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="76cea-120">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-121">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="76cea-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="76cea-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="76cea-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="76cea-123">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-124">Listar taskGroups</span><span class="sxs-lookup"><span data-stu-id="76cea-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="76cea-125">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="76cea-126">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-127">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="76cea-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="76cea-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="76cea-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="76cea-129">Crie uma tarefa do Outlook no grupo de tarefas padrão`My Tasks`() e na pasta de`Tasks`tarefas padrão () na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-130">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="76cea-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="76cea-131">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="76cea-132">Obter todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="76cea-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="76cea-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="76cea-134">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="76cea-135">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="76cea-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="76cea-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="76cea-137">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="76cea-138">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="76cea-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76cea-139">Properties</span></span>
<span data-ttu-id="76cea-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="76cea-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="76cea-141">Relações</span><span class="sxs-lookup"><span data-stu-id="76cea-141">Relationships</span></span>
| <span data-ttu-id="76cea-142">Relação</span><span class="sxs-lookup"><span data-stu-id="76cea-142">Relationship</span></span> | <span data-ttu-id="76cea-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="76cea-143">Type</span></span>   |<span data-ttu-id="76cea-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="76cea-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76cea-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="76cea-145">masterCategories</span></span>|<span data-ttu-id="76cea-146">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="76cea-147">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="76cea-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="76cea-148">taskFolders</span></span>|<span data-ttu-id="76cea-149">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="76cea-150">As pastas de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-150">The user's Outlook task folders.</span></span> <span data-ttu-id="76cea-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76cea-151">Read-only.</span></span> <span data-ttu-id="76cea-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="76cea-152">Nullable.</span></span>|
|<span data-ttu-id="76cea-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="76cea-153">taskGroups</span></span>|<span data-ttu-id="76cea-154">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="76cea-155">Grupos de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-155">The user's Outlook task groups.</span></span> <span data-ttu-id="76cea-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76cea-156">Read-only.</span></span> <span data-ttu-id="76cea-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="76cea-157">Nullable.</span></span>|
|<span data-ttu-id="76cea-158">tarefas</span><span class="sxs-lookup"><span data-stu-id="76cea-158">tasks</span></span>|<span data-ttu-id="76cea-159">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="76cea-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="76cea-160">As tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="76cea-160">The user's Outlook tasks.</span></span> <span data-ttu-id="76cea-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76cea-161">Read-only.</span></span> <span data-ttu-id="76cea-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="76cea-162">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76cea-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76cea-163">JSON representation</span></span>

<span data-ttu-id="76cea-164">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="76cea-164">Here is a JSON representation of the resource</span></span>

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
