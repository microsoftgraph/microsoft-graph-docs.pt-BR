---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d57f116adac652cb55a3a270383ddb5c65d8e40f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507468"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="da85b-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="da85b-103">connectorGroup resource type</span></span>

<span data-ttu-id="da85b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da85b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="da85b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="da85b-105">Methods</span></span>

| <span data-ttu-id="da85b-106">Método</span><span class="sxs-lookup"><span data-stu-id="da85b-106">Method</span></span>           | <span data-ttu-id="da85b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="da85b-107">Return Type</span></span>    |<span data-ttu-id="da85b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="da85b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da85b-109">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="da85b-109">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="da85b-110">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="da85b-110">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="da85b-111">Leia as propriedades e as relações do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="da85b-111">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="da85b-112">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="da85b-112">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="da85b-113">application</span><span class="sxs-lookup"><span data-stu-id="da85b-113">application</span></span>](application.md)| <span data-ttu-id="da85b-114">Associe um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="da85b-114">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="da85b-115">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="da85b-115">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="da85b-116">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="da85b-116">[application](application.md) collection</span></span>| <span data-ttu-id="da85b-117">Obtenha a coleção de objetos de aplicativo associada.</span><span class="sxs-lookup"><span data-stu-id="da85b-117">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="da85b-118">Criar conector</span><span class="sxs-lookup"><span data-stu-id="da85b-118">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="da85b-119">conector</span><span class="sxs-lookup"><span data-stu-id="da85b-119">connector</span></span>](connector.md)| <span data-ttu-id="da85b-120">Adicionar um conector ao grupo de conectores postando na coleção Members.</span><span class="sxs-lookup"><span data-stu-id="da85b-120">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="da85b-121">Listar membros</span><span class="sxs-lookup"><span data-stu-id="da85b-121">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="da85b-122">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="da85b-122">[connector](connector.md) collection</span></span>| <span data-ttu-id="da85b-123">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="da85b-123">Get a connector object collection.</span></span>|
|[<span data-ttu-id="da85b-124">Update</span><span class="sxs-lookup"><span data-stu-id="da85b-124">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="da85b-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="da85b-125">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="da85b-126">Atualize o objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="da85b-126">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="da85b-127">Delete</span><span class="sxs-lookup"><span data-stu-id="da85b-127">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="da85b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da85b-128">None</span></span> |<span data-ttu-id="da85b-129">Exclua objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="da85b-129">Delete connectorGroup object.</span></span> <span data-ttu-id="da85b-130">Todos os conectores devem ser removidos para que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="da85b-130">All connectors must be remove before a connector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="da85b-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da85b-131">Properties</span></span>
| <span data-ttu-id="da85b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da85b-132">Property</span></span>     | <span data-ttu-id="da85b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="da85b-133">Type</span></span>   |<span data-ttu-id="da85b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="da85b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da85b-135">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="da85b-135">connectorGroupType</span></span>|<span data-ttu-id="da85b-136">string</span><span class="sxs-lookup"><span data-stu-id="da85b-136">string</span></span>| <span data-ttu-id="da85b-137">O tipo de conectores que serão usados com o grupo.</span><span class="sxs-lookup"><span data-stu-id="da85b-137">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="da85b-138">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="da85b-138">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="da85b-139">id</span><span class="sxs-lookup"><span data-stu-id="da85b-139">id</span></span>|<span data-ttu-id="da85b-140">String</span><span class="sxs-lookup"><span data-stu-id="da85b-140">String</span></span>| <span data-ttu-id="da85b-141">A ID do objeto do conector</span><span class="sxs-lookup"><span data-stu-id="da85b-141">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="da85b-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="da85b-142">isDefault</span></span>|<span data-ttu-id="da85b-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="da85b-143">Boolean</span></span>| <span data-ttu-id="da85b-144">Indica se o grupo de conectores é o padrão.</span><span class="sxs-lookup"><span data-stu-id="da85b-144">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="da85b-145">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="da85b-145">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="da85b-146">nome</span><span class="sxs-lookup"><span data-stu-id="da85b-146">name</span></span>|<span data-ttu-id="da85b-147">String</span><span class="sxs-lookup"><span data-stu-id="da85b-147">String</span></span>| <span data-ttu-id="da85b-148">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="da85b-148">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da85b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="da85b-149">Relationships</span></span>
| <span data-ttu-id="da85b-150">Relação</span><span class="sxs-lookup"><span data-stu-id="da85b-150">Relationship</span></span> | <span data-ttu-id="da85b-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="da85b-151">Type</span></span>   |<span data-ttu-id="da85b-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="da85b-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da85b-153">Emprego</span><span class="sxs-lookup"><span data-stu-id="da85b-153">applications</span></span>|<span data-ttu-id="da85b-154">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="da85b-154">[application](application.md) collection</span></span>| <span data-ttu-id="da85b-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da85b-155">Read-only.</span></span> <span data-ttu-id="da85b-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="da85b-156">Nullable.</span></span>|
|<span data-ttu-id="da85b-157">members</span><span class="sxs-lookup"><span data-stu-id="da85b-157">members</span></span>|<span data-ttu-id="da85b-158">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="da85b-158">[connector](connector.md) collection</span></span>| <span data-ttu-id="da85b-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="da85b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da85b-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da85b-161">JSON representation</span></span>

<span data-ttu-id="da85b-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da85b-162">Here is a JSON representation of the resource.</span></span>

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
