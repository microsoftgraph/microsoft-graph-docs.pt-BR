---
title: Tipo de recurso de ponto de extremidade
description: 'Pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos. Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 39a6a2d8213e809f426c492654272aa994c25a6d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574479"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="2fc70-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="2fc70-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fc70-108">Pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="2fc70-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="2fc70-109">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2fc70-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="2fc70-110">Eles incluem coisas como uma caixa de correio de grupo para conversas e uma pasta de OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="2fc70-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="2fc70-111">Mais informações sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associado agora podem ser lido usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="2fc70-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="2fc70-112">Isso permite que aplicativos entender esses recursos e até mesmo incorporar o recurso que URL experiências em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="2fc70-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="2fc70-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="2fc70-113">Methods</span></span>

| <span data-ttu-id="2fc70-114">Método</span><span class="sxs-lookup"><span data-stu-id="2fc70-114">Method</span></span>           | <span data-ttu-id="2fc70-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2fc70-115">Return Type</span></span>    |<span data-ttu-id="2fc70-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc70-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fc70-117">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="2fc70-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="2fc70-118">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="2fc70-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="2fc70-119">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2fc70-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="2fc70-120">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="2fc70-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="2fc70-121">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="2fc70-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="2fc70-122">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2fc70-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2fc70-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fc70-123">Properties</span></span>
| <span data-ttu-id="2fc70-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fc70-124">Property</span></span>     | <span data-ttu-id="2fc70-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fc70-125">Type</span></span>   |<span data-ttu-id="2fc70-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc70-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fc70-127">recurso</span><span class="sxs-lookup"><span data-stu-id="2fc70-127">capability</span></span>     | <span data-ttu-id="2fc70-128">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-128">String</span></span>  | <span data-ttu-id="2fc70-129">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="2fc70-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="2fc70-130">(por exemplo, mensagens, conversas, etc.)  Não são nulas.</span><span class="sxs-lookup"><span data-stu-id="2fc70-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="2fc70-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-131">Read-only.</span></span> |
| <span data-ttu-id="2fc70-132">id</span><span class="sxs-lookup"><span data-stu-id="2fc70-132">id</span></span>             | <span data-ttu-id="2fc70-133">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-133">String</span></span>  | <span data-ttu-id="2fc70-134">Identificador exclusivo para o ponto de extremidade; Tecla.</span><span class="sxs-lookup"><span data-stu-id="2fc70-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="2fc70-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2fc70-135">Not nullable.</span></span> <span data-ttu-id="2fc70-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-136">Read-only.</span></span>|
| <span data-ttu-id="2fc70-137">providerId</span><span class="sxs-lookup"><span data-stu-id="2fc70-137">providerId</span></span>     | <span data-ttu-id="2fc70-138">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-138">String</span></span>  | <span data-ttu-id="2fc70-139">Id do aplicativo de publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="2fc70-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="2fc70-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2fc70-140">Not nullable.</span></span> <span data-ttu-id="2fc70-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-141">Read-only.</span></span>|
| <span data-ttu-id="2fc70-142">providerName</span><span class="sxs-lookup"><span data-stu-id="2fc70-142">providerName</span></span>   | <span data-ttu-id="2fc70-143">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-143">String</span></span>  | <span data-ttu-id="2fc70-144">Nome da publicação do serviço subjacente.</span><span class="sxs-lookup"><span data-stu-id="2fc70-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="2fc70-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-145">Read-only.</span></span>|
| <span data-ttu-id="2fc70-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="2fc70-146">providerResourceId</span></span>|<span data-ttu-id="2fc70-147">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-147">String</span></span>| <span data-ttu-id="2fc70-148">Para grupos do Office 365, isso é definido como um nome conhecido do recurso (por exemplo, Yammer.FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="2fc70-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="2fc70-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2fc70-149">Not nullable.</span></span> <span data-ttu-id="2fc70-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-150">Read-only.</span></span>|
| <span data-ttu-id="2fc70-151">URI</span><span class="sxs-lookup"><span data-stu-id="2fc70-151">uri</span></span>            | <span data-ttu-id="2fc70-152">String</span><span class="sxs-lookup"><span data-stu-id="2fc70-152">String</span></span>  | <span data-ttu-id="2fc70-153">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="2fc70-153">URL of the published resource.</span></span> <span data-ttu-id="2fc70-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="2fc70-154">Not nullable.</span></span> <span data-ttu-id="2fc70-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fc70-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fc70-156">Relações</span><span class="sxs-lookup"><span data-stu-id="2fc70-156">Relationships</span></span>

<span data-ttu-id="2fc70-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fc70-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2fc70-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fc70-158">JSON representation</span></span>
<span data-ttu-id="2fc70-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fc70-159">Here is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
