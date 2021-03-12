---
title: Tipo de recurso emailFileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 956097a95016ce24d0935dea7f770476499052f2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721989"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="7904f-103">Tipo de recurso emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7904f-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="7904f-104">Usado para criar e recuperar uma avaliação de ameaça de arquivo de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="7904f-104">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="7904f-105">O arquivo de email pode ser um tipo de arquivo .eml.</span><span class="sxs-lookup"><span data-stu-id="7904f-105">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="7904f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="7904f-106">Methods</span></span>

| <span data-ttu-id="7904f-107">Método</span><span class="sxs-lookup"><span data-stu-id="7904f-107">Method</span></span>       | <span data-ttu-id="7904f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7904f-108">Return Type</span></span> | <span data-ttu-id="7904f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7904f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7904f-110">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7904f-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="7904f-111">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7904f-111">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="7904f-112">Crie uma nova solicitação de avaliação de arquivo de email postando um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="7904f-112">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="7904f-113">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7904f-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="7904f-114">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7904f-114">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="7904f-115">Leia as propriedades e as relações de um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="7904f-115">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7904f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7904f-116">Properties</span></span>

| <span data-ttu-id="7904f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7904f-117">Property</span></span>     | <span data-ttu-id="7904f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="7904f-118">Type</span></span>        | <span data-ttu-id="7904f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7904f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7904f-120">contentData</span><span class="sxs-lookup"><span data-stu-id="7904f-120">contentData</span></span>|<span data-ttu-id="7904f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7904f-121">String</span></span>|<span data-ttu-id="7904f-122">Conteúdo de arquivo de email .eml codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="7904f-122">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="7904f-123">O conteúdo do arquivo não pode ser buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="7904f-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="7904f-124">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="7904f-124">destinationRoutingReason</span></span>|[<span data-ttu-id="7904f-125">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="7904f-125">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="7904f-126">O motivo do email roteado para seu destino.</span><span class="sxs-lookup"><span data-stu-id="7904f-126">The reason for mail routed to its destination.</span></span> <span data-ttu-id="7904f-127">Os valores possíveis são: `none` , , , , , , , , , `mailFlowRule` , , `safeSender` , , , `blockedSender` `advancedSpamFiltering` `domainAllowList` , `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .</span><span class="sxs-lookup"><span data-stu-id="7904f-127">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="7904f-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="7904f-128">recipientEmail</span></span>|<span data-ttu-id="7904f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7904f-129">String</span></span>|<span data-ttu-id="7904f-130">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="7904f-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="7904f-131">category</span><span class="sxs-lookup"><span data-stu-id="7904f-131">category</span></span>|[<span data-ttu-id="7904f-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="7904f-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="7904f-133">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="7904f-133">The threat category.</span></span> <span data-ttu-id="7904f-134">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="7904f-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="7904f-135">contentType</span><span class="sxs-lookup"><span data-stu-id="7904f-135">contentType</span></span>|[<span data-ttu-id="7904f-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="7904f-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="7904f-137">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7904f-137">The content type of threat assessment.</span></span> <span data-ttu-id="7904f-138">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="7904f-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="7904f-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="7904f-139">createdBy</span></span>|[<span data-ttu-id="7904f-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="7904f-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="7904f-141">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7904f-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="7904f-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7904f-142">createdDateTime</span></span>|<span data-ttu-id="7904f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7904f-143">DateTimeOffset</span></span>|<span data-ttu-id="7904f-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7904f-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7904f-145">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7904f-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="7904f-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="7904f-146">expectedAssessment</span></span>|[<span data-ttu-id="7904f-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="7904f-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="7904f-148">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="7904f-148">The expected assessment from submitter.</span></span> <span data-ttu-id="7904f-149">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="7904f-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="7904f-150">id</span><span class="sxs-lookup"><span data-stu-id="7904f-150">id</span></span>|<span data-ttu-id="7904f-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7904f-151">String</span></span>|<span data-ttu-id="7904f-152">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="7904f-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="7904f-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="7904f-153">requestSource</span></span>|[<span data-ttu-id="7904f-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="7904f-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="7904f-155">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7904f-155">The source of threat assessment request.</span></span> <span data-ttu-id="7904f-156">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="7904f-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="7904f-157">status</span><span class="sxs-lookup"><span data-stu-id="7904f-157">status</span></span>|[<span data-ttu-id="7904f-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="7904f-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="7904f-159">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="7904f-159">The assessment process status.</span></span> <span data-ttu-id="7904f-160">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="7904f-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7904f-161">Relações</span><span class="sxs-lookup"><span data-stu-id="7904f-161">Relationships</span></span>

| <span data-ttu-id="7904f-162">Relação</span><span class="sxs-lookup"><span data-stu-id="7904f-162">Relationship</span></span> | <span data-ttu-id="7904f-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="7904f-163">Type</span></span>        | <span data-ttu-id="7904f-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="7904f-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7904f-165">results</span><span class="sxs-lookup"><span data-stu-id="7904f-165">results</span></span>|<span data-ttu-id="7904f-166">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="7904f-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="7904f-167">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="7904f-167">A collection of threat assessment results.</span></span> <span data-ttu-id="7904f-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7904f-168">Read-only.</span></span> <span data-ttu-id="7904f-169">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="7904f-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7904f-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7904f-170">JSON representation</span></span>

<span data-ttu-id="7904f-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7904f-171">The following is a JSON representation of the resource.</span></span>

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

