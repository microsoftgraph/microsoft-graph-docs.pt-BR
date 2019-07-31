---
title: tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8dfb996c863e3b2aa5e319fcd2b4dc6dd246751a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972595"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="b37a6-104">tipo de recurso educationResource</span><span class="sxs-lookup"><span data-stu-id="b37a6-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b37a6-105">Uma superclasse para todos os objetos de recurso no sistema.</span><span class="sxs-lookup"><span data-stu-id="b37a6-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="b37a6-106">Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo entregue ou entregue.</span><span class="sxs-lookup"><span data-stu-id="b37a6-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="b37a6-107">Você não pode criar uma instância de um recurso diretamente; Você deve criar uma subclasse que representará o tipo de recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="b37a6-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="b37a6-108">Esse recurso armazena as propriedades comuns em todos os tipos de recurso.</span><span class="sxs-lookup"><span data-stu-id="b37a6-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="b37a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b37a6-109">Properties</span></span>
| <span data-ttu-id="b37a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b37a6-110">Property</span></span>     | <span data-ttu-id="b37a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b37a6-111">Type</span></span>   |<span data-ttu-id="b37a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b37a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b37a6-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="b37a6-113">createdBy</span></span>|[<span data-ttu-id="b37a6-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="b37a6-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="b37a6-115">Quem criou o recurso.</span><span class="sxs-lookup"><span data-stu-id="b37a6-115">Who created the resource.</span></span>|
|<span data-ttu-id="b37a6-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b37a6-116">createdDateTime</span></span>|<span data-ttu-id="b37a6-117">Momento no momento em que o recurso foi criado.</span><span class="sxs-lookup"><span data-stu-id="b37a6-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="b37a6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b37a6-118">DateTimeOffset</span></span>|<span data-ttu-id="b37a6-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b37a6-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b37a6-121">displayName</span><span class="sxs-lookup"><span data-stu-id="b37a6-121">displayName</span></span>|<span data-ttu-id="b37a6-122">String</span><span class="sxs-lookup"><span data-stu-id="b37a6-122">String</span></span>|<span data-ttu-id="b37a6-123">Exibe o nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="b37a6-123">Display name of resource.</span></span>|
|<span data-ttu-id="b37a6-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b37a6-124">lastModifiedBy</span></span>|[<span data-ttu-id="b37a6-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="b37a6-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="b37a6-126">Quem foi o último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="b37a6-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="b37a6-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b37a6-127">lastModifiedDateTime</span></span>|<span data-ttu-id="b37a6-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b37a6-128">DateTimeOffset</span></span>|<span data-ttu-id="b37a6-129">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b37a6-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="b37a6-130">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b37a6-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b37a6-131">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b37a6-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b37a6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b37a6-132">JSON representation</span></span>

<span data-ttu-id="b37a6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b37a6-133">The following is a JSON representation of the resource.</span></span>

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
