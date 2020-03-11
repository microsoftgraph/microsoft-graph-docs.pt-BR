---
title: tipo de recurso mailAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bfd9dbcb7084759350161c947a1ba4759ca0e185
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591471"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="36013-103">tipo de recurso mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="36013-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="36013-104">Usado para criar e recuperar uma avaliação de ameaça de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="36013-104">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="36013-105">Quando você cria uma solicitação de avaliação de ameaça de email, os emails devem ser recebidos pelo `recipientEmail`usuário especificado em.</span><span class="sxs-lookup"><span data-stu-id="36013-105">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="36013-106">Permissões de [email](/graph/permissions-reference#mail-permissions) delegadas (mail. Read ou mail. Read. Shared) são requried para acessar as mensagens recebidas pelo usuário ou compartilhadas por outra pessoa.</span><span class="sxs-lookup"><span data-stu-id="36013-106">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="36013-107">Methods</span><span class="sxs-lookup"><span data-stu-id="36013-107">Methods</span></span>

| <span data-ttu-id="36013-108">Método</span><span class="sxs-lookup"><span data-stu-id="36013-108">Method</span></span>       | <span data-ttu-id="36013-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36013-109">Return Type</span></span> | <span data-ttu-id="36013-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="36013-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="36013-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="36013-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="36013-112">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="36013-112">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="36013-113">Crie uma nova solicitação de avaliação de email postando um objeto **mailAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="36013-113">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="36013-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="36013-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="36013-115">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="36013-115">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="36013-116">Leia as propriedades e os relacionamentos de um objeto **mailAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="36013-116">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="36013-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36013-117">Properties</span></span>

| <span data-ttu-id="36013-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36013-118">Property</span></span>     | <span data-ttu-id="36013-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="36013-119">Type</span></span>        | <span data-ttu-id="36013-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="36013-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36013-121">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="36013-121">destinationRoutingReason</span></span>|[<span data-ttu-id="36013-122">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="36013-122">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="36013-123">A razão para emails roteados para seu destino.</span><span class="sxs-lookup"><span data-stu-id="36013-123">The reason for mail routed to its destination.</span></span> <span data-ttu-id="36013-124">Os valores possíveis são `none`: `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span><span class="sxs-lookup"><span data-stu-id="36013-124">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="36013-125">messageUri</span><span class="sxs-lookup"><span data-stu-id="36013-125">messageUri</span></span>|<span data-ttu-id="36013-126">String</span><span class="sxs-lookup"><span data-stu-id="36013-126">String</span></span>|<span data-ttu-id="36013-127">O URI do recurso da mensagem de email para avaliação.</span><span class="sxs-lookup"><span data-stu-id="36013-127">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="36013-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="36013-128">recipientEmail</span></span>|<span data-ttu-id="36013-129">String</span><span class="sxs-lookup"><span data-stu-id="36013-129">String</span></span>|<span data-ttu-id="36013-130">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="36013-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="36013-131">category</span><span class="sxs-lookup"><span data-stu-id="36013-131">category</span></span>|[<span data-ttu-id="36013-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="36013-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="36013-133">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="36013-133">The threat category.</span></span> <span data-ttu-id="36013-134">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="36013-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="36013-135">contentType</span><span class="sxs-lookup"><span data-stu-id="36013-135">contentType</span></span>|[<span data-ttu-id="36013-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="36013-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="36013-137">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="36013-137">The content type of threat assessment.</span></span> <span data-ttu-id="36013-138">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="36013-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="36013-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="36013-139">createdBy</span></span>|[<span data-ttu-id="36013-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="36013-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="36013-141">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="36013-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="36013-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36013-142">createdDateTime</span></span>|<span data-ttu-id="36013-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36013-143">DateTimeOffset</span></span>|<span data-ttu-id="36013-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="36013-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="36013-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="36013-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="36013-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="36013-146">expectedAssessment</span></span>|[<span data-ttu-id="36013-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="36013-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="36013-148">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="36013-148">The expected assessment from submitter.</span></span> <span data-ttu-id="36013-149">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="36013-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="36013-150">id</span><span class="sxs-lookup"><span data-stu-id="36013-150">id</span></span>|<span data-ttu-id="36013-151">String</span><span class="sxs-lookup"><span data-stu-id="36013-151">String</span></span>|<span data-ttu-id="36013-152">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="36013-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="36013-153">objectrequest</span><span class="sxs-lookup"><span data-stu-id="36013-153">requestSource</span></span>|[<span data-ttu-id="36013-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="36013-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="36013-155">A origem da solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="36013-155">The source of threat assessment request.</span></span> <span data-ttu-id="36013-156">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="36013-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="36013-157">status</span><span class="sxs-lookup"><span data-stu-id="36013-157">status</span></span>|[<span data-ttu-id="36013-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="36013-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="36013-159">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="36013-159">The assessment process status.</span></span> <span data-ttu-id="36013-160">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="36013-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36013-161">Relações</span><span class="sxs-lookup"><span data-stu-id="36013-161">Relationships</span></span>

| <span data-ttu-id="36013-162">Relação</span><span class="sxs-lookup"><span data-stu-id="36013-162">Relationship</span></span> | <span data-ttu-id="36013-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="36013-163">Type</span></span>        | <span data-ttu-id="36013-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="36013-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36013-165">resultados</span><span class="sxs-lookup"><span data-stu-id="36013-165">results</span></span>|<span data-ttu-id="36013-166">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="36013-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="36013-167">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="36013-167">A collection of threat assessment results.</span></span> <span data-ttu-id="36013-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36013-168">Read-only.</span></span> <span data-ttu-id="36013-169">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="36013-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36013-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36013-170">JSON representation</span></span>

<span data-ttu-id="36013-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36013-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
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
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
