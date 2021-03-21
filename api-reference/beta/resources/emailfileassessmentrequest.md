---
title: Tipo de recurso emailFileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo de email.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 77c95b18056487f94a5cb75b946d0ee8f75e46f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960443"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="5c3a1-103">Tipo de recurso emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3a1-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="5c3a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c3a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c3a1-105">Usado para criar e recuperar uma avaliação de ameaça de arquivo de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="5c3a1-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="5c3a1-106">O arquivo de email pode ser um tipo de arquivo .eml.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="5c3a1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5c3a1-107">Methods</span></span>

| <span data-ttu-id="5c3a1-108">Método</span><span class="sxs-lookup"><span data-stu-id="5c3a1-108">Method</span></span>       | <span data-ttu-id="5c3a1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5c3a1-109">Return Type</span></span> | <span data-ttu-id="5c3a1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c3a1-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5c3a1-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3a1-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5c3a1-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3a1-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="5c3a1-113">Crie uma nova solicitação de avaliação de arquivo de email postando um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5c3a1-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="5c3a1-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3a1-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5c3a1-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3a1-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="5c3a1-116">Leia as propriedades e as relações de um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5c3a1-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c3a1-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c3a1-117">Properties</span></span>

| <span data-ttu-id="5c3a1-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c3a1-118">Property</span></span>     | <span data-ttu-id="5c3a1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c3a1-119">Type</span></span>        | <span data-ttu-id="5c3a1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c3a1-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c3a1-121">contentData</span><span class="sxs-lookup"><span data-stu-id="5c3a1-121">contentData</span></span>|<span data-ttu-id="5c3a1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c3a1-122">String</span></span>|<span data-ttu-id="5c3a1-123">Conteúdo de arquivo de email .eml codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="5c3a1-124">O conteúdo do arquivo não pode ser buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="5c3a1-125">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5c3a1-125">destinationRoutingReason</span></span>|[<span data-ttu-id="5c3a1-126">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5c3a1-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="5c3a1-127">O motivo do email roteado para seu destino.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="5c3a1-128">Os valores possíveis são: `none` , , , , , , , , , `mailFlowRule` , , `safeSender` , , , `blockedSender` `advancedSpamFiltering` `domainAllowList` , `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .</span><span class="sxs-lookup"><span data-stu-id="5c3a1-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="5c3a1-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="5c3a1-129">recipientEmail</span></span>|<span data-ttu-id="5c3a1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c3a1-130">String</span></span>|<span data-ttu-id="5c3a1-131">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="5c3a1-132">category</span><span class="sxs-lookup"><span data-stu-id="5c3a1-132">category</span></span>|[<span data-ttu-id="5c3a1-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="5c3a1-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5c3a1-134">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-134">The threat category.</span></span> <span data-ttu-id="5c3a1-135">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5c3a1-136">contentType</span><span class="sxs-lookup"><span data-stu-id="5c3a1-136">contentType</span></span>|[<span data-ttu-id="5c3a1-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="5c3a1-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5c3a1-138">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-138">The content type of threat assessment.</span></span> <span data-ttu-id="5c3a1-139">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5c3a1-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="5c3a1-140">createdBy</span></span>|[<span data-ttu-id="5c3a1-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="5c3a1-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="5c3a1-142">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5c3a1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c3a1-143">createdDateTime</span></span>|<span data-ttu-id="5c3a1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c3a1-144">DateTimeOffset</span></span>|<span data-ttu-id="5c3a1-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c3a1-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5c3a1-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5c3a1-147">expectedAssessment</span></span>|[<span data-ttu-id="5c3a1-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5c3a1-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5c3a1-149">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-149">The expected assessment from submitter.</span></span> <span data-ttu-id="5c3a1-150">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5c3a1-151">id</span><span class="sxs-lookup"><span data-stu-id="5c3a1-151">id</span></span>|<span data-ttu-id="5c3a1-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c3a1-152">String</span></span>|<span data-ttu-id="5c3a1-153">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="5c3a1-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5c3a1-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="5c3a1-154">requestSource</span></span>|[<span data-ttu-id="5c3a1-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="5c3a1-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5c3a1-156">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-156">The source of threat assessment request.</span></span> <span data-ttu-id="5c3a1-157">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5c3a1-158">status</span><span class="sxs-lookup"><span data-stu-id="5c3a1-158">status</span></span>|[<span data-ttu-id="5c3a1-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="5c3a1-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5c3a1-160">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-160">The assessment process status.</span></span> <span data-ttu-id="5c3a1-161">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c3a1-162">Relações</span><span class="sxs-lookup"><span data-stu-id="5c3a1-162">Relationships</span></span>

| <span data-ttu-id="5c3a1-163">Relação</span><span class="sxs-lookup"><span data-stu-id="5c3a1-163">Relationship</span></span> | <span data-ttu-id="5c3a1-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c3a1-164">Type</span></span>        | <span data-ttu-id="5c3a1-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c3a1-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c3a1-166">results</span><span class="sxs-lookup"><span data-stu-id="5c3a1-166">results</span></span>|<span data-ttu-id="5c3a1-167">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5c3a1-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5c3a1-168">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-168">A collection of threat assessment results.</span></span> <span data-ttu-id="5c3a1-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-169">Read-only.</span></span> <span data-ttu-id="5c3a1-170">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c3a1-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c3a1-171">JSON representation</span></span>

<span data-ttu-id="5c3a1-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c3a1-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String",
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
  "description": "emailFileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


