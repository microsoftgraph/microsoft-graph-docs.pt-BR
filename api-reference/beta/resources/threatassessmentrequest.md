---
title: Tipo de recurso threatAssessmentRequest
description: Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0be6931bf2589f20d26ee7fa37310f3181447b2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950258"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="eca66-103">Tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="eca66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eca66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eca66-105">Um tipo de resouce abstrato usado para representar um item de solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="eca66-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="eca66-106">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="eca66-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="eca66-107">Mail ([recurso mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="eca66-108">Arquivo de email ([recurso emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="eca66-109">Arquivo ([recurso fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="eca66-110">URL ([recurso urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="eca66-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="eca66-111">Methods</span></span>

| <span data-ttu-id="eca66-112">Método</span><span class="sxs-lookup"><span data-stu-id="eca66-112">Method</span></span>       | <span data-ttu-id="eca66-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eca66-113">Return Type</span></span> | <span data-ttu-id="eca66-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca66-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eca66-115">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="eca66-116">[Coleção threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="eca66-117">Listar todas as solicitações de avaliação de ameaças em locatário.</span><span class="sxs-lookup"><span data-stu-id="eca66-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="eca66-118">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="eca66-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="eca66-120">Crie uma nova solicitação de avaliação de ameaças postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="eca66-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="eca66-121">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="eca66-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="eca66-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="eca66-123">Recupere as propriedades e as relações de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="eca66-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="eca66-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eca66-124">Properties</span></span>

| <span data-ttu-id="eca66-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eca66-125">Property</span></span>     | <span data-ttu-id="eca66-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="eca66-126">Type</span></span>        | <span data-ttu-id="eca66-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca66-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="eca66-128">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="eca66-128">category</span></span>|<span data-ttu-id="eca66-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="eca66-129">threatCategory</span></span>|<span data-ttu-id="eca66-130">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="eca66-130">The threat category.</span></span> <span data-ttu-id="eca66-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="eca66-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="eca66-132">contentType</span><span class="sxs-lookup"><span data-stu-id="eca66-132">contentType</span></span>|<span data-ttu-id="eca66-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="eca66-133">threatAssessmentContentType</span></span>|<span data-ttu-id="eca66-134">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eca66-134">The content type of threat assessment.</span></span> <span data-ttu-id="eca66-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="eca66-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="eca66-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="eca66-136">createdBy</span></span>|[<span data-ttu-id="eca66-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="eca66-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="eca66-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eca66-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="eca66-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eca66-139">createdDateTime</span></span>|<span data-ttu-id="eca66-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca66-140">DateTimeOffset</span></span>|<span data-ttu-id="eca66-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eca66-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eca66-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eca66-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="eca66-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="eca66-143">expectedAssessment</span></span>|<span data-ttu-id="eca66-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="eca66-144">threatExpectedAssessment</span></span>|<span data-ttu-id="eca66-145">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="eca66-145">The expected assessment from submitter.</span></span> <span data-ttu-id="eca66-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="eca66-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="eca66-147">id</span><span class="sxs-lookup"><span data-stu-id="eca66-147">id</span></span>|<span data-ttu-id="eca66-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eca66-148">String</span></span>|<span data-ttu-id="eca66-149">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="eca66-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="eca66-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="eca66-150">requestSource</span></span>|<span data-ttu-id="eca66-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="eca66-151">threatAssessmentRequestSource</span></span>|<span data-ttu-id="eca66-152">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eca66-152">The source of the threat assessment request.</span></span> <span data-ttu-id="eca66-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="eca66-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="eca66-154">status</span><span class="sxs-lookup"><span data-stu-id="eca66-154">status</span></span>|<span data-ttu-id="eca66-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="eca66-155">threatAssessmentStatus</span></span>|<span data-ttu-id="eca66-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="eca66-156">The assessment process status.</span></span> <span data-ttu-id="eca66-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="eca66-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca66-158">Relações</span><span class="sxs-lookup"><span data-stu-id="eca66-158">Relationships</span></span>

| <span data-ttu-id="eca66-159">Relação</span><span class="sxs-lookup"><span data-stu-id="eca66-159">Relationship</span></span> | <span data-ttu-id="eca66-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="eca66-160">Type</span></span>        | <span data-ttu-id="eca66-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca66-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eca66-162">results</span><span class="sxs-lookup"><span data-stu-id="eca66-162">results</span></span>|<span data-ttu-id="eca66-163">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="eca66-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="eca66-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="eca66-164">A collection of threat assessment results.</span></span> <span data-ttu-id="eca66-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eca66-165">Read-only.</span></span> <span data-ttu-id="eca66-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="eca66-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eca66-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eca66-167">JSON representation</span></span>

<span data-ttu-id="eca66-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eca66-168">The following is a JSON representation of the resource.</span></span>

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


