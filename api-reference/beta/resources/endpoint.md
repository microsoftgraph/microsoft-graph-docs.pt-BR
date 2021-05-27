---
title: Tipo de recurso do ponto de extremidade
description: Os pontos de extremidade representam URLs para recursos associados a uma entidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: groups
author: Jordanndahl
ms.openlocfilehash: 1b5c9f401a659f1461cb9c2185dd412154dbeeda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680406"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="f3643-103">Tipo de recurso do ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f3643-103">Endpoint resource type</span></span>

<span data-ttu-id="f3643-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3643-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3643-105">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="f3643-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="f3643-106">Por exemplo, quando um novo grupo Microsoft 365 é criado, recursos adicionais também são criados como parte do Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="f3643-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="f3643-107">Isso inclui coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="f3643-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="f3643-108">Mais informações sobre esses Microsoft 365 de grupo, incluindo suas URLs de recurso associadas agora podem ser *lidas* usando a navegação de pontos de extremidade no tipo de recurso do grupo.</span><span class="sxs-lookup"><span data-stu-id="f3643-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="f3643-109">Isso permite que os aplicativos compreendam esses recursos e até mesmo insembutam as experiências de URL de recursos em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="f3643-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="f3643-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3643-110">Methods</span></span>

| <span data-ttu-id="f3643-111">Método</span><span class="sxs-lookup"><span data-stu-id="f3643-111">Method</span></span>           | <span data-ttu-id="f3643-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3643-112">Return Type</span></span>    |<span data-ttu-id="f3643-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3643-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3643-114">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="f3643-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="f3643-115">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="f3643-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="f3643-116">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="f3643-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="f3643-117">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f3643-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="f3643-118">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f3643-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="f3643-119">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="f3643-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3643-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3643-120">Properties</span></span>
| <span data-ttu-id="f3643-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3643-121">Property</span></span>     | <span data-ttu-id="f3643-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3643-122">Type</span></span>   |<span data-ttu-id="f3643-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3643-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3643-124">capability</span><span class="sxs-lookup"><span data-stu-id="f3643-124">capability</span></span>     | <span data-ttu-id="f3643-125">String</span><span class="sxs-lookup"><span data-stu-id="f3643-125">String</span></span>  | <span data-ttu-id="f3643-126">Descreve a funcionalidade associada a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="f3643-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="f3643-127">(por exemplo, mensagens, conversas etc.)  Não anulada.</span><span class="sxs-lookup"><span data-stu-id="f3643-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="f3643-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-128">Read-only.</span></span> |
| <span data-ttu-id="f3643-129">id</span><span class="sxs-lookup"><span data-stu-id="f3643-129">id</span></span>             | <span data-ttu-id="f3643-130">String</span><span class="sxs-lookup"><span data-stu-id="f3643-130">String</span></span>  | <span data-ttu-id="f3643-131">Identificador exclusivo do ponto de extremidade; Chave.</span><span class="sxs-lookup"><span data-stu-id="f3643-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="f3643-132">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="f3643-132">Not nullable.</span></span> <span data-ttu-id="f3643-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-133">Read-only.</span></span>|
| <span data-ttu-id="f3643-134">providerId</span><span class="sxs-lookup"><span data-stu-id="f3643-134">providerId</span></span>     | <span data-ttu-id="f3643-135">String</span><span class="sxs-lookup"><span data-stu-id="f3643-135">String</span></span>  | <span data-ttu-id="f3643-136">ID do aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="f3643-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="f3643-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="f3643-137">Not nullable.</span></span> <span data-ttu-id="f3643-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-138">Read-only.</span></span>|
| <span data-ttu-id="f3643-139">providerName</span><span class="sxs-lookup"><span data-stu-id="f3643-139">providerName</span></span>   | <span data-ttu-id="f3643-140">String</span><span class="sxs-lookup"><span data-stu-id="f3643-140">String</span></span>  | <span data-ttu-id="f3643-141">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="f3643-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="f3643-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-142">Read-only.</span></span>|
| <span data-ttu-id="f3643-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="f3643-143">providerResourceId</span></span>|<span data-ttu-id="f3643-144">String</span><span class="sxs-lookup"><span data-stu-id="f3643-144">String</span></span>| <span data-ttu-id="f3643-145">Para Microsoft 365 grupos, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="f3643-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="f3643-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="f3643-146">Not nullable.</span></span> <span data-ttu-id="f3643-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-147">Read-only.</span></span>|
| <span data-ttu-id="f3643-148">uri</span><span class="sxs-lookup"><span data-stu-id="f3643-148">uri</span></span>            | <span data-ttu-id="f3643-149">String</span><span class="sxs-lookup"><span data-stu-id="f3643-149">String</span></span>  | <span data-ttu-id="f3643-150">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="f3643-150">URL of the published resource.</span></span> <span data-ttu-id="f3643-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="f3643-151">Not nullable.</span></span> <span data-ttu-id="f3643-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3643-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3643-153">Relações</span><span class="sxs-lookup"><span data-stu-id="f3643-153">Relationships</span></span>

<span data-ttu-id="f3643-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3643-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3643-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3643-155">JSON representation</span></span>
<span data-ttu-id="f3643-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3643-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


