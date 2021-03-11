---
title: Tipo de recurso urlAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de URL.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 226e4fff9114fbf13bc0e8bcdc9290180cc487f4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720953"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="edf48-103">Tipo de recurso urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="edf48-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="edf48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edf48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edf48-105">Usado para criar e recuperar uma avaliação de ameaça de URL, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="edf48-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="edf48-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="edf48-106">Methods</span></span>

| <span data-ttu-id="edf48-107">Método</span><span class="sxs-lookup"><span data-stu-id="edf48-107">Method</span></span>       | <span data-ttu-id="edf48-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="edf48-108">Return Type</span></span> | <span data-ttu-id="edf48-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="edf48-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="edf48-110">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="edf48-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="edf48-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="edf48-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="edf48-112">Crie uma nova solicitação de avaliação de URL postando um **objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="edf48-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="edf48-113">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="edf48-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="edf48-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="edf48-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="edf48-115">Leia as propriedades e as relações de um **objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="edf48-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="edf48-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edf48-116">Properties</span></span>

| <span data-ttu-id="edf48-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edf48-117">Property</span></span>     | <span data-ttu-id="edf48-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="edf48-118">Type</span></span>        | <span data-ttu-id="edf48-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="edf48-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edf48-120">url</span><span class="sxs-lookup"><span data-stu-id="edf48-120">url</span></span>|<span data-ttu-id="edf48-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edf48-121">String</span></span>|<span data-ttu-id="edf48-122">A cadeia de caracteres url.</span><span class="sxs-lookup"><span data-stu-id="edf48-122">The URL string.</span></span>|
|<span data-ttu-id="edf48-123">category</span><span class="sxs-lookup"><span data-stu-id="edf48-123">category</span></span>|[<span data-ttu-id="edf48-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="edf48-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="edf48-125">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="edf48-125">The threat category.</span></span> <span data-ttu-id="edf48-126">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="edf48-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="edf48-127">contentType</span><span class="sxs-lookup"><span data-stu-id="edf48-127">contentType</span></span>|[<span data-ttu-id="edf48-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="edf48-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="edf48-129">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="edf48-129">The content type of the threat assessment.</span></span> <span data-ttu-id="edf48-130">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="edf48-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="edf48-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="edf48-131">createdBy</span></span>|[<span data-ttu-id="edf48-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="edf48-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="edf48-133">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="edf48-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="edf48-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edf48-134">createdDateTime</span></span>|<span data-ttu-id="edf48-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf48-135">DateTimeOffset</span></span>|<span data-ttu-id="edf48-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="edf48-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edf48-137">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="edf48-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="edf48-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="edf48-138">expectedAssessment</span></span>|[<span data-ttu-id="edf48-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="edf48-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="edf48-140">A avaliação esperada do ubmitter.</span><span class="sxs-lookup"><span data-stu-id="edf48-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="edf48-141">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="edf48-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="edf48-142">id</span><span class="sxs-lookup"><span data-stu-id="edf48-142">id</span></span>|<span data-ttu-id="edf48-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edf48-143">String</span></span>|<span data-ttu-id="edf48-144">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="edf48-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="edf48-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="edf48-145">requestSource</span></span>|[<span data-ttu-id="edf48-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="edf48-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="edf48-147">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="edf48-147">The source of the threat assessment request.</span></span> <span data-ttu-id="edf48-148">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="edf48-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="edf48-149">status</span><span class="sxs-lookup"><span data-stu-id="edf48-149">status</span></span>|[<span data-ttu-id="edf48-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="edf48-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="edf48-151">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="edf48-151">The assessment process status.</span></span> <span data-ttu-id="edf48-152">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="edf48-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edf48-153">Relações</span><span class="sxs-lookup"><span data-stu-id="edf48-153">Relationships</span></span>

| <span data-ttu-id="edf48-154">Relação</span><span class="sxs-lookup"><span data-stu-id="edf48-154">Relationship</span></span> | <span data-ttu-id="edf48-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="edf48-155">Type</span></span>        | <span data-ttu-id="edf48-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="edf48-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edf48-157">results</span><span class="sxs-lookup"><span data-stu-id="edf48-157">results</span></span>|<span data-ttu-id="edf48-158">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="edf48-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="edf48-159">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="edf48-159">A collection of threat assessment results.</span></span> <span data-ttu-id="edf48-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="edf48-160">Read-only.</span></span> <span data-ttu-id="edf48-161">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="edf48-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edf48-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edf48-162">JSON representation</span></span>

<span data-ttu-id="edf48-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edf48-163">The following is a JSON representation of the resource.</span></span>

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


