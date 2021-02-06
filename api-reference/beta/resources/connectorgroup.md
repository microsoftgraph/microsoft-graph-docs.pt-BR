---
title: Tipo de recurso connectorGroup
description: Representa um Application Proxy connectorGroup.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 78716646f4bf5cbba7a66da4cdef88d94d1984aa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132318"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="29f20-103">Tipo de recurso connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-103">connectorGroup resource type</span></span>

<span data-ttu-id="29f20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29f20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f20-105">Cada [conector de Proxy de Aplicativo do Azure AD](https://aka.ms/whyappproxy) sempre faz parte de um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="29f20-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="29f20-106">Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para alta disponibilidade e balanceamento de carga.</span><span class="sxs-lookup"><span data-stu-id="29f20-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="29f20-107">Se você não criar grupos de conectores, todos os conectores serão parte do grupo padrão.</span><span class="sxs-lookup"><span data-stu-id="29f20-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="29f20-108">Ao configurar um aplicativo com o Proxy de Aplicativo, você também deve especificar a qual grupo de conector atribuir o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29f20-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="29f20-109">Depois que um grupo de conectores é criado, você pode adicionar ou mover conectores para o grupo de conectores usando [Adicionar conector.](../api/connectorgroup-post-members.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="29f20-110">Você também pode usar [Adicionar aplicativo](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="29f20-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="29f20-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="29f20-111">Methods</span></span>

| <span data-ttu-id="29f20-112">Método</span><span class="sxs-lookup"><span data-stu-id="29f20-112">Method</span></span>           | <span data-ttu-id="29f20-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29f20-113">Return Type</span></span>    |<span data-ttu-id="29f20-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="29f20-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29f20-115">Listar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="29f20-116">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="29f20-117">Recupere uma lista de objetos connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="29f20-118">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="29f20-119">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="29f20-120">Crie um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="29f20-121">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="29f20-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="29f20-123">Ler propriedades e relações de um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="29f20-124">Atualizar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="29f20-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="29f20-126">Atualize um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="29f20-127">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="29f20-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="29f20-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="29f20-128">None</span></span> | <span data-ttu-id="29f20-129">Exclua um objeto connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="29f20-130">Todos os conectores devem ser removidos do connectorGroup antes que um connectorGroup possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="29f20-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="29f20-131">Listar membros</span><span class="sxs-lookup"><span data-stu-id="29f20-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="29f20-132">[conjunto de conectores](connector.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="29f20-133">Obter uma coleção de objetos do conector.</span><span class="sxs-lookup"><span data-stu-id="29f20-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="29f20-134">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="29f20-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="29f20-135">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-135">[application](application.md) collection</span></span>| <span data-ttu-id="29f20-136">Obter a coleção de objetos de aplicativo associada ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="29f20-137">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="29f20-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="29f20-138">aplicativo</span><span class="sxs-lookup"><span data-stu-id="29f20-138">application</span></span>](application.md)| <span data-ttu-id="29f20-139">Associe um aplicativo ao connectorGroup postando na coleção applications.</span><span class="sxs-lookup"><span data-stu-id="29f20-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="29f20-140">Adicionar conector</span><span class="sxs-lookup"><span data-stu-id="29f20-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="29f20-141">connector</span><span class="sxs-lookup"><span data-stu-id="29f20-141">connector</span></span>](connector.md)| <span data-ttu-id="29f20-142">Adicione um conector ao connectorGroup postando na coleção connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="29f20-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29f20-143">Properties</span></span>
| <span data-ttu-id="29f20-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29f20-144">Property</span></span>     | <span data-ttu-id="29f20-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="29f20-145">Type</span></span>   |<span data-ttu-id="29f20-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="29f20-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f20-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="29f20-147">connectorGroupType</span></span>|<span data-ttu-id="29f20-148">string</span><span class="sxs-lookup"><span data-stu-id="29f20-148">string</span></span>| <span data-ttu-id="29f20-149">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="29f20-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="29f20-150">Isso é pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="29f20-150">This pre-set by the system.</span></span> <span data-ttu-id="29f20-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29f20-151">Read-only.</span></span> |
|<span data-ttu-id="29f20-152">id</span><span class="sxs-lookup"><span data-stu-id="29f20-152">id</span></span>|<span data-ttu-id="29f20-153">string</span><span class="sxs-lookup"><span data-stu-id="29f20-153">string</span></span>| <span data-ttu-id="29f20-154">Identificador exclusivo deste connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-154">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="29f20-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29f20-155">Read-only.</span></span> |
|<span data-ttu-id="29f20-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="29f20-156">isDefault</span></span>|<span data-ttu-id="29f20-157">booliano</span><span class="sxs-lookup"><span data-stu-id="29f20-157">boolean</span></span>| <span data-ttu-id="29f20-158">Indica se o connectorGroup é o connectorGroup padrão.</span><span class="sxs-lookup"><span data-stu-id="29f20-158">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="29f20-159">Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="29f20-159">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="29f20-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29f20-160">Read-only.</span></span> |
|<span data-ttu-id="29f20-161">name</span><span class="sxs-lookup"><span data-stu-id="29f20-161">name</span></span>|<span data-ttu-id="29f20-162">string</span><span class="sxs-lookup"><span data-stu-id="29f20-162">string</span></span>| <span data-ttu-id="29f20-163">O nome associado ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-163">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="29f20-164">region</span><span class="sxs-lookup"><span data-stu-id="29f20-164">region</span></span>|<span data-ttu-id="29f20-165">string</span><span class="sxs-lookup"><span data-stu-id="29f20-165">string</span></span>| <span data-ttu-id="29f20-166">A região à que o connectorGroup está atribuído e otimizará o tráfego.</span><span class="sxs-lookup"><span data-stu-id="29f20-166">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="29f20-167">Essa região só poderá ser definida se **nenhum conector ou aplicativo** estiver atribuído ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="29f20-167">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="29f20-168">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="29f20-168">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="29f20-169">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="29f20-169">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29f20-170">Relações</span><span class="sxs-lookup"><span data-stu-id="29f20-170">Relationships</span></span>
| <span data-ttu-id="29f20-171">Relação</span><span class="sxs-lookup"><span data-stu-id="29f20-171">Relationship</span></span> | <span data-ttu-id="29f20-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="29f20-172">Type</span></span>   |<span data-ttu-id="29f20-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="29f20-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f20-174">applications</span><span class="sxs-lookup"><span data-stu-id="29f20-174">applications</span></span>|<span data-ttu-id="29f20-175">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-175">[application](application.md) collection</span></span>| <span data-ttu-id="29f20-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29f20-176">Read-only.</span></span> <span data-ttu-id="29f20-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="29f20-177">Nullable.</span></span>|
|<span data-ttu-id="29f20-178">members</span><span class="sxs-lookup"><span data-stu-id="29f20-178">members</span></span>|<span data-ttu-id="29f20-179">[conjunto de conectores](connector.md)</span><span class="sxs-lookup"><span data-stu-id="29f20-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="29f20-p109">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="29f20-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f20-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29f20-182">JSON representation</span></span>

<span data-ttu-id="29f20-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29f20-183">The following is a JSON representation of the resource.</span></span>

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



