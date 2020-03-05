---
title: tipo de recurso threatAssessmentRequest
description: Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1a6a8f0f1448522d624b9c9e97bb2fab426b6988
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519775"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="b58c0-103">tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="b58c0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b58c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58c0-105">Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="b58c0-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="b58c0-106">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="b58c0-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="b58c0-107">Email (recurso[mailAssessmentRequest](mailAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="b58c0-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="b58c0-108">Arquivo de email (recurso[emailFileAssessmentRequest](emailFileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="b58c0-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="b58c0-109">Arquivo (recurso[fileAssessmentRequest](fileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="b58c0-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="b58c0-110">URL (recurso[urlAssessmentRequest](urlAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="b58c0-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="b58c0-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="b58c0-111">Methods</span></span>

| <span data-ttu-id="b58c0-112">Método</span><span class="sxs-lookup"><span data-stu-id="b58c0-112">Method</span></span>       | <span data-ttu-id="b58c0-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b58c0-113">Return Type</span></span> | <span data-ttu-id="b58c0-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b58c0-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b58c0-115">List threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="b58c0-116">coleção [threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b58c0-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="b58c0-117">Listar todas as solicitações de avaliação de ameaça sob locatário.</span><span class="sxs-lookup"><span data-stu-id="b58c0-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="b58c0-118">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="b58c0-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="b58c0-120">Crie uma nova solicitação de avaliação de ameaça postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="b58c0-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="b58c0-121">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="b58c0-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="b58c0-123">Recupere as propriedades e os relacionamentos de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="b58c0-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="b58c0-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b58c0-124">Properties</span></span>

| <span data-ttu-id="b58c0-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b58c0-125">Property</span></span>     | <span data-ttu-id="b58c0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b58c0-126">Type</span></span>        | <span data-ttu-id="b58c0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b58c0-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="b58c0-128">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="b58c0-128">category</span></span>|[<span data-ttu-id="b58c0-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="b58c0-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="b58c0-130">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="b58c0-130">The threat category.</span></span> <span data-ttu-id="b58c0-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="b58c0-132">contentType</span><span class="sxs-lookup"><span data-stu-id="b58c0-132">contentType</span></span>|[<span data-ttu-id="b58c0-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="b58c0-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="b58c0-134">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="b58c0-134">The content type of threat assessment.</span></span> <span data-ttu-id="b58c0-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="b58c0-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="b58c0-136">createdBy</span></span>|[<span data-ttu-id="b58c0-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="b58c0-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="b58c0-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="b58c0-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="b58c0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b58c0-139">createdDateTime</span></span>|<span data-ttu-id="b58c0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b58c0-140">DateTimeOffset</span></span>|<span data-ttu-id="b58c0-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b58c0-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b58c0-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b58c0-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="b58c0-143">expectedAssessment</span></span>|[<span data-ttu-id="b58c0-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="b58c0-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="b58c0-145">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="b58c0-145">The expected assessment from submitter.</span></span> <span data-ttu-id="b58c0-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="b58c0-147">id</span><span class="sxs-lookup"><span data-stu-id="b58c0-147">id</span></span>|<span data-ttu-id="b58c0-148">String</span><span class="sxs-lookup"><span data-stu-id="b58c0-148">String</span></span>|<span data-ttu-id="b58c0-149">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="b58c0-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="b58c0-150">objectrequest</span><span class="sxs-lookup"><span data-stu-id="b58c0-150">requestSource</span></span>|[<span data-ttu-id="b58c0-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="b58c0-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="b58c0-152">A origem da solicitação de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="b58c0-152">The source of the threat assessment request.</span></span> <span data-ttu-id="b58c0-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="b58c0-154">status</span><span class="sxs-lookup"><span data-stu-id="b58c0-154">status</span></span>|[<span data-ttu-id="b58c0-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="b58c0-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="b58c0-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="b58c0-156">The assessment process status.</span></span> <span data-ttu-id="b58c0-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="b58c0-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b58c0-158">Relações</span><span class="sxs-lookup"><span data-stu-id="b58c0-158">Relationships</span></span>

| <span data-ttu-id="b58c0-159">Relação</span><span class="sxs-lookup"><span data-stu-id="b58c0-159">Relationship</span></span> | <span data-ttu-id="b58c0-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="b58c0-160">Type</span></span>        | <span data-ttu-id="b58c0-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="b58c0-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b58c0-162">resultados</span><span class="sxs-lookup"><span data-stu-id="b58c0-162">results</span></span>|<span data-ttu-id="b58c0-163">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="b58c0-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="b58c0-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="b58c0-164">A collection of threat assessment results.</span></span> <span data-ttu-id="b58c0-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b58c0-165">Read-only.</span></span> <span data-ttu-id="b58c0-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="b58c0-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b58c0-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b58c0-167">JSON representation</span></span>

<span data-ttu-id="b58c0-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b58c0-168">The following is a JSON representation of the resource.</span></span>

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
