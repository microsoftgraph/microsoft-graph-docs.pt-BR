---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6d32bcb2e480fe0589368ce06a995e3590f6b82e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520960"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="74a32-103">tipo de recurso schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-103">schedulingGroup resource type</span></span>

<span data-ttu-id="74a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74a32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74a32-105">Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função).</span><span class="sxs-lookup"><span data-stu-id="74a32-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="74a32-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="74a32-106">Methods</span></span>

| <span data-ttu-id="74a32-107">Método</span><span class="sxs-lookup"><span data-stu-id="74a32-107">Method</span></span>       | <span data-ttu-id="74a32-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74a32-108">Return Type</span></span>  |<span data-ttu-id="74a32-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74a32-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74a32-110">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-110">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="74a32-111">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-111">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="74a32-112">Criar uma página `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-112">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="74a32-113">Lista schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="74a32-113">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="74a32-114">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="74a32-114">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="74a32-115">Obter uma lista dos `schedulingGroups` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="74a32-115">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="74a32-116">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-116">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="74a32-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="74a32-118">Obter um `schedulingGroup` por ID.</span><span class="sxs-lookup"><span data-stu-id="74a32-118">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="74a32-119">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-119">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="74a32-120">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-120">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="74a32-121">Substituir um `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-121">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="74a32-122">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="74a32-122">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="74a32-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74a32-123">None</span></span> | <span data-ttu-id="74a32-124">Marcar `schedulingGroup` como inativa.</span><span class="sxs-lookup"><span data-stu-id="74a32-124">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="74a32-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74a32-125">Properties</span></span>
|<span data-ttu-id="74a32-126">Nome</span><span class="sxs-lookup"><span data-stu-id="74a32-126">Name</span></span>          |<span data-ttu-id="74a32-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="74a32-127">Type</span></span>           |<span data-ttu-id="74a32-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="74a32-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="74a32-129">id</span><span class="sxs-lookup"><span data-stu-id="74a32-129">id</span></span>            | `string`      |<span data-ttu-id="74a32-130">A ID da tarefa `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-130">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="74a32-131">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="74a32-131">displayName</span></span>   | `string`      | <span data-ttu-id="74a32-132">O nome de exibição do grupo `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-132">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="74a32-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74a32-133">Required.</span></span> |
| <span data-ttu-id="74a32-134">isActive</span><span class="sxs-lookup"><span data-stu-id="74a32-134">isActive</span></span>          |`bool`      | <span data-ttu-id="74a32-135">Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="74a32-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="74a32-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74a32-136">Required.</span></span> |
| <span data-ttu-id="74a32-137">userIds</span><span class="sxs-lookup"><span data-stu-id="74a32-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="74a32-138">A lista de IDs é membro de usuários da `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-138">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="74a32-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74a32-139">Required.</span></span> |
| <span data-ttu-id="74a32-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74a32-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="74a32-141">O carimbo de hora em que isso `schedulingGroup` foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="74a32-141">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="74a32-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="74a32-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74a32-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="74a32-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="74a32-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74a32-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="74a32-145">O carimbo de hora em que isso `schedulingGroup` foi criado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="74a32-145">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="74a32-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="74a32-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74a32-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="74a32-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="74a32-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="74a32-148">lastModifiedBy</span></span>        | [<span data-ttu-id="74a32-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="74a32-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="74a32-150">A identidade da última atualização `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="74a32-150">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74a32-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74a32-151">JSON representation</span></span>

<span data-ttu-id="74a32-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74a32-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
