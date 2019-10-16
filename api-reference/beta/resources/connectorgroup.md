---
title: tipo de recurso do The Connector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 02ef418f0f2124b4bd0c7489db8c732398005761
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538382"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="f89aa-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="f89aa-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="f89aa-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="f89aa-104">Methods</span></span>

| <span data-ttu-id="f89aa-105">Método</span><span class="sxs-lookup"><span data-stu-id="f89aa-105">Method</span></span>           | <span data-ttu-id="f89aa-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f89aa-106">Return Type</span></span>    |<span data-ttu-id="f89aa-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f89aa-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f89aa-108">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="f89aa-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="f89aa-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f89aa-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="f89aa-110">Leia as propriedades e as relações do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="f89aa-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="f89aa-111">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f89aa-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="f89aa-112">application</span><span class="sxs-lookup"><span data-stu-id="f89aa-112">application</span></span>](application.md)| <span data-ttu-id="f89aa-113">Associe um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f89aa-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="f89aa-114">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="f89aa-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="f89aa-115">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="f89aa-115">[application](application.md) collection</span></span>| <span data-ttu-id="f89aa-116">Obtenha a coleção de objetos de aplicativo associada.</span><span class="sxs-lookup"><span data-stu-id="f89aa-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="f89aa-117">Criar conector</span><span class="sxs-lookup"><span data-stu-id="f89aa-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="f89aa-118">conector</span><span class="sxs-lookup"><span data-stu-id="f89aa-118">connector</span></span>](connector.md)| <span data-ttu-id="f89aa-119">Adicionar um conector ao grupo de conectores postando na coleção Members.</span><span class="sxs-lookup"><span data-stu-id="f89aa-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="f89aa-120">Listar membros</span><span class="sxs-lookup"><span data-stu-id="f89aa-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="f89aa-121">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f89aa-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="f89aa-122">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="f89aa-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="f89aa-123">Update</span><span class="sxs-lookup"><span data-stu-id="f89aa-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="f89aa-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f89aa-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="f89aa-125">Atualize o objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="f89aa-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="f89aa-126">Delete</span><span class="sxs-lookup"><span data-stu-id="f89aa-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="f89aa-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f89aa-127">None</span></span> |<span data-ttu-id="f89aa-128">Exclua objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="f89aa-128">Delete connectorGroup object.</span></span> <span data-ttu-id="f89aa-129">Todos os conectores devem ser removidos para que um grupo de conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="f89aa-129">All connectors must be remove before a connector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="f89aa-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f89aa-130">Properties</span></span>
| <span data-ttu-id="f89aa-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f89aa-131">Property</span></span>     | <span data-ttu-id="f89aa-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f89aa-132">Type</span></span>   |<span data-ttu-id="f89aa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f89aa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89aa-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="f89aa-134">connectorGroupType</span></span>|<span data-ttu-id="f89aa-135">string</span><span class="sxs-lookup"><span data-stu-id="f89aa-135">string</span></span>| <span data-ttu-id="f89aa-136">O tipo de conectores que serão usados com o grupo.</span><span class="sxs-lookup"><span data-stu-id="f89aa-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="f89aa-137">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="f89aa-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="f89aa-138">id</span><span class="sxs-lookup"><span data-stu-id="f89aa-138">id</span></span>|<span data-ttu-id="f89aa-139">String</span><span class="sxs-lookup"><span data-stu-id="f89aa-139">String</span></span>| <span data-ttu-id="f89aa-140">A ID do objeto do conector</span><span class="sxs-lookup"><span data-stu-id="f89aa-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="f89aa-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="f89aa-141">isDefault</span></span>|<span data-ttu-id="f89aa-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89aa-142">Boolean</span></span>| <span data-ttu-id="f89aa-143">Indica se o grupo de conectores é o padrão.</span><span class="sxs-lookup"><span data-stu-id="f89aa-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="f89aa-144">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f89aa-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="f89aa-145">name</span><span class="sxs-lookup"><span data-stu-id="f89aa-145">name</span></span>|<span data-ttu-id="f89aa-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f89aa-146">String</span></span>| <span data-ttu-id="f89aa-147">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="f89aa-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f89aa-148">Relações</span><span class="sxs-lookup"><span data-stu-id="f89aa-148">Relationships</span></span>
| <span data-ttu-id="f89aa-149">Relação</span><span class="sxs-lookup"><span data-stu-id="f89aa-149">Relationship</span></span> | <span data-ttu-id="f89aa-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="f89aa-150">Type</span></span>   |<span data-ttu-id="f89aa-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="f89aa-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89aa-152">Emprego</span><span class="sxs-lookup"><span data-stu-id="f89aa-152">applications</span></span>|<span data-ttu-id="f89aa-153">coleção [Application](application.md)</span><span class="sxs-lookup"><span data-stu-id="f89aa-153">[application](application.md) collection</span></span>| <span data-ttu-id="f89aa-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f89aa-154">Read-only.</span></span> <span data-ttu-id="f89aa-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f89aa-155">Nullable.</span></span>|
|<span data-ttu-id="f89aa-156">members</span><span class="sxs-lookup"><span data-stu-id="f89aa-156">members</span></span>|<span data-ttu-id="f89aa-157">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f89aa-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="f89aa-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f89aa-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f89aa-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f89aa-160">JSON representation</span></span>

<span data-ttu-id="f89aa-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f89aa-161">Here is a JSON representation of the resource.</span></span>

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
