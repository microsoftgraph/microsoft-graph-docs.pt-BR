---
title: tipo de recurso de connectorGroup
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517495"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="0c215-103">tipo de recurso de connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0c215-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="0c215-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c215-104">Methods</span></span>

| <span data-ttu-id="0c215-105">Método</span><span class="sxs-lookup"><span data-stu-id="0c215-105">Method</span></span>           | <span data-ttu-id="0c215-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c215-106">Return Type</span></span>    |<span data-ttu-id="0c215-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c215-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c215-108">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0c215-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="0c215-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0c215-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="0c215-110">Leia as propriedades e os relacionamentos do objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="0c215-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="0c215-111">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c215-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="0c215-112">application</span><span class="sxs-lookup"><span data-stu-id="0c215-112">application</span></span>](application.md)| <span data-ttu-id="0c215-113">Associe um aplicativo com o grupo de conector pelo lançamento para o conjunto de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0c215-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="0c215-114">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="0c215-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="0c215-115">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="0c215-115">[application](application.md) collection</span></span>| <span data-ttu-id="0c215-116">Obter a coleção de objeto do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="0c215-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="0c215-117">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="0c215-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="0c215-118">Connector</span><span class="sxs-lookup"><span data-stu-id="0c215-118">connector</span></span>](connector.md)| <span data-ttu-id="0c215-119">Adicione um conector para o grupo de conector pelo lançamento para o conjunto de membros.</span><span class="sxs-lookup"><span data-stu-id="0c215-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="0c215-120">Listar membros</span><span class="sxs-lookup"><span data-stu-id="0c215-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="0c215-121">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="0c215-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="0c215-122">Obtenha um conector a coleção de objetos.</span><span class="sxs-lookup"><span data-stu-id="0c215-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="0c215-123">Update</span><span class="sxs-lookup"><span data-stu-id="0c215-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="0c215-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0c215-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="0c215-125">Atualize o objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="0c215-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="0c215-126">Delete</span><span class="sxs-lookup"><span data-stu-id="0c215-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="0c215-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c215-127">None</span></span> |<span data-ttu-id="0c215-128">Exclua objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="0c215-128">Delete connectorGroup object.</span></span> <span data-ttu-id="0c215-129">Todos os conectores devem ser remove antes de um conector de grupo pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="0c215-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c215-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c215-130">Properties</span></span>
| <span data-ttu-id="0c215-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c215-131">Property</span></span>     | <span data-ttu-id="0c215-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c215-132">Type</span></span>   |<span data-ttu-id="0c215-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c215-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c215-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="0c215-134">connectorGroupType</span></span>|<span data-ttu-id="0c215-135">string</span><span class="sxs-lookup"><span data-stu-id="0c215-135">string</span></span>| <span data-ttu-id="0c215-136">O tipo de conectores que será usado com o grupo.</span><span class="sxs-lookup"><span data-stu-id="0c215-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="0c215-137">Os valores possíveis são: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="0c215-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="0c215-138">id</span><span class="sxs-lookup"><span data-stu-id="0c215-138">id</span></span>|<span data-ttu-id="0c215-139">String</span><span class="sxs-lookup"><span data-stu-id="0c215-139">String</span></span>| <span data-ttu-id="0c215-140">O id de objeto do connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0c215-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="0c215-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="0c215-141">isDefault</span></span>|<span data-ttu-id="0c215-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c215-142">Boolean</span></span>| <span data-ttu-id="0c215-143">Indica se o connectorGroup é o grupo de conector padrão.</span><span class="sxs-lookup"><span data-stu-id="0c215-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="0c215-144">Apenas um conector grupo pode ser o connectorGroup padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="0c215-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="0c215-145">name</span><span class="sxs-lookup"><span data-stu-id="0c215-145">name</span></span>|<span data-ttu-id="0c215-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c215-146">String</span></span>| <span data-ttu-id="0c215-147">O nome associado a connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="0c215-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c215-148">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="0c215-148">Relationships</span></span>
| <span data-ttu-id="0c215-149">Relação</span><span class="sxs-lookup"><span data-stu-id="0c215-149">Relationship</span></span> | <span data-ttu-id="0c215-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c215-150">Type</span></span>   |<span data-ttu-id="0c215-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c215-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c215-152">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="0c215-152">applications</span></span>|<span data-ttu-id="0c215-153">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="0c215-153">[application](application.md) collection</span></span>| <span data-ttu-id="0c215-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0c215-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="0c215-156">membros</span><span class="sxs-lookup"><span data-stu-id="0c215-156">members</span></span>|<span data-ttu-id="0c215-157">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="0c215-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="0c215-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0c215-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c215-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c215-160">JSON representation</span></span>

<span data-ttu-id="0c215-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c215-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
