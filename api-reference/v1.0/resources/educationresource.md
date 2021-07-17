---
title: Tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f817740ff7879d20788b46debad0824499f56498
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442434"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="ee3fc-103">Tipo de recurso educationResource</span><span class="sxs-lookup"><span data-stu-id="ee3fc-103">educationResource resource type</span></span>

<span data-ttu-id="ee3fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee3fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee3fc-105">Uma superclasse para todos os objetos de recurso no sistema.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="ee3fc-106">Um recurso é associado a um **Assignment** and/or **Submission**, que representa o objeto de aprendizagem que está sendo entregue ou entregue.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="ee3fc-107">Não é possível instaurá-lo diretamente; você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="ee3fc-108">Esse recurso armazena as propriedades comuns em todos os tipos de recursos.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="ee3fc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee3fc-109">Properties</span></span>
| <span data-ttu-id="ee3fc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee3fc-110">Property</span></span>     | <span data-ttu-id="ee3fc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee3fc-111">Type</span></span>   |<span data-ttu-id="ee3fc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee3fc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee3fc-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="ee3fc-113">createdBy</span></span>|[<span data-ttu-id="ee3fc-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee3fc-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="ee3fc-115">O indivíduo que criou o recurso.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-115">The individual who created the resource.</span></span>|
|<span data-ttu-id="ee3fc-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee3fc-116">createdDateTime</span></span>|<span data-ttu-id="ee3fc-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee3fc-117">DateTimeOffset</span></span>|<span data-ttu-id="ee3fc-118">Momento no tempo em que o recurso foi criado.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-118">Moment in time when the resource was created.</span></span> <span data-ttu-id="ee3fc-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee3fc-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ee3fc-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ee3fc-121">displayName</span><span class="sxs-lookup"><span data-stu-id="ee3fc-121">displayName</span></span>|<span data-ttu-id="ee3fc-122">String</span><span class="sxs-lookup"><span data-stu-id="ee3fc-122">String</span></span>|<span data-ttu-id="ee3fc-123">Nome de exibição do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-123">Display name of resource.</span></span>|
|<span data-ttu-id="ee3fc-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ee3fc-124">lastModifiedBy</span></span>|[<span data-ttu-id="ee3fc-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee3fc-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="ee3fc-126">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-126">The last user to modify the resource.</span></span>|
|<span data-ttu-id="ee3fc-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee3fc-127">lastModifiedDateTime</span></span>|<span data-ttu-id="ee3fc-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee3fc-128">DateTimeOffset</span></span>|<span data-ttu-id="ee3fc-129">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="ee3fc-130">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee3fc-131">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee3fc-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee3fc-132">JSON representation</span></span>

<span data-ttu-id="ee3fc-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee3fc-133">The following is a JSON representation of the resource.</span></span>

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


