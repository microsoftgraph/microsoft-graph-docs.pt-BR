---
title: Tipo de recurso fileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c08a520f28adb470f6c92b037bad967714a9a593
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722444"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="e927f-103">Tipo de recurso fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e927f-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="e927f-104">Usado para criar e recuperar uma avaliação de ameaça de arquivo, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="e927f-104">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="e927f-105">O arquivo pode ser um arquivo de texto ou documento do Word ou arquivo binário recebido em um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="e927f-105">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="e927f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e927f-106">Methods</span></span>

| <span data-ttu-id="e927f-107">Método</span><span class="sxs-lookup"><span data-stu-id="e927f-107">Method</span></span>       | <span data-ttu-id="e927f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e927f-108">Return Type</span></span> | <span data-ttu-id="e927f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e927f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e927f-110">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e927f-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="e927f-111">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e927f-111">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="e927f-112">Crie uma nova solicitação de avaliação de arquivo postando um **objeto fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="e927f-112">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="e927f-113">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e927f-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="e927f-114">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e927f-114">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="e927f-115">Leia as propriedades e as relações de um **objeto fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="e927f-115">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e927f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e927f-116">Properties</span></span>

| <span data-ttu-id="e927f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e927f-117">Property</span></span>     | <span data-ttu-id="e927f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e927f-118">Type</span></span>        | <span data-ttu-id="e927f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e927f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e927f-120">contentData</span><span class="sxs-lookup"><span data-stu-id="e927f-120">contentData</span></span>|<span data-ttu-id="e927f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e927f-121">String</span></span>|<span data-ttu-id="e927f-122">Conteúdo de arquivo codificado base64.</span><span class="sxs-lookup"><span data-stu-id="e927f-122">Base64 encoded file content.</span></span> <span data-ttu-id="e927f-123">O conteúdo do arquivo não pode ser buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="e927f-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="e927f-124">fileName</span><span class="sxs-lookup"><span data-stu-id="e927f-124">fileName</span></span>|<span data-ttu-id="e927f-125">String</span><span class="sxs-lookup"><span data-stu-id="e927f-125">String</span></span>|<span data-ttu-id="e927f-126">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e927f-126">The file name.</span></span>|
|<span data-ttu-id="e927f-127">category</span><span class="sxs-lookup"><span data-stu-id="e927f-127">category</span></span>|[<span data-ttu-id="e927f-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="e927f-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="e927f-129">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="e927f-129">The threat category.</span></span> <span data-ttu-id="e927f-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="e927f-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="e927f-131">contentType</span><span class="sxs-lookup"><span data-stu-id="e927f-131">contentType</span></span>|[<span data-ttu-id="e927f-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="e927f-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="e927f-133">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="e927f-133">The content type of threat assessment.</span></span> <span data-ttu-id="e927f-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="e927f-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="e927f-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="e927f-135">createdBy</span></span>|[<span data-ttu-id="e927f-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="e927f-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="e927f-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="e927f-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="e927f-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e927f-138">createdDateTime</span></span>|<span data-ttu-id="e927f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e927f-139">DateTimeOffset</span></span>|<span data-ttu-id="e927f-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e927f-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e927f-141">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e927f-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e927f-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e927f-142">expectedAssessment</span></span>|[<span data-ttu-id="e927f-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e927f-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="e927f-144">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="e927f-144">The expected assessment from submitter.</span></span> <span data-ttu-id="e927f-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="e927f-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="e927f-146">id</span><span class="sxs-lookup"><span data-stu-id="e927f-146">id</span></span>|<span data-ttu-id="e927f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e927f-147">String</span></span>|<span data-ttu-id="e927f-148">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="e927f-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e927f-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="e927f-149">requestSource</span></span>|[<span data-ttu-id="e927f-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="e927f-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="e927f-151">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="e927f-151">The source of threat assessment request.</span></span> <span data-ttu-id="e927f-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e927f-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="e927f-153">status</span><span class="sxs-lookup"><span data-stu-id="e927f-153">status</span></span>|[<span data-ttu-id="e927f-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="e927f-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="e927f-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="e927f-155">The assessment process status.</span></span> <span data-ttu-id="e927f-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="e927f-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e927f-157">Relações</span><span class="sxs-lookup"><span data-stu-id="e927f-157">Relationships</span></span>

| <span data-ttu-id="e927f-158">Relação</span><span class="sxs-lookup"><span data-stu-id="e927f-158">Relationship</span></span> | <span data-ttu-id="e927f-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="e927f-159">Type</span></span>        | <span data-ttu-id="e927f-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="e927f-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e927f-161">results</span><span class="sxs-lookup"><span data-stu-id="e927f-161">results</span></span>|<span data-ttu-id="e927f-162">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="e927f-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="e927f-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="e927f-163">A collection of threat assessment results.</span></span> <span data-ttu-id="e927f-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e927f-164">Read-only.</span></span> <span data-ttu-id="e927f-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="e927f-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e927f-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e927f-166">JSON representation</span></span>

<span data-ttu-id="e927f-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e927f-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
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

