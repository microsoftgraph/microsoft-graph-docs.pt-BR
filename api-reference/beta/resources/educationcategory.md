---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 18ddcd32a2ab4a8d44505adbc92445a0feeae8b6
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911316"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="ec30e-103">Tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="ec30e-103">educationCategory resource type</span></span>

<span data-ttu-id="ec30e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec30e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec30e-105">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="ec30e-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="ec30e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec30e-106">Methods</span></span>

| <span data-ttu-id="ec30e-107">Método</span><span class="sxs-lookup"><span data-stu-id="ec30e-107">Method</span></span>           | <span data-ttu-id="ec30e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec30e-108">Return Type</span></span>    |<span data-ttu-id="ec30e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec30e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec30e-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="ec30e-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="ec30e-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="ec30e-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="ec30e-112">Criar uma nova **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="ec30e-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="ec30e-113">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="ec30e-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="ec30e-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="ec30e-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="ec30e-115">Obter uma **educationCategory existente**.</span><span class="sxs-lookup"><span data-stu-id="ec30e-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="ec30e-116">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="ec30e-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="ec30e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec30e-117">None</span></span> | <span data-ttu-id="ec30e-118">Remover uma **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="ec30e-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="ec30e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec30e-119">Properties</span></span>
| <span data-ttu-id="ec30e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec30e-120">Property</span></span>     | <span data-ttu-id="ec30e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec30e-121">Type</span></span>   |<span data-ttu-id="ec30e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec30e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec30e-123">id</span><span class="sxs-lookup"><span data-stu-id="ec30e-123">id</span></span>|<span data-ttu-id="ec30e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec30e-124">String</span></span>|<span data-ttu-id="ec30e-125">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="ec30e-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="ec30e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="ec30e-126">displayName</span></span>|<span data-ttu-id="ec30e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec30e-127">String</span></span>|<span data-ttu-id="ec30e-128">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="ec30e-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec30e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec30e-129">JSON representation</span></span>

<span data-ttu-id="ec30e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec30e-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


