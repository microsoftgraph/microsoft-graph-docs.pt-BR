---
title: Tipo de recurso connectorGroup
description: Representa um Application Proxy connectorGroup.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: df3a80c6dfd4004daccfe33045c8775c2e2e6e48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958805"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="bb63d-103">Tipo de recurso connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-103">connectorGroup resource type</span></span>

<span data-ttu-id="bb63d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb63d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb63d-105">Cada conector proxy de aplicativo [do Azure AD](https://aka.ms/whyappproxy) sempre faz parte de um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="bb63d-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="bb63d-106">Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para balanceamento de carga e alta disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="bb63d-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="bb63d-107">Se você não criar grupos de conectores, todos os conectores serão parte do grupo padrão.</span><span class="sxs-lookup"><span data-stu-id="bb63d-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="bb63d-108">Ao configurar um aplicativo com Proxy de Aplicativo, você também deve especificar a qual grupo de conectores atribuir o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bb63d-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="bb63d-109">Depois que um grupo de conectores for criado, você poderá adicionar ou mover conectores para o grupo do conector usando [Add connector](../api/connectorgroup-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="bb63d-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="bb63d-110">Você também pode usar [o aplicativo Add](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="bb63d-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="bb63d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="bb63d-111">Methods</span></span>

| <span data-ttu-id="bb63d-112">Método</span><span class="sxs-lookup"><span data-stu-id="bb63d-112">Method</span></span>           | <span data-ttu-id="bb63d-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb63d-113">Return Type</span></span>    |<span data-ttu-id="bb63d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb63d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb63d-115">Listar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="bb63d-116">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="bb63d-117">Recupere uma lista de objetos connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="bb63d-118">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="bb63d-119">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="bb63d-120">Crie um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="bb63d-121">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="bb63d-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="bb63d-123">Ler propriedades e relações de um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="bb63d-124">Atualizar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="bb63d-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="bb63d-126">Atualize um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="bb63d-127">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb63d-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="bb63d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb63d-128">None</span></span> | <span data-ttu-id="bb63d-129">Exclua um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="bb63d-130">Todos os conectores devem ser removidos do connectorGroup antes que um connectorGroup possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="bb63d-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="bb63d-131">Listar membros</span><span class="sxs-lookup"><span data-stu-id="bb63d-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="bb63d-132">[coleção connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="bb63d-133">Obter uma coleção de objetos do conector.</span><span class="sxs-lookup"><span data-stu-id="bb63d-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="bb63d-134">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="bb63d-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="bb63d-135">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-135">[application](application.md) collection</span></span>| <span data-ttu-id="bb63d-136">Obter a coleção de objetos de aplicativo associada ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="bb63d-137">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb63d-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="bb63d-138">application</span><span class="sxs-lookup"><span data-stu-id="bb63d-138">application</span></span>](application.md)| <span data-ttu-id="bb63d-139">Associe um aplicativo ao connectorGroup postando na coleção applications.</span><span class="sxs-lookup"><span data-stu-id="bb63d-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="bb63d-140">Adicionar conector</span><span class="sxs-lookup"><span data-stu-id="bb63d-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="bb63d-141">connector</span><span class="sxs-lookup"><span data-stu-id="bb63d-141">connector</span></span>](connector.md)| <span data-ttu-id="bb63d-142">Adicione um conector ao connectorGroup postando na coleção connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb63d-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb63d-143">Properties</span></span>
| <span data-ttu-id="bb63d-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb63d-144">Property</span></span>     | <span data-ttu-id="bb63d-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb63d-145">Type</span></span>   |<span data-ttu-id="bb63d-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb63d-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb63d-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="bb63d-147">connectorGroupType</span></span>|<span data-ttu-id="bb63d-148">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="bb63d-148">connectorGroupType</span></span>| <span data-ttu-id="bb63d-149">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="bb63d-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="bb63d-150">Este pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="bb63d-150">This pre-set by the system.</span></span> <span data-ttu-id="bb63d-151">Os valores possíveis são: `applicationProxy` .</span><span class="sxs-lookup"><span data-stu-id="bb63d-151">Possible values are: `applicationProxy`.</span></span> <span data-ttu-id="bb63d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb63d-152">Read-only.</span></span> |
|<span data-ttu-id="bb63d-153">id</span><span class="sxs-lookup"><span data-stu-id="bb63d-153">id</span></span>|<span data-ttu-id="bb63d-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb63d-154">string</span></span>| <span data-ttu-id="bb63d-155">Identificador exclusivo para este connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-155">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="bb63d-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb63d-156">Read-only.</span></span> |
|<span data-ttu-id="bb63d-157">isDefault</span><span class="sxs-lookup"><span data-stu-id="bb63d-157">isDefault</span></span>|<span data-ttu-id="bb63d-158">booliano</span><span class="sxs-lookup"><span data-stu-id="bb63d-158">boolean</span></span>| <span data-ttu-id="bb63d-159">Indica se o connectorGroup é o connectorGroup padrão.</span><span class="sxs-lookup"><span data-stu-id="bb63d-159">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="bb63d-160">Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="bb63d-160">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="bb63d-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb63d-161">Read-only.</span></span> |
|<span data-ttu-id="bb63d-162">name</span><span class="sxs-lookup"><span data-stu-id="bb63d-162">name</span></span>|<span data-ttu-id="bb63d-163">string</span><span class="sxs-lookup"><span data-stu-id="bb63d-163">string</span></span>| <span data-ttu-id="bb63d-164">O nome associado ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-164">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="bb63d-165">region</span><span class="sxs-lookup"><span data-stu-id="bb63d-165">region</span></span>|<span data-ttu-id="bb63d-166">connectorGroupRegion</span><span class="sxs-lookup"><span data-stu-id="bb63d-166">connectorGroupRegion</span></span>| <span data-ttu-id="bb63d-167">A região à que o connectorGroup é atribuído e otimizará o tráfego.</span><span class="sxs-lookup"><span data-stu-id="bb63d-167">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="bb63d-168">Essa região só poderá ser definida se **nenhum conector ou aplicativo** for atribuído ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="bb63d-168">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="bb63d-169">Os valores possíveis são: `nam` (para **a América do Norte**), (para a `eur` Europa), (para a `aus` Austrália), (para a `asia` Ásia), `ind` (para a Índia) e `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="bb63d-169">The possible values are: `nam` (for **North America**), `eur` (for Europe), `aus` (for Australia), `asia` (for Asia), `ind` (for India), and `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb63d-170">Relações</span><span class="sxs-lookup"><span data-stu-id="bb63d-170">Relationships</span></span>
| <span data-ttu-id="bb63d-171">Relação</span><span class="sxs-lookup"><span data-stu-id="bb63d-171">Relationship</span></span> | <span data-ttu-id="bb63d-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb63d-172">Type</span></span>   |<span data-ttu-id="bb63d-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb63d-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb63d-174">applications</span><span class="sxs-lookup"><span data-stu-id="bb63d-174">applications</span></span>|<span data-ttu-id="bb63d-175">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-175">[application](application.md) collection</span></span>| <span data-ttu-id="bb63d-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb63d-176">Read-only.</span></span> <span data-ttu-id="bb63d-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb63d-177">Nullable.</span></span>|
|<span data-ttu-id="bb63d-178">members</span><span class="sxs-lookup"><span data-stu-id="bb63d-178">members</span></span>|<span data-ttu-id="bb63d-179">[coleção connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="bb63d-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="bb63d-p109">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb63d-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb63d-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb63d-182">JSON representation</span></span>

<span data-ttu-id="bb63d-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb63d-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
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



