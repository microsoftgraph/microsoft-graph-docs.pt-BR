---
title: Tipo de recurso de ponto de extremidade
description: 'Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871279"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="9ab6c-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="9ab6c-107">Endpoint resource type</span></span>

> <span data-ttu-id="9ab6c-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ab6c-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ab6c-110">Pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="9ab6c-111">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="9ab6c-112">Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="9ab6c-113">Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="9ab6c-114">Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="9ab6c-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ab6c-115">Methods</span></span>

| <span data-ttu-id="9ab6c-116">Método</span><span class="sxs-lookup"><span data-stu-id="9ab6c-116">Method</span></span>           | <span data-ttu-id="9ab6c-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ab6c-117">Return Type</span></span>    |<span data-ttu-id="9ab6c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab6c-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ab6c-119">Lista de pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="9ab6c-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="9ab6c-120">Coleção de [ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="9ab6c-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="9ab6c-121">Obtenha uma coleção de objetos de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="9ab6c-122">Obtenha o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="9ab6c-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="9ab6c-123">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="9ab6c-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="9ab6c-124">Leia as propriedades e os relacionamentos de um objeto de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ab6c-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ab6c-125">Properties</span></span>
| <span data-ttu-id="9ab6c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ab6c-126">Property</span></span>     | <span data-ttu-id="9ab6c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ab6c-127">Type</span></span>   |<span data-ttu-id="9ab6c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab6c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ab6c-129">recurso</span><span class="sxs-lookup"><span data-stu-id="9ab6c-129">capability</span></span>     | <span data-ttu-id="9ab6c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-130">String</span></span>  | <span data-ttu-id="9ab6c-131">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="9ab6c-132">(por exemplo, mensagens, conversas, etc.)  Não são nulas.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="9ab6c-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-133">Read-only.</span></span> |
| <span data-ttu-id="9ab6c-134">id</span><span class="sxs-lookup"><span data-stu-id="9ab6c-134">id</span></span>             | <span data-ttu-id="9ab6c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-135">String</span></span>  | <span data-ttu-id="9ab6c-136">Identificador exclusivo para o ponto de extremidade; Tecla.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="9ab6c-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-137">Not nullable.</span></span> <span data-ttu-id="9ab6c-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-138">Read-only.</span></span>|
| <span data-ttu-id="9ab6c-139">providerId</span><span class="sxs-lookup"><span data-stu-id="9ab6c-139">providerId</span></span>     | <span data-ttu-id="9ab6c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-140">String</span></span>  | <span data-ttu-id="9ab6c-141">Id do aplicativo de publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="9ab6c-142">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-142">Not nullable.</span></span> <span data-ttu-id="9ab6c-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-143">Read-only.</span></span>|
| <span data-ttu-id="9ab6c-144">providerName</span><span class="sxs-lookup"><span data-stu-id="9ab6c-144">providerName</span></span>   | <span data-ttu-id="9ab6c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-145">String</span></span>  | <span data-ttu-id="9ab6c-146">Nome da publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="9ab6c-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-147">Read-only.</span></span>|
| <span data-ttu-id="9ab6c-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="9ab6c-148">providerResourceId</span></span>|<span data-ttu-id="9ab6c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-149">String</span></span>| <span data-ttu-id="9ab6c-150">Para grupos do Office 365, isso é definido como um nome conhecido do recurso (por exemplo, Yammer.FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="9ab6c-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="9ab6c-151">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-151">Not nullable.</span></span> <span data-ttu-id="9ab6c-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-152">Read-only.</span></span>|
| <span data-ttu-id="9ab6c-153">URI</span><span class="sxs-lookup"><span data-stu-id="9ab6c-153">uri</span></span>            | <span data-ttu-id="9ab6c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab6c-154">String</span></span>  | <span data-ttu-id="9ab6c-155">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-155">URL of the published resource.</span></span> <span data-ttu-id="9ab6c-156">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-156">Not nullable.</span></span> <span data-ttu-id="9ab6c-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ab6c-158">Relações</span><span class="sxs-lookup"><span data-stu-id="9ab6c-158">Relationships</span></span>

<span data-ttu-id="9ab6c-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ab6c-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9ab6c-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ab6c-160">JSON representation</span></span>
<span data-ttu-id="9ab6c-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ab6c-161">Here is a JSON representation of the resource.</span></span>

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
