---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f8265f9da285ce0f52e6201ffdb1298893b86753
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574093"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="bf8e5-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="bf8e5-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf8e5-104">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="bf8e5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="bf8e5-105">Methods</span></span>

| <span data-ttu-id="bf8e5-106">Método</span><span class="sxs-lookup"><span data-stu-id="bf8e5-106">Method</span></span>           | <span data-ttu-id="bf8e5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bf8e5-107">Return Type</span></span>    |<span data-ttu-id="bf8e5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf8e5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf8e5-109">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="bf8e5-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="bf8e5-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bf8e5-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="bf8e5-111">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="bf8e5-112">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="bf8e5-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="bf8e5-113">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="bf8e5-114">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="bf8e5-115">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="bf8e5-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="bf8e5-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="bf8e5-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="bf8e5-117">Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-118">Lista taskFolders</span><span class="sxs-lookup"><span data-stu-id="bf8e5-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="bf8e5-119">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bf8e5-120">Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-121">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bf8e5-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="bf8e5-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bf8e5-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="bf8e5-123">Crie um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-124">Lista taskGroups</span><span class="sxs-lookup"><span data-stu-id="bf8e5-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="bf8e5-125">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="bf8e5-126">Obtenha todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-127">Criar outlookTask</span><span class="sxs-lookup"><span data-stu-id="bf8e5-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="bf8e5-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="bf8e5-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="bf8e5-129">Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-130">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="bf8e5-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="bf8e5-131">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="bf8e5-132">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="bf8e5-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="bf8e5-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="bf8e5-134">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="bf8e5-135">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="bf8e5-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="bf8e5-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="bf8e5-137">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="bf8e5-138">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="bf8e5-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf8e5-139">Properties</span></span>
<span data-ttu-id="bf8e5-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf8e5-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bf8e5-141">Relações</span><span class="sxs-lookup"><span data-stu-id="bf8e5-141">Relationships</span></span>
| <span data-ttu-id="bf8e5-142">Relação</span><span class="sxs-lookup"><span data-stu-id="bf8e5-142">Relationship</span></span> | <span data-ttu-id="bf8e5-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf8e5-143">Type</span></span>   |<span data-ttu-id="bf8e5-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf8e5-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf8e5-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="bf8e5-145">masterCategories</span></span>|<span data-ttu-id="bf8e5-146">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="bf8e5-147">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="bf8e5-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="bf8e5-148">taskFolders</span></span>|<span data-ttu-id="bf8e5-149">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bf8e5-150">Pastas de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-150">The user's Outlook task folders.</span></span> <span data-ttu-id="bf8e5-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-151">Read-only.</span></span> <span data-ttu-id="bf8e5-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-152">Nullable.</span></span>|
|<span data-ttu-id="bf8e5-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="bf8e5-153">taskGroups</span></span>|<span data-ttu-id="bf8e5-154">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="bf8e5-155">Grupos de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-155">The user's Outlook task groups.</span></span> <span data-ttu-id="bf8e5-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-156">Read-only.</span></span> <span data-ttu-id="bf8e5-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-157">Nullable.</span></span>|
|<span data-ttu-id="bf8e5-158">tarefas</span><span class="sxs-lookup"><span data-stu-id="bf8e5-158">tasks</span></span>|<span data-ttu-id="bf8e5-159">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="bf8e5-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="bf8e5-160">Tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-160">The user's Outlook tasks.</span></span> <span data-ttu-id="bf8e5-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-161">Read-only.</span></span> <span data-ttu-id="bf8e5-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bf8e5-162">Nullable.</span></span>|


<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.outlookUser"
}-->
```json
{
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
