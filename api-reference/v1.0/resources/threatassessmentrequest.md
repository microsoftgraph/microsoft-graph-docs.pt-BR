---
title: tipo de recurso threatAssessmentRequest
description: Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 498698fc394c62ba296e5806cec27428312bd878
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591506"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="7f82c-103">tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="7f82c-104">Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="7f82c-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="7f82c-105">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="7f82c-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="7f82c-106">Email (recurso[mailAssessmentRequest](mailAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="7f82c-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="7f82c-107">Arquivo de email (recurso[emailFileAssessmentRequest](emailFileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="7f82c-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="7f82c-108">Arquivo (recurso[fileAssessmentRequest](fileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="7f82c-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="7f82c-109">URL (recurso[urlAssessmentRequest](urlAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="7f82c-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="7f82c-110">Methods</span><span class="sxs-lookup"><span data-stu-id="7f82c-110">Methods</span></span>

| <span data-ttu-id="7f82c-111">Método</span><span class="sxs-lookup"><span data-stu-id="7f82c-111">Method</span></span>       | <span data-ttu-id="7f82c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f82c-112">Return Type</span></span> | <span data-ttu-id="7f82c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f82c-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7f82c-114">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="7f82c-115">coleção [threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7f82c-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="7f82c-116">Listar todas as solicitações de avaliação de ameaça sob locatário.</span><span class="sxs-lookup"><span data-stu-id="7f82c-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="7f82c-117">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="7f82c-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="7f82c-119">Crie uma nova solicitação de avaliação de ameaça postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="7f82c-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="7f82c-120">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="7f82c-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="7f82c-122">Recupere as propriedades e os relacionamentos de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="7f82c-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="7f82c-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f82c-123">Properties</span></span>

| <span data-ttu-id="7f82c-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f82c-124">Property</span></span>     | <span data-ttu-id="7f82c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f82c-125">Type</span></span>        | <span data-ttu-id="7f82c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f82c-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="7f82c-127">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="7f82c-127">category</span></span>|[<span data-ttu-id="7f82c-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="7f82c-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="7f82c-129">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="7f82c-129">The threat category.</span></span> <span data-ttu-id="7f82c-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="7f82c-131">contentType</span><span class="sxs-lookup"><span data-stu-id="7f82c-131">contentType</span></span>|[<span data-ttu-id="7f82c-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="7f82c-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="7f82c-133">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="7f82c-133">The content type of threat assessment.</span></span> <span data-ttu-id="7f82c-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="7f82c-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="7f82c-135">createdBy</span></span>|[<span data-ttu-id="7f82c-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="7f82c-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="7f82c-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7f82c-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="7f82c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f82c-138">createdDateTime</span></span>|<span data-ttu-id="7f82c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f82c-139">DateTimeOffset</span></span>|<span data-ttu-id="7f82c-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7f82c-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f82c-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7f82c-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="7f82c-142">expectedAssessment</span></span>|[<span data-ttu-id="7f82c-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="7f82c-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="7f82c-144">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="7f82c-144">The expected assessment from submitter.</span></span> <span data-ttu-id="7f82c-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="7f82c-146">id</span><span class="sxs-lookup"><span data-stu-id="7f82c-146">id</span></span>|<span data-ttu-id="7f82c-147">String</span><span class="sxs-lookup"><span data-stu-id="7f82c-147">String</span></span>|<span data-ttu-id="7f82c-148">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="7f82c-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="7f82c-149">objectrequest</span><span class="sxs-lookup"><span data-stu-id="7f82c-149">requestSource</span></span>|[<span data-ttu-id="7f82c-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="7f82c-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="7f82c-151">A origem da solicitação de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="7f82c-151">The source of the threat assessment request.</span></span> <span data-ttu-id="7f82c-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="7f82c-153">status</span><span class="sxs-lookup"><span data-stu-id="7f82c-153">status</span></span>|[<span data-ttu-id="7f82c-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="7f82c-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="7f82c-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="7f82c-155">The assessment process status.</span></span> <span data-ttu-id="7f82c-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="7f82c-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f82c-157">Relações</span><span class="sxs-lookup"><span data-stu-id="7f82c-157">Relationships</span></span>

| <span data-ttu-id="7f82c-158">Relação</span><span class="sxs-lookup"><span data-stu-id="7f82c-158">Relationship</span></span> | <span data-ttu-id="7f82c-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f82c-159">Type</span></span>        | <span data-ttu-id="7f82c-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f82c-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f82c-161">resultados</span><span class="sxs-lookup"><span data-stu-id="7f82c-161">results</span></span>|<span data-ttu-id="7f82c-162">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="7f82c-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="7f82c-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7f82c-163">A collection of threat assessment results.</span></span> <span data-ttu-id="7f82c-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f82c-164">Read-only.</span></span> <span data-ttu-id="7f82c-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="7f82c-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f82c-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f82c-166">JSON representation</span></span>

<span data-ttu-id="7f82c-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f82c-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "",
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
