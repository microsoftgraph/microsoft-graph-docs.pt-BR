---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9f4f494b21a1139ba9a9e0771dcbc41d363bab2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965296"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="a1356-103">tipo de recurso schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1356-104">Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função).</span><span class="sxs-lookup"><span data-stu-id="a1356-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="a1356-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a1356-105">Methods</span></span>

| <span data-ttu-id="a1356-106">Método</span><span class="sxs-lookup"><span data-stu-id="a1356-106">Method</span></span>       | <span data-ttu-id="a1356-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a1356-107">Return Type</span></span>  |<span data-ttu-id="a1356-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1356-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1356-109">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="a1356-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a1356-111">Criar uma página `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="a1356-112">Lista schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="a1356-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="a1356-113">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="a1356-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="a1356-114">Obter uma lista dos `schedulingGroups` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="a1356-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="a1356-115">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="a1356-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a1356-117">Obter um `schedulingGroup` por ID.</span><span class="sxs-lookup"><span data-stu-id="a1356-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="a1356-118">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="a1356-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="a1356-120">Substituir um `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="a1356-121">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a1356-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="a1356-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1356-122">None</span></span> | <span data-ttu-id="a1356-123">Marcar `schedulingGroup` como inativa.</span><span class="sxs-lookup"><span data-stu-id="a1356-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1356-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1356-124">Properties</span></span>
|<span data-ttu-id="a1356-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a1356-125">Name</span></span>          |<span data-ttu-id="a1356-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1356-126">Type</span></span>           |<span data-ttu-id="a1356-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1356-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="a1356-128">id</span><span class="sxs-lookup"><span data-stu-id="a1356-128">id</span></span>            | `string`      |<span data-ttu-id="a1356-129">A ID da tarefa `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="a1356-130">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="a1356-130">displayName</span></span>   | `string`      | <span data-ttu-id="a1356-131">O nome de exibição do grupo `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="a1356-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1356-132">Required.</span></span> |
| <span data-ttu-id="a1356-133">isActive</span><span class="sxs-lookup"><span data-stu-id="a1356-133">isActive</span></span>          |`bool`      | <span data-ttu-id="a1356-134">Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="a1356-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="a1356-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1356-135">Required.</span></span> |
| <span data-ttu-id="a1356-136">userIds</span><span class="sxs-lookup"><span data-stu-id="a1356-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="a1356-137">A lista de IDs é membro de usuários da `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="a1356-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1356-138">Required.</span></span> |
| <span data-ttu-id="a1356-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1356-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="a1356-140">O carimbo de hora em que isso `schedulingGroup` foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="a1356-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="a1356-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a1356-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a1356-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="a1356-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="a1356-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1356-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="a1356-144">O carimbo de hora em que isso `schedulingGroup` foi criado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a1356-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="a1356-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a1356-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a1356-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="a1356-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="a1356-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a1356-147">lastModifiedBy</span></span>        | [<span data-ttu-id="a1356-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1356-148">identitySet</span></span>](identityset.md) |<span data-ttu-id="a1356-149">A identidade da última atualização `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="a1356-149">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1356-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1356-150">JSON representation</span></span>

<span data-ttu-id="a1356-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1356-151">Here is a JSON representation of the resource.</span></span>

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
