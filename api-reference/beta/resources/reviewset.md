---
title: tipo de recurso reviewset
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 411de013df02bcd71e851a694664ae010edaf4ab
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597259"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="6985e-103">tipo de recurso reviewset</span><span class="sxs-lookup"><span data-stu-id="6985e-103">reviewSet resource type</span></span>

<span data-ttu-id="6985e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6985e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6985e-105">Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em litígio, investigação ou solicitação regulatória.</span><span class="sxs-lookup"><span data-stu-id="6985e-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="6985e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="6985e-106">Methods</span></span>

| <span data-ttu-id="6985e-107">Método</span><span class="sxs-lookup"><span data-stu-id="6985e-107">Method</span></span>       | <span data-ttu-id="6985e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6985e-108">Return Type</span></span> | <span data-ttu-id="6985e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6985e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6985e-110">Reviewset de lista</span><span class="sxs-lookup"><span data-stu-id="6985e-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="6985e-111">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="6985e-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="6985e-112">Obter uma coleção de conjuntos de revisão.</span><span class="sxs-lookup"><span data-stu-id="6985e-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="6985e-113">Obter reviewset</span><span class="sxs-lookup"><span data-stu-id="6985e-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="6985e-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6985e-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="6985e-115">Leia as propriedades e os relacionamentos de um objeto **reviewset** .</span><span class="sxs-lookup"><span data-stu-id="6985e-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="6985e-116">Criar reviewset</span><span class="sxs-lookup"><span data-stu-id="6985e-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="6985e-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6985e-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="6985e-118">Criar um novo conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="6985e-118">Create a new review set.</span></span> |
| [<span data-ttu-id="6985e-119">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="6985e-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="6985e-120">coleção [reviewSetQuery](../resources/reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="6985e-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="6985e-121">Obtenha os recursos reviewSetQuery da propriedade de navegação queries.</span><span class="sxs-lookup"><span data-stu-id="6985e-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="6985e-122">Criar consultas</span><span class="sxs-lookup"><span data-stu-id="6985e-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="6985e-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="6985e-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="6985e-124">Criar um novo objeto reviewSetQuery.</span><span class="sxs-lookup"><span data-stu-id="6985e-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6985e-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6985e-125">Properties</span></span>

| <span data-ttu-id="6985e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6985e-126">Property</span></span>     | <span data-ttu-id="6985e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6985e-127">Type</span></span>        | <span data-ttu-id="6985e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6985e-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6985e-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="6985e-129">createdBy</span></span>        | [<span data-ttu-id="6985e-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="6985e-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="6985e-131">O usuário que criou o conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="6985e-131">The user who created the review set.</span></span> <span data-ttu-id="6985e-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6985e-132">Read-only.</span></span> |
|<span data-ttu-id="6985e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6985e-133">createdDateTime</span></span>  |<span data-ttu-id="6985e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6985e-134">DateTimeOffset</span></span>| <span data-ttu-id="6985e-135">O DateTime quando o conjunto de revisão foi criado.</span><span class="sxs-lookup"><span data-stu-id="6985e-135">The datetime when the review set was created.</span></span> <span data-ttu-id="6985e-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6985e-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6985e-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6985e-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6985e-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6985e-138">Read-only.</span></span> |
|<span data-ttu-id="6985e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6985e-139">displayName</span></span>      |<span data-ttu-id="6985e-140">String</span><span class="sxs-lookup"><span data-stu-id="6985e-140">String</span></span>| <span data-ttu-id="6985e-141">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="6985e-141">The review set name.</span></span> <span data-ttu-id="6985e-142">O nome é exclusivo com um limite máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6985e-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="6985e-143">id</span><span class="sxs-lookup"><span data-stu-id="6985e-143">id</span></span>               |<span data-ttu-id="6985e-144">String</span><span class="sxs-lookup"><span data-stu-id="6985e-144">String</span></span>| <span data-ttu-id="6985e-145">O identificador exclusivo do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="6985e-145">The review set unique identifier.</span></span> <span data-ttu-id="6985e-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6985e-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6985e-147">Relações</span><span class="sxs-lookup"><span data-stu-id="6985e-147">Relationships</span></span>

| <span data-ttu-id="6985e-148">Relação</span><span class="sxs-lookup"><span data-stu-id="6985e-148">Relationship</span></span> | <span data-ttu-id="6985e-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="6985e-149">Type</span></span>        | <span data-ttu-id="6985e-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="6985e-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6985e-151">Analisar consulta de definição</span><span class="sxs-lookup"><span data-stu-id="6985e-151">Review set query</span></span> |<span data-ttu-id="6985e-152">coleção [reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="6985e-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="6985e-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6985e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6985e-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6985e-155">JSON representation</span></span>

<span data-ttu-id="6985e-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6985e-156">The following is a JSON representation of the resource.</span></span>

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
