---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a3f3b76f84d081d11005a567b318d9f0ea83a667
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077671"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="7b535-103">tipo de recurso schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="7b535-103">schedulingGroup resource type</span></span>

<span data-ttu-id="7b535-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b535-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b535-105">Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função).</span><span class="sxs-lookup"><span data-stu-id="7b535-105">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="7b535-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b535-106">Methods</span></span>

| <span data-ttu-id="7b535-107">Método</span><span class="sxs-lookup"><span data-stu-id="7b535-107">Method</span></span>       | <span data-ttu-id="7b535-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b535-108">Return Type</span></span>  |<span data-ttu-id="7b535-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b535-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b535-110">Listar</span><span class="sxs-lookup"><span data-stu-id="7b535-110">List</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="7b535-111">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="7b535-111">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="7b535-112">Obtenha a lista de **schedulingGroups** em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="7b535-112">Get the list of **schedulingGroups** in a schedule.</span></span>|
|[<span data-ttu-id="7b535-113">Criar</span><span class="sxs-lookup"><span data-stu-id="7b535-113">Create</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="7b535-114">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="7b535-114">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="7b535-115">Criar um nov **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-115">Create a new **schedulingGroup**.</span></span>|
|[<span data-ttu-id="7b535-116">Obter</span><span class="sxs-lookup"><span data-stu-id="7b535-116">Get</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="7b535-117">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="7b535-117">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="7b535-118">Obtenha um **schedulingGroup** por ID.</span><span class="sxs-lookup"><span data-stu-id="7b535-118">Get a **schedulingGroup** by ID.</span></span>|
|[<span data-ttu-id="7b535-119">Delete</span><span class="sxs-lookup"><span data-stu-id="7b535-119">Delete</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="7b535-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b535-120">None</span></span> | <span data-ttu-id="7b535-121">Marque **schedulingGroup** como inativo.</span><span class="sxs-lookup"><span data-stu-id="7b535-121">Mark **schedulingGroup** as inactive.</span></span>|
|[<span data-ttu-id="7b535-122">Substituir</span><span class="sxs-lookup"><span data-stu-id="7b535-122">Replace</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="7b535-123">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="7b535-123">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="7b535-124">Substituir **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-124">Replace a **schedulingGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b535-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b535-125">Properties</span></span>
|<span data-ttu-id="7b535-126">Nome</span><span class="sxs-lookup"><span data-stu-id="7b535-126">Name</span></span>          |<span data-ttu-id="7b535-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b535-127">Type</span></span>           |<span data-ttu-id="7b535-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b535-128">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="7b535-129">id</span><span class="sxs-lookup"><span data-stu-id="7b535-129">id</span></span>            | `string`      |<span data-ttu-id="7b535-130">ID do **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-130">ID of the **schedulingGroup**.</span></span>|
| <span data-ttu-id="7b535-131">displayName</span><span class="sxs-lookup"><span data-stu-id="7b535-131">displayName</span></span>   | `string`      | <span data-ttu-id="7b535-132">O nome de exibição do**schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-132">The display name for the **schedulingGroup**.</span></span> <span data-ttu-id="7b535-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b535-133">Required.</span></span> |
| <span data-ttu-id="7b535-134">isActive</span><span class="sxs-lookup"><span data-stu-id="7b535-134">isActive</span></span>          |`bool`      | <span data-ttu-id="7b535-135">Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="7b535-135">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="7b535-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b535-136">Required.</span></span> |
| <span data-ttu-id="7b535-137">userIds</span><span class="sxs-lookup"><span data-stu-id="7b535-137">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="7b535-138">A lista de IDs de usuários que são membros do**schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-138">The list of user IDs that are a member of the **schedulingGroup**.</span></span> <span data-ttu-id="7b535-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b535-139">Required.</span></span> |
| <span data-ttu-id="7b535-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b535-140">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="7b535-141">O carimbo de hora em que esse **schedulingGroup** foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="7b535-141">The time stamp in which this **schedulingGroup** was first created.</span></span> <span data-ttu-id="7b535-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7b535-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7b535-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7b535-143">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7b535-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b535-144">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="7b535-145">O carimbo de hora em que esse **schedulingGroup** foi criado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7b535-145">The time stamp in which this **schedulingGroup** was last updated.</span></span> <span data-ttu-id="7b535-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7b535-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7b535-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7b535-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7b535-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7b535-148">lastModifiedBy</span></span>        | [<span data-ttu-id="7b535-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="7b535-149">identitySet</span></span>](identityset.md) |<span data-ttu-id="7b535-150">A identidade da última atualização desse **schedulingGroup**.</span><span class="sxs-lookup"><span data-stu-id="7b535-150">The identity that last updated this **schedulingGroup**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b535-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b535-151">JSON representation</span></span>

<span data-ttu-id="7b535-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b535-152">The following is a JSON representation of the resource.</span></span>

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

