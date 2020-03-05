---
title: Tipo de recurso de ponto de extremidade
description: 'Os pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36c69a616cfd1d1aa531f42e9622b4f0c63ec83d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499390"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="e88cd-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="e88cd-107">Endpoint resource type</span></span>

<span data-ttu-id="e88cd-108">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e88cd-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e88cd-109">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="e88cd-109">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="e88cd-110">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e88cd-110">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="e88cd-111">Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="e88cd-111">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="e88cd-112">Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="e88cd-112">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="e88cd-113">Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="e88cd-113">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="e88cd-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="e88cd-114">Methods</span></span>

| <span data-ttu-id="e88cd-115">Método</span><span class="sxs-lookup"><span data-stu-id="e88cd-115">Method</span></span>           | <span data-ttu-id="e88cd-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e88cd-116">Return Type</span></span>    |<span data-ttu-id="e88cd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e88cd-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e88cd-118">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="e88cd-118">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="e88cd-119">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="e88cd-119">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="e88cd-120">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="e88cd-120">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="e88cd-121">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="e88cd-121">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="e88cd-122">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="e88cd-122">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="e88cd-123">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="e88cd-123">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e88cd-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e88cd-124">Properties</span></span>
| <span data-ttu-id="e88cd-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e88cd-125">Property</span></span>     | <span data-ttu-id="e88cd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e88cd-126">Type</span></span>   |<span data-ttu-id="e88cd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e88cd-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e88cd-128">função</span><span class="sxs-lookup"><span data-stu-id="e88cd-128">capability</span></span>     | <span data-ttu-id="e88cd-129">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-129">String</span></span>  | <span data-ttu-id="e88cd-130">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="e88cd-130">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="e88cd-131">(por exemplo, mensagens, conversas etc.)  Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e88cd-131">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="e88cd-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-132">Read-only.</span></span> |
| <span data-ttu-id="e88cd-133">id</span><span class="sxs-lookup"><span data-stu-id="e88cd-133">id</span></span>             | <span data-ttu-id="e88cd-134">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-134">String</span></span>  | <span data-ttu-id="e88cd-135">Identificador exclusivo do ponto de extremidade; Chaves.</span><span class="sxs-lookup"><span data-stu-id="e88cd-135">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="e88cd-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e88cd-136">Not nullable.</span></span> <span data-ttu-id="e88cd-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-137">Read-only.</span></span>|
| <span data-ttu-id="e88cd-138">providerId</span><span class="sxs-lookup"><span data-stu-id="e88cd-138">providerId</span></span>     | <span data-ttu-id="e88cd-139">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-139">String</span></span>  | <span data-ttu-id="e88cd-140">ID de aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="e88cd-140">Application id of the publishing underlying service.</span></span> <span data-ttu-id="e88cd-141">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e88cd-141">Not nullable.</span></span> <span data-ttu-id="e88cd-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-142">Read-only.</span></span>|
| <span data-ttu-id="e88cd-143">providerName</span><span class="sxs-lookup"><span data-stu-id="e88cd-143">providerName</span></span>   | <span data-ttu-id="e88cd-144">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-144">String</span></span>  | <span data-ttu-id="e88cd-145">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="e88cd-145">Name of the publishing underlying service.</span></span> <span data-ttu-id="e88cd-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-146">Read-only.</span></span>|
| <span data-ttu-id="e88cd-147">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="e88cd-147">providerResourceId</span></span>|<span data-ttu-id="e88cd-148">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-148">String</span></span>| <span data-ttu-id="e88cd-149">Para grupos do Office 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="e88cd-149">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="e88cd-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e88cd-150">Not nullable.</span></span> <span data-ttu-id="e88cd-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-151">Read-only.</span></span>|
| <span data-ttu-id="e88cd-152">URI</span><span class="sxs-lookup"><span data-stu-id="e88cd-152">uri</span></span>            | <span data-ttu-id="e88cd-153">String</span><span class="sxs-lookup"><span data-stu-id="e88cd-153">String</span></span>  | <span data-ttu-id="e88cd-154">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="e88cd-154">URL of the published resource.</span></span> <span data-ttu-id="e88cd-155">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e88cd-155">Not nullable.</span></span> <span data-ttu-id="e88cd-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e88cd-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e88cd-157">Relações</span><span class="sxs-lookup"><span data-stu-id="e88cd-157">Relationships</span></span>

<span data-ttu-id="e88cd-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e88cd-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e88cd-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e88cd-159">JSON representation</span></span>
<span data-ttu-id="e88cd-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e88cd-160">Here is a JSON representation of the resource.</span></span>

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
