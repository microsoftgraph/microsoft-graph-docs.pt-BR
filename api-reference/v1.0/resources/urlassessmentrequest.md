---
title: Tipo de recurso urlAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de URL.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e180d09c2e76b817d2022a7de993b7a98db48d3d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941383"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="f454e-103">Tipo de recurso urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f454e-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="f454e-104">Usado para criar e recuperar uma avaliação de ameaça de URL, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="f454e-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f454e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f454e-105">Methods</span></span>

| <span data-ttu-id="f454e-106">Método</span><span class="sxs-lookup"><span data-stu-id="f454e-106">Method</span></span>       | <span data-ttu-id="f454e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f454e-107">Return Type</span></span> | <span data-ttu-id="f454e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f454e-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f454e-109">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f454e-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="f454e-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f454e-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="f454e-111">Crie uma nova solicitação de avaliação de URL postando um **objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="f454e-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="f454e-112">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f454e-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="f454e-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f454e-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="f454e-114">Leia as propriedades e as relações de um **objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="f454e-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f454e-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f454e-115">Properties</span></span>

| <span data-ttu-id="f454e-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f454e-116">Property</span></span>     | <span data-ttu-id="f454e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f454e-117">Type</span></span>        | <span data-ttu-id="f454e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f454e-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f454e-119">url</span><span class="sxs-lookup"><span data-stu-id="f454e-119">url</span></span>|<span data-ttu-id="f454e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f454e-120">String</span></span>|<span data-ttu-id="f454e-121">A cadeia de caracteres url.</span><span class="sxs-lookup"><span data-stu-id="f454e-121">The URL string.</span></span>|
|<span data-ttu-id="f454e-122">category</span><span class="sxs-lookup"><span data-stu-id="f454e-122">category</span></span>|[<span data-ttu-id="f454e-123">threatCategory</span><span class="sxs-lookup"><span data-stu-id="f454e-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="f454e-124">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="f454e-124">The threat category.</span></span> <span data-ttu-id="f454e-125">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="f454e-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="f454e-126">contentType</span><span class="sxs-lookup"><span data-stu-id="f454e-126">contentType</span></span>|[<span data-ttu-id="f454e-127">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="f454e-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="f454e-128">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f454e-128">The content type of the threat assessment.</span></span> <span data-ttu-id="f454e-129">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="f454e-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="f454e-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="f454e-130">createdBy</span></span>|[<span data-ttu-id="f454e-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="f454e-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="f454e-132">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f454e-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="f454e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f454e-133">createdDateTime</span></span>|<span data-ttu-id="f454e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f454e-134">DateTimeOffset</span></span>|<span data-ttu-id="f454e-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f454e-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f454e-136">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f454e-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="f454e-137">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="f454e-137">expectedAssessment</span></span>|[<span data-ttu-id="f454e-138">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="f454e-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="f454e-139">A avaliação esperada do ubmitter.</span><span class="sxs-lookup"><span data-stu-id="f454e-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="f454e-140">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="f454e-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="f454e-141">id</span><span class="sxs-lookup"><span data-stu-id="f454e-141">id</span></span>|<span data-ttu-id="f454e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f454e-142">String</span></span>|<span data-ttu-id="f454e-143">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="f454e-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="f454e-144">requestSource</span><span class="sxs-lookup"><span data-stu-id="f454e-144">requestSource</span></span>|[<span data-ttu-id="f454e-145">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="f454e-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="f454e-146">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f454e-146">The source of the threat assessment request.</span></span> <span data-ttu-id="f454e-147">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="f454e-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="f454e-148">status</span><span class="sxs-lookup"><span data-stu-id="f454e-148">status</span></span>|[<span data-ttu-id="f454e-149">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="f454e-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="f454e-150">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="f454e-150">The assessment process status.</span></span> <span data-ttu-id="f454e-151">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="f454e-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f454e-152">Relações</span><span class="sxs-lookup"><span data-stu-id="f454e-152">Relationships</span></span>

| <span data-ttu-id="f454e-153">Relação</span><span class="sxs-lookup"><span data-stu-id="f454e-153">Relationship</span></span> | <span data-ttu-id="f454e-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="f454e-154">Type</span></span>        | <span data-ttu-id="f454e-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="f454e-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f454e-156">results</span><span class="sxs-lookup"><span data-stu-id="f454e-156">results</span></span>|<span data-ttu-id="f454e-157">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="f454e-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="f454e-158">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f454e-158">A collection of threat assessment results.</span></span> <span data-ttu-id="f454e-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f454e-159">Read-only.</span></span> <span data-ttu-id="f454e-160">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="f454e-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f454e-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f454e-161">JSON representation</span></span>

<span data-ttu-id="f454e-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f454e-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "url": "String",
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
  "description": "urlAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

