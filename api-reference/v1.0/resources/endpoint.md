---
title: Tipo de recurso de ponto de extremidade
description: Os pontos de extremidade representam URLs para recursos associados a uma entidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 46c43087ef31537f60a2079e72be71378c140612
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383669"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="ff4ff-103">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-103">Endpoint resource type</span></span>

<span data-ttu-id="ff4ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff4ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff4ff-105">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="ff4ff-106">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-106">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="ff4ff-107">Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="ff4ff-108">Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-108">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="ff4ff-109">Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="ff4ff-110">Methods</span><span class="sxs-lookup"><span data-stu-id="ff4ff-110">Methods</span></span>

| <span data-ttu-id="ff4ff-111">Método</span><span class="sxs-lookup"><span data-stu-id="ff4ff-111">Method</span></span>           | <span data-ttu-id="ff4ff-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff4ff-112">Return Type</span></span>    |<span data-ttu-id="ff4ff-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4ff-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff4ff-114">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="ff4ff-115">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ff-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="ff4ff-116">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="ff4ff-117">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="ff4ff-118">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="ff4ff-119">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff4ff-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff4ff-120">Properties</span></span>
| <span data-ttu-id="ff4ff-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff4ff-121">Property</span></span>     | <span data-ttu-id="ff4ff-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff4ff-122">Type</span></span>   |<span data-ttu-id="ff4ff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4ff-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff4ff-124">função</span><span class="sxs-lookup"><span data-stu-id="ff4ff-124">capability</span></span>     | <span data-ttu-id="ff4ff-125">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-125">String</span></span>  | <span data-ttu-id="ff4ff-126">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="ff4ff-127">(por exemplo, mensagens, conversas etc.)  Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="ff4ff-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-128">Read-only.</span></span> |
| <span data-ttu-id="ff4ff-129">id</span><span class="sxs-lookup"><span data-stu-id="ff4ff-129">id</span></span>             | <span data-ttu-id="ff4ff-130">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-130">String</span></span>  | <span data-ttu-id="ff4ff-131">Identificador exclusivo do ponto de extremidade; Chaves.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="ff4ff-132">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-132">Not nullable.</span></span> <span data-ttu-id="ff4ff-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-133">Read-only.</span></span>|
| <span data-ttu-id="ff4ff-134">providerId</span><span class="sxs-lookup"><span data-stu-id="ff4ff-134">providerId</span></span>     | <span data-ttu-id="ff4ff-135">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-135">String</span></span>  | <span data-ttu-id="ff4ff-136">ID de aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="ff4ff-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-137">Not nullable.</span></span> <span data-ttu-id="ff4ff-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-138">Read-only.</span></span>|
| <span data-ttu-id="ff4ff-139">providerName</span><span class="sxs-lookup"><span data-stu-id="ff4ff-139">providerName</span></span>   | <span data-ttu-id="ff4ff-140">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-140">String</span></span>  | <span data-ttu-id="ff4ff-141">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="ff4ff-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-142">Read-only.</span></span>|
| <span data-ttu-id="ff4ff-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="ff4ff-143">providerResourceId</span></span>|<span data-ttu-id="ff4ff-144">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-144">String</span></span>| <span data-ttu-id="ff4ff-145">Para grupos do Office 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="ff4ff-145">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="ff4ff-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-146">Not nullable.</span></span> <span data-ttu-id="ff4ff-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-147">Read-only.</span></span>|
| <span data-ttu-id="ff4ff-148">URI</span><span class="sxs-lookup"><span data-stu-id="ff4ff-148">uri</span></span>            | <span data-ttu-id="ff4ff-149">String</span><span class="sxs-lookup"><span data-stu-id="ff4ff-149">String</span></span>  | <span data-ttu-id="ff4ff-150">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-150">URL of the published resource.</span></span> <span data-ttu-id="ff4ff-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-151">Not nullable.</span></span> <span data-ttu-id="ff4ff-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4ff-153">Relações</span><span class="sxs-lookup"><span data-stu-id="ff4ff-153">Relationships</span></span>

<span data-ttu-id="ff4ff-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff4ff-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff4ff-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff4ff-155">JSON representation</span></span>
<span data-ttu-id="ff4ff-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff4ff-156">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
     "Error: microsoft.graph.servicePrincipal/endpoints:\r\n      Referenced type microsoft.graph.endPoint is not defined in the doc  set! Potential suggestion: microsoft.graph.callRecords.endpoint"
    ]
}
-->
