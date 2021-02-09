---
title: Tipo de recurso reviewSet
description: Representa um conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação regulamentar, investigação ou litígio.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b6234fafbf0d6e36d5dcbb4143956447e26d3a0f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153491"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="b901b-103">Tipo de recurso reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-103">reviewSet resource type</span></span>

<span data-ttu-id="b901b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b901b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b901b-105">Representa um conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação regulamentar, investigação ou litígio.</span><span class="sxs-lookup"><span data-stu-id="b901b-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="b901b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b901b-106">Methods</span></span>

| <span data-ttu-id="b901b-107">Método</span><span class="sxs-lookup"><span data-stu-id="b901b-107">Method</span></span>       | <span data-ttu-id="b901b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b901b-108">Return Type</span></span> | <span data-ttu-id="b901b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b901b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b901b-110">Listar reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="b901b-111">[coleção reviewSet](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="b901b-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="b901b-112">Obter uma coleção de conjuntos de revisão.</span><span class="sxs-lookup"><span data-stu-id="b901b-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="b901b-113">Obter reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="b901b-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="b901b-115">Leia as propriedades e os relacionamentos de um **objeto reviewSet.**</span><span class="sxs-lookup"><span data-stu-id="b901b-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="b901b-116">Criar reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="b901b-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="b901b-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="b901b-118">Criar um novo conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="b901b-118">Create a new review set.</span></span> |
| [<span data-ttu-id="b901b-119">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="b901b-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="b901b-120">[Coleção reviewSetQuery](../resources/reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="b901b-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="b901b-121">Obter os recursos reviewSetQuery da propriedade de navegação de consultas.</span><span class="sxs-lookup"><span data-stu-id="b901b-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="b901b-122">Criar consultas</span><span class="sxs-lookup"><span data-stu-id="b901b-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="b901b-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="b901b-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="b901b-124">Crie um novo objeto reviewSetQuery.</span><span class="sxs-lookup"><span data-stu-id="b901b-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b901b-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b901b-125">Properties</span></span>

| <span data-ttu-id="b901b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b901b-126">Property</span></span>     | <span data-ttu-id="b901b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b901b-127">Type</span></span>        | <span data-ttu-id="b901b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b901b-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b901b-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="b901b-129">createdBy</span></span>        | [<span data-ttu-id="b901b-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="b901b-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="b901b-131">O usuário que criou o conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="b901b-131">The user who created the review set.</span></span> <span data-ttu-id="b901b-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b901b-132">Read-only.</span></span> |
|<span data-ttu-id="b901b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b901b-133">createdDateTime</span></span>  |<span data-ttu-id="b901b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b901b-134">DateTimeOffset</span></span>| <span data-ttu-id="b901b-135">A data e a hora em que o conjunto de revisão foi criado.</span><span class="sxs-lookup"><span data-stu-id="b901b-135">The datetime when the review set was created.</span></span> <span data-ttu-id="b901b-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b901b-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b901b-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b901b-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b901b-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b901b-138">Read-only.</span></span> |
|<span data-ttu-id="b901b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b901b-139">displayName</span></span>      |<span data-ttu-id="b901b-140">String</span><span class="sxs-lookup"><span data-stu-id="b901b-140">String</span></span>| <span data-ttu-id="b901b-141">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="b901b-141">The review set name.</span></span> <span data-ttu-id="b901b-142">O nome é exclusivo com um limite máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b901b-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="b901b-143">id</span><span class="sxs-lookup"><span data-stu-id="b901b-143">id</span></span>               |<span data-ttu-id="b901b-144">String</span><span class="sxs-lookup"><span data-stu-id="b901b-144">String</span></span>| <span data-ttu-id="b901b-145">O identificador exclusivo do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="b901b-145">The review set unique identifier.</span></span> <span data-ttu-id="b901b-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b901b-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b901b-147">Relações</span><span class="sxs-lookup"><span data-stu-id="b901b-147">Relationships</span></span>

| <span data-ttu-id="b901b-148">Relação</span><span class="sxs-lookup"><span data-stu-id="b901b-148">Relationship</span></span> | <span data-ttu-id="b901b-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="b901b-149">Type</span></span>        | <span data-ttu-id="b901b-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="b901b-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b901b-151">Revisar a consulta do conjunto</span><span class="sxs-lookup"><span data-stu-id="b901b-151">Review set query</span></span> |<span data-ttu-id="b901b-152">[Coleção reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="b901b-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="b901b-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b901b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b901b-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b901b-155">JSON representation</span></span>

<span data-ttu-id="b901b-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b901b-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
