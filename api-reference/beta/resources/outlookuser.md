---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 15afe75d10bad489b913eaf7215cbc8327e02317
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130666"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="70a8b-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="70a8b-103">outlookUser resource type</span></span>

<span data-ttu-id="70a8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="70a8b-105">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="70a8b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="70a8b-106">Methods</span></span>

| <span data-ttu-id="70a8b-107">Método</span><span class="sxs-lookup"><span data-stu-id="70a8b-107">Method</span></span>           | <span data-ttu-id="70a8b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70a8b-108">Return Type</span></span>    |<span data-ttu-id="70a8b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a8b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70a8b-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="70a8b-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="70a8b-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="70a8b-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="70a8b-112">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="70a8b-113">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="70a8b-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="70a8b-114">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="70a8b-115">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="70a8b-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="70a8b-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="70a8b-117">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="70a8b-118">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="70a8b-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="70a8b-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="70a8b-120">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="70a8b-121">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |
|<span data-ttu-id="70a8b-122">[Criar outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span></span> |[<span data-ttu-id="70a8b-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="70a8b-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="70a8b-124">Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-124">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|<span data-ttu-id="70a8b-125">[Listar taskFolders](../api/outlookuser-list-taskfolders.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-125">[List taskFolders](../api/outlookuser-list-taskfolders.md) (deprecated)</span></span> |<span data-ttu-id="70a8b-126">[Coleção outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-126">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="70a8b-127">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-127">Get all the Outlook task folders in the user's mailbox.</span></span>|
|<span data-ttu-id="70a8b-128">[Criar outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-128">[Create outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (deprecated)</span></span> |[<span data-ttu-id="70a8b-129">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="70a8b-129">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="70a8b-130">Crie um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-130">Create an Outlook task group in the user's mailbox.</span></span>|
|<span data-ttu-id="70a8b-131">[Listar taskGroups](../api/outlookuser-list-taskgroups.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-131">[List taskGroups](../api/outlookuser-list-taskgroups.md) (deprecated)</span></span> |<span data-ttu-id="70a8b-132">[Coleção outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-132">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="70a8b-133">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-133">Get all the Outlook task groups in the user's mailbox.</span></span>|
|<span data-ttu-id="70a8b-134">[Criar outlookTask](../api/outlookuser-post-tasks.md)(obsoleto)</span><span class="sxs-lookup"><span data-stu-id="70a8b-134">[Create outlookTask](../api/outlookuser-post-tasks.md) (deprecated)</span></span> |[<span data-ttu-id="70a8b-135">outlookTask</span><span class="sxs-lookup"><span data-stu-id="70a8b-135">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="70a8b-136">Crie uma tarefa do Outlook no grupo de tarefas padrão ( ) e na pasta de tarefas `My Tasks` padrão ( ) na caixa de correio do `Tasks` usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-136">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|<span data-ttu-id="70a8b-137">[Listar de tarefas](../api/outlookuser-list-tasks.md) (obsoleto)</span><span class="sxs-lookup"><span data-stu-id="70a8b-137">[List tasks](../api/outlookuser-list-tasks.md) (deprecated)</span></span> |<span data-ttu-id="70a8b-138">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-138">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="70a8b-139">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-139">Get all the Outlook tasks in the user's mailbox.</span></span>|



## <a name="properties"></a><span data-ttu-id="70a8b-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70a8b-140">Properties</span></span>
<span data-ttu-id="70a8b-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="70a8b-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="70a8b-142">Relações</span><span class="sxs-lookup"><span data-stu-id="70a8b-142">Relationships</span></span>
| <span data-ttu-id="70a8b-143">Relação</span><span class="sxs-lookup"><span data-stu-id="70a8b-143">Relationship</span></span> | <span data-ttu-id="70a8b-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a8b-144">Type</span></span>   |<span data-ttu-id="70a8b-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a8b-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70a8b-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="70a8b-146">masterCategories</span></span>|<span data-ttu-id="70a8b-147">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="70a8b-148">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="70a8b-149">taskFolders (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-149">taskFolders (deprecated)</span></span>|<span data-ttu-id="70a8b-150">[Coleção outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="70a8b-151">As pastas de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-151">The user's Outlook task folders.</span></span> <span data-ttu-id="70a8b-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70a8b-152">Read-only.</span></span> <span data-ttu-id="70a8b-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="70a8b-153">Nullable.</span></span>|
|<span data-ttu-id="70a8b-154">taskGroups (preterido)</span><span class="sxs-lookup"><span data-stu-id="70a8b-154">taskGroups (deprecated)</span></span>|<span data-ttu-id="70a8b-155">[Coleção outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="70a8b-156">Os grupos de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-156">The user's Outlook task groups.</span></span> <span data-ttu-id="70a8b-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70a8b-157">Read-only.</span></span> <span data-ttu-id="70a8b-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="70a8b-158">Nullable.</span></span>|
|<span data-ttu-id="70a8b-159">tarefas (preterida)</span><span class="sxs-lookup"><span data-stu-id="70a8b-159">tasks (deprecated)</span></span>|<span data-ttu-id="70a8b-160">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="70a8b-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="70a8b-161">As tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a8b-161">The user's Outlook tasks.</span></span> <span data-ttu-id="70a8b-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70a8b-162">Read-only.</span></span> <span data-ttu-id="70a8b-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="70a8b-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70a8b-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70a8b-164">JSON representation</span></span>

<span data-ttu-id="70a8b-165">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="70a8b-165">Here is a JSON representation of the resource</span></span>

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


