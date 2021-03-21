---
title: Tipo de recurso mailAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de email.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3e45cddeb7d0a9814a1feb6732828ef7363602bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961269"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="cb57e-103">Tipo de recurso mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cb57e-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="cb57e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb57e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb57e-105">Usado para criar e recuperar uma avaliação de ameaça de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="cb57e-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="cb57e-106">Quando você cria uma solicitação de avaliação de ameaça de email, o email deve ser recebido pelo usuário especificado em `recipientEmail` .</span><span class="sxs-lookup"><span data-stu-id="cb57e-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="cb57e-107">As permissões [de email delegadas](/graph/permissions-reference#mail-permissions) (Mail.Read ou Mail.Read.Shared) são requriadas para acessar o email recebido pelo usuário ou compartilhado por outra pessoa.</span><span class="sxs-lookup"><span data-stu-id="cb57e-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="cb57e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb57e-108">Methods</span></span>

| <span data-ttu-id="cb57e-109">Método</span><span class="sxs-lookup"><span data-stu-id="cb57e-109">Method</span></span>       | <span data-ttu-id="cb57e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb57e-110">Return Type</span></span> | <span data-ttu-id="cb57e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb57e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb57e-112">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cb57e-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="cb57e-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cb57e-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="cb57e-114">Crie uma nova solicitação de avaliação de email postando um **objeto mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="cb57e-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="cb57e-115">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cb57e-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="cb57e-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cb57e-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="cb57e-117">Leia as propriedades e as relações de um **objeto mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="cb57e-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="cb57e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb57e-118">Properties</span></span>

| <span data-ttu-id="cb57e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb57e-119">Property</span></span>     | <span data-ttu-id="cb57e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb57e-120">Type</span></span>        | <span data-ttu-id="cb57e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb57e-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb57e-122">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="cb57e-122">destinationRoutingReason</span></span>|[<span data-ttu-id="cb57e-123">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="cb57e-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="cb57e-124">O motivo do email roteado para seu destino.</span><span class="sxs-lookup"><span data-stu-id="cb57e-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="cb57e-125">Os valores possíveis são: `none` , , , , , , , , , `mailFlowRule` , , `safeSender` , , , `blockedSender` `advancedSpamFiltering` `domainAllowList` , `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .</span><span class="sxs-lookup"><span data-stu-id="cb57e-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="cb57e-126">messageUri</span><span class="sxs-lookup"><span data-stu-id="cb57e-126">messageUri</span></span>|<span data-ttu-id="cb57e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb57e-127">String</span></span>|<span data-ttu-id="cb57e-128">O URI de recurso da mensagem de email para avaliação.</span><span class="sxs-lookup"><span data-stu-id="cb57e-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="cb57e-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="cb57e-129">recipientEmail</span></span>|<span data-ttu-id="cb57e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb57e-130">String</span></span>|<span data-ttu-id="cb57e-131">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="cb57e-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="cb57e-132">category</span><span class="sxs-lookup"><span data-stu-id="cb57e-132">category</span></span>|[<span data-ttu-id="cb57e-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="cb57e-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="cb57e-134">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="cb57e-134">The threat category.</span></span> <span data-ttu-id="cb57e-135">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="cb57e-136">contentType</span><span class="sxs-lookup"><span data-stu-id="cb57e-136">contentType</span></span>|[<span data-ttu-id="cb57e-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="cb57e-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="cb57e-138">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="cb57e-138">The content type of threat assessment.</span></span> <span data-ttu-id="cb57e-139">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="cb57e-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="cb57e-140">createdBy</span></span>|[<span data-ttu-id="cb57e-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="cb57e-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="cb57e-142">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="cb57e-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="cb57e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb57e-143">createdDateTime</span></span>|<span data-ttu-id="cb57e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb57e-144">DateTimeOffset</span></span>|<span data-ttu-id="cb57e-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cb57e-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cb57e-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="cb57e-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="cb57e-147">expectedAssessment</span></span>|[<span data-ttu-id="cb57e-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="cb57e-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="cb57e-149">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="cb57e-149">The expected assessment from submitter.</span></span> <span data-ttu-id="cb57e-150">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="cb57e-151">id</span><span class="sxs-lookup"><span data-stu-id="cb57e-151">id</span></span>|<span data-ttu-id="cb57e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb57e-152">String</span></span>|<span data-ttu-id="cb57e-153">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="cb57e-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="cb57e-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="cb57e-154">requestSource</span></span>|[<span data-ttu-id="cb57e-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="cb57e-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="cb57e-156">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="cb57e-156">The source of threat assessment request.</span></span> <span data-ttu-id="cb57e-157">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="cb57e-158">status</span><span class="sxs-lookup"><span data-stu-id="cb57e-158">status</span></span>|[<span data-ttu-id="cb57e-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="cb57e-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="cb57e-160">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="cb57e-160">The assessment process status.</span></span> <span data-ttu-id="cb57e-161">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="cb57e-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb57e-162">Relações</span><span class="sxs-lookup"><span data-stu-id="cb57e-162">Relationships</span></span>

| <span data-ttu-id="cb57e-163">Relação</span><span class="sxs-lookup"><span data-stu-id="cb57e-163">Relationship</span></span> | <span data-ttu-id="cb57e-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb57e-164">Type</span></span>        | <span data-ttu-id="cb57e-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb57e-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb57e-166">results</span><span class="sxs-lookup"><span data-stu-id="cb57e-166">results</span></span>|<span data-ttu-id="cb57e-167">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb57e-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="cb57e-168">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="cb57e-168">A collection of threat assessment results.</span></span> <span data-ttu-id="cb57e-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb57e-169">Read-only.</span></span> <span data-ttu-id="cb57e-170">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="cb57e-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb57e-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb57e-171">JSON representation</span></span>

<span data-ttu-id="cb57e-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb57e-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
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


