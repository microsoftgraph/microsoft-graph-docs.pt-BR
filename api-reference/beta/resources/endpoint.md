---
title: Tipo de recurso Endpoint
description: Os pontos de extremidade representam URLs de recursos associados a uma entidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: 47bef2bfa14fb8a00fd1ca2356d7f880ff3207d6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013594"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="aad59-103">Tipo de recurso Endpoint</span><span class="sxs-lookup"><span data-stu-id="aad59-103">Endpoint resource type</span></span>

<span data-ttu-id="aad59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aad59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad59-105">Os pontos de extremidade representam URLs de recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="aad59-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="aad59-106">Por exemplo, quando um novo grupo do Microsoft 365 é criado, recursos adicionais também são criados como parte do grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="aad59-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="aad59-107">Isso inclui coisas como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="aad59-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="aad59-108">Mais informações sobre esses recursos de grupo do Microsoft 365, incluindo suas URLs de recursos associadas agora podem ser *lidas* usando a navegação de pontos de extremidade no tipo de recurso do grupo.</span><span class="sxs-lookup"><span data-stu-id="aad59-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="aad59-109">Isso permite que os aplicativos compreendam esses recursos e, até mesmo, incorporam as experiências de URL do recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="aad59-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="aad59-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="aad59-110">Methods</span></span>

| <span data-ttu-id="aad59-111">Método</span><span class="sxs-lookup"><span data-stu-id="aad59-111">Method</span></span>           | <span data-ttu-id="aad59-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aad59-112">Return Type</span></span>    |<span data-ttu-id="aad59-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="aad59-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aad59-114">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="aad59-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="aad59-115">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="aad59-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="aad59-116">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="aad59-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="aad59-117">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="aad59-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="aad59-118">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="aad59-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="aad59-119">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="aad59-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aad59-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aad59-120">Properties</span></span>
| <span data-ttu-id="aad59-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aad59-121">Property</span></span>     | <span data-ttu-id="aad59-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="aad59-122">Type</span></span>   |<span data-ttu-id="aad59-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aad59-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aad59-124">capability</span><span class="sxs-lookup"><span data-stu-id="aad59-124">capability</span></span>     | <span data-ttu-id="aad59-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-125">String</span></span>  | <span data-ttu-id="aad59-126">Descreve a funcionalidade associada a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="aad59-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="aad59-127">(por exemplo, mensagens, conversas, etc.)  Não anulada.</span><span class="sxs-lookup"><span data-stu-id="aad59-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="aad59-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-128">Read-only.</span></span> |
| <span data-ttu-id="aad59-129">id</span><span class="sxs-lookup"><span data-stu-id="aad59-129">id</span></span>             | <span data-ttu-id="aad59-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-130">String</span></span>  | <span data-ttu-id="aad59-131">Identificador exclusivo do ponto de extremidade; Tecla.</span><span class="sxs-lookup"><span data-stu-id="aad59-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="aad59-132">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="aad59-132">Not nullable.</span></span> <span data-ttu-id="aad59-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-133">Read-only.</span></span>|
| <span data-ttu-id="aad59-134">providerId</span><span class="sxs-lookup"><span data-stu-id="aad59-134">providerId</span></span>     | <span data-ttu-id="aad59-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-135">String</span></span>  | <span data-ttu-id="aad59-136">ID do aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="aad59-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="aad59-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="aad59-137">Not nullable.</span></span> <span data-ttu-id="aad59-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-138">Read-only.</span></span>|
| <span data-ttu-id="aad59-139">providerName</span><span class="sxs-lookup"><span data-stu-id="aad59-139">providerName</span></span>   | <span data-ttu-id="aad59-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-140">String</span></span>  | <span data-ttu-id="aad59-141">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="aad59-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="aad59-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-142">Read-only.</span></span>|
| <span data-ttu-id="aad59-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="aad59-143">providerResourceId</span></span>|<span data-ttu-id="aad59-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-144">String</span></span>| <span data-ttu-id="aad59-145">Para grupos do Microsoft 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer.FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="aad59-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="aad59-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="aad59-146">Not nullable.</span></span> <span data-ttu-id="aad59-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-147">Read-only.</span></span>|
| <span data-ttu-id="aad59-148">uri</span><span class="sxs-lookup"><span data-stu-id="aad59-148">uri</span></span>            | <span data-ttu-id="aad59-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad59-149">String</span></span>  | <span data-ttu-id="aad59-150">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="aad59-150">URL of the published resource.</span></span> <span data-ttu-id="aad59-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="aad59-151">Not nullable.</span></span> <span data-ttu-id="aad59-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aad59-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aad59-153">Relações</span><span class="sxs-lookup"><span data-stu-id="aad59-153">Relationships</span></span>

<span data-ttu-id="aad59-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aad59-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="aad59-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aad59-155">JSON representation</span></span>
<span data-ttu-id="aad59-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aad59-156">Here is a JSON representation of the resource.</span></span>

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


