---
title: Tipo de recurso urlAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaças de URL.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 68df999766bd7fd1b548e0db7e96a8819c04c75a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156669"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="87eaa-103">Tipo de recurso urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="87eaa-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="87eaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87eaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87eaa-105">Usado para criar e recuperar uma avaliação de ameaça de URL, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="87eaa-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="87eaa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="87eaa-106">Methods</span></span>

| <span data-ttu-id="87eaa-107">Método</span><span class="sxs-lookup"><span data-stu-id="87eaa-107">Method</span></span>       | <span data-ttu-id="87eaa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87eaa-108">Return Type</span></span> | <span data-ttu-id="87eaa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87eaa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87eaa-110">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="87eaa-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="87eaa-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="87eaa-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="87eaa-112">Crie uma nova solicitação de avaliação de URL postando um **objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="87eaa-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="87eaa-113">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="87eaa-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="87eaa-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="87eaa-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="87eaa-115">Leia as propriedades e os relacionamentos de **um objeto urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="87eaa-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="87eaa-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87eaa-116">Properties</span></span>

| <span data-ttu-id="87eaa-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87eaa-117">Property</span></span>     | <span data-ttu-id="87eaa-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="87eaa-118">Type</span></span>        | <span data-ttu-id="87eaa-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="87eaa-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87eaa-120">url</span><span class="sxs-lookup"><span data-stu-id="87eaa-120">url</span></span>|<span data-ttu-id="87eaa-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87eaa-121">String</span></span>|<span data-ttu-id="87eaa-122">A cadeia de caracteres da URL.</span><span class="sxs-lookup"><span data-stu-id="87eaa-122">The URL string.</span></span>|
|<span data-ttu-id="87eaa-123">category</span><span class="sxs-lookup"><span data-stu-id="87eaa-123">category</span></span>|[<span data-ttu-id="87eaa-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="87eaa-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="87eaa-125">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="87eaa-125">The threat category.</span></span> <span data-ttu-id="87eaa-126">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="87eaa-127">contentType</span><span class="sxs-lookup"><span data-stu-id="87eaa-127">contentType</span></span>|[<span data-ttu-id="87eaa-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="87eaa-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="87eaa-129">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="87eaa-129">The content type of the threat assessment.</span></span> <span data-ttu-id="87eaa-130">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="87eaa-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="87eaa-131">createdBy</span></span>|[<span data-ttu-id="87eaa-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="87eaa-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="87eaa-133">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="87eaa-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="87eaa-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87eaa-134">createdDateTime</span></span>|<span data-ttu-id="87eaa-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87eaa-135">DateTimeOffset</span></span>|<span data-ttu-id="87eaa-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="87eaa-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87eaa-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="87eaa-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="87eaa-138">expectedAssessment</span></span>|[<span data-ttu-id="87eaa-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="87eaa-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="87eaa-140">A avaliação esperada do ubmitter.</span><span class="sxs-lookup"><span data-stu-id="87eaa-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="87eaa-141">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="87eaa-142">id</span><span class="sxs-lookup"><span data-stu-id="87eaa-142">id</span></span>|<span data-ttu-id="87eaa-143">String</span><span class="sxs-lookup"><span data-stu-id="87eaa-143">String</span></span>|<span data-ttu-id="87eaa-144">A ID da solicitação de avaliação de ameaças é um IDENTIFICADOr global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="87eaa-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="87eaa-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="87eaa-145">requestSource</span></span>|[<span data-ttu-id="87eaa-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="87eaa-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="87eaa-147">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="87eaa-147">The source of the threat assessment request.</span></span> <span data-ttu-id="87eaa-148">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="87eaa-149">status</span><span class="sxs-lookup"><span data-stu-id="87eaa-149">status</span></span>|[<span data-ttu-id="87eaa-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="87eaa-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="87eaa-151">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="87eaa-151">The assessment process status.</span></span> <span data-ttu-id="87eaa-152">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="87eaa-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87eaa-153">Relações</span><span class="sxs-lookup"><span data-stu-id="87eaa-153">Relationships</span></span>

| <span data-ttu-id="87eaa-154">Relação</span><span class="sxs-lookup"><span data-stu-id="87eaa-154">Relationship</span></span> | <span data-ttu-id="87eaa-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="87eaa-155">Type</span></span>        | <span data-ttu-id="87eaa-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="87eaa-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87eaa-157">resultados</span><span class="sxs-lookup"><span data-stu-id="87eaa-157">results</span></span>|<span data-ttu-id="87eaa-158">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="87eaa-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="87eaa-159">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="87eaa-159">A collection of threat assessment results.</span></span> <span data-ttu-id="87eaa-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87eaa-160">Read-only.</span></span> <span data-ttu-id="87eaa-161">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você aplique `$expand` a ele.</span><span class="sxs-lookup"><span data-stu-id="87eaa-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87eaa-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87eaa-162">JSON representation</span></span>

<span data-ttu-id="87eaa-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87eaa-163">The following is a JSON representation of the resource.</span></span>

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


