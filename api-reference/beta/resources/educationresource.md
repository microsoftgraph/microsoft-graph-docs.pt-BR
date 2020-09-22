---
title: tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f48d9b0bab9fbabd7e76da7c8d4bc738de5a137b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979571"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="4da33-104">tipo de recurso educationResource</span><span class="sxs-lookup"><span data-stu-id="4da33-104">educationResource resource type</span></span>

<span data-ttu-id="4da33-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4da33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4da33-106">Uma superclasse para todos os objetos de recurso no sistema.</span><span class="sxs-lookup"><span data-stu-id="4da33-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="4da33-107">Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo entregue ou entregue.</span><span class="sxs-lookup"><span data-stu-id="4da33-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="4da33-108">Você não pode criar uma instância de um recurso diretamente; Você deve criar uma subclasse que representará o tipo de recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4da33-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="4da33-109">Esse recurso armazena as propriedades comuns em todos os tipos de recurso.</span><span class="sxs-lookup"><span data-stu-id="4da33-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="4da33-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4da33-110">Properties</span></span>
| <span data-ttu-id="4da33-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4da33-111">Property</span></span>     | <span data-ttu-id="4da33-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4da33-112">Type</span></span>   |<span data-ttu-id="4da33-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4da33-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4da33-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="4da33-114">createdBy</span></span>|[<span data-ttu-id="4da33-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="4da33-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="4da33-116">Quem criou o recurso.</span><span class="sxs-lookup"><span data-stu-id="4da33-116">Who created the resource.</span></span>|
|<span data-ttu-id="4da33-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4da33-117">createdDateTime</span></span>|<span data-ttu-id="4da33-118">Momento no momento em que o recurso foi criado.</span><span class="sxs-lookup"><span data-stu-id="4da33-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="4da33-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da33-119">DateTimeOffset</span></span>|<span data-ttu-id="4da33-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4da33-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4da33-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4da33-122">displayName</span></span>|<span data-ttu-id="4da33-123">String</span><span class="sxs-lookup"><span data-stu-id="4da33-123">String</span></span>|<span data-ttu-id="4da33-124">Exibe o nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="4da33-124">Display name of resource.</span></span>|
|<span data-ttu-id="4da33-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4da33-125">lastModifiedBy</span></span>|[<span data-ttu-id="4da33-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="4da33-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="4da33-127">Quem foi o último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="4da33-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="4da33-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4da33-128">lastModifiedDateTime</span></span>|<span data-ttu-id="4da33-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da33-129">DateTimeOffset</span></span>|<span data-ttu-id="4da33-130">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4da33-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="4da33-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4da33-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4da33-132">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4da33-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4da33-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4da33-133">JSON representation</span></span>

<span data-ttu-id="4da33-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4da33-134">The following is a JSON representation of the resource.</span></span>

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


