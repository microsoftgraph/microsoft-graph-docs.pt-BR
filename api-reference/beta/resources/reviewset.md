---
title: tipo de recurso reviewset
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 76e63c5aece7f7254afa282469a1dc8ce664217f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026229"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="c16ba-103">tipo de recurso reviewset</span><span class="sxs-lookup"><span data-stu-id="c16ba-103">reviewSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c16ba-104">Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.</span><span class="sxs-lookup"><span data-stu-id="c16ba-104">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="c16ba-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c16ba-105">Methods</span></span>

| <span data-ttu-id="c16ba-106">Método</span><span class="sxs-lookup"><span data-stu-id="c16ba-106">Method</span></span>       | <span data-ttu-id="c16ba-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c16ba-107">Return Type</span></span> | <span data-ttu-id="c16ba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16ba-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c16ba-109">List</span><span class="sxs-lookup"><span data-stu-id="c16ba-109">List</span></span>](../api/reviewset-list.md) | <span data-ttu-id="c16ba-110">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="c16ba-110">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="c16ba-111">Obter uma coleção de conjuntos de revisão.</span><span class="sxs-lookup"><span data-stu-id="c16ba-111">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="c16ba-112">Get</span><span class="sxs-lookup"><span data-stu-id="c16ba-112">Get</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="c16ba-113">reviewSet</span><span class="sxs-lookup"><span data-stu-id="c16ba-113">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="c16ba-114">Leia as propriedades e os relacionamentos de um objeto **reviewset** .</span><span class="sxs-lookup"><span data-stu-id="c16ba-114">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="c16ba-115">Create</span><span class="sxs-lookup"><span data-stu-id="c16ba-115">Create</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="c16ba-116">reviewSet</span><span class="sxs-lookup"><span data-stu-id="c16ba-116">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="c16ba-117">Criar um novo conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="c16ba-117">Create a new review set.</span></span> |

## <a name="properties"></a><span data-ttu-id="c16ba-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c16ba-118">Properties</span></span>

| <span data-ttu-id="c16ba-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c16ba-119">Property</span></span>     | <span data-ttu-id="c16ba-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c16ba-120">Type</span></span>        | <span data-ttu-id="c16ba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16ba-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c16ba-122">createdBy</span><span class="sxs-lookup"><span data-stu-id="c16ba-122">createdBy</span></span>| [<span data-ttu-id="c16ba-123">identitySet</span><span class="sxs-lookup"><span data-stu-id="c16ba-123">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="c16ba-124">O usuário que criou o conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="c16ba-124">The user who created the review set.</span></span> <span data-ttu-id="c16ba-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c16ba-125">Read-only.</span></span> |
|<span data-ttu-id="c16ba-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c16ba-126">createdDateTime</span></span>|<span data-ttu-id="c16ba-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c16ba-127">DateTimeOffset</span></span>| <span data-ttu-id="c16ba-128">O DateTime quando o conjunto de revisão foi criado.</span><span class="sxs-lookup"><span data-stu-id="c16ba-128">The datetime when the review set was created.</span></span> <span data-ttu-id="c16ba-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c16ba-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c16ba-130">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c16ba-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c16ba-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c16ba-131">Read-only.</span></span> |
|<span data-ttu-id="c16ba-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c16ba-132">displayName</span></span>|<span data-ttu-id="c16ba-133">String</span><span class="sxs-lookup"><span data-stu-id="c16ba-133">String</span></span>| <span data-ttu-id="c16ba-134">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="c16ba-134">The review set name.</span></span> <span data-ttu-id="c16ba-135">O nome é exclusivo com um limite máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c16ba-135">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="c16ba-136">id</span><span class="sxs-lookup"><span data-stu-id="c16ba-136">id</span></span>|<span data-ttu-id="c16ba-137">String</span><span class="sxs-lookup"><span data-stu-id="c16ba-137">String</span></span>| <span data-ttu-id="c16ba-138">O identificador exclusivo do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="c16ba-138">The review set unique identifier.</span></span> <span data-ttu-id="c16ba-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c16ba-139">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c16ba-140">Relações</span><span class="sxs-lookup"><span data-stu-id="c16ba-140">Relationships</span></span>

| <span data-ttu-id="c16ba-141">Relação</span><span class="sxs-lookup"><span data-stu-id="c16ba-141">Relationship</span></span> | <span data-ttu-id="c16ba-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="c16ba-142">Type</span></span>        | <span data-ttu-id="c16ba-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16ba-143">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c16ba-144">Analisar consulta de definição</span><span class="sxs-lookup"><span data-stu-id="c16ba-144">Review set query</span></span> |<span data-ttu-id="c16ba-145">coleção [reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="c16ba-145">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="c16ba-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c16ba-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c16ba-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c16ba-148">JSON representation</span></span>

<span data-ttu-id="c16ba-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c16ba-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


