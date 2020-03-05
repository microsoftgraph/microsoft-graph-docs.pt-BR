---
title: tipo de recurso urlAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de URL.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2eb3372b92a3665129bb0b4eb4d0f27bc77884f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519565"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="eb7ef-103">tipo de recurso urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="eb7ef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb7ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb7ef-105">Usado para criar e recuperar uma avaliação de ameaça de URL, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="eb7ef-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb7ef-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb7ef-106">Methods</span></span>

| <span data-ttu-id="eb7ef-107">Método</span><span class="sxs-lookup"><span data-stu-id="eb7ef-107">Method</span></span>       | <span data-ttu-id="eb7ef-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb7ef-108">Return Type</span></span> | <span data-ttu-id="eb7ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7ef-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb7ef-110">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="eb7ef-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="eb7ef-112">Crie uma nova solicitação de avaliação de URL postando um objeto **urlAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="eb7ef-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="eb7ef-113">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="eb7ef-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="eb7ef-115">Leia as propriedades e os relacionamentos de um objeto **urlAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="eb7ef-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb7ef-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb7ef-116">Properties</span></span>

| <span data-ttu-id="eb7ef-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb7ef-117">Property</span></span>     | <span data-ttu-id="eb7ef-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb7ef-118">Type</span></span>        | <span data-ttu-id="eb7ef-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7ef-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb7ef-120">url</span><span class="sxs-lookup"><span data-stu-id="eb7ef-120">url</span></span>|<span data-ttu-id="eb7ef-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb7ef-121">String</span></span>|<span data-ttu-id="eb7ef-122">A cadeia de caracteres da URL.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-122">The URL string.</span></span>|
|<span data-ttu-id="eb7ef-123">category</span><span class="sxs-lookup"><span data-stu-id="eb7ef-123">category</span></span>|[<span data-ttu-id="eb7ef-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="eb7ef-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="eb7ef-125">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-125">The threat category.</span></span> <span data-ttu-id="eb7ef-126">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="eb7ef-127">contentType</span><span class="sxs-lookup"><span data-stu-id="eb7ef-127">contentType</span></span>|[<span data-ttu-id="eb7ef-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="eb7ef-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="eb7ef-129">O tipo de conteúdo da avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-129">The content type of the threat assessment.</span></span> <span data-ttu-id="eb7ef-130">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="eb7ef-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="eb7ef-131">createdBy</span></span>|[<span data-ttu-id="eb7ef-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="eb7ef-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="eb7ef-133">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="eb7ef-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb7ef-134">createdDateTime</span></span>|<span data-ttu-id="eb7ef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb7ef-135">DateTimeOffset</span></span>|<span data-ttu-id="eb7ef-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb7ef-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="eb7ef-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="eb7ef-138">expectedAssessment</span></span>|[<span data-ttu-id="eb7ef-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="eb7ef-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="eb7ef-140">A avaliação esperada do ubmitter.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="eb7ef-141">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="eb7ef-142">id</span><span class="sxs-lookup"><span data-stu-id="eb7ef-142">id</span></span>|<span data-ttu-id="eb7ef-143">String</span><span class="sxs-lookup"><span data-stu-id="eb7ef-143">String</span></span>|<span data-ttu-id="eb7ef-144">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="eb7ef-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="eb7ef-145">objectrequest</span><span class="sxs-lookup"><span data-stu-id="eb7ef-145">requestSource</span></span>|[<span data-ttu-id="eb7ef-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="eb7ef-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="eb7ef-147">A origem da solicitação de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-147">The source of the threat assessment request.</span></span> <span data-ttu-id="eb7ef-148">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="eb7ef-149">status</span><span class="sxs-lookup"><span data-stu-id="eb7ef-149">status</span></span>|[<span data-ttu-id="eb7ef-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="eb7ef-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="eb7ef-151">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-151">The assessment process status.</span></span> <span data-ttu-id="eb7ef-152">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb7ef-153">Relações</span><span class="sxs-lookup"><span data-stu-id="eb7ef-153">Relationships</span></span>

| <span data-ttu-id="eb7ef-154">Relação</span><span class="sxs-lookup"><span data-stu-id="eb7ef-154">Relationship</span></span> | <span data-ttu-id="eb7ef-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb7ef-155">Type</span></span>        | <span data-ttu-id="eb7ef-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7ef-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb7ef-157">resultados</span><span class="sxs-lookup"><span data-stu-id="eb7ef-157">results</span></span>|<span data-ttu-id="eb7ef-158">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb7ef-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="eb7ef-159">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-159">A collection of threat assessment results.</span></span> <span data-ttu-id="eb7ef-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-160">Read-only.</span></span> <span data-ttu-id="eb7ef-161">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb7ef-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb7ef-162">JSON representation</span></span>

<span data-ttu-id="eb7ef-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb7ef-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "baseType": "",
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
