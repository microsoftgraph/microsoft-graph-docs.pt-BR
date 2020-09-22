---
title: tipo de recurso fileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62c295899a230aab944dfbfd22249f945c6ae567
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076439"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="8ff32-103">tipo de recurso fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="8ff32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff32-105">Usado para criar e recuperar uma avaliação de ameaça de arquivo, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="8ff32-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="8ff32-106">O arquivo pode ser um arquivo de texto ou um documento do Word ou um arquivo binário recebido em um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="8ff32-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="8ff32-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ff32-107">Methods</span></span>

| <span data-ttu-id="8ff32-108">Método</span><span class="sxs-lookup"><span data-stu-id="8ff32-108">Method</span></span>       | <span data-ttu-id="8ff32-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ff32-109">Return Type</span></span> | <span data-ttu-id="8ff32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff32-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8ff32-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="8ff32-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="8ff32-113">Crie uma nova solicitação de avaliação de arquivo postando um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="8ff32-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="8ff32-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="8ff32-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="8ff32-116">Leia as propriedades e os relacionamentos de um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="8ff32-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ff32-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ff32-117">Properties</span></span>

| <span data-ttu-id="8ff32-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ff32-118">Property</span></span>     | <span data-ttu-id="8ff32-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff32-119">Type</span></span>        | <span data-ttu-id="8ff32-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff32-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ff32-121">contentData</span><span class="sxs-lookup"><span data-stu-id="8ff32-121">contentData</span></span>|<span data-ttu-id="8ff32-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff32-122">String</span></span>|<span data-ttu-id="8ff32-123">Conteúdo de arquivo codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="8ff32-123">Base64 encoded file content.</span></span> <span data-ttu-id="8ff32-124">O conteúdo do arquivo não pode buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="8ff32-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="8ff32-125">fileName</span><span class="sxs-lookup"><span data-stu-id="8ff32-125">fileName</span></span>|<span data-ttu-id="8ff32-126">String</span><span class="sxs-lookup"><span data-stu-id="8ff32-126">String</span></span>|<span data-ttu-id="8ff32-127">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8ff32-127">The file name.</span></span>|
|<span data-ttu-id="8ff32-128">category</span><span class="sxs-lookup"><span data-stu-id="8ff32-128">category</span></span>|[<span data-ttu-id="8ff32-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="8ff32-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="8ff32-130">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="8ff32-130">The threat category.</span></span> <span data-ttu-id="8ff32-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="8ff32-132">contentType</span><span class="sxs-lookup"><span data-stu-id="8ff32-132">contentType</span></span>|[<span data-ttu-id="8ff32-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="8ff32-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="8ff32-134">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="8ff32-134">The content type of threat assessment.</span></span> <span data-ttu-id="8ff32-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="8ff32-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="8ff32-136">createdBy</span></span>|[<span data-ttu-id="8ff32-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="8ff32-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="8ff32-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="8ff32-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="8ff32-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff32-139">createdDateTime</span></span>|<span data-ttu-id="8ff32-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff32-140">DateTimeOffset</span></span>|<span data-ttu-id="8ff32-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8ff32-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ff32-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8ff32-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="8ff32-143">expectedAssessment</span></span>|[<span data-ttu-id="8ff32-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="8ff32-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="8ff32-145">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="8ff32-145">The expected assessment from submitter.</span></span> <span data-ttu-id="8ff32-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="8ff32-147">id</span><span class="sxs-lookup"><span data-stu-id="8ff32-147">id</span></span>|<span data-ttu-id="8ff32-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff32-148">String</span></span>|<span data-ttu-id="8ff32-149">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="8ff32-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="8ff32-150">objectrequest</span><span class="sxs-lookup"><span data-stu-id="8ff32-150">requestSource</span></span>|[<span data-ttu-id="8ff32-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="8ff32-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="8ff32-152">A origem da solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="8ff32-152">The source of threat assessment request.</span></span> <span data-ttu-id="8ff32-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="8ff32-154">status</span><span class="sxs-lookup"><span data-stu-id="8ff32-154">status</span></span>|[<span data-ttu-id="8ff32-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="8ff32-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="8ff32-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="8ff32-156">The assessment process status.</span></span> <span data-ttu-id="8ff32-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="8ff32-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ff32-158">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="8ff32-158">Relationships</span></span>

| <span data-ttu-id="8ff32-159">Relação</span><span class="sxs-lookup"><span data-stu-id="8ff32-159">Relationship</span></span> | <span data-ttu-id="8ff32-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff32-160">Type</span></span>        | <span data-ttu-id="8ff32-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff32-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ff32-162">resultados</span><span class="sxs-lookup"><span data-stu-id="8ff32-162">results</span></span>|<span data-ttu-id="8ff32-163">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="8ff32-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="8ff32-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="8ff32-164">A collection of threat assessment results.</span></span> <span data-ttu-id="8ff32-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ff32-165">Read-only.</span></span> <span data-ttu-id="8ff32-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você a aplique `$expand` .</span><span class="sxs-lookup"><span data-stu-id="8ff32-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ff32-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ff32-167">JSON representation</span></span>

<span data-ttu-id="8ff32-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ff32-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "fileName": "String",
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
  "description": "fileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


