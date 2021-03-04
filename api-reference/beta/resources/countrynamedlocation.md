---
title: Tipo de recurso countryNamedLocation
description: Representa um Azure Active Directory nomeado local definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dcd31478a82e6e132264b31f070d5bad317edae7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444249"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="75bf8-104">Tipo de recurso countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="75bf8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75bf8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75bf8-106">Representa um Azure Active Directory nomeado local definido por países e regiões.</span><span class="sxs-lookup"><span data-stu-id="75bf8-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="75bf8-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="75bf8-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="75bf8-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="75bf8-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75bf8-109">Methods</span><span class="sxs-lookup"><span data-stu-id="75bf8-109">Methods</span></span>

| <span data-ttu-id="75bf8-110">Método</span><span class="sxs-lookup"><span data-stu-id="75bf8-110">Method</span></span>       | <span data-ttu-id="75bf8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75bf8-111">Return Type</span></span> | <span data-ttu-id="75bf8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="75bf8-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="75bf8-113">Listar countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="75bf8-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="75bf8-114">[coleção countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="75bf8-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="75bf8-115">Obter todos os **objetos countryNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="75bf8-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="75bf8-116">Criar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="75bf8-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="75bf8-118">Crie um novo **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="75bf8-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="75bf8-119">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="75bf8-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="75bf8-121">Leia as propriedades e as relações de um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="75bf8-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="75bf8-122">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="75bf8-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="75bf8-124">Atualize um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="75bf8-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="75bf8-125">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="75bf8-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="75bf8-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="75bf8-126">None</span></span> | <span data-ttu-id="75bf8-127">Exclua **um objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="75bf8-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75bf8-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75bf8-128">Properties</span></span>

| <span data-ttu-id="75bf8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75bf8-129">Property</span></span>     | <span data-ttu-id="75bf8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75bf8-130">Type</span></span>        | <span data-ttu-id="75bf8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75bf8-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75bf8-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="75bf8-132">countriesAndRegions</span></span>|<span data-ttu-id="75bf8-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="75bf8-133">String collection</span></span>|<span data-ttu-id="75bf8-134">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="75bf8-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="75bf8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75bf8-135">createdDateTime</span></span>|<span data-ttu-id="75bf8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75bf8-136">DateTimeOffset</span></span>|<span data-ttu-id="75bf8-137">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="75bf8-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75bf8-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="75bf8-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75bf8-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75bf8-139">Read-only.</span></span> <span data-ttu-id="75bf8-140">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="75bf8-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="75bf8-141">displayName</span><span class="sxs-lookup"><span data-stu-id="75bf8-141">displayName</span></span>|<span data-ttu-id="75bf8-142">String</span><span class="sxs-lookup"><span data-stu-id="75bf8-142">String</span></span>|<span data-ttu-id="75bf8-143">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="75bf8-143">Human-readable name of the location.</span></span> <span data-ttu-id="75bf8-144">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="75bf8-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="75bf8-145">id</span><span class="sxs-lookup"><span data-stu-id="75bf8-145">id</span></span>|<span data-ttu-id="75bf8-146">String</span><span class="sxs-lookup"><span data-stu-id="75bf8-146">String</span></span>|<span data-ttu-id="75bf8-147">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="75bf8-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="75bf8-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75bf8-148">Read-only.</span></span> <span data-ttu-id="75bf8-149">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="75bf8-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="75bf8-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="75bf8-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="75bf8-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="75bf8-151">Boolean</span></span>|<span data-ttu-id="75bf8-152">True se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="75bf8-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="75bf8-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75bf8-153">modifiedDateTime</span></span>|<span data-ttu-id="75bf8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75bf8-154">DateTimeOffset</span></span>|<span data-ttu-id="75bf8-155">O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="75bf8-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75bf8-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="75bf8-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75bf8-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75bf8-157">Read-only.</span></span> <span data-ttu-id="75bf8-158">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="75bf8-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="75bf8-159">Relações</span><span class="sxs-lookup"><span data-stu-id="75bf8-159">Relationships</span></span>

<span data-ttu-id="75bf8-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75bf8-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75bf8-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75bf8-161">JSON representation</span></span>

<span data-ttu-id="75bf8-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75bf8-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
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


