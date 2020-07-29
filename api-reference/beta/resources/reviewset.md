---
title: tipo de recurso reviewset
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 374984f2d44050c1332ec016f83a1ccdea909ba0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509913"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="f96ee-103">tipo de recurso reviewset</span><span class="sxs-lookup"><span data-stu-id="f96ee-103">reviewSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f96ee-104">Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.</span><span class="sxs-lookup"><span data-stu-id="f96ee-104">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="f96ee-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f96ee-105">Methods</span></span>

| <span data-ttu-id="f96ee-106">Método</span><span class="sxs-lookup"><span data-stu-id="f96ee-106">Method</span></span>       | <span data-ttu-id="f96ee-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f96ee-107">Return Type</span></span> | <span data-ttu-id="f96ee-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96ee-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f96ee-109">Listar</span><span class="sxs-lookup"><span data-stu-id="f96ee-109">List</span></span>](../api/reviewset-list.md) | <span data-ttu-id="f96ee-110">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="f96ee-110">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="f96ee-111">Obter uma coleção de conjuntos de revisão.</span><span class="sxs-lookup"><span data-stu-id="f96ee-111">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="f96ee-112">Get</span><span class="sxs-lookup"><span data-stu-id="f96ee-112">Get</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="f96ee-113">reviewset</span><span class="sxs-lookup"><span data-stu-id="f96ee-113">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="f96ee-114">Leia as propriedades e os relacionamentos de um objeto **reviewset** .</span><span class="sxs-lookup"><span data-stu-id="f96ee-114">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="f96ee-115">Create</span><span class="sxs-lookup"><span data-stu-id="f96ee-115">Create</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="f96ee-116">reviewset</span><span class="sxs-lookup"><span data-stu-id="f96ee-116">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="f96ee-117">Criar um novo conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="f96ee-117">Create a new review set.</span></span> |

## <a name="properties"></a><span data-ttu-id="f96ee-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f96ee-118">Properties</span></span>

| <span data-ttu-id="f96ee-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f96ee-119">Property</span></span>     | <span data-ttu-id="f96ee-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f96ee-120">Type</span></span>        | <span data-ttu-id="f96ee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96ee-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f96ee-122">createdBy</span><span class="sxs-lookup"><span data-stu-id="f96ee-122">createdBy</span></span>| [<span data-ttu-id="f96ee-123">identitySet</span><span class="sxs-lookup"><span data-stu-id="f96ee-123">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="f96ee-124">O usuário que criou o conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="f96ee-124">The user who created the review set.</span></span> <span data-ttu-id="f96ee-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f96ee-125">Read-only.</span></span> |
|<span data-ttu-id="f96ee-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f96ee-126">createdDateTime</span></span>|<span data-ttu-id="f96ee-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f96ee-127">DateTimeOffset</span></span>| <span data-ttu-id="f96ee-128">O DateTime quando o conjunto de revisão foi criado.</span><span class="sxs-lookup"><span data-stu-id="f96ee-128">The datetime when the review set was created.</span></span> <span data-ttu-id="f96ee-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f96ee-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f96ee-130">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f96ee-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f96ee-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f96ee-131">Read-only.</span></span> |
|<span data-ttu-id="f96ee-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f96ee-132">displayName</span></span>|<span data-ttu-id="f96ee-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f96ee-133">String</span></span>| <span data-ttu-id="f96ee-134">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="f96ee-134">The review set name.</span></span> <span data-ttu-id="f96ee-135">O nome é exclusivo com um limite máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f96ee-135">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="f96ee-136">id</span><span class="sxs-lookup"><span data-stu-id="f96ee-136">id</span></span>|<span data-ttu-id="f96ee-137">String</span><span class="sxs-lookup"><span data-stu-id="f96ee-137">String</span></span>| <span data-ttu-id="f96ee-138">O identificador exclusivo do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="f96ee-138">The review set unique identifier.</span></span> <span data-ttu-id="f96ee-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f96ee-139">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f96ee-140">Relações</span><span class="sxs-lookup"><span data-stu-id="f96ee-140">Relationships</span></span>

| <span data-ttu-id="f96ee-141">Relação</span><span class="sxs-lookup"><span data-stu-id="f96ee-141">Relationship</span></span> | <span data-ttu-id="f96ee-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="f96ee-142">Type</span></span>        | <span data-ttu-id="f96ee-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96ee-143">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f96ee-144">Analisar consulta de definição</span><span class="sxs-lookup"><span data-stu-id="f96ee-144">Review set query</span></span> |<span data-ttu-id="f96ee-145">coleção [reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="f96ee-145">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="f96ee-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f96ee-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f96ee-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f96ee-148">JSON representation</span></span>

<span data-ttu-id="f96ee-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f96ee-149">The following is a JSON representation of the resource.</span></span>

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
