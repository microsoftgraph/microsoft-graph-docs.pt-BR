---
title: Tipo de recurso de ponto de extremidade
description: 'Os pontos de extremidade representam URLs para recursos associados a uma entidade.  Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365. Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos. Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo. Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências. '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542935"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="cc98c-107">Tipo de recurso de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="cc98c-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc98c-108">Os pontos de extremidade representam URLs para recursos associados a uma entidade.</span><span class="sxs-lookup"><span data-stu-id="cc98c-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="cc98c-109">Por exemplo, quando um novo grupo do Office 365 é criado, recursos adicionais também são criados como parte do grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cc98c-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="cc98c-110">Isso inclui itens como uma caixa de correio de grupo para conversas e uma pasta do OneDrive de grupo para documentos e arquivos.</span><span class="sxs-lookup"><span data-stu-id="cc98c-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="cc98c-111">Informações adicionais sobre esses recursos de grupo do Office 365, incluindo suas URLs de recurso associadas, agora podem ser lidas usando a navegação de *pontos de extremidade* no tipo de recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="cc98c-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="cc98c-112">Isso permite que os aplicativos entendam esses recursos e, até mesmo, incorpore as experiências de URL de recurso em suas próprias experiências.</span><span class="sxs-lookup"><span data-stu-id="cc98c-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="cc98c-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc98c-113">Methods</span></span>

| <span data-ttu-id="cc98c-114">Método</span><span class="sxs-lookup"><span data-stu-id="cc98c-114">Method</span></span>           | <span data-ttu-id="cc98c-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc98c-115">Return Type</span></span>    |<span data-ttu-id="cc98c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc98c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc98c-117">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="cc98c-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="cc98c-118">conjunto [Ponto de extremidade](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="cc98c-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="cc98c-119">Obtenha uma coleção de o objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="cc98c-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="cc98c-120">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="cc98c-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="cc98c-121">Ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="cc98c-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="cc98c-122">Leia as propriedades e os relacionamentos do objeto ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="cc98c-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc98c-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc98c-123">Properties</span></span>
| <span data-ttu-id="cc98c-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc98c-124">Property</span></span>     | <span data-ttu-id="cc98c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc98c-125">Type</span></span>   |<span data-ttu-id="cc98c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc98c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc98c-127">função</span><span class="sxs-lookup"><span data-stu-id="cc98c-127">capability</span></span>     | <span data-ttu-id="cc98c-128">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-128">String</span></span>  | <span data-ttu-id="cc98c-129">Descreve o recurso que está associado a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="cc98c-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="cc98c-130">(por exemplo, mensagens, conversas etc.)  Não anulável.</span><span class="sxs-lookup"><span data-stu-id="cc98c-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="cc98c-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-131">Read-only.</span></span> |
| <span data-ttu-id="cc98c-132">id</span><span class="sxs-lookup"><span data-stu-id="cc98c-132">id</span></span>             | <span data-ttu-id="cc98c-133">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-133">String</span></span>  | <span data-ttu-id="cc98c-134">Identificador exclusivo do ponto de extremidade; Chaves.</span><span class="sxs-lookup"><span data-stu-id="cc98c-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="cc98c-135">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="cc98c-135">Not nullable.</span></span> <span data-ttu-id="cc98c-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-136">Read-only.</span></span>|
| <span data-ttu-id="cc98c-137">providerId</span><span class="sxs-lookup"><span data-stu-id="cc98c-137">providerId</span></span>     | <span data-ttu-id="cc98c-138">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-138">String</span></span>  | <span data-ttu-id="cc98c-139">ID de aplicativo do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="cc98c-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="cc98c-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="cc98c-140">Not nullable.</span></span> <span data-ttu-id="cc98c-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-141">Read-only.</span></span>|
| <span data-ttu-id="cc98c-142">providerName</span><span class="sxs-lookup"><span data-stu-id="cc98c-142">providerName</span></span>   | <span data-ttu-id="cc98c-143">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-143">String</span></span>  | <span data-ttu-id="cc98c-144">Nome do serviço subjacente de publicação.</span><span class="sxs-lookup"><span data-stu-id="cc98c-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="cc98c-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-145">Read-only.</span></span>|
| <span data-ttu-id="cc98c-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="cc98c-146">providerResourceId</span></span>|<span data-ttu-id="cc98c-147">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-147">String</span></span>| <span data-ttu-id="cc98c-148">Para grupos do Office 365, isso é definido como um nome conhecido para o recurso (por exemplo, Yammer. FeedURL etc.).</span><span class="sxs-lookup"><span data-stu-id="cc98c-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="cc98c-149">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="cc98c-149">Not nullable.</span></span> <span data-ttu-id="cc98c-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-150">Read-only.</span></span>|
| <span data-ttu-id="cc98c-151">URI</span><span class="sxs-lookup"><span data-stu-id="cc98c-151">uri</span></span>            | <span data-ttu-id="cc98c-152">String</span><span class="sxs-lookup"><span data-stu-id="cc98c-152">String</span></span>  | <span data-ttu-id="cc98c-153">URL do recurso publicado.</span><span class="sxs-lookup"><span data-stu-id="cc98c-153">URL of the published resource.</span></span> <span data-ttu-id="cc98c-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="cc98c-154">Not nullable.</span></span> <span data-ttu-id="cc98c-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc98c-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc98c-156">Relações</span><span class="sxs-lookup"><span data-stu-id="cc98c-156">Relationships</span></span>

<span data-ttu-id="cc98c-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc98c-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cc98c-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc98c-158">JSON representation</span></span>
<span data-ttu-id="cc98c-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc98c-159">Here is a JSON representation of the resource.</span></span>

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
