---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543389"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="b8453-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="b8453-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="b8453-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8453-104">Methods</span></span>

| <span data-ttu-id="b8453-105">Método</span><span class="sxs-lookup"><span data-stu-id="b8453-105">Method</span></span>           | <span data-ttu-id="b8453-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b8453-106">Return Type</span></span>    |<span data-ttu-id="b8453-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8453-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8453-108">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="b8453-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="b8453-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b8453-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="b8453-110">Leia as propriedades e as relações do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="b8453-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="b8453-111">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8453-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="b8453-112">application</span><span class="sxs-lookup"><span data-stu-id="b8453-112">application</span></span>](application.md)| <span data-ttu-id="b8453-113">Associe um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b8453-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="b8453-114">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="b8453-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="b8453-115">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="b8453-115">[application](application.md) collection</span></span>| <span data-ttu-id="b8453-116">Obtenha a coleção de objetos de aplicativo associada.</span><span class="sxs-lookup"><span data-stu-id="b8453-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="b8453-117">Criar conector</span><span class="sxs-lookup"><span data-stu-id="b8453-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="b8453-118">conector</span><span class="sxs-lookup"><span data-stu-id="b8453-118">connector</span></span>](connector.md)| <span data-ttu-id="b8453-119">Adicionar um conector ao grupo de conectores postando na coleção Members.</span><span class="sxs-lookup"><span data-stu-id="b8453-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="b8453-120">Listar membros</span><span class="sxs-lookup"><span data-stu-id="b8453-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="b8453-121">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="b8453-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="b8453-122">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="b8453-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="b8453-123">Update</span><span class="sxs-lookup"><span data-stu-id="b8453-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="b8453-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="b8453-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="b8453-125">Atualize o objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="b8453-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="b8453-126">Excluir</span><span class="sxs-lookup"><span data-stu-id="b8453-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="b8453-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8453-127">None</span></span> |<span data-ttu-id="b8453-128">Exclua objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="b8453-128">Delete connectorGroup object.</span></span> <span data-ttu-id="b8453-129">Todos os conectores devem ser removidos para que um grupo do conector possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="b8453-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8453-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8453-130">Properties</span></span>
| <span data-ttu-id="b8453-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8453-131">Property</span></span>     | <span data-ttu-id="b8453-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8453-132">Type</span></span>   |<span data-ttu-id="b8453-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8453-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8453-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="b8453-134">connectorGroupType</span></span>|<span data-ttu-id="b8453-135">string</span><span class="sxs-lookup"><span data-stu-id="b8453-135">string</span></span>| <span data-ttu-id="b8453-136">O tipo de conectores que serão usados com o grupo.</span><span class="sxs-lookup"><span data-stu-id="b8453-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="b8453-137">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="b8453-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="b8453-138">id</span><span class="sxs-lookup"><span data-stu-id="b8453-138">id</span></span>|<span data-ttu-id="b8453-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8453-139">String</span></span>| <span data-ttu-id="b8453-140">A ID do objeto do conector</span><span class="sxs-lookup"><span data-stu-id="b8453-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="b8453-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="b8453-141">isDefault</span></span>|<span data-ttu-id="b8453-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8453-142">Boolean</span></span>| <span data-ttu-id="b8453-143">Indica se o grupo de conectores é o padrão.</span><span class="sxs-lookup"><span data-stu-id="b8453-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="b8453-144">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b8453-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="b8453-145">name</span><span class="sxs-lookup"><span data-stu-id="b8453-145">name</span></span>|<span data-ttu-id="b8453-146">String</span><span class="sxs-lookup"><span data-stu-id="b8453-146">String</span></span>| <span data-ttu-id="b8453-147">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="b8453-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8453-148">Relações</span><span class="sxs-lookup"><span data-stu-id="b8453-148">Relationships</span></span>
| <span data-ttu-id="b8453-149">Relação</span><span class="sxs-lookup"><span data-stu-id="b8453-149">Relationship</span></span> | <span data-ttu-id="b8453-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8453-150">Type</span></span>   |<span data-ttu-id="b8453-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8453-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8453-152">Emprego</span><span class="sxs-lookup"><span data-stu-id="b8453-152">applications</span></span>|<span data-ttu-id="b8453-153">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="b8453-153">[application](application.md) collection</span></span>| <span data-ttu-id="b8453-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8453-154">Read-only.</span></span> <span data-ttu-id="b8453-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b8453-155">Nullable.</span></span>|
|<span data-ttu-id="b8453-156">members</span><span class="sxs-lookup"><span data-stu-id="b8453-156">members</span></span>|<span data-ttu-id="b8453-157">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="b8453-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="b8453-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b8453-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8453-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8453-160">JSON representation</span></span>

<span data-ttu-id="b8453-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8453-161">Here is a JSON representation of the resource.</span></span>

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
