---
title: Tipo de recurso de ponto de extremidade
description: Os pontos de extremidade representam URLs para recursos associados a uma entidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 43843a3b6847c261326574e7a73f607b10e5e05d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895612"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="ed75c-103">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed75c-103">Endpoint resource type</span></span>

<span data-ttu-id="ed75c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed75c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed75c-105">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="ed75c-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="ed75c-106">Por exemplo, quando um novo grupo Microsoft 365 é criado, recursos adicionais também são criados como parte do grupo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ed75c-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="ed75c-107">Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="ed75c-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="ed75c-108">Informações adicionais sobre esses recursos de grupo do Microsoft 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="ed75c-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="ed75c-109">Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="ed75c-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="ed75c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed75c-110">Methods</span></span>

| <span data-ttu-id="ed75c-111">Método</span><span class="sxs-lookup"><span data-stu-id="ed75c-111">Method</span></span>           | <span data-ttu-id="ed75c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed75c-112">Return Type</span></span>    |<span data-ttu-id="ed75c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed75c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed75c-114">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed75c-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="ed75c-115">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="ed75c-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="ed75c-116">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ed75c-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="ed75c-117">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed75c-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="ed75c-118">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed75c-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="ed75c-119">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ed75c-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed75c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed75c-120">Properties</span></span>
| <span data-ttu-id="ed75c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed75c-121">Property</span></span>     | <span data-ttu-id="ed75c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed75c-122">Type</span></span>   |<span data-ttu-id="ed75c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed75c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed75c-124">função</span><span class="sxs-lookup"><span data-stu-id="ed75c-124">capability</span></span>     | <span data-ttu-id="ed75c-125">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-125">String</span></span>  | <span data-ttu-id="ed75c-126">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ed75c-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="ed75c-127">(por exemplo, mensagens, conversas etc.)  Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed75c-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="ed75c-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-128">Read-only.</span></span> |
| <span data-ttu-id="ed75c-129">id</span><span class="sxs-lookup"><span data-stu-id="ed75c-129">id</span></span>             | <span data-ttu-id="ed75c-130">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-130">String</span></span>  | <span data-ttu-id="ed75c-131">Identificador exclusivo do ponto de extremidade; Chaves.</span><span class="sxs-lookup"><span data-stu-id="ed75c-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="ed75c-132">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed75c-132">Not nullable.</span></span> <span data-ttu-id="ed75c-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-133">Read-only.</span></span>|
| <span data-ttu-id="ed75c-134">providerId</span><span class="sxs-lookup"><span data-stu-id="ed75c-134">providerId</span></span>     | <span data-ttu-id="ed75c-135">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-135">String</span></span>  | <span data-ttu-id="ed75c-136">ID de aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ed75c-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="ed75c-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed75c-137">Not nullable.</span></span> <span data-ttu-id="ed75c-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-138">Read-only.</span></span>|
| <span data-ttu-id="ed75c-139">providerName</span><span class="sxs-lookup"><span data-stu-id="ed75c-139">providerName</span></span>   | <span data-ttu-id="ed75c-140">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-140">String</span></span>  | <span data-ttu-id="ed75c-141">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ed75c-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="ed75c-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-142">Read-only.</span></span>|
| <span data-ttu-id="ed75c-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="ed75c-143">providerResourceId</span></span>|<span data-ttu-id="ed75c-144">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-144">String</span></span>| <span data-ttu-id="ed75c-145">Para os grupos do Microsoft 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="ed75c-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="ed75c-146">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed75c-146">Not nullable.</span></span> <span data-ttu-id="ed75c-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-147">Read-only.</span></span>|
| <span data-ttu-id="ed75c-148">URI</span><span class="sxs-lookup"><span data-stu-id="ed75c-148">uri</span></span>            | <span data-ttu-id="ed75c-149">String</span><span class="sxs-lookup"><span data-stu-id="ed75c-149">String</span></span>  | <span data-ttu-id="ed75c-150">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="ed75c-150">URL of the published resource.</span></span> <span data-ttu-id="ed75c-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed75c-151">Not nullable.</span></span> <span data-ttu-id="ed75c-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed75c-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed75c-153">Relações</span><span class="sxs-lookup"><span data-stu-id="ed75c-153">Relationships</span></span>

<span data-ttu-id="ed75c-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed75c-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed75c-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed75c-155">JSON representation</span></span>
<span data-ttu-id="ed75c-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed75c-156">Here is a JSON representation of the resource.</span></span>

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
