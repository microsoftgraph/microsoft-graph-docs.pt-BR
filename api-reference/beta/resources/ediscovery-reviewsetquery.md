---
title: Tipo de recurso reviewSetQuery
description: Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em um eDiscovery reviewSet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8eb674ed70eac47d4e29d127ebfc9f48b7b988a1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720314"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="ce33e-103">Tipo de recurso reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ce33e-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="ce33e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ce33e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce33e-105">Representa uma consulta de conjunto de revisão, que é usada para consultar e excluir dados armazenados em uma revisão de descoberta [de eDiscoverySet](ediscovery-reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="ce33e-105">Represents a review set query, which is used to query and cull data stored in an eDiscovery [reviewSet](ediscovery-reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ce33e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce33e-106">Methods</span></span>

| <span data-ttu-id="ce33e-107">Método</span><span class="sxs-lookup"><span data-stu-id="ce33e-107">Method</span></span>       | <span data-ttu-id="ce33e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce33e-108">Return Type</span></span> | <span data-ttu-id="ce33e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce33e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ce33e-110">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="ce33e-110">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md) | <span data-ttu-id="ce33e-111">[coleção microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="ce33e-111">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span> | <span data-ttu-id="ce33e-112">Listar as consultas de conjunto de revisão em um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="ce33e-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="ce33e-113">Criar consultas</span><span class="sxs-lookup"><span data-stu-id="ce33e-113">Create queries</span></span>](../api/ediscovery-reviewsetquery-post.md) | [<span data-ttu-id="ce33e-114">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ce33e-114">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="ce33e-115">Crie uma nova consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="ce33e-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="ce33e-116">Obter consultas</span><span class="sxs-lookup"><span data-stu-id="ce33e-116">Get queries</span></span>](../api/ediscovery-reviewsetquery-get.md) | [<span data-ttu-id="ce33e-117">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ce33e-117">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="ce33e-118">Leia as propriedades e as relações de um **objeto reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="ce33e-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="ce33e-119">Atualizar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ce33e-119">Update reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-update.md) | <span data-ttu-id="ce33e-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="ce33e-120">None</span></span> | <span data-ttu-id="ce33e-121">Atualize uma consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="ce33e-121">Update a review set query.</span></span> |
| [<span data-ttu-id="ce33e-122">Excluir reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="ce33e-122">Delete reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-delete.md) | <span data-ttu-id="ce33e-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="ce33e-123">None</span></span> | <span data-ttu-id="ce33e-124">Excluir consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="ce33e-124">Delete review set query.</span></span> |
| [<span data-ttu-id="ce33e-125">applyTags</span><span class="sxs-lookup"><span data-stu-id="ce33e-125">applyTags</span></span>](../api/ediscovery-reviewsetquery-applytags.md)|<span data-ttu-id="ce33e-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="ce33e-126">None</span></span>|<span data-ttu-id="ce33e-127">Aplique marcas a documentos que corresponderem à consulta especificada.</span><span class="sxs-lookup"><span data-stu-id="ce33e-127">Apply tags to documents that match the specified query.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce33e-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce33e-128">Properties</span></span>

| <span data-ttu-id="ce33e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce33e-129">Property</span></span>     | <span data-ttu-id="ce33e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce33e-130">Type</span></span>        | <span data-ttu-id="ce33e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce33e-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce33e-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="ce33e-132">createdBy</span></span> | [<span data-ttu-id="ce33e-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="ce33e-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="ce33e-134">O usuário que criou a consulta.</span><span class="sxs-lookup"><span data-stu-id="ce33e-134">The user who created the query.</span></span> |
| <span data-ttu-id="ce33e-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce33e-135">createdDateTime</span></span> |<span data-ttu-id="ce33e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce33e-136">DateTimeOffset</span></span>| <span data-ttu-id="ce33e-137">A hora e a data em que a consulta foi criada.</span><span class="sxs-lookup"><span data-stu-id="ce33e-137">The time and date when the query was created.</span></span> <span data-ttu-id="ce33e-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ce33e-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce33e-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ce33e-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
| <span data-ttu-id="ce33e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ce33e-140">displayName</span></span> | <span data-ttu-id="ce33e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce33e-141">String</span></span> | <span data-ttu-id="ce33e-142">O nome da consulta.</span><span class="sxs-lookup"><span data-stu-id="ce33e-142">The name of the query.</span></span>|
| <span data-ttu-id="ce33e-143">id</span><span class="sxs-lookup"><span data-stu-id="ce33e-143">id</span></span> |<span data-ttu-id="ce33e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce33e-144">String</span></span>| <span data-ttu-id="ce33e-145">O identificador exclusivo da consulta.</span><span class="sxs-lookup"><span data-stu-id="ce33e-145">The unique identifier of the query.</span></span> <span data-ttu-id="ce33e-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce33e-146">Read-only.</span></span>|
| <span data-ttu-id="ce33e-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ce33e-147">lastModifiedBy</span></span> | [<span data-ttu-id="ce33e-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="ce33e-148">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="ce33e-149">O usuário que modificou a consulta pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ce33e-149">The user who last modified the query.</span></span> |
| <span data-ttu-id="ce33e-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce33e-150">lastModifiedDateTime</span></span> |<span data-ttu-id="ce33e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce33e-151">DateTimeOffset</span></span> | <span data-ttu-id="ce33e-152">A data e a hora em que a consulta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ce33e-152">The date and time the query was last modified.</span></span> <span data-ttu-id="ce33e-153">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ce33e-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce33e-154">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ce33e-154">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
| <span data-ttu-id="ce33e-155">consulta</span><span class="sxs-lookup"><span data-stu-id="ce33e-155">query</span></span> | <span data-ttu-id="ce33e-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce33e-156">String</span></span> | <span data-ttu-id="ce33e-157">A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language).</span><span class="sxs-lookup"><span data-stu-id="ce33e-157">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="ce33e-158">Para obter detalhes, consulte [Campos de metadados de documento em Descoberta Avançada em eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="ce33e-158">For details, see [Document metadata fields in Advanced eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="ce33e-159">Este campo mapeia diretamente para a condição de palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="ce33e-159">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="ce33e-160">Você pode refinar pesquisas usando campos listados *no* nome de campo pesquisável emparelhados com valores; por exemplo, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span><span class="sxs-lookup"><span data-stu-id="ce33e-160">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce33e-161">Relações</span><span class="sxs-lookup"><span data-stu-id="ce33e-161">Relationships</span></span>

<span data-ttu-id="ce33e-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce33e-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce33e-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce33e-163">JSON representation</span></span>

<span data-ttu-id="ce33e-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce33e-164">The following is a JSON representation of the resource.</span></span>

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
