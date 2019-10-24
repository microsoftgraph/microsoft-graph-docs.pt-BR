---
title: tipo de recurso countryNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cb413aab72abe401152b67b985f023350f80f30
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653668"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="5cbfe-104">tipo de recurso countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-104">countryNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbfe-105">Representa um local nomeado do Azure Active Directory definido por países e regiões.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-105">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="5cbfe-106">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="5cbfe-107">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="5cbfe-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5cbfe-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5cbfe-108">Methods</span></span>

| <span data-ttu-id="5cbfe-109">Método</span><span class="sxs-lookup"><span data-stu-id="5cbfe-109">Method</span></span>       | <span data-ttu-id="5cbfe-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5cbfe-110">Return Type</span></span> | <span data-ttu-id="5cbfe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cbfe-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cbfe-112">Listar countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="5cbfe-112">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="5cbfe-113">coleção [countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="5cbfe-113">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="5cbfe-114">Obtenha todos os objetos **countryNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-114">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="5cbfe-115">Criar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-115">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="5cbfe-116">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-116">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="5cbfe-117">Criar um novo objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="5cbfe-117">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="5cbfe-118">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-118">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="5cbfe-119">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-119">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="5cbfe-120">Leia as propriedades e os relacionamentos de um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="5cbfe-120">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="5cbfe-121">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-121">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="5cbfe-122">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-122">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="5cbfe-123">Atualizar um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="5cbfe-123">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="5cbfe-124">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="5cbfe-124">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="5cbfe-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cbfe-125">None</span></span> | <span data-ttu-id="5cbfe-126">Excluir um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="5cbfe-126">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cbfe-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cbfe-127">Properties</span></span>

| <span data-ttu-id="5cbfe-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cbfe-128">Property</span></span>     | <span data-ttu-id="5cbfe-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cbfe-129">Type</span></span>        | <span data-ttu-id="5cbfe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cbfe-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cbfe-131">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="5cbfe-131">countriesAndRegions</span></span>|<span data-ttu-id="5cbfe-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cbfe-132">String collection</span></span>|<span data-ttu-id="5cbfe-133">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-133">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="5cbfe-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbfe-134">createdDateTime</span></span>|<span data-ttu-id="5cbfe-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbfe-135">DateTimeOffset</span></span>|<span data-ttu-id="5cbfe-136">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-136">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cbfe-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5cbfe-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-138">Read-only.</span></span> <span data-ttu-id="5cbfe-139">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfe-139">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="5cbfe-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5cbfe-140">displayName</span></span>|<span data-ttu-id="5cbfe-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cbfe-141">String</span></span>|<span data-ttu-id="5cbfe-142">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-142">Human-readable name of the location.</span></span> <span data-ttu-id="5cbfe-143">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfe-143">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="5cbfe-144">id</span><span class="sxs-lookup"><span data-stu-id="5cbfe-144">id</span></span>|<span data-ttu-id="5cbfe-145">String</span><span class="sxs-lookup"><span data-stu-id="5cbfe-145">String</span></span>|<span data-ttu-id="5cbfe-146">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-146">Identifier of a namedLocation object.</span></span> <span data-ttu-id="5cbfe-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-147">Read-only.</span></span> <span data-ttu-id="5cbfe-148">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfe-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="5cbfe-149">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="5cbfe-149">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="5cbfe-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="5cbfe-150">Boolean</span></span>|<span data-ttu-id="5cbfe-151">True se endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-151">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="5cbfe-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbfe-152">modifiedDateTime</span></span>|<span data-ttu-id="5cbfe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbfe-153">DateTimeOffset</span></span>|<span data-ttu-id="5cbfe-154">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cbfe-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5cbfe-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-156">Read-only.</span></span> <span data-ttu-id="5cbfe-157">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="5cbfe-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cbfe-158">Relações</span><span class="sxs-lookup"><span data-stu-id="5cbfe-158">Relationships</span></span>

<span data-ttu-id="5cbfe-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cbfe-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cbfe-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cbfe-160">JSON representation</span></span>

<span data-ttu-id="5cbfe-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cbfe-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": ""
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
