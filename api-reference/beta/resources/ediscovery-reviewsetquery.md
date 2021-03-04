---
title: Tipo de recurso reviewSetQuery
description: Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em um eDiscovery reviewSet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f9c535cb1adbb62f33aee1324b6dc06a910f4b46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445897"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="2b1cc-103">Tipo de recurso reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="2b1cc-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b1cc-105">Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em uma revisão de descoberta [de eDiscoverySet](ediscovery-reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="2b1cc-105">Represents a review set query, which is used to query and cull data stored in an eDiscovery [reviewSet](ediscovery-reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2b1cc-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2b1cc-106">Methods</span></span>

| <span data-ttu-id="2b1cc-107">Método</span><span class="sxs-lookup"><span data-stu-id="2b1cc-107">Method</span></span>       | <span data-ttu-id="2b1cc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b1cc-108">Return Type</span></span> | <span data-ttu-id="2b1cc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b1cc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2b1cc-110">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="2b1cc-110">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md) | <span data-ttu-id="2b1cc-111">[coleção microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="2b1cc-111">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span> | <span data-ttu-id="2b1cc-112">Listar as consultas de conjunto de revisão em um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="2b1cc-113">Criar consultas</span><span class="sxs-lookup"><span data-stu-id="2b1cc-113">Create queries</span></span>](../api/ediscovery-reviewsetquery-post.md) | [<span data-ttu-id="2b1cc-114">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-114">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="2b1cc-115">Crie uma nova consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="2b1cc-116">Obter consultas</span><span class="sxs-lookup"><span data-stu-id="2b1cc-116">Get queries</span></span>](../api/ediscovery-reviewsetquery-get.md) | [<span data-ttu-id="2b1cc-117">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-117">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="2b1cc-118">Leia as propriedades e as relações de um **objeto reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="2b1cc-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="2b1cc-119">Atualizar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-119">Update reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-update.md) | <span data-ttu-id="2b1cc-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2b1cc-120">None</span></span> | <span data-ttu-id="2b1cc-121">Atualize uma consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-121">Update a review set query.</span></span> |
| [<span data-ttu-id="2b1cc-122">Excluir reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2b1cc-122">Delete reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-delete.md) | <span data-ttu-id="2b1cc-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2b1cc-123">None</span></span> | <span data-ttu-id="2b1cc-124">Excluir consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-124">Delete review set query.</span></span> |
| [<span data-ttu-id="2b1cc-125">applyTags</span><span class="sxs-lookup"><span data-stu-id="2b1cc-125">applyTags</span></span>](../api/ediscovery-reviewsetquery-applytags.md)|<span data-ttu-id="2b1cc-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2b1cc-126">None</span></span>|<span data-ttu-id="2b1cc-127">Aplique marcas a documentos que corresponderem à consulta especificada.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-127">Apply tags to documents that match the specified query.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b1cc-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b1cc-128">Properties</span></span>

| <span data-ttu-id="2b1cc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b1cc-129">Property</span></span>     | <span data-ttu-id="2b1cc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b1cc-130">Type</span></span>        | <span data-ttu-id="2b1cc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b1cc-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2b1cc-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="2b1cc-132">createdBy</span></span> | [<span data-ttu-id="2b1cc-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b1cc-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="2b1cc-134">O usuário que criou a consulta.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-134">The user who created the query.</span></span> |
| <span data-ttu-id="2b1cc-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1cc-135">createdDateTime</span></span> |<span data-ttu-id="2b1cc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1cc-136">DateTimeOffset</span></span>| <span data-ttu-id="2b1cc-137">A hora e a data em que a consulta foi criada.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-137">The time and date when the query was created.</span></span> <span data-ttu-id="2b1cc-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b1cc-139">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2b1cc-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="2b1cc-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2b1cc-140">displayName</span></span> | <span data-ttu-id="2b1cc-141">String</span><span class="sxs-lookup"><span data-stu-id="2b1cc-141">String</span></span> | <span data-ttu-id="2b1cc-142">O nome da consulta.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-142">The name of the query.</span></span>|
| <span data-ttu-id="2b1cc-143">id</span><span class="sxs-lookup"><span data-stu-id="2b1cc-143">id</span></span> |<span data-ttu-id="2b1cc-144">String</span><span class="sxs-lookup"><span data-stu-id="2b1cc-144">String</span></span>| <span data-ttu-id="2b1cc-145">O identificador exclusivo da consulta.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-145">The unique identifier of the query.</span></span> <span data-ttu-id="2b1cc-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-146">Read-only.</span></span>|
| <span data-ttu-id="2b1cc-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2b1cc-147">lastModifiedBy</span></span> | [<span data-ttu-id="2b1cc-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="2b1cc-148">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="2b1cc-149">O usuário que modificou a consulta pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-149">The user who last modified the query.</span></span> |
| <span data-ttu-id="2b1cc-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1cc-150">lastModifiedDateTime</span></span> |<span data-ttu-id="2b1cc-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1cc-151">DateTimeOffset</span></span> | <span data-ttu-id="2b1cc-152">A data e a hora em que a consulta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-152">The date and time the query was last modified.</span></span> <span data-ttu-id="2b1cc-153">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b1cc-154">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2b1cc-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="2b1cc-155">consulta</span><span class="sxs-lookup"><span data-stu-id="2b1cc-155">query</span></span> | <span data-ttu-id="2b1cc-156">String</span><span class="sxs-lookup"><span data-stu-id="2b1cc-156">String</span></span> | <span data-ttu-id="2b1cc-157">A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language).</span><span class="sxs-lookup"><span data-stu-id="2b1cc-157">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="2b1cc-158">Para obter detalhes, consulte [Campos de metadados de documento em Descoberta Avançada em eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="2b1cc-158">For details, see [Document metadata fields in Advanced eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="2b1cc-159">Este campo mapeia diretamente para a condição de palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-159">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="2b1cc-160">Você pode refinar pesquisas usando campos listados *no* nome de campo pesquisável emparelhados com valores; por exemplo, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-160">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b1cc-161">Relações</span><span class="sxs-lookup"><span data-stu-id="2b1cc-161">Relationships</span></span>

<span data-ttu-id="2b1cc-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b1cc-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b1cc-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b1cc-163">JSON representation</span></span>

<span data-ttu-id="2b1cc-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b1cc-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
