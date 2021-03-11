---
title: Tipo de recurso reviewSet
description: Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação de litígio, investigação ou regulamentação.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bcb21fece207e9e4d98fa7a0fc612f886e5ab0e6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720330"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="588b8-103">Tipo de recurso reviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-103">reviewSet resource type</span></span>

<span data-ttu-id="588b8-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="588b8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588b8-105">Representa o conjunto estático de informações armazenadas eletronicamente coletadas para uso em uma solicitação de litígio, investigação ou regulamentação.</span><span class="sxs-lookup"><span data-stu-id="588b8-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="588b8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="588b8-106">Methods</span></span>

| <span data-ttu-id="588b8-107">Método</span><span class="sxs-lookup"><span data-stu-id="588b8-107">Method</span></span>       | <span data-ttu-id="588b8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="588b8-108">Return Type</span></span> | <span data-ttu-id="588b8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="588b8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="588b8-110">Listar reviewSets</span><span class="sxs-lookup"><span data-stu-id="588b8-110">List reviewSets</span></span>](../api/ediscovery-case-list-reviewsets.md) | <span data-ttu-id="588b8-111">[coleção microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="588b8-111">[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) collection</span></span> | <span data-ttu-id="588b8-112">Obter uma coleção de **objetos reviewset.**</span><span class="sxs-lookup"><span data-stu-id="588b8-112">Get a collection of **reviewset** objects.</span></span> |
| [<span data-ttu-id="588b8-113">Criar reviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-113">Create reviewSet</span></span>](../api/ediscovery-case-post-reviewsets.md) | [<span data-ttu-id="588b8-114">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-114">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="588b8-115">Criar um novo **conjuntos de revisão**.</span><span class="sxs-lookup"><span data-stu-id="588b8-115">Create a new **reviewset**.</span></span> |
| [<span data-ttu-id="588b8-116">Obter reviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-116">Get reviewSet</span></span>](../api/ediscovery-reviewset-get.md) | [<span data-ttu-id="588b8-117">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-117">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="588b8-118">Leia as propriedades e as relações de um **objeto reviewSet.**</span><span class="sxs-lookup"><span data-stu-id="588b8-118">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="588b8-119">Listar consultas</span><span class="sxs-lookup"><span data-stu-id="588b8-119">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md)|<span data-ttu-id="588b8-120">[coleção microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="588b8-120">[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) collection</span></span>|<span data-ttu-id="588b8-121">Obter uma lista de **recursos reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="588b8-121">Get a list of **reviewSetQuery** resources.</span></span>|
| [<span data-ttu-id="588b8-122">export</span><span class="sxs-lookup"><span data-stu-id="588b8-122">export</span></span>](../api/ediscovery-reviewset-export.md) | <span data-ttu-id="588b8-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="588b8-123">None</span></span> | <span data-ttu-id="588b8-124">Inicie uma exportação de dados do **conjuntos de revisão.**</span><span class="sxs-lookup"><span data-stu-id="588b8-124">Initiate an export of data from the **reviewset**.</span></span> |
| [<span data-ttu-id="588b8-125">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="588b8-125">addToReviewSet</span></span>](../api/ediscovery-reviewset-addtoreviewset.md)|<span data-ttu-id="588b8-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="588b8-126">None</span></span>|<span data-ttu-id="588b8-127">Adicione dados de **uma sourceCollection** a um **conjuntos de revisão**.</span><span class="sxs-lookup"><span data-stu-id="588b8-127">Add data from a **sourceCollection** to a **reviewset**.</span></span>|

## <a name="properties"></a><span data-ttu-id="588b8-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="588b8-128">Properties</span></span>

| <span data-ttu-id="588b8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="588b8-129">Property</span></span>     | <span data-ttu-id="588b8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="588b8-130">Type</span></span>        | <span data-ttu-id="588b8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="588b8-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="588b8-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="588b8-132">createdBy</span></span>        | [<span data-ttu-id="588b8-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="588b8-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="588b8-134">O usuário que criou o conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="588b8-134">The user who created the review set.</span></span> <span data-ttu-id="588b8-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="588b8-135">Read-only.</span></span> |
|<span data-ttu-id="588b8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="588b8-136">createdDateTime</span></span>  |<span data-ttu-id="588b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="588b8-137">DateTimeOffset</span></span>| <span data-ttu-id="588b8-138">A data em que o conjunto de revisão foi criado.</span><span class="sxs-lookup"><span data-stu-id="588b8-138">The datetime when the review set was created.</span></span> <span data-ttu-id="588b8-139">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="588b8-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="588b8-140">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="588b8-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="588b8-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="588b8-141">Read-only.</span></span> |
|<span data-ttu-id="588b8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="588b8-142">displayName</span></span>      |<span data-ttu-id="588b8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="588b8-143">String</span></span>| <span data-ttu-id="588b8-144">O nome do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="588b8-144">The review set name.</span></span> <span data-ttu-id="588b8-145">O nome é exclusivo com um limite máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="588b8-145">The name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="588b8-146">id</span><span class="sxs-lookup"><span data-stu-id="588b8-146">id</span></span>               |<span data-ttu-id="588b8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="588b8-147">String</span></span>| <span data-ttu-id="588b8-148">O identificador exclusivo do conjunto de revisão.</span><span class="sxs-lookup"><span data-stu-id="588b8-148">The review set unique identifier.</span></span> <span data-ttu-id="588b8-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="588b8-149">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="588b8-150">Relações</span><span class="sxs-lookup"><span data-stu-id="588b8-150">Relationships</span></span>

| <span data-ttu-id="588b8-151">Relação</span><span class="sxs-lookup"><span data-stu-id="588b8-151">Relationship</span></span> | <span data-ttu-id="588b8-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="588b8-152">Type</span></span>        | <span data-ttu-id="588b8-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="588b8-153">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="588b8-154">consultas</span><span class="sxs-lookup"><span data-stu-id="588b8-154">queries</span></span> |<span data-ttu-id="588b8-155">[coleção microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="588b8-155">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span>| <span data-ttu-id="588b8-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="588b8-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="588b8-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="588b8-158">JSON representation</span></span>

<span data-ttu-id="588b8-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="588b8-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
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
