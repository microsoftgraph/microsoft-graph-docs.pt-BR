---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6473a7a3808982467f50bafc810cbca80e4ce0dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998338"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="2ffa4-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="2ffa4-103">outlookUser resource type</span></span>

<span data-ttu-id="2ffa4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ffa4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="2ffa4-105">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="2ffa4-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2ffa4-106">Methods</span></span>

| <span data-ttu-id="2ffa4-107">Método</span><span class="sxs-lookup"><span data-stu-id="2ffa4-107">Method</span></span>           | <span data-ttu-id="2ffa4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ffa4-108">Return Type</span></span>    |<span data-ttu-id="2ffa4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffa4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ffa4-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="2ffa4-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="2ffa4-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2ffa4-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="2ffa4-112">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="2ffa4-113">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="2ffa4-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="2ffa4-114">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="2ffa4-115">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="2ffa4-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="2ffa4-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="2ffa4-117">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="2ffa4-118">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="2ffa4-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="2ffa4-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="2ffa4-120">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="2ffa4-121">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |
|<span data-ttu-id="2ffa4-122">[Criar outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span></span> |[<span data-ttu-id="2ffa4-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2ffa4-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="2ffa4-124">Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-124">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|<span data-ttu-id="2ffa4-125">[Listar taskFolders](../api/outlookuser-list-taskfolders.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-125">[List taskFolders](../api/outlookuser-list-taskfolders.md) (deprecated)</span></span> |<span data-ttu-id="2ffa4-126">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-126">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="2ffa4-127">Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-127">Get all the Outlook task folders in the user's mailbox.</span></span>|
|<span data-ttu-id="2ffa4-128">[Criar outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-128">[Create outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (deprecated)</span></span> |[<span data-ttu-id="2ffa4-129">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2ffa4-129">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="2ffa4-130">Criar um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-130">Create an Outlook task group in the user's mailbox.</span></span>|
|<span data-ttu-id="2ffa4-131">[Listar taskGroups](../api/outlookuser-list-taskgroups.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-131">[List taskGroups](../api/outlookuser-list-taskgroups.md) (deprecated)</span></span> |<span data-ttu-id="2ffa4-132">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-132">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="2ffa4-133">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-133">Get all the Outlook task groups in the user's mailbox.</span></span>|
|<span data-ttu-id="2ffa4-134">[Criar outlookTask](../api/outlookuser-post-tasks.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-134">[Create outlookTask](../api/outlookuser-post-tasks.md) (deprecated)</span></span> |[<span data-ttu-id="2ffa4-135">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2ffa4-135">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="2ffa4-136">Crie uma tarefa do Outlook no grupo de tarefas padrão ( `My Tasks` ) e na pasta de tarefas padrão ( `Tasks` ) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-136">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|<span data-ttu-id="2ffa4-137">[Listar tarefas](../api/outlookuser-list-tasks.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-137">[List tasks](../api/outlookuser-list-tasks.md) (deprecated)</span></span> |<span data-ttu-id="2ffa4-138">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-138">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="2ffa4-139">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-139">Get all the Outlook tasks in the user's mailbox.</span></span>|



## <a name="properties"></a><span data-ttu-id="2ffa4-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ffa4-140">Properties</span></span>
<span data-ttu-id="2ffa4-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2ffa4-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2ffa4-142">Relações</span><span class="sxs-lookup"><span data-stu-id="2ffa4-142">Relationships</span></span>
| <span data-ttu-id="2ffa4-143">Relação</span><span class="sxs-lookup"><span data-stu-id="2ffa4-143">Relationship</span></span> | <span data-ttu-id="2ffa4-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ffa4-144">Type</span></span>   |<span data-ttu-id="2ffa4-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffa4-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ffa4-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="2ffa4-146">masterCategories</span></span>|<span data-ttu-id="2ffa4-147">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="2ffa4-148">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="2ffa4-149">taskFolders (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-149">taskFolders (deprecated)</span></span>|<span data-ttu-id="2ffa4-150">coleção [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="2ffa4-151">As pastas de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-151">The user's Outlook task folders.</span></span> <span data-ttu-id="2ffa4-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-152">Read-only.</span></span> <span data-ttu-id="2ffa4-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-153">Nullable.</span></span>|
|<span data-ttu-id="2ffa4-154">taskGroups (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-154">taskGroups (deprecated)</span></span>|<span data-ttu-id="2ffa4-155">coleção [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="2ffa4-156">Grupos de tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-156">The user's Outlook task groups.</span></span> <span data-ttu-id="2ffa4-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-157">Read-only.</span></span> <span data-ttu-id="2ffa4-158">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-158">Nullable.</span></span>|
|<span data-ttu-id="2ffa4-159">tarefas (preterido)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-159">tasks (deprecated)</span></span>|<span data-ttu-id="2ffa4-160">coleção [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="2ffa4-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="2ffa4-161">As tarefas do Outlook do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-161">The user's Outlook tasks.</span></span> <span data-ttu-id="2ffa4-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-162">Read-only.</span></span> <span data-ttu-id="2ffa4-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ffa4-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ffa4-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ffa4-164">JSON representation</span></span>

<span data-ttu-id="2ffa4-165">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2ffa4-165">Here is a JSON representation of the resource</span></span>

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


