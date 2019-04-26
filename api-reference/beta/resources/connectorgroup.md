---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 5de46f480ff101e6d149bbfbe246ef47baff2604
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341189"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="8f3e9-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="8f3e9-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="8f3e9-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f3e9-104">Methods</span></span>

| <span data-ttu-id="8f3e9-105">Método</span><span class="sxs-lookup"><span data-stu-id="8f3e9-105">Method</span></span>           | <span data-ttu-id="8f3e9-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f3e9-106">Return Type</span></span>    |<span data-ttu-id="8f3e9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f3e9-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f3e9-108">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="8f3e9-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="8f3e9-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8f3e9-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="8f3e9-110">Leia as propriedades e as relações do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="8f3e9-111">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f3e9-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="8f3e9-112">application</span><span class="sxs-lookup"><span data-stu-id="8f3e9-112">application</span></span>](application.md)| <span data-ttu-id="8f3e9-113">Associe um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="8f3e9-114">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="8f3e9-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="8f3e9-115">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="8f3e9-115">[application](application.md) collection</span></span>| <span data-ttu-id="8f3e9-116">Obtenha a coleção de objetos de aplicativo associada.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="8f3e9-117">Criar conector</span><span class="sxs-lookup"><span data-stu-id="8f3e9-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="8f3e9-118">conector</span><span class="sxs-lookup"><span data-stu-id="8f3e9-118">connector</span></span>](connector.md)| <span data-ttu-id="8f3e9-119">Adicionar um conector ao grupo de conectores postando na coleção Members.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="8f3e9-120">Listar membros</span><span class="sxs-lookup"><span data-stu-id="8f3e9-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="8f3e9-121">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="8f3e9-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="8f3e9-122">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="8f3e9-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="8f3e9-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="8f3e9-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8f3e9-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="8f3e9-125">Atualize o objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="8f3e9-126">Delete</span><span class="sxs-lookup"><span data-stu-id="8f3e9-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="8f3e9-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f3e9-127">None</span></span> |<span data-ttu-id="8f3e9-128">Exclua objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-128">Delete connectorGroup object.</span></span> <span data-ttu-id="8f3e9-129">Todos os conectores devem ser removidos para que um grupo do conector possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f3e9-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f3e9-130">Properties</span></span>
| <span data-ttu-id="8f3e9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f3e9-131">Property</span></span>     | <span data-ttu-id="8f3e9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f3e9-132">Type</span></span>   |<span data-ttu-id="8f3e9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f3e9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f3e9-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="8f3e9-134">connectorGroupType</span></span>|<span data-ttu-id="8f3e9-135">string</span><span class="sxs-lookup"><span data-stu-id="8f3e9-135">string</span></span>| <span data-ttu-id="8f3e9-136">O tipo de conectores que serão usados com o grupo.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="8f3e9-137">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="8f3e9-138">id</span><span class="sxs-lookup"><span data-stu-id="8f3e9-138">id</span></span>|<span data-ttu-id="8f3e9-139">String</span><span class="sxs-lookup"><span data-stu-id="8f3e9-139">String</span></span>| <span data-ttu-id="8f3e9-140">A ID do objeto do conector</span><span class="sxs-lookup"><span data-stu-id="8f3e9-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="8f3e9-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="8f3e9-141">isDefault</span></span>|<span data-ttu-id="8f3e9-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f3e9-142">Boolean</span></span>| <span data-ttu-id="8f3e9-143">Indica se o grupo de conectores é o padrão.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="8f3e9-144">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="8f3e9-145">name</span><span class="sxs-lookup"><span data-stu-id="8f3e9-145">name</span></span>|<span data-ttu-id="8f3e9-146">String</span><span class="sxs-lookup"><span data-stu-id="8f3e9-146">String</span></span>| <span data-ttu-id="8f3e9-147">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f3e9-148">Relações</span><span class="sxs-lookup"><span data-stu-id="8f3e9-148">Relationships</span></span>
| <span data-ttu-id="8f3e9-149">Relação</span><span class="sxs-lookup"><span data-stu-id="8f3e9-149">Relationship</span></span> | <span data-ttu-id="8f3e9-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f3e9-150">Type</span></span>   |<span data-ttu-id="8f3e9-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f3e9-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f3e9-152">Emprego</span><span class="sxs-lookup"><span data-stu-id="8f3e9-152">applications</span></span>|<span data-ttu-id="8f3e9-153">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="8f3e9-153">[application](application.md) collection</span></span>| <span data-ttu-id="8f3e9-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-154">Read-only.</span></span> <span data-ttu-id="8f3e9-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-155">Nullable.</span></span>|
|<span data-ttu-id="8f3e9-156">members</span><span class="sxs-lookup"><span data-stu-id="8f3e9-156">members</span></span>|<span data-ttu-id="8f3e9-157">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="8f3e9-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="8f3e9-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f3e9-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f3e9-160">JSON representation</span></span>

<span data-ttu-id="8f3e9-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f3e9-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "suppressions": []
}
-->
