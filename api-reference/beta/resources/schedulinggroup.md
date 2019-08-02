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
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="9cffa-103">tipo de recurso schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cffa-104">Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função).</span><span class="sxs-lookup"><span data-stu-id="9cffa-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="9cffa-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9cffa-105">Methods</span></span>

| <span data-ttu-id="9cffa-106">Método</span><span class="sxs-lookup"><span data-stu-id="9cffa-106">Method</span></span>       | <span data-ttu-id="9cffa-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9cffa-107">Return Type</span></span>  |<span data-ttu-id="9cffa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cffa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cffa-109">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="9cffa-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9cffa-111">Criar uma página `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="9cffa-112">Lista schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="9cffa-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="9cffa-113">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="9cffa-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="9cffa-114">Obter uma lista dos `schedulingGroups` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="9cffa-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="9cffa-115">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="9cffa-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9cffa-117">Obter um `schedulingGroup` por ID.</span><span class="sxs-lookup"><span data-stu-id="9cffa-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="9cffa-118">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="9cffa-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="9cffa-120">Substituir um `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="9cffa-121">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9cffa-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="9cffa-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9cffa-122">None</span></span> | <span data-ttu-id="9cffa-123">Marcar `schedulingGroup` como inativa.</span><span class="sxs-lookup"><span data-stu-id="9cffa-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cffa-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cffa-124">Properties</span></span>
|<span data-ttu-id="9cffa-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9cffa-125">Name</span></span>          |<span data-ttu-id="9cffa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cffa-126">Type</span></span>           |<span data-ttu-id="9cffa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cffa-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="9cffa-128">id</span><span class="sxs-lookup"><span data-stu-id="9cffa-128">id</span></span>            | `string`      |<span data-ttu-id="9cffa-129">A ID da tarefa `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="9cffa-130">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="9cffa-130">displayName</span></span>   | `string`      | <span data-ttu-id="9cffa-131">O nome de exibição do grupo `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="9cffa-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cffa-132">Required.</span></span> |
| <span data-ttu-id="9cffa-133">isActive</span><span class="sxs-lookup"><span data-stu-id="9cffa-133">isActive</span></span>          |`bool`      | <span data-ttu-id="9cffa-134">Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="9cffa-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="9cffa-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cffa-135">Required.</span></span> |
| <span data-ttu-id="9cffa-136">userIds</span><span class="sxs-lookup"><span data-stu-id="9cffa-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="9cffa-137">A lista de IDs é membro de usuários da `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="9cffa-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cffa-138">Required.</span></span> |
| <span data-ttu-id="9cffa-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cffa-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="9cffa-140">O carimbo de hora em que isso `schedulingGroup` foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="9cffa-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="9cffa-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9cffa-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cffa-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9cffa-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9cffa-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cffa-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="9cffa-144">O carimbo de hora em que isso `schedulingGroup` foi criado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9cffa-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="9cffa-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9cffa-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cffa-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9cffa-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9cffa-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9cffa-147">lastModifiedBy</span></span>        | [<span data-ttu-id="9cffa-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="9cffa-148">identitySet</span></span>](identityset.md) |<span data-ttu-id="9cffa-149">A identidade da última atualização `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="9cffa-149">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cffa-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cffa-150">JSON representation</span></span>

<span data-ttu-id="9cffa-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cffa-151">Here is a JSON representation of the resource.</span></span>

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
