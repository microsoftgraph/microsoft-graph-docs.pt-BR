---
title: tipo de recurso de connectorGroup
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a3131b887216f1f400f70ed8d607477f65793cc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038205"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="454f5-103">tipo de recurso de connectorGroup</span><span class="sxs-lookup"><span data-stu-id="454f5-103">connectorGroup resource type</span></span>

> <span data-ttu-id="454f5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="454f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="454f5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="454f5-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="454f5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="454f5-106">Methods</span></span>

| <span data-ttu-id="454f5-107">Método</span><span class="sxs-lookup"><span data-stu-id="454f5-107">Method</span></span>           | <span data-ttu-id="454f5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="454f5-108">Return Type</span></span>    |<span data-ttu-id="454f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="454f5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="454f5-110">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="454f5-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="454f5-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="454f5-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="454f5-112">Leia as propriedades e os relacionamentos do objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="454f5-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="454f5-113">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="454f5-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="454f5-114">application</span><span class="sxs-lookup"><span data-stu-id="454f5-114">application</span></span>](application.md)| <span data-ttu-id="454f5-115">Associe um aplicativo com o grupo de conector pelo lançamento para o conjunto de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="454f5-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="454f5-116">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="454f5-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="454f5-117">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="454f5-117">[application](application.md) collection</span></span>| <span data-ttu-id="454f5-118">Obter a coleção de objeto do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="454f5-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="454f5-119">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="454f5-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="454f5-120">conector</span><span class="sxs-lookup"><span data-stu-id="454f5-120">connector</span></span>](connector.md)| <span data-ttu-id="454f5-121">Adicione um conector para o grupo de conector pelo lançamento para o conjunto de membros.</span><span class="sxs-lookup"><span data-stu-id="454f5-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="454f5-122">Listar membros</span><span class="sxs-lookup"><span data-stu-id="454f5-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="454f5-123">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="454f5-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="454f5-124">Obtenha um conector a coleção de objetos.</span><span class="sxs-lookup"><span data-stu-id="454f5-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="454f5-125">Update</span><span class="sxs-lookup"><span data-stu-id="454f5-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="454f5-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="454f5-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="454f5-127">Atualize o objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="454f5-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="454f5-128">Delete</span><span class="sxs-lookup"><span data-stu-id="454f5-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="454f5-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="454f5-129">None</span></span> |<span data-ttu-id="454f5-130">Exclua objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="454f5-130">Delete connectorGroup object.</span></span> <span data-ttu-id="454f5-131">Todos os conectores devem ser remove antes de um conector de grupo pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="454f5-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="454f5-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="454f5-132">Properties</span></span>
| <span data-ttu-id="454f5-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="454f5-133">Property</span></span>     | <span data-ttu-id="454f5-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="454f5-134">Type</span></span>   |<span data-ttu-id="454f5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="454f5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="454f5-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="454f5-136">connectorGroupType</span></span>|<span data-ttu-id="454f5-137">string</span><span class="sxs-lookup"><span data-stu-id="454f5-137">string</span></span>| <span data-ttu-id="454f5-138">O tipo de conectores que será usado com o grupo.</span><span class="sxs-lookup"><span data-stu-id="454f5-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="454f5-139">Os valores possíveis são: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="454f5-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="454f5-140">id</span><span class="sxs-lookup"><span data-stu-id="454f5-140">id</span></span>|<span data-ttu-id="454f5-141">String</span><span class="sxs-lookup"><span data-stu-id="454f5-141">String</span></span>| <span data-ttu-id="454f5-142">O id de objeto do connectorGroup</span><span class="sxs-lookup"><span data-stu-id="454f5-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="454f5-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="454f5-143">isDefault</span></span>|<span data-ttu-id="454f5-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="454f5-144">Boolean</span></span>| <span data-ttu-id="454f5-145">Indica se o connectorGroup é o grupo de conector padrão.</span><span class="sxs-lookup"><span data-stu-id="454f5-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="454f5-146">Apenas um conector grupo pode ser o connectorGroup padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="454f5-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="454f5-147">name</span><span class="sxs-lookup"><span data-stu-id="454f5-147">name</span></span>|<span data-ttu-id="454f5-148">String</span><span class="sxs-lookup"><span data-stu-id="454f5-148">String</span></span>| <span data-ttu-id="454f5-149">O nome associado a connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="454f5-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="454f5-150">Relações</span><span class="sxs-lookup"><span data-stu-id="454f5-150">Relationships</span></span>
| <span data-ttu-id="454f5-151">Relação</span><span class="sxs-lookup"><span data-stu-id="454f5-151">Relationship</span></span> | <span data-ttu-id="454f5-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="454f5-152">Type</span></span>   |<span data-ttu-id="454f5-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="454f5-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="454f5-154">aplicativos</span><span class="sxs-lookup"><span data-stu-id="454f5-154">applications</span></span>|<span data-ttu-id="454f5-155">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="454f5-155">[application](application.md) collection</span></span>| <span data-ttu-id="454f5-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="454f5-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="454f5-158">membros</span><span class="sxs-lookup"><span data-stu-id="454f5-158">members</span></span>|<span data-ttu-id="454f5-159">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="454f5-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="454f5-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="454f5-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="454f5-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="454f5-162">JSON representation</span></span>

<span data-ttu-id="454f5-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="454f5-163">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
