---
title: tipo de recurso de educationResource
description: Uma superclasse para todos os objetos de recursos no sistema. Um recurso é associado a uma **atribuição** e/ou o **envio**, que representa o objeto de aprendizado que está sendo
ms.openlocfilehash: b7e64a946992bb0b43c5bfe50e8d92b5f7176856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038549"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="16a75-104">tipo de recurso de educationResource</span><span class="sxs-lookup"><span data-stu-id="16a75-104">educationResource resource type</span></span>

> <span data-ttu-id="16a75-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16a75-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16a75-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16a75-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16a75-107">Uma superclasse para todos os objetos de recursos no sistema.</span><span class="sxs-lookup"><span data-stu-id="16a75-107">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="16a75-108">Um recurso é associado a uma **atribuição** e/ou o **envio**, que representa o objeto de aprendizado que está sendo atribuídas ou fornecidos.</span><span class="sxs-lookup"><span data-stu-id="16a75-108">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="16a75-109">Você não pode instanciar um recurso diretamente; Você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="16a75-109">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="16a75-110">Este recurso armazena as propriedades comuns em todos os tipos de recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-110">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="16a75-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16a75-111">Properties</span></span>
| <span data-ttu-id="16a75-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16a75-112">Property</span></span>     | <span data-ttu-id="16a75-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="16a75-113">Type</span></span>   |<span data-ttu-id="16a75-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a75-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16a75-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="16a75-115">createdBy</span></span>|[<span data-ttu-id="16a75-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="16a75-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="16a75-117">Quem criou o recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-117">Who created the resource.</span></span>|
|<span data-ttu-id="16a75-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16a75-118">createdDateTime</span></span>|<span data-ttu-id="16a75-119">Momento em que o recurso foi criado.</span><span class="sxs-lookup"><span data-stu-id="16a75-119">Moment in time when the resource was created.</span></span>  <span data-ttu-id="16a75-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16a75-120">DateTimeOffset</span></span>|<span data-ttu-id="16a75-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16a75-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="16a75-123">displayName</span><span class="sxs-lookup"><span data-stu-id="16a75-123">displayName</span></span>|<span data-ttu-id="16a75-124">String</span><span class="sxs-lookup"><span data-stu-id="16a75-124">String</span></span>|<span data-ttu-id="16a75-125">Exibe o nome do recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-125">Display name of resource.</span></span>|
|<span data-ttu-id="16a75-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="16a75-126">lastModifiedBy</span></span>|[<span data-ttu-id="16a75-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="16a75-127">identitySet</span></span>](identityset.md)|<span data-ttu-id="16a75-128">Quem foi o último usuário para modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-128">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="16a75-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16a75-129">lastModifiedDateTime</span></span>|<span data-ttu-id="16a75-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16a75-130">DateTimeOffset</span></span>|<span data-ttu-id="16a75-131">Momento no tempo de última modificação do recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-131">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="16a75-132">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="16a75-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="16a75-133">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16a75-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16a75-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16a75-134">JSON representation</span></span>

<span data-ttu-id="16a75-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16a75-135">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->