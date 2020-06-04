---
title: tipo de recurso do The Connector
description: Representa uma conexão de proxy de aplicativo.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556167"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="dd8b5-103">tipo de recurso do The Connector</span><span class="sxs-lookup"><span data-stu-id="dd8b5-103">connectorGroup resource type</span></span>

<span data-ttu-id="dd8b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd8b5-105">Cada conector de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) é sempre parte de um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="dd8b5-106">Todos os conectores que pertencem ao mesmo grupo de conectores atuam como uma unidade separada para alta disponibilidade e balanceamento de carga.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="dd8b5-107">Se você não criar grupos de conectores, todos os seus conectores farão parte do grupo padrão.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="dd8b5-108">Ao configurar um aplicativo com o proxy de aplicativo, você também deve especificar o grupo de conectores ao qual o aplicativo será atribuído.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="dd8b5-109">Depois que um grupo de conectores é criado, você pode adicionar ou mover conectores para o grupo de conectores usando [Adicionar conector](../api/connectorgroup-post-members.md).</span><span class="sxs-lookup"><span data-stu-id="dd8b5-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="dd8b5-110">Você também pode usar [Adicionar aplicativo](../api/connectorgroup-post-applications.md) para atribuir um aplicativo a um grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="dd8b5-111">Methods</span><span class="sxs-lookup"><span data-stu-id="dd8b5-111">Methods</span></span>

| <span data-ttu-id="dd8b5-112">Método</span><span class="sxs-lookup"><span data-stu-id="dd8b5-112">Method</span></span>           | <span data-ttu-id="dd8b5-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd8b5-113">Return Type</span></span>    |<span data-ttu-id="dd8b5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8b5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd8b5-115">Lista de conectores de lista</span><span class="sxs-lookup"><span data-stu-id="dd8b5-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="dd8b5-116">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="dd8b5-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="dd8b5-117">Recupere uma lista de objetos de conexão.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="dd8b5-118">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="dd8b5-118">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="dd8b5-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="dd8b5-119">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="dd8b5-120">Leia as propriedades e as relações de um objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-120">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="dd8b5-121">Atualizar o beficador de conexão</span><span class="sxs-lookup"><span data-stu-id="dd8b5-121">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="dd8b5-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="dd8b5-122">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="dd8b5-123">Atualize um objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-123">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="dd8b5-124">Excluir um ou de conector</span><span class="sxs-lookup"><span data-stu-id="dd8b5-124">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="dd8b5-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dd8b5-125">None</span></span> | <span data-ttu-id="dd8b5-126">Excluir um objeto de um.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-126">Delete a connectorGroup object.</span></span> <span data-ttu-id="dd8b5-127">Todos os conectores devem ser removidos do conector para que um dos conectores possa ser excluído.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-127">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="dd8b5-128">Listar membros</span><span class="sxs-lookup"><span data-stu-id="dd8b5-128">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="dd8b5-129">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="dd8b5-129">[connector](connector.md) collection</span></span>| <span data-ttu-id="dd8b5-130">Obtenha uma coleção de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-130">Get a connector object collection.</span></span> |
|[<span data-ttu-id="dd8b5-131">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="dd8b5-131">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="dd8b5-132">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="dd8b5-132">[application](application.md) collection</span></span>| <span data-ttu-id="dd8b5-133">Obter a coleção de objetos Application associada ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-133">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="dd8b5-134">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd8b5-134">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="dd8b5-135">aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd8b5-135">application</span></span>](application.md)| <span data-ttu-id="dd8b5-136">Associar um aplicativo ao grupo de conectores postando na coleção de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-136">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="dd8b5-137">Adicionar conector</span><span class="sxs-lookup"><span data-stu-id="dd8b5-137">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="dd8b5-138">conector</span><span class="sxs-lookup"><span data-stu-id="dd8b5-138">connector</span></span>](connector.md)| <span data-ttu-id="dd8b5-139">Adicionar um conector ao grupo de conectores postando na coleção de conectores.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-139">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd8b5-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd8b5-140">Properties</span></span>
| <span data-ttu-id="dd8b5-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd8b5-141">Property</span></span>     | <span data-ttu-id="dd8b5-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8b5-142">Type</span></span>   |<span data-ttu-id="dd8b5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8b5-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd8b5-144">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="dd8b5-144">connectorGroupType</span></span>|<span data-ttu-id="dd8b5-145">string</span><span class="sxs-lookup"><span data-stu-id="dd8b5-145">string</span></span>| <span data-ttu-id="dd8b5-146">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-146">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="dd8b5-147">Isso é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-147">This pre-set by the system.</span></span> <span data-ttu-id="dd8b5-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-148">Read-only.</span></span> |
|<span data-ttu-id="dd8b5-149">id</span><span class="sxs-lookup"><span data-stu-id="dd8b5-149">id</span></span>|<span data-ttu-id="dd8b5-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd8b5-150">string</span></span>| <span data-ttu-id="dd8b5-151">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-151">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="dd8b5-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-152">Read-only.</span></span> |
|<span data-ttu-id="dd8b5-153">isDefault</span><span class="sxs-lookup"><span data-stu-id="dd8b5-153">isDefault</span></span>|<span data-ttu-id="dd8b5-154">booliano</span><span class="sxs-lookup"><span data-stu-id="dd8b5-154">boolean</span></span>| <span data-ttu-id="dd8b5-155">Indica se o conector de conexão é o padrão.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-155">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="dd8b5-156">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-156">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="dd8b5-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-157">Read-only.</span></span> |
|<span data-ttu-id="dd8b5-158">name</span><span class="sxs-lookup"><span data-stu-id="dd8b5-158">name</span></span>|<span data-ttu-id="dd8b5-159">string</span><span class="sxs-lookup"><span data-stu-id="dd8b5-159">string</span></span>| <span data-ttu-id="dd8b5-160">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-160">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="dd8b5-161">região</span><span class="sxs-lookup"><span data-stu-id="dd8b5-161">region</span></span>|<span data-ttu-id="dd8b5-162">string</span><span class="sxs-lookup"><span data-stu-id="dd8b5-162">string</span></span>| <span data-ttu-id="dd8b5-163">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-163">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="dd8b5-164">Essa região só poderá ser definida se **nenhum conector ou aplicativo** for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-164">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="dd8b5-165">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-165">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="dd8b5-166">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-166">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd8b5-167">Relações</span><span class="sxs-lookup"><span data-stu-id="dd8b5-167">Relationships</span></span>
| <span data-ttu-id="dd8b5-168">Relação</span><span class="sxs-lookup"><span data-stu-id="dd8b5-168">Relationship</span></span> | <span data-ttu-id="dd8b5-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8b5-169">Type</span></span>   |<span data-ttu-id="dd8b5-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8b5-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd8b5-171">Emprego</span><span class="sxs-lookup"><span data-stu-id="dd8b5-171">applications</span></span>|<span data-ttu-id="dd8b5-172">Coleção [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="dd8b5-172">[application](application.md) collection</span></span>| <span data-ttu-id="dd8b5-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-173">Read-only.</span></span> <span data-ttu-id="dd8b5-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-174">Nullable.</span></span>|
|<span data-ttu-id="dd8b5-175">members</span><span class="sxs-lookup"><span data-stu-id="dd8b5-175">members</span></span>|<span data-ttu-id="dd8b5-176">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="dd8b5-176">[connector](connector.md) collection</span></span>| <span data-ttu-id="dd8b5-p109">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd8b5-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd8b5-179">JSON representation</span></span>

<span data-ttu-id="dd8b5-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd8b5-180">The following is a JSON representation of the resource.</span></span>

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
