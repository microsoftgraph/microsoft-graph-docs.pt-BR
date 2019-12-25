---
title: tipo de recurso fileAssessmentRequest
description: Usado para criar e recuperar uma avaliação de ameaça de arquivo.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 24bad37d6b01ed4fd7901890bfd8692da8f8a51e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867140"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="2c1a0-103">tipo de recurso fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-103">fileAssessmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c1a0-104">Usado para criar e recuperar uma avaliação de ameaça de arquivo, derivada de [threatAssessmentRequest](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="2c1a0-104">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="2c1a0-105">O arquivo pode ser um arquivo de texto ou um documento do Word ou um arquivo binário recebido em um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-105">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="2c1a0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c1a0-106">Methods</span></span>

| <span data-ttu-id="2c1a0-107">Método</span><span class="sxs-lookup"><span data-stu-id="2c1a0-107">Method</span></span>       | <span data-ttu-id="2c1a0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c1a0-108">Return Type</span></span> | <span data-ttu-id="2c1a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1a0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2c1a0-110">Criar threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="2c1a0-111">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-111">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="2c1a0-112">Crie uma nova solicitação de avaliação de arquivo postando um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="2c1a0-112">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="2c1a0-113">Obter threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="2c1a0-114">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-114">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="2c1a0-115">Leia as propriedades e os relacionamentos de um objeto **fileAssessmentRequest** .</span><span class="sxs-lookup"><span data-stu-id="2c1a0-115">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c1a0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c1a0-116">Properties</span></span>

| <span data-ttu-id="2c1a0-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c1a0-117">Property</span></span>     | <span data-ttu-id="2c1a0-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c1a0-118">Type</span></span>        | <span data-ttu-id="2c1a0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1a0-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c1a0-120">contentData</span><span class="sxs-lookup"><span data-stu-id="2c1a0-120">contentData</span></span>|<span data-ttu-id="2c1a0-121">String</span><span class="sxs-lookup"><span data-stu-id="2c1a0-121">String</span></span>|<span data-ttu-id="2c1a0-122">Conteúdo de arquivo codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-122">Base64 encoded file content.</span></span> <span data-ttu-id="2c1a0-123">O conteúdo do arquivo não pode buscar de volta porque não está armazenado.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="2c1a0-124">fileName</span><span class="sxs-lookup"><span data-stu-id="2c1a0-124">fileName</span></span>|<span data-ttu-id="2c1a0-125">String</span><span class="sxs-lookup"><span data-stu-id="2c1a0-125">String</span></span>|<span data-ttu-id="2c1a0-126">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-126">The file name.</span></span>|
|<span data-ttu-id="2c1a0-127">category</span><span class="sxs-lookup"><span data-stu-id="2c1a0-127">category</span></span>|[<span data-ttu-id="2c1a0-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="2c1a0-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="2c1a0-129">A categoria da ameaça.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-129">The threat category.</span></span> <span data-ttu-id="2c1a0-130">Os valores possíveis são: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="2c1a0-131">contentType</span><span class="sxs-lookup"><span data-stu-id="2c1a0-131">contentType</span></span>|[<span data-ttu-id="2c1a0-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="2c1a0-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="2c1a0-133">O tipo de conteúdo de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-133">The content type of threat assessment.</span></span> <span data-ttu-id="2c1a0-134">Os valores possíveis são: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="2c1a0-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="2c1a0-135">createdBy</span></span>|[<span data-ttu-id="2c1a0-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c1a0-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="2c1a0-137">O criador da solicitação de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="2c1a0-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c1a0-138">createdDateTime</span></span>|<span data-ttu-id="2c1a0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c1a0-139">DateTimeOffset</span></span>|<span data-ttu-id="2c1a0-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c1a0-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2c1a0-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2c1a0-142">expectedAssessment</span></span>|[<span data-ttu-id="2c1a0-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2c1a0-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="2c1a0-144">A avaliação esperada do emissor.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-144">The expected assessment from submitter.</span></span> <span data-ttu-id="2c1a0-145">Os valores possíveis são: `block` e `unblock`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="2c1a0-146">id</span><span class="sxs-lookup"><span data-stu-id="2c1a0-146">id</span></span>|<span data-ttu-id="2c1a0-147">String</span><span class="sxs-lookup"><span data-stu-id="2c1a0-147">String</span></span>|<span data-ttu-id="2c1a0-148">A ID da solicitação de avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="2c1a0-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="2c1a0-149">objectrequest</span><span class="sxs-lookup"><span data-stu-id="2c1a0-149">requestSource</span></span>|[<span data-ttu-id="2c1a0-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="2c1a0-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="2c1a0-151">A origem da solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-151">The source of threat assessment request.</span></span> <span data-ttu-id="2c1a0-152">Os valores possíveis são: `user` e `administrator`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="2c1a0-153">status</span><span class="sxs-lookup"><span data-stu-id="2c1a0-153">status</span></span>|[<span data-ttu-id="2c1a0-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="2c1a0-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="2c1a0-155">O status do processo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-155">The assessment process status.</span></span> <span data-ttu-id="2c1a0-156">Os valores possíveis são: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c1a0-157">Relações</span><span class="sxs-lookup"><span data-stu-id="2c1a0-157">Relationships</span></span>

| <span data-ttu-id="2c1a0-158">Relação</span><span class="sxs-lookup"><span data-stu-id="2c1a0-158">Relationship</span></span> | <span data-ttu-id="2c1a0-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c1a0-159">Type</span></span>        | <span data-ttu-id="2c1a0-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1a0-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c1a0-161">resultados</span><span class="sxs-lookup"><span data-stu-id="2c1a0-161">results</span></span>|<span data-ttu-id="2c1a0-162">coleção [threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="2c1a0-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="2c1a0-163">Uma coleção de resultados de avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-163">A collection of threat assessment results.</span></span> <span data-ttu-id="2c1a0-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-164">Read-only.</span></span> <span data-ttu-id="2c1a0-165">Por padrão, um `GET /threatAssessmentRequests/{id}` não retorna essa propriedade, a menos que `$expand` você a aplique.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c1a0-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c1a0-166">JSON representation</span></span>

<span data-ttu-id="2c1a0-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c1a0-167">The following is a JSON representation of the resource.</span></span>

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
