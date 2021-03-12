---
title: Tipo de recurso threatAssessmentRequest
description: Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dddb7416e18c802b0fbca60c0d134629763f2a03
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721016"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="483d3-103">Tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="483d3-104">Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="483d3-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="483d3-105">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="483d3-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="483d3-106">Mail ([recurso mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="483d3-107">Arquivo de email ([recurso emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="483d3-108">Arquivo ([recurso fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="483d3-109">URL ([recurso urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="483d3-110">Methods</span><span class="sxs-lookup"><span data-stu-id="483d3-110">Methods</span></span>

| <span data-ttu-id="483d3-111">Método</span><span class="sxs-lookup"><span data-stu-id="483d3-111">Method</span></span>       | <span data-ttu-id="483d3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="483d3-112">Return Type</span></span> | <span data-ttu-id="483d3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="483d3-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="483d3-114">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="483d3-115">[Coleção threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="483d3-116">Listar todas as solicitações de avaliação de ameaças em locatário.</span><span class="sxs-lookup"><span data-stu-id="483d3-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="483d3-117">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="483d3-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="483d3-119">Crie uma nova solicitação de avaliação de ameaças postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="483d3-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="483d3-120">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="483d3-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="483d3-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="483d3-122">Recupere as propriedades e as relações de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="483d3-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="483d3-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="483d3-123">Properties</span></span>

| <span data-ttu-id="483d3-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="483d3-124">Property</span></span>     | <span data-ttu-id="483d3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="483d3-125">Type</span></span>        | <span data-ttu-id="483d3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="483d3-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="483d3-127">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="483d3-127">category</span></span>|[<span data-ttu-id="483d3-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="483d3-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="483d3-129">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="483d3-129">The threat category.</span></span> <span data-ttu-id="483d3-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="483d3-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="483d3-131">contentType</span><span class="sxs-lookup"><span data-stu-id="483d3-131">contentType</span></span>|[<span data-ttu-id="483d3-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="483d3-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="483d3-133">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="483d3-133">The content type of threat assessment.</span></span> <span data-ttu-id="483d3-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="483d3-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="483d3-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="483d3-135">createdBy</span></span>|[<span data-ttu-id="483d3-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="483d3-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="483d3-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="483d3-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="483d3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="483d3-138">createdDateTime</span></span>|<span data-ttu-id="483d3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="483d3-139">DateTimeOffset</span></span>|<span data-ttu-id="483d3-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="483d3-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="483d3-141">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="483d3-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="483d3-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="483d3-142">expectedAssessment</span></span>|[<span data-ttu-id="483d3-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="483d3-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="483d3-144">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="483d3-144">The expected assessment from submitter.</span></span> <span data-ttu-id="483d3-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="483d3-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="483d3-146">id</span><span class="sxs-lookup"><span data-stu-id="483d3-146">id</span></span>|<span data-ttu-id="483d3-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="483d3-147">String</span></span>|<span data-ttu-id="483d3-148">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="483d3-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="483d3-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="483d3-149">requestSource</span></span>|[<span data-ttu-id="483d3-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="483d3-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="483d3-151">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="483d3-151">The source of the threat assessment request.</span></span> <span data-ttu-id="483d3-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="483d3-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="483d3-153">status</span><span class="sxs-lookup"><span data-stu-id="483d3-153">status</span></span>|[<span data-ttu-id="483d3-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="483d3-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="483d3-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="483d3-155">The assessment process status.</span></span> <span data-ttu-id="483d3-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="483d3-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="483d3-157">Relações</span><span class="sxs-lookup"><span data-stu-id="483d3-157">Relationships</span></span>

| <span data-ttu-id="483d3-158">Relação</span><span class="sxs-lookup"><span data-stu-id="483d3-158">Relationship</span></span> | <span data-ttu-id="483d3-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="483d3-159">Type</span></span>        | <span data-ttu-id="483d3-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="483d3-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="483d3-161">results</span><span class="sxs-lookup"><span data-stu-id="483d3-161">results</span></span>|<span data-ttu-id="483d3-162">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="483d3-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="483d3-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="483d3-163">A collection of threat assessment results.</span></span> <span data-ttu-id="483d3-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="483d3-164">Read-only.</span></span> <span data-ttu-id="483d3-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="483d3-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="483d3-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="483d3-166">JSON representation</span></span>

<span data-ttu-id="483d3-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="483d3-167">The following is a JSON representation of the resource.</span></span>

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

