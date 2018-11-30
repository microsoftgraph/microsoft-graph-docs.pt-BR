---
title: Tipo de recurso de ponto de extremidade
description: 'Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. '
ms.openlocfilehash: 8d95cef8e25095512e94d5aed5ec7540562862bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034774"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="af0d2-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="af0d2-107">Endpoint resource type</span></span>

> <span data-ttu-id="af0d2-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af0d2-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af0d2-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af0d2-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af0d2-110">Pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="af0d2-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="af0d2-111">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="af0d2-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="af0d2-112">Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="af0d2-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="af0d2-113">Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="af0d2-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="af0d2-114">Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="af0d2-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="af0d2-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="af0d2-115">Methods</span></span>

| <span data-ttu-id="af0d2-116">Método</span><span class="sxs-lookup"><span data-stu-id="af0d2-116">Method</span></span>           | <span data-ttu-id="af0d2-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af0d2-117">Return Type</span></span>    |<span data-ttu-id="af0d2-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="af0d2-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af0d2-119">Lista de pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="af0d2-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="af0d2-120">Coleção de [ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="af0d2-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="af0d2-121">Obtenha uma coleção de objetos de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="af0d2-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="af0d2-122">Obtenha o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="af0d2-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="af0d2-123">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="af0d2-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="af0d2-124">Leia as propriedades e os relacionamentos de um objeto de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="af0d2-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af0d2-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af0d2-125">Properties</span></span>
| <span data-ttu-id="af0d2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af0d2-126">Property</span></span>     | <span data-ttu-id="af0d2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="af0d2-127">Type</span></span>   |<span data-ttu-id="af0d2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="af0d2-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af0d2-129">recurso</span><span class="sxs-lookup"><span data-stu-id="af0d2-129">capability</span></span>     | <span data-ttu-id="af0d2-130">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-130">String</span></span>  | <span data-ttu-id="af0d2-131">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="af0d2-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="af0d2-132">(por exemplo, mensagens, conversas, etc.)  Não são nulas.</span><span class="sxs-lookup"><span data-stu-id="af0d2-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="af0d2-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-133">Read-only.</span></span> |
| <span data-ttu-id="af0d2-134">id</span><span class="sxs-lookup"><span data-stu-id="af0d2-134">id</span></span>             | <span data-ttu-id="af0d2-135">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-135">String</span></span>  | <span data-ttu-id="af0d2-136">Identificador exclusivo para o ponto de extremidade; Tecla.</span><span class="sxs-lookup"><span data-stu-id="af0d2-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="af0d2-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="af0d2-137">Not nullable.</span></span> <span data-ttu-id="af0d2-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-138">Read-only.</span></span>|
| <span data-ttu-id="af0d2-139">providerId</span><span class="sxs-lookup"><span data-stu-id="af0d2-139">providerId</span></span>     | <span data-ttu-id="af0d2-140">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-140">String</span></span>  | <span data-ttu-id="af0d2-141">Id do aplicativo de publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="af0d2-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="af0d2-142">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="af0d2-142">Not nullable.</span></span> <span data-ttu-id="af0d2-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-143">Read-only.</span></span>|
| <span data-ttu-id="af0d2-144">providerName</span><span class="sxs-lookup"><span data-stu-id="af0d2-144">providerName</span></span>   | <span data-ttu-id="af0d2-145">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-145">String</span></span>  | <span data-ttu-id="af0d2-146">Nome da publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="af0d2-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="af0d2-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-147">Read-only.</span></span>|
| <span data-ttu-id="af0d2-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="af0d2-148">providerResourceId</span></span>|<span data-ttu-id="af0d2-149">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-149">String</span></span>| <span data-ttu-id="af0d2-150">Para grupos do Office 365, isso é definido como um nome conhecido do recurso (por exemplo, Yammer.FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="af0d2-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="af0d2-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="af0d2-151">Not nullable.</span></span> <span data-ttu-id="af0d2-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-152">Read-only.</span></span>|
| <span data-ttu-id="af0d2-153">URI</span><span class="sxs-lookup"><span data-stu-id="af0d2-153">uri</span></span>            | <span data-ttu-id="af0d2-154">String</span><span class="sxs-lookup"><span data-stu-id="af0d2-154">String</span></span>  | <span data-ttu-id="af0d2-155">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="af0d2-155">URL of the published resource.</span></span> <span data-ttu-id="af0d2-156">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="af0d2-156">Not nullable.</span></span> <span data-ttu-id="af0d2-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af0d2-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af0d2-158">Relações</span><span class="sxs-lookup"><span data-stu-id="af0d2-158">Relationships</span></span>

<span data-ttu-id="af0d2-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af0d2-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="af0d2-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af0d2-160">JSON representation</span></span>
<span data-ttu-id="af0d2-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af0d2-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->