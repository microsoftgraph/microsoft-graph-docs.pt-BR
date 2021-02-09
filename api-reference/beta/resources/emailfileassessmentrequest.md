---
title: Tipo de recurso emailFileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaças de arquivo de email.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1aa31301c4283d1adf6bfeb352eeaea7474823a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159136"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="2b819-103">Tipo de recurso emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2b819-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="2b819-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b819-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b819-105">Usado para criar e recuperar uma avaliação de ameaça de arquivo de email, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="2b819-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="2b819-106">O arquivo de email pode ser um tipo de arquivo .eml.</span><span class="sxs-lookup"><span data-stu-id="2b819-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="2b819-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b819-107">Methods</span></span>

| <span data-ttu-id="2b819-108">Método</span><span class="sxs-lookup"><span data-stu-id="2b819-108">Method</span></span>       | <span data-ttu-id="2b819-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b819-109">Return Type</span></span> | <span data-ttu-id="2b819-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b819-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2b819-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2b819-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="2b819-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2b819-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="2b819-113">Crie uma nova solicitação de avaliação de arquivo de email postando um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="2b819-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="2b819-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2b819-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="2b819-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2b819-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="2b819-116">Leia as propriedades e os relacionamentos de um **objeto emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="2b819-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b819-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b819-117">Properties</span></span>

| <span data-ttu-id="2b819-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b819-118">Property</span></span>     | <span data-ttu-id="2b819-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b819-119">Type</span></span>        | <span data-ttu-id="2b819-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b819-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b819-121">contentData</span><span class="sxs-lookup"><span data-stu-id="2b819-121">contentData</span></span>|<span data-ttu-id="2b819-122">String</span><span class="sxs-lookup"><span data-stu-id="2b819-122">String</span></span>|<span data-ttu-id="2b819-123">Conteúdo do arquivo de email .eml codificado em Base64.</span><span class="sxs-lookup"><span data-stu-id="2b819-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="2b819-124">O conteúdo do arquivo não pode ser buscado de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="2b819-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="2b819-125">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2b819-125">destinationRoutingReason</span></span>|[<span data-ttu-id="2b819-126">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2b819-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="2b819-127">O motivo do email roteado para seu destino.</span><span class="sxs-lookup"><span data-stu-id="2b819-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="2b819-128">Os valores possíveis `none` são: `mailFlowRule` , , , , , , , , `safeSender` , , `blockedSender` , , , `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` .</span><span class="sxs-lookup"><span data-stu-id="2b819-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="2b819-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="2b819-129">recipientEmail</span></span>|<span data-ttu-id="2b819-130">String</span><span class="sxs-lookup"><span data-stu-id="2b819-130">String</span></span>|<span data-ttu-id="2b819-131">O destinatário de email cujas políticas são usadas para avaliar o email.</span><span class="sxs-lookup"><span data-stu-id="2b819-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="2b819-132">category</span><span class="sxs-lookup"><span data-stu-id="2b819-132">category</span></span>|[<span data-ttu-id="2b819-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="2b819-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="2b819-134">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="2b819-134">The threat category.</span></span> <span data-ttu-id="2b819-135">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="2b819-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="2b819-136">contentType</span><span class="sxs-lookup"><span data-stu-id="2b819-136">contentType</span></span>|[<span data-ttu-id="2b819-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="2b819-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="2b819-138">O tipo de conteúdo de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2b819-138">The content type of threat assessment.</span></span> <span data-ttu-id="2b819-139">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="2b819-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="2b819-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="2b819-140">createdBy</span></span>|[<span data-ttu-id="2b819-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b819-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="2b819-142">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2b819-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="2b819-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b819-143">createdDateTime</span></span>|<span data-ttu-id="2b819-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b819-144">DateTimeOffset</span></span>|<span data-ttu-id="2b819-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2b819-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b819-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2b819-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2b819-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2b819-147">expectedAssessment</span></span>|[<span data-ttu-id="2b819-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2b819-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="2b819-149">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="2b819-149">The expected assessment from submitter.</span></span> <span data-ttu-id="2b819-150">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="2b819-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="2b819-151">id</span><span class="sxs-lookup"><span data-stu-id="2b819-151">id</span></span>|<span data-ttu-id="2b819-152">String</span><span class="sxs-lookup"><span data-stu-id="2b819-152">String</span></span>|<span data-ttu-id="2b819-153">A ID da solicitação de avaliação de ameaças é um IDENTIFICADOr global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="2b819-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="2b819-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="2b819-154">requestSource</span></span>|[<span data-ttu-id="2b819-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="2b819-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="2b819-156">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2b819-156">The source of threat assessment request.</span></span> <span data-ttu-id="2b819-157">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="2b819-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="2b819-158">status</span><span class="sxs-lookup"><span data-stu-id="2b819-158">status</span></span>|[<span data-ttu-id="2b819-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="2b819-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="2b819-160">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="2b819-160">The assessment process status.</span></span> <span data-ttu-id="2b819-161">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="2b819-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b819-162">Relações</span><span class="sxs-lookup"><span data-stu-id="2b819-162">Relationships</span></span>

| <span data-ttu-id="2b819-163">Relação</span><span class="sxs-lookup"><span data-stu-id="2b819-163">Relationship</span></span> | <span data-ttu-id="2b819-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b819-164">Type</span></span>        | <span data-ttu-id="2b819-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b819-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b819-166">resultados</span><span class="sxs-lookup"><span data-stu-id="2b819-166">results</span></span>|<span data-ttu-id="2b819-167">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="2b819-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="2b819-168">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2b819-168">A collection of threat assessment results.</span></span> <span data-ttu-id="2b819-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b819-169">Read-only.</span></span> <span data-ttu-id="2b819-170">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você aplique `$expand` a ele.</span><span class="sxs-lookup"><span data-stu-id="2b819-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b819-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b819-171">JSON representation</span></span>

<span data-ttu-id="2b819-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b819-172">The following is a JSON representation of the resource.</span></span>

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


