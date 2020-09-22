---
title: tipo de recurso reviewSetQuery
description: As consultas set de revisão são usadas para consultar e analisar dados armazenados em um revisor de descoberta eletrônica
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d03fae8340f9513e8fb6a26f409682e72b86842e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026219"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="644da-103">tipo de recurso reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="644da-103">reviewSetQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="644da-104">As consultas set de revisão são usadas para consultar e analisar os dados armazenados em um [revisor](reviewset.md)de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="644da-104">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="644da-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="644da-105">Methods</span></span>

| <span data-ttu-id="644da-106">Método</span><span class="sxs-lookup"><span data-stu-id="644da-106">Method</span></span>       | <span data-ttu-id="644da-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="644da-107">Return Type</span></span> | <span data-ttu-id="644da-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="644da-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="644da-109">List</span><span class="sxs-lookup"><span data-stu-id="644da-109">List</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="644da-110">coleção [reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="644da-110">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="644da-111">Listar as consultas de conjunto de revisão em um conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="644da-111">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="644da-112">Create</span><span class="sxs-lookup"><span data-stu-id="644da-112">Create</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="644da-113">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="644da-113">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="644da-114">Criar uma nova consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="644da-114">Create a new review set query.</span></span> |
| [<span data-ttu-id="644da-115">Get</span><span class="sxs-lookup"><span data-stu-id="644da-115">Get</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="644da-116">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="644da-116">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="644da-117">Leia as propriedades e os relacionamentos de um objeto **reviewSetQuery** .</span><span class="sxs-lookup"><span data-stu-id="644da-117">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="644da-118">Atualizar</span><span class="sxs-lookup"><span data-stu-id="644da-118">Update</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="644da-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="644da-119">None</span></span> | <span data-ttu-id="644da-120">Atualizar uma consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="644da-120">Update a review set query.</span></span> |
| [<span data-ttu-id="644da-121">Delete</span><span class="sxs-lookup"><span data-stu-id="644da-121">Delete</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="644da-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="644da-122">None</span></span> | <span data-ttu-id="644da-123">Excluir consulta de conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="644da-123">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="644da-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="644da-124">Properties</span></span>

| <span data-ttu-id="644da-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="644da-125">Property</span></span>     | <span data-ttu-id="644da-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="644da-126">Type</span></span>        | <span data-ttu-id="644da-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="644da-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="644da-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="644da-128">createdBy</span></span> | [<span data-ttu-id="644da-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="644da-129">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="644da-130">O usuário que criou a consulta.</span><span class="sxs-lookup"><span data-stu-id="644da-130">The user who created the query.</span></span> |
| <span data-ttu-id="644da-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="644da-131">createdDateTime</span></span> |<span data-ttu-id="644da-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644da-132">DateTimeOffset</span></span>| <span data-ttu-id="644da-133">A hora e a data em que a consulta foi criada.</span><span class="sxs-lookup"><span data-stu-id="644da-133">The time and date when the query was created.</span></span> <span data-ttu-id="644da-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="644da-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="644da-135">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="644da-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="644da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="644da-136">displayName</span></span> | <span data-ttu-id="644da-137">String</span><span class="sxs-lookup"><span data-stu-id="644da-137">String</span></span> | <span data-ttu-id="644da-138">O nome da consulta</span><span class="sxs-lookup"><span data-stu-id="644da-138">The name of the query</span></span>|
| <span data-ttu-id="644da-139">id</span><span class="sxs-lookup"><span data-stu-id="644da-139">id</span></span> |<span data-ttu-id="644da-140">String</span><span class="sxs-lookup"><span data-stu-id="644da-140">String</span></span>| <span data-ttu-id="644da-141">O identificador exclusivo da consulta.</span><span class="sxs-lookup"><span data-stu-id="644da-141">The unique identifier of the query.</span></span> <span data-ttu-id="644da-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="644da-142">Read-only.</span></span>|
| <span data-ttu-id="644da-143">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="644da-143">lastModifiedBy</span></span> | [<span data-ttu-id="644da-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="644da-144">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="644da-145">O usuário que modificou a consulta pela última vez.</span><span class="sxs-lookup"><span data-stu-id="644da-145">The user who last modified the query.</span></span> |
| <span data-ttu-id="644da-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="644da-146">lastModifiedDateTime</span></span> |<span data-ttu-id="644da-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644da-147">DateTimeOffset</span></span> | <span data-ttu-id="644da-148">A data e a hora em que a consulta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="644da-148">The date and time the query was last modified.</span></span> <span data-ttu-id="644da-149">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="644da-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="644da-150">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="644da-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="644da-151">consulta</span><span class="sxs-lookup"><span data-stu-id="644da-151">query</span></span> | <span data-ttu-id="644da-152">String</span><span class="sxs-lookup"><span data-stu-id="644da-152">String</span></span> | <span data-ttu-id="644da-153">A cadeia de caracteres de consulta na consulta KQL (linguagem de consulta de palavra-chave).</span><span class="sxs-lookup"><span data-stu-id="644da-153">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="644da-154">Consulte para https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="644da-154">Please refer to https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery for more details.</span></span>  <span data-ttu-id="644da-155">Este campo é mapeado diretamente para a condição de palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="644da-155">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="644da-156">Você pode refinar pesquisas usando campos listados no *nome de campo pesquisável* emparelhado com valores, por exemplo, *Subject: "Financials trimestrais" e date>= 06/01/2016 e date<= 07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="644da-156">You can refine searches by using fields listed in the *searchable field name* paired with values, e.g. *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="644da-157">Relações</span><span class="sxs-lookup"><span data-stu-id="644da-157">Relationships</span></span>

<span data-ttu-id="644da-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="644da-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="644da-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="644da-159">JSON representation</span></span>

<span data-ttu-id="644da-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="644da-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
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


