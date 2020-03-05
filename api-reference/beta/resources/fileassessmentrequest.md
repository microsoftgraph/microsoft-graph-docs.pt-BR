---
title: tipo de recurso fileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a7b0b4d83b68acf90aacf71c83169881a2ecdde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498328"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="078d4-103">tipo de recurso fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="078d4-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="078d4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="078d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078d4-105">Usado para criar e recuperar uma avaliação de ameaça de arquivo, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="078d4-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="078d4-106">O arquivo pode ser um arquivo de texto ou um documento do Word ou um arquivo binário recebido em um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="078d4-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="078d4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="078d4-107">Methods</span></span>

| <span data-ttu-id="078d4-108">Método</span><span class="sxs-lookup"><span data-stu-id="078d4-108">Method</span></span>       | <span data-ttu-id="078d4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="078d4-109">Return Type</span></span> | <span data-ttu-id="078d4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="078d4-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="078d4-111">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="078d4-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="078d4-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="078d4-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="078d4-113">Crie uma nova solicitação de avaliação de arquivo postando um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="078d4-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="078d4-114">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="078d4-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="078d4-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="078d4-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="078d4-116">Leia as propriedades e os relacionamentos de um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="078d4-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="078d4-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="078d4-117">Properties</span></span>

| <span data-ttu-id="078d4-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="078d4-118">Property</span></span>     | <span data-ttu-id="078d4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="078d4-119">Type</span></span>        | <span data-ttu-id="078d4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="078d4-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="078d4-121">contentData</span><span class="sxs-lookup"><span data-stu-id="078d4-121">contentData</span></span>|<span data-ttu-id="078d4-122">String</span><span class="sxs-lookup"><span data-stu-id="078d4-122">String</span></span>|<span data-ttu-id="078d4-123">Conteúdo de arquivo codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="078d4-123">Base64 encoded file content.</span></span> <span data-ttu-id="078d4-124">O conteúdo do arquivo não pode buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="078d4-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="078d4-125">fileName</span><span class="sxs-lookup"><span data-stu-id="078d4-125">fileName</span></span>|<span data-ttu-id="078d4-126">String</span><span class="sxs-lookup"><span data-stu-id="078d4-126">String</span></span>|<span data-ttu-id="078d4-127">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="078d4-127">The file name.</span></span>|
|<span data-ttu-id="078d4-128">category</span><span class="sxs-lookup"><span data-stu-id="078d4-128">category</span></span>|[<span data-ttu-id="078d4-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="078d4-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="078d4-130">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="078d4-130">The threat category.</span></span> <span data-ttu-id="078d4-131">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="078d4-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="078d4-132">contentType</span><span class="sxs-lookup"><span data-stu-id="078d4-132">contentType</span></span>|[<span data-ttu-id="078d4-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="078d4-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="078d4-134">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="078d4-134">The content type of threat assessment.</span></span> <span data-ttu-id="078d4-135">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="078d4-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="078d4-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="078d4-136">createdBy</span></span>|[<span data-ttu-id="078d4-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="078d4-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="078d4-138">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="078d4-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="078d4-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="078d4-139">createdDateTime</span></span>|<span data-ttu-id="078d4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="078d4-140">DateTimeOffset</span></span>|<span data-ttu-id="078d4-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="078d4-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="078d4-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="078d4-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="078d4-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="078d4-143">expectedAssessment</span></span>|[<span data-ttu-id="078d4-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="078d4-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="078d4-145">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="078d4-145">The expected assessment from submitter.</span></span> <span data-ttu-id="078d4-146">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="078d4-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="078d4-147">id</span><span class="sxs-lookup"><span data-stu-id="078d4-147">id</span></span>|<span data-ttu-id="078d4-148">String</span><span class="sxs-lookup"><span data-stu-id="078d4-148">String</span></span>|<span data-ttu-id="078d4-149">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="078d4-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="078d4-150">objectrequest</span><span class="sxs-lookup"><span data-stu-id="078d4-150">requestSource</span></span>|[<span data-ttu-id="078d4-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="078d4-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="078d4-152">A origem da solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="078d4-152">The source of threat assessment request.</span></span> <span data-ttu-id="078d4-153">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="078d4-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="078d4-154">status</span><span class="sxs-lookup"><span data-stu-id="078d4-154">status</span></span>|[<span data-ttu-id="078d4-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="078d4-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="078d4-156">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="078d4-156">The assessment process status.</span></span> <span data-ttu-id="078d4-157">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="078d4-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="078d4-158">Relações</span><span class="sxs-lookup"><span data-stu-id="078d4-158">Relationships</span></span>

| <span data-ttu-id="078d4-159">Relação</span><span class="sxs-lookup"><span data-stu-id="078d4-159">Relationship</span></span> | <span data-ttu-id="078d4-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="078d4-160">Type</span></span>        | <span data-ttu-id="078d4-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="078d4-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="078d4-162">resultados</span><span class="sxs-lookup"><span data-stu-id="078d4-162">results</span></span>|<span data-ttu-id="078d4-163">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="078d4-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="078d4-164">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="078d4-164">A collection of threat assessment results.</span></span> <span data-ttu-id="078d4-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="078d4-165">Read-only.</span></span> <span data-ttu-id="078d4-166">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="078d4-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="078d4-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="078d4-167">JSON representation</span></span>

<span data-ttu-id="078d4-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="078d4-168">The following is a JSON representation of the resource.</span></span>

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
