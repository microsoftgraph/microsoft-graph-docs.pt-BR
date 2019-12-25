---
title: tipo de recurso urlAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de URL.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 27e728e172ec8870082f6b7d668f1f19f29f22dc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867134"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="672de-103">tipo de recurso urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="672de-103">urlAssessmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672de-104">Usado para criar e recuperar uma avaliação de ameaça de URL, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="672de-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="672de-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="672de-105">Methods</span></span>

| <span data-ttu-id="672de-106">Método</span><span class="sxs-lookup"><span data-stu-id="672de-106">Method</span></span>       | <span data-ttu-id="672de-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="672de-107">Return Type</span></span> | <span data-ttu-id="672de-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="672de-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="672de-109">Criar threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="672de-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="672de-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="672de-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="672de-111">Crie uma nova solicitação de avaliação de URL postando um objeto **urlAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="672de-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="672de-112">Obter threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="672de-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="672de-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="672de-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="672de-114">Leia as propriedades e os relacionamentos de um objeto **urlAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="672de-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="672de-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="672de-115">Properties</span></span>

| <span data-ttu-id="672de-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="672de-116">Property</span></span>     | <span data-ttu-id="672de-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="672de-117">Type</span></span>        | <span data-ttu-id="672de-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="672de-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="672de-119">url</span><span class="sxs-lookup"><span data-stu-id="672de-119">url</span></span>|<span data-ttu-id="672de-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="672de-120">String</span></span>|<span data-ttu-id="672de-121">A cadeia de caracteres da URL.</span><span class="sxs-lookup"><span data-stu-id="672de-121">The URL string.</span></span>|
|<span data-ttu-id="672de-122">category</span><span class="sxs-lookup"><span data-stu-id="672de-122">category</span></span>|[<span data-ttu-id="672de-123">threatCategory</span><span class="sxs-lookup"><span data-stu-id="672de-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="672de-124">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="672de-124">The threat category.</span></span> <span data-ttu-id="672de-125">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="672de-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="672de-126">contentType</span><span class="sxs-lookup"><span data-stu-id="672de-126">contentType</span></span>|[<span data-ttu-id="672de-127">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="672de-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="672de-128">O tipo de conteúdo da avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="672de-128">The content type of the threat assessment.</span></span> <span data-ttu-id="672de-129">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="672de-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="672de-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="672de-130">createdBy</span></span>|[<span data-ttu-id="672de-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="672de-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="672de-132">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="672de-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="672de-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="672de-133">createdDateTime</span></span>|<span data-ttu-id="672de-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="672de-134">DateTimeOffset</span></span>|<span data-ttu-id="672de-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="672de-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="672de-136">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="672de-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="672de-137">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="672de-137">expectedAssessment</span></span>|[<span data-ttu-id="672de-138">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="672de-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="672de-139">A avaliação esperada do ubmitter.</span><span class="sxs-lookup"><span data-stu-id="672de-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="672de-140">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="672de-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="672de-141">id</span><span class="sxs-lookup"><span data-stu-id="672de-141">id</span></span>|<span data-ttu-id="672de-142">String</span><span class="sxs-lookup"><span data-stu-id="672de-142">String</span></span>|<span data-ttu-id="672de-143">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="672de-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="672de-144">objectrequest</span><span class="sxs-lookup"><span data-stu-id="672de-144">requestSource</span></span>|[<span data-ttu-id="672de-145">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="672de-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="672de-146">A origem da solicitação de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="672de-146">The source of the threat assessment request.</span></span> <span data-ttu-id="672de-147">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="672de-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="672de-148">status</span><span class="sxs-lookup"><span data-stu-id="672de-148">status</span></span>|[<span data-ttu-id="672de-149">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="672de-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="672de-150">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="672de-150">The assessment process status.</span></span> <span data-ttu-id="672de-151">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="672de-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="672de-152">Relações</span><span class="sxs-lookup"><span data-stu-id="672de-152">Relationships</span></span>

| <span data-ttu-id="672de-153">Relação</span><span class="sxs-lookup"><span data-stu-id="672de-153">Relationship</span></span> | <span data-ttu-id="672de-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="672de-154">Type</span></span>        | <span data-ttu-id="672de-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="672de-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="672de-156">resultados</span><span class="sxs-lookup"><span data-stu-id="672de-156">results</span></span>|<span data-ttu-id="672de-157">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="672de-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="672de-158">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="672de-158">A collection of threat assessment results.</span></span> <span data-ttu-id="672de-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="672de-159">Read-only.</span></span> <span data-ttu-id="672de-160">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="672de-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="672de-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="672de-161">JSON representation</span></span>

<span data-ttu-id="672de-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="672de-162">The following is a JSON representation of the resource.</span></span>

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
