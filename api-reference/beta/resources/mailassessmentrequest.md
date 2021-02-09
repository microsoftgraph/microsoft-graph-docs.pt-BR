---
title: Tipo de recurso mailAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaças de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ea2a227b414317942b0c0ea48109f0056543a60
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161417"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="03835-103">Tipo de recurso mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="03835-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="03835-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03835-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03835-105">Usado para criar e recuperar uma avaliação de ameaças de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="03835-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="03835-106">Quando você cria uma solicitação de avaliação de ameaça de email, o email deve ser recebido pelo usuário especificado em `recipientEmail` .</span><span class="sxs-lookup"><span data-stu-id="03835-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="03835-107">Permissões de [email delegadas](/graph/permissions-reference#mail-permissions) (Mail.Read ou Mail.Read.Shared) são requriadas para acessar o email recebido pelo usuário ou compartilhado por outra pessoa.</span><span class="sxs-lookup"><span data-stu-id="03835-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="03835-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="03835-108">Methods</span></span>

| <span data-ttu-id="03835-109">Método</span><span class="sxs-lookup"><span data-stu-id="03835-109">Method</span></span>       | <span data-ttu-id="03835-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03835-110">Return Type</span></span> | <span data-ttu-id="03835-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="03835-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="03835-112">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="03835-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="03835-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="03835-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="03835-114">Crie uma nova solicitação de avaliação de email postando um **objeto mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="03835-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="03835-115">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="03835-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="03835-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="03835-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="03835-117">Leia as propriedades e os relacionamentos de um **objeto mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="03835-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="03835-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03835-118">Properties</span></span>

| <span data-ttu-id="03835-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03835-119">Property</span></span>     | <span data-ttu-id="03835-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="03835-120">Type</span></span>        | <span data-ttu-id="03835-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="03835-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03835-122">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="03835-122">destinationRoutingReason</span></span>|[<span data-ttu-id="03835-123">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="03835-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="03835-124">O motivo do email roteado para seu destino.</span><span class="sxs-lookup"><span data-stu-id="03835-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="03835-125">Os valores possíveis `none` são: `mailFlowRule` , , , , , , , , `safeSender` , , `blockedSender` , , , `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .</span><span class="sxs-lookup"><span data-stu-id="03835-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="03835-126">messageUri</span><span class="sxs-lookup"><span data-stu-id="03835-126">messageUri</span></span>|<span data-ttu-id="03835-127">String</span><span class="sxs-lookup"><span data-stu-id="03835-127">String</span></span>|<span data-ttu-id="03835-128">O URI do recurso da mensagem de email para avaliação.</span><span class="sxs-lookup"><span data-stu-id="03835-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="03835-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="03835-129">recipientEmail</span></span>|<span data-ttu-id="03835-130">String</span><span class="sxs-lookup"><span data-stu-id="03835-130">String</span></span>|<span data-ttu-id="03835-131">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="03835-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="03835-132">category</span><span class="sxs-lookup"><span data-stu-id="03835-132">category</span></span>|[<span data-ttu-id="03835-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="03835-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="03835-134">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="03835-134">The threat category.</span></span> <span data-ttu-id="03835-135">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="03835-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="03835-136">contentType</span><span class="sxs-lookup"><span data-stu-id="03835-136">contentType</span></span>|[<span data-ttu-id="03835-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="03835-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="03835-138">O tipo de conteúdo de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="03835-138">The content type of threat assessment.</span></span> <span data-ttu-id="03835-139">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="03835-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="03835-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="03835-140">createdBy</span></span>|[<span data-ttu-id="03835-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="03835-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="03835-142">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="03835-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="03835-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03835-143">createdDateTime</span></span>|<span data-ttu-id="03835-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03835-144">DateTimeOffset</span></span>|<span data-ttu-id="03835-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="03835-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03835-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03835-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="03835-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="03835-147">expectedAssessment</span></span>|[<span data-ttu-id="03835-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="03835-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="03835-149">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="03835-149">The expected assessment from submitter.</span></span> <span data-ttu-id="03835-150">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="03835-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="03835-151">id</span><span class="sxs-lookup"><span data-stu-id="03835-151">id</span></span>|<span data-ttu-id="03835-152">String</span><span class="sxs-lookup"><span data-stu-id="03835-152">String</span></span>|<span data-ttu-id="03835-153">A ID da solicitação de avaliação de ameaças é um IDENTIFICADOr global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="03835-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="03835-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="03835-154">requestSource</span></span>|[<span data-ttu-id="03835-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="03835-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="03835-156">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="03835-156">The source of threat assessment request.</span></span> <span data-ttu-id="03835-157">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="03835-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="03835-158">status</span><span class="sxs-lookup"><span data-stu-id="03835-158">status</span></span>|[<span data-ttu-id="03835-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="03835-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="03835-160">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="03835-160">The assessment process status.</span></span> <span data-ttu-id="03835-161">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="03835-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03835-162">Relações</span><span class="sxs-lookup"><span data-stu-id="03835-162">Relationships</span></span>

| <span data-ttu-id="03835-163">Relação</span><span class="sxs-lookup"><span data-stu-id="03835-163">Relationship</span></span> | <span data-ttu-id="03835-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="03835-164">Type</span></span>        | <span data-ttu-id="03835-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="03835-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03835-166">resultados</span><span class="sxs-lookup"><span data-stu-id="03835-166">results</span></span>|<span data-ttu-id="03835-167">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="03835-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="03835-168">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="03835-168">A collection of threat assessment results.</span></span> <span data-ttu-id="03835-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03835-169">Read-only.</span></span> <span data-ttu-id="03835-170">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você aplique `$expand` a ele.</span><span class="sxs-lookup"><span data-stu-id="03835-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03835-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03835-171">JSON representation</span></span>

<span data-ttu-id="03835-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03835-172">The following is a JSON representation of the resource.</span></span>

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


