---
title: Tipo de recurso de ponto de extremidade
description: 'Os pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 474da77d10d9b433dd6d4914f9b75812e040a9e4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340198"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="ed55d-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed55d-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed55d-108">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="ed55d-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="ed55d-109">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed55d-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="ed55d-110">Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="ed55d-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="ed55d-111">Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="ed55d-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="ed55d-112">Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="ed55d-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="ed55d-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed55d-113">Methods</span></span>

| <span data-ttu-id="ed55d-114">Método</span><span class="sxs-lookup"><span data-stu-id="ed55d-114">Method</span></span>           | <span data-ttu-id="ed55d-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed55d-115">Return Type</span></span>    |<span data-ttu-id="ed55d-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed55d-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed55d-117">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed55d-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="ed55d-118">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="ed55d-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="ed55d-119">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ed55d-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="ed55d-120">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed55d-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="ed55d-121">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="ed55d-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="ed55d-122">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ed55d-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed55d-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed55d-123">Properties</span></span>
| <span data-ttu-id="ed55d-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed55d-124">Property</span></span>     | <span data-ttu-id="ed55d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed55d-125">Type</span></span>   |<span data-ttu-id="ed55d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed55d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed55d-127">função</span><span class="sxs-lookup"><span data-stu-id="ed55d-127">capability</span></span>     | <span data-ttu-id="ed55d-128">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-128">String</span></span>  | <span data-ttu-id="ed55d-129">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ed55d-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="ed55d-130">(por exemplo, mensagens, conversas etc.)  Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed55d-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="ed55d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-131">Read-only.</span></span> |
| <span data-ttu-id="ed55d-132">id</span><span class="sxs-lookup"><span data-stu-id="ed55d-132">id</span></span>             | <span data-ttu-id="ed55d-133">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-133">String</span></span>  | <span data-ttu-id="ed55d-134">Identificador exclusivo do ponto de extremidade; Chaves.</span><span class="sxs-lookup"><span data-stu-id="ed55d-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="ed55d-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed55d-135">Not nullable.</span></span> <span data-ttu-id="ed55d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-136">Read-only.</span></span>|
| <span data-ttu-id="ed55d-137">providerId</span><span class="sxs-lookup"><span data-stu-id="ed55d-137">providerId</span></span>     | <span data-ttu-id="ed55d-138">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-138">String</span></span>  | <span data-ttu-id="ed55d-139">ID de aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ed55d-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="ed55d-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed55d-140">Not nullable.</span></span> <span data-ttu-id="ed55d-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-141">Read-only.</span></span>|
| <span data-ttu-id="ed55d-142">providerName</span><span class="sxs-lookup"><span data-stu-id="ed55d-142">providerName</span></span>   | <span data-ttu-id="ed55d-143">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-143">String</span></span>  | <span data-ttu-id="ed55d-144">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="ed55d-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="ed55d-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-145">Read-only.</span></span>|
| <span data-ttu-id="ed55d-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="ed55d-146">providerResourceId</span></span>|<span data-ttu-id="ed55d-147">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-147">String</span></span>| <span data-ttu-id="ed55d-148">Para grupos do Office 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="ed55d-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="ed55d-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed55d-149">Not nullable.</span></span> <span data-ttu-id="ed55d-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-150">Read-only.</span></span>|
| <span data-ttu-id="ed55d-151">URI</span><span class="sxs-lookup"><span data-stu-id="ed55d-151">uri</span></span>            | <span data-ttu-id="ed55d-152">String</span><span class="sxs-lookup"><span data-stu-id="ed55d-152">String</span></span>  | <span data-ttu-id="ed55d-153">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="ed55d-153">URL of the published resource.</span></span> <span data-ttu-id="ed55d-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ed55d-154">Not nullable.</span></span> <span data-ttu-id="ed55d-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed55d-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed55d-156">Relações</span><span class="sxs-lookup"><span data-stu-id="ed55d-156">Relationships</span></span>

<span data-ttu-id="ed55d-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed55d-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed55d-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed55d-158">JSON representation</span></span>
<span data-ttu-id="ed55d-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed55d-159">Here is a JSON representation of the resource.</span></span>

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
