---
title: tipo de recurso namedLocation
description: Esta é a classe base que representa um local nomeado do Azure Active Directory. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f1e0b7c86a8b2c026c44b46fd833594aadad5a9
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653850"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="9230f-104">tipo de recurso namedLocation</span><span class="sxs-lookup"><span data-stu-id="9230f-104">namedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9230f-105">Esta é a classe base que representa um local nomeado do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9230f-105">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="9230f-106">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="9230f-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9230f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9230f-107">Methods</span></span>

| <span data-ttu-id="9230f-108">Método</span><span class="sxs-lookup"><span data-stu-id="9230f-108">Method</span></span>       | <span data-ttu-id="9230f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9230f-109">Return Type</span></span> | <span data-ttu-id="9230f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9230f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9230f-111">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="9230f-111">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="9230f-112">coleção [namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="9230f-112">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="9230f-113">Obtenha todos os objetos **namedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="9230f-113">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="9230f-114">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="9230f-114">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="9230f-115">namedLocation</span><span class="sxs-lookup"><span data-stu-id="9230f-115">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="9230f-116">Leia as propriedades e os relacionamentos de um objeto **namedLocation** .</span><span class="sxs-lookup"><span data-stu-id="9230f-116">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="9230f-117">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="9230f-117">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="9230f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9230f-118">None</span></span> | <span data-ttu-id="9230f-119">Excluir um objeto **namedLocation** .</span><span class="sxs-lookup"><span data-stu-id="9230f-119">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9230f-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9230f-120">Properties</span></span>

| <span data-ttu-id="9230f-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9230f-121">Property</span></span>     | <span data-ttu-id="9230f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9230f-122">Type</span></span>        | <span data-ttu-id="9230f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9230f-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9230f-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9230f-124">createdDateTime</span></span>|<span data-ttu-id="9230f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9230f-125">DateTimeOffset</span></span>|<span data-ttu-id="9230f-126">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9230f-126">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9230f-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9230f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9230f-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9230f-128">Read-only.</span></span>|
|<span data-ttu-id="9230f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="9230f-129">displayName</span></span>|<span data-ttu-id="9230f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9230f-130">String</span></span>|<span data-ttu-id="9230f-131">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="9230f-131">Human-readable name of the location.</span></span>|
|<span data-ttu-id="9230f-132">id</span><span class="sxs-lookup"><span data-stu-id="9230f-132">id</span></span>|<span data-ttu-id="9230f-133">String</span><span class="sxs-lookup"><span data-stu-id="9230f-133">String</span></span>|<span data-ttu-id="9230f-134">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="9230f-134">Identifier of a namedLocation object.</span></span> <span data-ttu-id="9230f-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9230f-135">Read-only.</span></span>|
|<span data-ttu-id="9230f-136">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9230f-136">modifiedDateTime</span></span>|<span data-ttu-id="9230f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9230f-137">DateTimeOffset</span></span>|<span data-ttu-id="9230f-138">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9230f-138">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9230f-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9230f-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9230f-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9230f-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9230f-141">Relações</span><span class="sxs-lookup"><span data-stu-id="9230f-141">Relationships</span></span>

<span data-ttu-id="9230f-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9230f-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9230f-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9230f-143">JSON representation</span></span>

<span data-ttu-id="9230f-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9230f-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
