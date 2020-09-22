---
title: tipo de recurso namedLocation
description: Esta é a classe base que representa um local nomeado do Azure Active Directory. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fda5c1854dee5e6ce108f2cc46b95c6a69c64230
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089305"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="9b034-104">tipo de recurso namedLocation</span><span class="sxs-lookup"><span data-stu-id="9b034-104">namedLocation resource type</span></span>

<span data-ttu-id="9b034-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b034-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b034-106">Esta é a classe base que representa um local nomeado do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9b034-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="9b034-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="9b034-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9b034-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b034-108">Methods</span></span>

| <span data-ttu-id="9b034-109">Método</span><span class="sxs-lookup"><span data-stu-id="9b034-109">Method</span></span>       | <span data-ttu-id="9b034-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b034-110">Return Type</span></span> | <span data-ttu-id="9b034-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b034-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9b034-112">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="9b034-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="9b034-113">coleção [namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="9b034-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="9b034-114">Obtenha todos os objetos **namedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="9b034-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="9b034-115">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="9b034-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="9b034-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="9b034-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="9b034-117">Leia as propriedades e os relacionamentos de um objeto **namedLocation** .</span><span class="sxs-lookup"><span data-stu-id="9b034-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="9b034-118">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="9b034-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="9b034-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b034-119">None</span></span> | <span data-ttu-id="9b034-120">Excluir um objeto **namedLocation** .</span><span class="sxs-lookup"><span data-stu-id="9b034-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b034-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b034-121">Properties</span></span>

| <span data-ttu-id="9b034-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b034-122">Property</span></span>     | <span data-ttu-id="9b034-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b034-123">Type</span></span>        | <span data-ttu-id="9b034-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b034-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b034-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b034-125">createdDateTime</span></span>|<span data-ttu-id="9b034-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b034-126">DateTimeOffset</span></span>|<span data-ttu-id="9b034-127">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9b034-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9b034-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9b034-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9b034-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b034-129">Read-only.</span></span>|
|<span data-ttu-id="9b034-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9b034-130">displayName</span></span>|<span data-ttu-id="9b034-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b034-131">String</span></span>|<span data-ttu-id="9b034-132">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="9b034-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="9b034-133">id</span><span class="sxs-lookup"><span data-stu-id="9b034-133">id</span></span>|<span data-ttu-id="9b034-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b034-134">String</span></span>|<span data-ttu-id="9b034-135">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="9b034-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="9b034-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b034-136">Read-only.</span></span>|
|<span data-ttu-id="9b034-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b034-137">modifiedDateTime</span></span>|<span data-ttu-id="9b034-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b034-138">DateTimeOffset</span></span>|<span data-ttu-id="9b034-139">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9b034-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9b034-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9b034-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9b034-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b034-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b034-142">Relações</span><span class="sxs-lookup"><span data-stu-id="9b034-142">Relationships</span></span>

<span data-ttu-id="9b034-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b034-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b034-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b034-144">JSON representation</span></span>

<span data-ttu-id="9b034-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b034-145">The following is a JSON representation of the resource.</span></span>

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


