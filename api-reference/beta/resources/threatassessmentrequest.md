---
title: Tipo de recurso threatAssessmentRequest
description: Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaças.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1896123151680bfc6b69075d7f8888ccaa64b9ee
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155521"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="6f918-103">Tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="6f918-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f918-105">Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f918-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="6f918-106">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="6f918-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="6f918-107">Mail ([recurso mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="6f918-108">Arquivo de email[(recurso emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="6f918-109">File ([recurso fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="6f918-110">URL ([recurso urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="6f918-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f918-111">Methods</span></span>

| <span data-ttu-id="6f918-112">Método</span><span class="sxs-lookup"><span data-stu-id="6f918-112">Method</span></span>       | <span data-ttu-id="6f918-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f918-113">Return Type</span></span> | <span data-ttu-id="6f918-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f918-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6f918-115">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="6f918-116">[Coleção threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="6f918-117">Listar todas as solicitações de avaliação de ameaças no locatário.</span><span class="sxs-lookup"><span data-stu-id="6f918-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="6f918-118">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="6f918-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="6f918-120">Crie uma nova solicitação de avaliação de ameaças postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="6f918-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="6f918-121">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="6f918-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f918-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="6f918-123">Recupere as propriedades e os relacionamentos de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="6f918-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f918-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f918-124">Properties</span></span>

| <span data-ttu-id="6f918-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f918-125">Property</span></span>     | <span data-ttu-id="6f918-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f918-126">Type</span></span>        | <span data-ttu-id="6f918-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f918-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="6f918-128">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="6f918-128">category</span></span>|[<span data-ttu-id="6f918-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="6f918-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="6f918-130">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="6f918-130">The threat category.</span></span> <span data-ttu-id="6f918-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="6f918-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="6f918-132">contentType</span><span class="sxs-lookup"><span data-stu-id="6f918-132">contentType</span></span>|[<span data-ttu-id="6f918-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="6f918-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="6f918-134">O tipo de conteúdo de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f918-134">The content type of threat assessment.</span></span> <span data-ttu-id="6f918-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="6f918-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="6f918-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="6f918-136">createdBy</span></span>|[<span data-ttu-id="6f918-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="6f918-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="6f918-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f918-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="6f918-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f918-139">createdDateTime</span></span>|<span data-ttu-id="6f918-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f918-140">DateTimeOffset</span></span>|<span data-ttu-id="6f918-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6f918-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6f918-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6f918-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6f918-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="6f918-143">expectedAssessment</span></span>|[<span data-ttu-id="6f918-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="6f918-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="6f918-145">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="6f918-145">The expected assessment from submitter.</span></span> <span data-ttu-id="6f918-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="6f918-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="6f918-147">id</span><span class="sxs-lookup"><span data-stu-id="6f918-147">id</span></span>|<span data-ttu-id="6f918-148">String</span><span class="sxs-lookup"><span data-stu-id="6f918-148">String</span></span>|<span data-ttu-id="6f918-149">A ID da solicitação de avaliação de ameaças é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="6f918-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="6f918-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="6f918-150">requestSource</span></span>|[<span data-ttu-id="6f918-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="6f918-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="6f918-152">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f918-152">The source of the threat assessment request.</span></span> <span data-ttu-id="6f918-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="6f918-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="6f918-154">status</span><span class="sxs-lookup"><span data-stu-id="6f918-154">status</span></span>|[<span data-ttu-id="6f918-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="6f918-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="6f918-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="6f918-156">The assessment process status.</span></span> <span data-ttu-id="6f918-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="6f918-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f918-158">Relações</span><span class="sxs-lookup"><span data-stu-id="6f918-158">Relationships</span></span>

| <span data-ttu-id="6f918-159">Relação</span><span class="sxs-lookup"><span data-stu-id="6f918-159">Relationship</span></span> | <span data-ttu-id="6f918-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f918-160">Type</span></span>        | <span data-ttu-id="6f918-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f918-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f918-162">resultados</span><span class="sxs-lookup"><span data-stu-id="6f918-162">results</span></span>|<span data-ttu-id="6f918-163">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f918-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="6f918-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f918-164">A collection of threat assessment results.</span></span> <span data-ttu-id="6f918-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f918-165">Read-only.</span></span> <span data-ttu-id="6f918-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você aplique `$expand` a ele.</span><span class="sxs-lookup"><span data-stu-id="6f918-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f918-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f918-167">JSON representation</span></span>

<span data-ttu-id="6f918-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f918-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


