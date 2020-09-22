---
title: tipo de recurso do The Connector
description: Representa uma conexão de proxy de aplicativo.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: ec56137fab8a929ae3823dcdd339ea6e3b8e174b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027143"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="ad3a3-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="ad3a3-103">connectorGroup resource type</span></span>

<span data-ttu-id="ad3a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad3a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad3a3-105">Cada conector de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) é sempre parte de um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="ad3a3-106">Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para alta disponibilidade e balanceamento de carga.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="ad3a3-107">Se você não criar grupos de conectores, todos os seus conectores farão parte do grupo padrão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="ad3a3-108">Ao configurar um aplicativo com o proxy de aplicativo, você também deve especificar o grupo de conectores ao qual o aplicativo será atribuído.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="ad3a3-109">Depois que um grupo de conectores é criado, você pode adicionar ou mover conectores para o grupo de conectores usando [Adicionar conector](../api/connectorgroup-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="ad3a3-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="ad3a3-110">Você também pode usar [Adicionar aplicativo](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="ad3a3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad3a3-111">Methods</span></span>

| <span data-ttu-id="ad3a3-112">Método</span><span class="sxs-lookup"><span data-stu-id="ad3a3-112">Method</span></span>           | <span data-ttu-id="ad3a3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad3a3-113">Return Type</span></span>    |<span data-ttu-id="ad3a3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3a3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad3a3-115">Lista de conectores de lista</span><span class="sxs-lookup"><span data-stu-id="ad3a3-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="ad3a3-116">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="ad3a3-117">Recupere uma lista de objetos de conexão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="ad3a3-118">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="ad3a3-119">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="ad3a3-120">Criar um objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="ad3a3-121">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="ad3a3-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="ad3a3-123">Leia as propriedades e as relações de um objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="ad3a3-124">Atualizar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="ad3a3-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="ad3a3-126">Atualize um objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="ad3a3-127">Excluir connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ad3a3-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="ad3a3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad3a3-128">None</span></span> | <span data-ttu-id="ad3a3-129">Excluir um objeto de um.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="ad3a3-130">Todos os conectores devem ser removidos do conector para que um dos conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="ad3a3-131">Listar membros</span><span class="sxs-lookup"><span data-stu-id="ad3a3-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="ad3a3-132">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="ad3a3-133">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="ad3a3-134">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="ad3a3-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="ad3a3-135">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-135">[application](application.md) collection</span></span>| <span data-ttu-id="ad3a3-136">Obter a coleção de objetos Application associada ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="ad3a3-137">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad3a3-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="ad3a3-138">aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad3a3-138">application</span></span>](application.md)| <span data-ttu-id="ad3a3-139">Associar um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="ad3a3-140">Adicionar conector</span><span class="sxs-lookup"><span data-stu-id="ad3a3-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="ad3a3-141">conector</span><span class="sxs-lookup"><span data-stu-id="ad3a3-141">connector</span></span>](connector.md)| <span data-ttu-id="ad3a3-142">Adicionar um conector ao grupo de conectores postando na coleção de conectores.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="ad3a3-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad3a3-143">Properties</span></span>
| <span data-ttu-id="ad3a3-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad3a3-144">Property</span></span>     | <span data-ttu-id="ad3a3-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad3a3-145">Type</span></span>   |<span data-ttu-id="ad3a3-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3a3-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad3a3-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="ad3a3-147">connectorGroupType</span></span>|<span data-ttu-id="ad3a3-148">string</span><span class="sxs-lookup"><span data-stu-id="ad3a3-148">string</span></span>| <span data-ttu-id="ad3a3-149">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="ad3a3-150">Isso é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-150">This pre-set by the system.</span></span> <span data-ttu-id="ad3a3-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-151">Read-only.</span></span> |
|<span data-ttu-id="ad3a3-152">id</span><span class="sxs-lookup"><span data-stu-id="ad3a3-152">id</span></span>|<span data-ttu-id="ad3a3-153">string</span><span class="sxs-lookup"><span data-stu-id="ad3a3-153">string</span></span>| <span data-ttu-id="ad3a3-154">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-154">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="ad3a3-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-155">Read-only.</span></span> |
|<span data-ttu-id="ad3a3-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="ad3a3-156">isDefault</span></span>|<span data-ttu-id="ad3a3-157">booliano</span><span class="sxs-lookup"><span data-stu-id="ad3a3-157">boolean</span></span>| <span data-ttu-id="ad3a3-158">Indica se o conector de conexão é o padrão.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-158">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="ad3a3-159">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-159">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="ad3a3-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-160">Read-only.</span></span> |
|<span data-ttu-id="ad3a3-161">name</span><span class="sxs-lookup"><span data-stu-id="ad3a3-161">name</span></span>|<span data-ttu-id="ad3a3-162">string</span><span class="sxs-lookup"><span data-stu-id="ad3a3-162">string</span></span>| <span data-ttu-id="ad3a3-163">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-163">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="ad3a3-164">região</span><span class="sxs-lookup"><span data-stu-id="ad3a3-164">region</span></span>|<span data-ttu-id="ad3a3-165">string</span><span class="sxs-lookup"><span data-stu-id="ad3a3-165">string</span></span>| <span data-ttu-id="ad3a3-166">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-166">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="ad3a3-167">Essa região só poderá ser definida se **nenhum conector ou aplicativo** for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-167">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="ad3a3-168">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-168">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="ad3a3-169">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-169">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad3a3-170">Relações</span><span class="sxs-lookup"><span data-stu-id="ad3a3-170">Relationships</span></span>
| <span data-ttu-id="ad3a3-171">Relação</span><span class="sxs-lookup"><span data-stu-id="ad3a3-171">Relationship</span></span> | <span data-ttu-id="ad3a3-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad3a3-172">Type</span></span>   |<span data-ttu-id="ad3a3-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3a3-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad3a3-174">Emprego</span><span class="sxs-lookup"><span data-stu-id="ad3a3-174">applications</span></span>|<span data-ttu-id="ad3a3-175">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-175">[application](application.md) collection</span></span>| <span data-ttu-id="ad3a3-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-176">Read-only.</span></span> <span data-ttu-id="ad3a3-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-177">Nullable.</span></span>|
|<span data-ttu-id="ad3a3-178">members</span><span class="sxs-lookup"><span data-stu-id="ad3a3-178">members</span></span>|<span data-ttu-id="ad3a3-179">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="ad3a3-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="ad3a3-p109">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad3a3-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad3a3-182">JSON representation</span></span>

<span data-ttu-id="ad3a3-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad3a3-183">The following is a JSON representation of the resource.</span></span>

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


