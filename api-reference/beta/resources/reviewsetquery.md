---
title: Tipo de recurso reviewSetQuery
description: As consultas de conjunto de revisão são usadas para consultar e excluir dados armazenados em um eDiscovery reviewSet
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f622f79c9103e704be93ffd97af37c1d188736f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153484"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="81219-103">Tipo de recurso reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="81219-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="81219-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81219-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81219-105">As consultas de conjunto de revisão são usadas para consultar e excluir dados armazenados em um eDiscovery [reviewSet](reviewset.md).</span><span class="sxs-lookup"><span data-stu-id="81219-105">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="81219-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="81219-106">Methods</span></span>

| <span data-ttu-id="81219-107">Método</span><span class="sxs-lookup"><span data-stu-id="81219-107">Method</span></span>       | <span data-ttu-id="81219-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81219-108">Return Type</span></span> | <span data-ttu-id="81219-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81219-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81219-110">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="81219-110">List queries</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="81219-111">[Coleção reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="81219-111">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="81219-112">Listar as consultas do conjunto de revisão em um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="81219-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="81219-113">Criar consultas</span><span class="sxs-lookup"><span data-stu-id="81219-113">Create queries</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="81219-114">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="81219-114">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="81219-115">Crie uma nova consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="81219-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="81219-116">Obter consultas</span><span class="sxs-lookup"><span data-stu-id="81219-116">Get queries</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="81219-117">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="81219-117">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="81219-118">Leia as propriedades e os relacionamentos de um **objeto reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="81219-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="81219-119">Atualizar consultas</span><span class="sxs-lookup"><span data-stu-id="81219-119">Update queries</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="81219-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="81219-120">None</span></span> | <span data-ttu-id="81219-121">Atualizar uma consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="81219-121">Update a review set query.</span></span> |
| [<span data-ttu-id="81219-122">Excluir consultas</span><span class="sxs-lookup"><span data-stu-id="81219-122">Delete queries</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="81219-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="81219-123">None</span></span> | <span data-ttu-id="81219-124">Exclua a consulta do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="81219-124">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="81219-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81219-125">Properties</span></span>

| <span data-ttu-id="81219-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81219-126">Property</span></span>     | <span data-ttu-id="81219-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="81219-127">Type</span></span>        | <span data-ttu-id="81219-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="81219-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="81219-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="81219-129">createdBy</span></span> | [<span data-ttu-id="81219-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="81219-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="81219-131">O usuário que criou a consulta.</span><span class="sxs-lookup"><span data-stu-id="81219-131">The user who created the query.</span></span> |
| <span data-ttu-id="81219-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81219-132">createdDateTime</span></span> |<span data-ttu-id="81219-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81219-133">DateTimeOffset</span></span>| <span data-ttu-id="81219-134">A hora e a data em que a consulta foi criada.</span><span class="sxs-lookup"><span data-stu-id="81219-134">The time and date when the query was created.</span></span> <span data-ttu-id="81219-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="81219-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81219-136">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="81219-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="81219-137">displayName</span><span class="sxs-lookup"><span data-stu-id="81219-137">displayName</span></span> | <span data-ttu-id="81219-138">String</span><span class="sxs-lookup"><span data-stu-id="81219-138">String</span></span> | <span data-ttu-id="81219-139">O nome da consulta</span><span class="sxs-lookup"><span data-stu-id="81219-139">The name of the query</span></span>|
| <span data-ttu-id="81219-140">id</span><span class="sxs-lookup"><span data-stu-id="81219-140">id</span></span> |<span data-ttu-id="81219-141">String</span><span class="sxs-lookup"><span data-stu-id="81219-141">String</span></span>| <span data-ttu-id="81219-142">O identificador exclusivo da consulta.</span><span class="sxs-lookup"><span data-stu-id="81219-142">The unique identifier of the query.</span></span> <span data-ttu-id="81219-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81219-143">Read-only.</span></span>|
| <span data-ttu-id="81219-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="81219-144">lastModifiedBy</span></span> | [<span data-ttu-id="81219-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="81219-145">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="81219-146">O usuário que modificou a consulta pela última vez.</span><span class="sxs-lookup"><span data-stu-id="81219-146">The user who last modified the query.</span></span> |
| <span data-ttu-id="81219-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81219-147">lastModifiedDateTime</span></span> |<span data-ttu-id="81219-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81219-148">DateTimeOffset</span></span> | <span data-ttu-id="81219-149">A data e a hora em que a consulta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="81219-149">The date and time the query was last modified.</span></span> <span data-ttu-id="81219-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="81219-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81219-151">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="81219-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="81219-152">consulta</span><span class="sxs-lookup"><span data-stu-id="81219-152">query</span></span> | <span data-ttu-id="81219-153">String</span><span class="sxs-lookup"><span data-stu-id="81219-153">String</span></span> | <span data-ttu-id="81219-154">A cadeia de caracteres de consulta na consulta KQL (Keyword Query Language).</span><span class="sxs-lookup"><span data-stu-id="81219-154">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="81219-155">Para obter detalhes, [consulte Os campos de metadados do documento na Descoberta Descoberta Avançada.](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="81219-155">For details, see [Document metadata fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="81219-156">Esse campo mapeia diretamente para a condição de palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="81219-156">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="81219-157">Você pode refinar pesquisas usando campos listados no nome do campo *pesquisável* emparelhados com valores; por exemplo, *assunto:"Finanças Trimestrais" E Data>=01/06/2016 E Data<=01/07/2016*</span><span class="sxs-lookup"><span data-stu-id="81219-157">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="81219-158">Relações</span><span class="sxs-lookup"><span data-stu-id="81219-158">Relationships</span></span>

<span data-ttu-id="81219-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81219-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81219-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81219-160">JSON representation</span></span>

<span data-ttu-id="81219-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81219-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
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
