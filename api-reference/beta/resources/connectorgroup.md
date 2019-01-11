---
title: tipo de recurso de connectorGroup
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823188"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="93400-103">tipo de recurso de connectorGroup</span><span class="sxs-lookup"><span data-stu-id="93400-103">connectorGroup resource type</span></span>

> <span data-ttu-id="93400-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93400-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93400-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93400-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="93400-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="93400-106">Methods</span></span>

| <span data-ttu-id="93400-107">Método</span><span class="sxs-lookup"><span data-stu-id="93400-107">Method</span></span>           | <span data-ttu-id="93400-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93400-108">Return Type</span></span>    |<span data-ttu-id="93400-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93400-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93400-110">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="93400-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="93400-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="93400-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="93400-112">Leia as propriedades e os relacionamentos do objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="93400-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="93400-113">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="93400-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="93400-114">application</span><span class="sxs-lookup"><span data-stu-id="93400-114">application</span></span>](application.md)| <span data-ttu-id="93400-115">Associe um aplicativo com o grupo de conector pelo lançamento para o conjunto de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="93400-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="93400-116">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="93400-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="93400-117">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="93400-117">[application](application.md) collection</span></span>| <span data-ttu-id="93400-118">Obter a coleção de objeto do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="93400-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="93400-119">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="93400-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="93400-120">conector</span><span class="sxs-lookup"><span data-stu-id="93400-120">connector</span></span>](connector.md)| <span data-ttu-id="93400-121">Adicione um conector para o grupo de conector pelo lançamento para o conjunto de membros.</span><span class="sxs-lookup"><span data-stu-id="93400-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="93400-122">Listar membros</span><span class="sxs-lookup"><span data-stu-id="93400-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="93400-123">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="93400-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="93400-124">Obtenha um conector a coleção de objetos.</span><span class="sxs-lookup"><span data-stu-id="93400-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="93400-125">Update</span><span class="sxs-lookup"><span data-stu-id="93400-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="93400-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="93400-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="93400-127">Atualize o objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="93400-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="93400-128">Delete</span><span class="sxs-lookup"><span data-stu-id="93400-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="93400-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93400-129">None</span></span> |<span data-ttu-id="93400-130">Exclua objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="93400-130">Delete connectorGroup object.</span></span> <span data-ttu-id="93400-131">Todos os conectores devem ser remove antes de um conector de grupo pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="93400-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="93400-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93400-132">Properties</span></span>
| <span data-ttu-id="93400-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93400-133">Property</span></span>     | <span data-ttu-id="93400-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="93400-134">Type</span></span>   |<span data-ttu-id="93400-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="93400-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93400-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="93400-136">connectorGroupType</span></span>|<span data-ttu-id="93400-137">string</span><span class="sxs-lookup"><span data-stu-id="93400-137">string</span></span>| <span data-ttu-id="93400-138">O tipo de conectores que será usado com o grupo.</span><span class="sxs-lookup"><span data-stu-id="93400-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="93400-139">Os valores possíveis são: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="93400-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="93400-140">id</span><span class="sxs-lookup"><span data-stu-id="93400-140">id</span></span>|<span data-ttu-id="93400-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93400-141">String</span></span>| <span data-ttu-id="93400-142">O id de objeto do connectorGroup</span><span class="sxs-lookup"><span data-stu-id="93400-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="93400-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="93400-143">isDefault</span></span>|<span data-ttu-id="93400-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="93400-144">Boolean</span></span>| <span data-ttu-id="93400-145">Indica se o connectorGroup é o grupo de conector padrão.</span><span class="sxs-lookup"><span data-stu-id="93400-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="93400-146">Apenas um conector grupo pode ser o connectorGroup padrão e é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="93400-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="93400-147">name</span><span class="sxs-lookup"><span data-stu-id="93400-147">name</span></span>|<span data-ttu-id="93400-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93400-148">String</span></span>| <span data-ttu-id="93400-149">O nome associado a connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="93400-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93400-150">Relações</span><span class="sxs-lookup"><span data-stu-id="93400-150">Relationships</span></span>
| <span data-ttu-id="93400-151">Relação</span><span class="sxs-lookup"><span data-stu-id="93400-151">Relationship</span></span> | <span data-ttu-id="93400-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="93400-152">Type</span></span>   |<span data-ttu-id="93400-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="93400-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93400-154">aplicativos</span><span class="sxs-lookup"><span data-stu-id="93400-154">applications</span></span>|<span data-ttu-id="93400-155">conjunto de [aplicativos](application.md)</span><span class="sxs-lookup"><span data-stu-id="93400-155">[application](application.md) collection</span></span>| <span data-ttu-id="93400-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="93400-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="93400-158">membros</span><span class="sxs-lookup"><span data-stu-id="93400-158">members</span></span>|<span data-ttu-id="93400-159">coleção de [conector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="93400-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="93400-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="93400-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93400-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93400-162">JSON representation</span></span>

<span data-ttu-id="93400-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93400-163">Here is a JSON representation of the resource.</span></span>

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
