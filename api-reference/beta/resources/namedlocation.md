---
title: Tipo de recurso namedLocation
description: Esta é a classe base que representa um local nomeado pelo Azure Active Directory. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ae3ec6235259001a453bac50e45d2b142cdbaa8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722115"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="e0793-104">Tipo de recurso namedLocation</span><span class="sxs-lookup"><span data-stu-id="e0793-104">namedLocation resource type</span></span>

<span data-ttu-id="e0793-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0793-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0793-106">Esta é a classe base que representa um local nomeado pelo Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e0793-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="e0793-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="e0793-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="e0793-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e0793-108">Methods</span></span>

| <span data-ttu-id="e0793-109">Método</span><span class="sxs-lookup"><span data-stu-id="e0793-109">Method</span></span>       | <span data-ttu-id="e0793-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e0793-110">Return Type</span></span> | <span data-ttu-id="e0793-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0793-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e0793-112">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="e0793-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="e0793-113">[coleção namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="e0793-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="e0793-114">Obter todos os **objetos namedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="e0793-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="e0793-115">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="e0793-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="e0793-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="e0793-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="e0793-117">Leia as propriedades e as relações de um **objeto namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e0793-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="e0793-118">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="e0793-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="e0793-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="e0793-119">None</span></span> | <span data-ttu-id="e0793-120">Exclua **um objeto namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e0793-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0793-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0793-121">Properties</span></span>

| <span data-ttu-id="e0793-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0793-122">Property</span></span>     | <span data-ttu-id="e0793-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0793-123">Type</span></span>        | <span data-ttu-id="e0793-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0793-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0793-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0793-125">createdDateTime</span></span>|<span data-ttu-id="e0793-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0793-126">DateTimeOffset</span></span>|<span data-ttu-id="e0793-127">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e0793-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0793-128">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0793-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e0793-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0793-129">Read-only.</span></span>|
|<span data-ttu-id="e0793-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e0793-130">displayName</span></span>|<span data-ttu-id="e0793-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0793-131">String</span></span>|<span data-ttu-id="e0793-132">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="e0793-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="e0793-133">id</span><span class="sxs-lookup"><span data-stu-id="e0793-133">id</span></span>|<span data-ttu-id="e0793-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0793-134">String</span></span>|<span data-ttu-id="e0793-135">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="e0793-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="e0793-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0793-136">Read-only.</span></span>|
|<span data-ttu-id="e0793-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0793-137">modifiedDateTime</span></span>|<span data-ttu-id="e0793-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0793-138">DateTimeOffset</span></span>|<span data-ttu-id="e0793-139">O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e0793-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0793-140">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0793-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e0793-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0793-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0793-142">Relações</span><span class="sxs-lookup"><span data-stu-id="e0793-142">Relationships</span></span>

<span data-ttu-id="e0793-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0793-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0793-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0793-144">JSON representation</span></span>

<span data-ttu-id="e0793-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0793-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
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


