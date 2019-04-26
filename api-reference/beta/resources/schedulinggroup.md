---
title: tipo de recurso schedulingGroup
description: Um agrupamento lógico de membros do cronograma (geralmente pela função).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562944"
---
# <a name="schedulinggroup-resource-type"></a><span data-ttu-id="941fd-103">tipo de recurso schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-103">schedulingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941fd-104">Um agrupamento lógico de usuários em um [cronograma](schedule.md) (geralmente pela função).</span><span class="sxs-lookup"><span data-stu-id="941fd-104">A logical grouping of users in a [schedule](schedule.md) (usually by role).</span></span> 

## <a name="methods"></a><span data-ttu-id="941fd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="941fd-105">Methods</span></span>

| <span data-ttu-id="941fd-106">Método</span><span class="sxs-lookup"><span data-stu-id="941fd-106">Method</span></span>       | <span data-ttu-id="941fd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="941fd-107">Return Type</span></span>  |<span data-ttu-id="941fd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="941fd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="941fd-109">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-109">Create schedulingGroup</span></span>](../api/schedule-post-schedulinggroups.md) | [<span data-ttu-id="941fd-110">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-110">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="941fd-111">Criar uma página `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-111">Create a new `schedulingGroup`.</span></span>|
|[<span data-ttu-id="941fd-112">Lista schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="941fd-112">List schedulingGroups</span></span>](../api/schedule-list-schedulinggroups.md) | <span data-ttu-id="941fd-113">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="941fd-113">[schedulingGroup](schedulinggroup.md) collection</span></span> | <span data-ttu-id="941fd-114">Obter uma lista dos `schedulingGroups` em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="941fd-114">Get the list of `schedulingGroups` in a schedule.</span></span>|
|[<span data-ttu-id="941fd-115">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-115">Get schedulingGroup</span></span>](../api/schedulinggroup-get.md) | [<span data-ttu-id="941fd-116">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-116">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="941fd-117">Obter um `schedulingGroup` por ID.</span><span class="sxs-lookup"><span data-stu-id="941fd-117">Get a `schedulingGroup` by ID.</span></span>|
|[<span data-ttu-id="941fd-118">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-118">Replace schedulingGroup</span></span>](../api/schedulinggroup-put.md) | [<span data-ttu-id="941fd-119">schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-119">schedulingGroup</span></span>](schedulinggroup.md) | <span data-ttu-id="941fd-120">Substituir um `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-120">Replace a `schedulingGroup`.</span></span>|
|[<span data-ttu-id="941fd-121">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="941fd-121">Delete schedulingGroup</span></span>](../api/schedulinggroup-delete.md) | <span data-ttu-id="941fd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="941fd-122">None</span></span> | <span data-ttu-id="941fd-123">Marcar `schedulingGroup` como inativa.</span><span class="sxs-lookup"><span data-stu-id="941fd-123">Mark `schedulingGroup` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="941fd-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="941fd-124">Properties</span></span>
|<span data-ttu-id="941fd-125">Nome</span><span class="sxs-lookup"><span data-stu-id="941fd-125">Name</span></span>          |<span data-ttu-id="941fd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="941fd-126">Type</span></span>           |<span data-ttu-id="941fd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="941fd-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="941fd-128">id</span><span class="sxs-lookup"><span data-stu-id="941fd-128">id</span></span>            | `string`      |<span data-ttu-id="941fd-129">A ID da tarefa `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-129">ID of the `schedulingGroup`.</span></span>|
| <span data-ttu-id="941fd-130">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="941fd-130">displayName</span></span>   | `string`      | <span data-ttu-id="941fd-131">O nome de exibição do grupo `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-131">The display name for the `schedulingGroup`.</span></span> <span data-ttu-id="941fd-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="941fd-132">Required.</span></span> |
| <span data-ttu-id="941fd-133">isActive</span><span class="sxs-lookup"><span data-stu-id="941fd-133">isActive</span></span>          |`bool`      | <span data-ttu-id="941fd-134">Indica se o `schedulingGroup` pode ser usada na criação de novas entidades ou atualizar as existentes.</span><span class="sxs-lookup"><span data-stu-id="941fd-134">Indicates whether the `schedulingGroup` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="941fd-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="941fd-135">Required.</span></span> |
| <span data-ttu-id="941fd-136">userIds</span><span class="sxs-lookup"><span data-stu-id="941fd-136">userIds</span></span>       | `collection(string)`    |  <span data-ttu-id="941fd-137">A lista de IDs é membro de usuários da `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-137">The list of user IDs that are a member of the `schedulingGroup`.</span></span> <span data-ttu-id="941fd-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="941fd-138">Required.</span></span> |
| <span data-ttu-id="941fd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="941fd-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="941fd-140">O carimbo de hora em que isso `schedulingGroup` foi criado pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="941fd-140">The time stamp in which this `schedulingGroup` was first created.</span></span> <span data-ttu-id="941fd-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="941fd-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="941fd-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="941fd-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="941fd-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="941fd-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="941fd-144">O carimbo de hora em que isso `schedulingGroup` foi criado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="941fd-144">The time stamp in which this `schedulingGroup` was last updated.</span></span> <span data-ttu-id="941fd-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="941fd-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="941fd-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="941fd-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="941fd-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="941fd-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="941fd-148">A identidade da última atualização `schedulingGroup`.</span><span class="sxs-lookup"><span data-stu-id="941fd-148">The identity that last updated this `schedulingGroup`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="941fd-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="941fd-149">JSON representation</span></span>

<span data-ttu-id="941fd-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="941fd-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
