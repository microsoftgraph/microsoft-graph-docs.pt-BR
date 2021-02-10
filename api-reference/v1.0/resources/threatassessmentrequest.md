---
title: Tipo de recurso threatAssessmentRequest
description: Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaças.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e316591f4f9db189b1b21dc2d9c3b8d83358c5da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158958"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="bc0bf-103">Tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="bc0bf-104">Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="bc0bf-105">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="bc0bf-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="bc0bf-106">Mail ([recurso mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="bc0bf-107">Arquivo de email[(recurso emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="bc0bf-108">File ([recurso fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="bc0bf-109">URL ([recurso urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="bc0bf-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc0bf-110">Methods</span></span>

| <span data-ttu-id="bc0bf-111">Método</span><span class="sxs-lookup"><span data-stu-id="bc0bf-111">Method</span></span>       | <span data-ttu-id="bc0bf-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc0bf-112">Return Type</span></span> | <span data-ttu-id="bc0bf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0bf-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bc0bf-114">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="bc0bf-115">[Coleção threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="bc0bf-116">Listar todas as solicitações de avaliação de ameaças no locatário.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="bc0bf-117">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="bc0bf-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="bc0bf-119">Crie uma nova solicitação de avaliação de ameaças postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="bc0bf-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="bc0bf-120">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="bc0bf-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc0bf-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="bc0bf-122">Recupere as propriedades e os relacionamentos de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc0bf-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc0bf-123">Properties</span></span>

| <span data-ttu-id="bc0bf-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc0bf-124">Property</span></span>     | <span data-ttu-id="bc0bf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0bf-125">Type</span></span>        | <span data-ttu-id="bc0bf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0bf-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="bc0bf-127">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="bc0bf-127">category</span></span>|[<span data-ttu-id="bc0bf-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="bc0bf-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="bc0bf-129">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-129">The threat category.</span></span> <span data-ttu-id="bc0bf-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="bc0bf-131">contentType</span><span class="sxs-lookup"><span data-stu-id="bc0bf-131">contentType</span></span>|[<span data-ttu-id="bc0bf-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="bc0bf-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="bc0bf-133">O tipo de conteúdo de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-133">The content type of threat assessment.</span></span> <span data-ttu-id="bc0bf-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="bc0bf-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="bc0bf-135">createdBy</span></span>|[<span data-ttu-id="bc0bf-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="bc0bf-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="bc0bf-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="bc0bf-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc0bf-138">createdDateTime</span></span>|<span data-ttu-id="bc0bf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc0bf-139">DateTimeOffset</span></span>|<span data-ttu-id="bc0bf-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bc0bf-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bc0bf-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="bc0bf-142">expectedAssessment</span></span>|[<span data-ttu-id="bc0bf-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="bc0bf-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="bc0bf-144">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-144">The expected assessment from submitter.</span></span> <span data-ttu-id="bc0bf-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="bc0bf-146">id</span><span class="sxs-lookup"><span data-stu-id="bc0bf-146">id</span></span>|<span data-ttu-id="bc0bf-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc0bf-147">String</span></span>|<span data-ttu-id="bc0bf-148">A ID da solicitação de avaliação de ameaças é um IDENTIFICADOr global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="bc0bf-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="bc0bf-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="bc0bf-149">requestSource</span></span>|[<span data-ttu-id="bc0bf-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="bc0bf-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="bc0bf-151">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-151">The source of the threat assessment request.</span></span> <span data-ttu-id="bc0bf-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="bc0bf-153">status</span><span class="sxs-lookup"><span data-stu-id="bc0bf-153">status</span></span>|[<span data-ttu-id="bc0bf-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="bc0bf-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="bc0bf-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-155">The assessment process status.</span></span> <span data-ttu-id="bc0bf-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc0bf-157">Relações</span><span class="sxs-lookup"><span data-stu-id="bc0bf-157">Relationships</span></span>

| <span data-ttu-id="bc0bf-158">Relação</span><span class="sxs-lookup"><span data-stu-id="bc0bf-158">Relationship</span></span> | <span data-ttu-id="bc0bf-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0bf-159">Type</span></span>        | <span data-ttu-id="bc0bf-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0bf-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc0bf-161">resultados</span><span class="sxs-lookup"><span data-stu-id="bc0bf-161">results</span></span>|<span data-ttu-id="bc0bf-162">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc0bf-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="bc0bf-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-163">A collection of threat assessment results.</span></span> <span data-ttu-id="bc0bf-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-164">Read-only.</span></span> <span data-ttu-id="bc0bf-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você aplique `$expand` a ele.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc0bf-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc0bf-166">JSON representation</span></span>

<span data-ttu-id="bc0bf-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc0bf-167">The following is a JSON representation of the resource.</span></span>

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

