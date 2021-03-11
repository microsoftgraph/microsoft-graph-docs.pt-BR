---
title: Tipo de recurso fileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ce0280eb465474dab26658c9d31bfc90e368ff21
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722150"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="3965b-103">Tipo de recurso fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3965b-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="3965b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3965b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3965b-105">Usado para criar e recuperar uma avaliação de ameaça de arquivo, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="3965b-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="3965b-106">O arquivo pode ser um arquivo de texto ou documento do Word ou arquivo binário recebido em um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="3965b-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="3965b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3965b-107">Methods</span></span>

| <span data-ttu-id="3965b-108">Método</span><span class="sxs-lookup"><span data-stu-id="3965b-108">Method</span></span>       | <span data-ttu-id="3965b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3965b-109">Return Type</span></span> | <span data-ttu-id="3965b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3965b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3965b-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3965b-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="3965b-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3965b-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="3965b-113">Crie uma nova solicitação de avaliação de arquivo postando um **objeto fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="3965b-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="3965b-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3965b-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="3965b-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3965b-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="3965b-116">Leia as propriedades e as relações de um **objeto fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="3965b-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3965b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3965b-117">Properties</span></span>

| <span data-ttu-id="3965b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3965b-118">Property</span></span>     | <span data-ttu-id="3965b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3965b-119">Type</span></span>        | <span data-ttu-id="3965b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3965b-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3965b-121">contentData</span><span class="sxs-lookup"><span data-stu-id="3965b-121">contentData</span></span>|<span data-ttu-id="3965b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3965b-122">String</span></span>|<span data-ttu-id="3965b-123">Conteúdo de arquivo codificado base64.</span><span class="sxs-lookup"><span data-stu-id="3965b-123">Base64 encoded file content.</span></span> <span data-ttu-id="3965b-124">O conteúdo do arquivo não pode ser buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="3965b-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="3965b-125">fileName</span><span class="sxs-lookup"><span data-stu-id="3965b-125">fileName</span></span>|<span data-ttu-id="3965b-126">String</span><span class="sxs-lookup"><span data-stu-id="3965b-126">String</span></span>|<span data-ttu-id="3965b-127">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3965b-127">The file name.</span></span>|
|<span data-ttu-id="3965b-128">category</span><span class="sxs-lookup"><span data-stu-id="3965b-128">category</span></span>|[<span data-ttu-id="3965b-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="3965b-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="3965b-130">A categoria de ameaça.</span><span class="sxs-lookup"><span data-stu-id="3965b-130">The threat category.</span></span> <span data-ttu-id="3965b-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="3965b-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="3965b-132">contentType</span><span class="sxs-lookup"><span data-stu-id="3965b-132">contentType</span></span>|[<span data-ttu-id="3965b-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="3965b-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="3965b-134">O tipo de conteúdo da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="3965b-134">The content type of threat assessment.</span></span> <span data-ttu-id="3965b-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="3965b-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="3965b-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="3965b-136">createdBy</span></span>|[<span data-ttu-id="3965b-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="3965b-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="3965b-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="3965b-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="3965b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3965b-139">createdDateTime</span></span>|<span data-ttu-id="3965b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3965b-140">DateTimeOffset</span></span>|<span data-ttu-id="3965b-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3965b-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3965b-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3965b-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="3965b-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="3965b-143">expectedAssessment</span></span>|[<span data-ttu-id="3965b-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="3965b-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="3965b-145">A avaliação esperada do enviador.</span><span class="sxs-lookup"><span data-stu-id="3965b-145">The expected assessment from submitter.</span></span> <span data-ttu-id="3965b-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="3965b-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="3965b-147">id</span><span class="sxs-lookup"><span data-stu-id="3965b-147">id</span></span>|<span data-ttu-id="3965b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3965b-148">String</span></span>|<span data-ttu-id="3965b-149">A ID da solicitação de avaliação de ameaça é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="3965b-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="3965b-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="3965b-150">requestSource</span></span>|[<span data-ttu-id="3965b-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="3965b-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="3965b-152">A origem da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="3965b-152">The source of threat assessment request.</span></span> <span data-ttu-id="3965b-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="3965b-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="3965b-154">status</span><span class="sxs-lookup"><span data-stu-id="3965b-154">status</span></span>|[<span data-ttu-id="3965b-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="3965b-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="3965b-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="3965b-156">The assessment process status.</span></span> <span data-ttu-id="3965b-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="3965b-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3965b-158">Relações</span><span class="sxs-lookup"><span data-stu-id="3965b-158">Relationships</span></span>

| <span data-ttu-id="3965b-159">Relação</span><span class="sxs-lookup"><span data-stu-id="3965b-159">Relationship</span></span> | <span data-ttu-id="3965b-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="3965b-160">Type</span></span>        | <span data-ttu-id="3965b-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="3965b-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3965b-162">results</span><span class="sxs-lookup"><span data-stu-id="3965b-162">results</span></span>|<span data-ttu-id="3965b-163">[Coleção threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="3965b-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="3965b-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="3965b-164">A collection of threat assessment results.</span></span> <span data-ttu-id="3965b-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3965b-165">Read-only.</span></span> <span data-ttu-id="3965b-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que você `$expand` se aplique a ela.</span><span class="sxs-lookup"><span data-stu-id="3965b-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3965b-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3965b-167">JSON representation</span></span>

<span data-ttu-id="3965b-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3965b-168">The following is a JSON representation of the resource.</span></span>

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


