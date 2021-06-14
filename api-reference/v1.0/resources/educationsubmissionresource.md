---
title: Tipo de recurso educationSubmissionResource
description: Um wrapper em torno de um recurso para uso em um envio.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d370e930e69e4dff93cbd22efb3104a9511cf880
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912108"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="ffcc9-103">Tipo de recurso educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ffcc9-103">educationSubmissionResource resource type</span></span>

<span data-ttu-id="ffcc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffcc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffcc9-105">Um wrapper em torno de um recurso para uso em um envio.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-105">A wrapper around a resource for use on a submission.</span></span> 

<span data-ttu-id="ffcc9-106">O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="ffcc9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ffcc9-107">Methods</span></span>

| <span data-ttu-id="ffcc9-108">Método</span><span class="sxs-lookup"><span data-stu-id="ffcc9-108">Method</span></span>           | <span data-ttu-id="ffcc9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ffcc9-109">Return Type</span></span>    |<span data-ttu-id="ffcc9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffcc9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffcc9-111">Obter educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ffcc9-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="ffcc9-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="ffcc9-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="ffcc9-113">Leia propriedades e relações de um **objeto educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="ffcc9-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="ffcc9-114">Delete</span><span class="sxs-lookup"><span data-stu-id="ffcc9-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="ffcc9-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ffcc9-115">None</span></span> |<span data-ttu-id="ffcc9-116">**Exclua um objeto educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="ffcc9-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ffcc9-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffcc9-117">Properties</span></span>
| <span data-ttu-id="ffcc9-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffcc9-118">Property</span></span>     | <span data-ttu-id="ffcc9-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffcc9-119">Type</span></span>   |<span data-ttu-id="ffcc9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffcc9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffcc9-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="ffcc9-121">assignmentResourceUrl</span></span>|<span data-ttu-id="ffcc9-122">String</span><span class="sxs-lookup"><span data-stu-id="ffcc9-122">String</span></span>|<span data-ttu-id="ffcc9-123">Ponteiro para a atribuição da qual esse recurso foi copiado.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="ffcc9-124">Se for nulo, o aluno carregará o recurso.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="ffcc9-125">id</span><span class="sxs-lookup"><span data-stu-id="ffcc9-125">id</span></span>|<span data-ttu-id="ffcc9-126">String</span><span class="sxs-lookup"><span data-stu-id="ffcc9-126">String</span></span>| <span data-ttu-id="ffcc9-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-127">Read-only.</span></span>|
|<span data-ttu-id="ffcc9-128">recurso</span><span class="sxs-lookup"><span data-stu-id="ffcc9-128">resource</span></span>|[<span data-ttu-id="ffcc9-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="ffcc9-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="ffcc9-130">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffcc9-131">Relações</span><span class="sxs-lookup"><span data-stu-id="ffcc9-131">Relationships</span></span>
<span data-ttu-id="ffcc9-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ffcc9-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ffcc9-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffcc9-133">JSON representation</span></span>

<span data-ttu-id="ffcc9-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffcc9-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


