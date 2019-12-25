---
title: tipo de recurso threatAssessmentRequest
description: Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8441fe14434733efda10c51d88e0750904ee1246
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867136"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="26d4e-103">tipo de recurso threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-103">threatAssessmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d4e-104">Um tipo de recurso abstrato usado para representar um item de solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="26d4e-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="26d4e-105">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="26d4e-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="26d4e-106">Email (recurso[mailAssessmentRequest](mailAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="26d4e-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="26d4e-107">Arquivo de email (recurso[emailFileAssessmentRequest](emailFileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="26d4e-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="26d4e-108">Arquivo (recurso[fileAssessmentRequest](fileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="26d4e-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="26d4e-109">URL (recurso[urlAssessmentRequest](urlAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="26d4e-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="26d4e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="26d4e-110">Methods</span></span>

| <span data-ttu-id="26d4e-111">Método</span><span class="sxs-lookup"><span data-stu-id="26d4e-111">Method</span></span>       | <span data-ttu-id="26d4e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26d4e-112">Return Type</span></span> | <span data-ttu-id="26d4e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d4e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="26d4e-114">Listar threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="26d4e-115">coleção [threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="26d4e-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="26d4e-116">Listar todas as solicitações de avaliação de ameaça sob locatário.</span><span class="sxs-lookup"><span data-stu-id="26d4e-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="26d4e-117">Criar threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="26d4e-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="26d4e-119">Crie uma nova solicitação de avaliação de ameaça postando um tipo de recurso derivado: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="26d4e-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="26d4e-120">Obter threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="26d4e-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="26d4e-122">Recupere as propriedades e os relacionamentos de um recurso **threatAssessmentRequest** especificado.</span><span class="sxs-lookup"><span data-stu-id="26d4e-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="26d4e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26d4e-123">Properties</span></span>

| <span data-ttu-id="26d4e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26d4e-124">Property</span></span>     | <span data-ttu-id="26d4e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="26d4e-125">Type</span></span>        | <span data-ttu-id="26d4e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d4e-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="26d4e-127">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="26d4e-127">category</span></span>|[<span data-ttu-id="26d4e-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="26d4e-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="26d4e-129">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="26d4e-129">The threat category.</span></span> <span data-ttu-id="26d4e-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="26d4e-131">contentType</span><span class="sxs-lookup"><span data-stu-id="26d4e-131">contentType</span></span>|[<span data-ttu-id="26d4e-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="26d4e-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="26d4e-133">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="26d4e-133">The content type of threat assessment.</span></span> <span data-ttu-id="26d4e-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="26d4e-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="26d4e-135">createdBy</span></span>|[<span data-ttu-id="26d4e-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="26d4e-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="26d4e-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="26d4e-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="26d4e-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26d4e-138">createdDateTime</span></span>|<span data-ttu-id="26d4e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d4e-139">DateTimeOffset</span></span>|<span data-ttu-id="26d4e-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="26d4e-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="26d4e-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="26d4e-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="26d4e-142">expectedAssessment</span></span>|[<span data-ttu-id="26d4e-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="26d4e-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="26d4e-144">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="26d4e-144">The expected assessment from submitter.</span></span> <span data-ttu-id="26d4e-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="26d4e-146">id</span><span class="sxs-lookup"><span data-stu-id="26d4e-146">id</span></span>|<span data-ttu-id="26d4e-147">String</span><span class="sxs-lookup"><span data-stu-id="26d4e-147">String</span></span>|<span data-ttu-id="26d4e-148">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="26d4e-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="26d4e-149">objectrequest</span><span class="sxs-lookup"><span data-stu-id="26d4e-149">requestSource</span></span>|[<span data-ttu-id="26d4e-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="26d4e-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="26d4e-151">A origem da solicitação de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="26d4e-151">The source of the threat assessment request.</span></span> <span data-ttu-id="26d4e-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="26d4e-153">status</span><span class="sxs-lookup"><span data-stu-id="26d4e-153">status</span></span>|[<span data-ttu-id="26d4e-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="26d4e-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="26d4e-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="26d4e-155">The assessment process status.</span></span> <span data-ttu-id="26d4e-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="26d4e-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26d4e-157">Relações</span><span class="sxs-lookup"><span data-stu-id="26d4e-157">Relationships</span></span>

| <span data-ttu-id="26d4e-158">Relação</span><span class="sxs-lookup"><span data-stu-id="26d4e-158">Relationship</span></span> | <span data-ttu-id="26d4e-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="26d4e-159">Type</span></span>        | <span data-ttu-id="26d4e-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d4e-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26d4e-161">resultados</span><span class="sxs-lookup"><span data-stu-id="26d4e-161">results</span></span>|<span data-ttu-id="26d4e-162">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="26d4e-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="26d4e-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="26d4e-163">A collection of threat assessment results.</span></span> <span data-ttu-id="26d4e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26d4e-164">Read-only.</span></span> <span data-ttu-id="26d4e-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="26d4e-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26d4e-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26d4e-166">JSON representation</span></span>

<span data-ttu-id="26d4e-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26d4e-167">The following is a JSON representation of the resource.</span></span>

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
