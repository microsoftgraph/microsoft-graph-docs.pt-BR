---
title: Tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a um **Assignment** and/or **Submission**, que representa o objeto de aprendizagem que está sendo
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f82274782f84204be288c67365288891f64fedf6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440943"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="94a93-104">Tipo de recurso educationResource</span><span class="sxs-lookup"><span data-stu-id="94a93-104">educationResource resource type</span></span>

<span data-ttu-id="94a93-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a93-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a93-106">Uma superclasse para todos os objetos de recurso no sistema.</span><span class="sxs-lookup"><span data-stu-id="94a93-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="94a93-107">Um recurso é associado a um **Assignment** and/or **Submission**, que representa o objeto de aprendizagem que está sendo entregue ou entregue.</span><span class="sxs-lookup"><span data-stu-id="94a93-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="94a93-108">Não é possível instaurá-lo diretamente; você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="94a93-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="94a93-109">Esse recurso armazena as propriedades comuns em todos os tipos de recursos.</span><span class="sxs-lookup"><span data-stu-id="94a93-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="94a93-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94a93-110">Properties</span></span>
| <span data-ttu-id="94a93-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94a93-111">Property</span></span>     | <span data-ttu-id="94a93-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="94a93-112">Type</span></span>   |<span data-ttu-id="94a93-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a93-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94a93-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="94a93-114">createdBy</span></span>|[<span data-ttu-id="94a93-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="94a93-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="94a93-116">Who criou o recurso.</span><span class="sxs-lookup"><span data-stu-id="94a93-116">Who created the resource.</span></span>|
|<span data-ttu-id="94a93-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94a93-117">createdDateTime</span></span>|<span data-ttu-id="94a93-118">Momento no tempo em que o recurso foi criado.</span><span class="sxs-lookup"><span data-stu-id="94a93-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="94a93-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a93-119">DateTimeOffset</span></span>|<span data-ttu-id="94a93-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="94a93-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94a93-121">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="94a93-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="94a93-122">displayName</span><span class="sxs-lookup"><span data-stu-id="94a93-122">displayName</span></span>|<span data-ttu-id="94a93-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94a93-123">String</span></span>|<span data-ttu-id="94a93-124">Nome de exibição do recurso.</span><span class="sxs-lookup"><span data-stu-id="94a93-124">Display name of resource.</span></span>|
|<span data-ttu-id="94a93-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="94a93-125">lastModifiedBy</span></span>|[<span data-ttu-id="94a93-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="94a93-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="94a93-127">Who foi o último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="94a93-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="94a93-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94a93-128">lastModifiedDateTime</span></span>|<span data-ttu-id="94a93-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a93-129">DateTimeOffset</span></span>|<span data-ttu-id="94a93-130">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="94a93-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="94a93-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="94a93-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94a93-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="94a93-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94a93-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94a93-133">JSON representation</span></span>

<span data-ttu-id="94a93-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94a93-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


