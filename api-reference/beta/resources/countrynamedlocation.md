---
title: tipo de recurso countryNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0683c967d56303cb092b7300e50312ab329ea4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458030"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="93aa9-104">tipo de recurso countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="93aa9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93aa9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93aa9-106">Representa um local nomeado do Azure Active Directory definido por países e regiões.</span><span class="sxs-lookup"><span data-stu-id="93aa9-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="93aa9-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="93aa9-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="93aa9-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="93aa9-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="93aa9-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="93aa9-109">Methods</span></span>

| <span data-ttu-id="93aa9-110">Método</span><span class="sxs-lookup"><span data-stu-id="93aa9-110">Method</span></span>       | <span data-ttu-id="93aa9-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93aa9-111">Return Type</span></span> | <span data-ttu-id="93aa9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="93aa9-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="93aa9-113">Listar countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="93aa9-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="93aa9-114">coleção [countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="93aa9-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="93aa9-115">Obtenha todos os objetos **countryNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="93aa9-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="93aa9-116">Criar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="93aa9-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="93aa9-118">Criar um novo objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="93aa9-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="93aa9-119">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="93aa9-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="93aa9-121">Leia as propriedades e os relacionamentos de um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="93aa9-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="93aa9-122">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="93aa9-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="93aa9-124">Atualizar um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="93aa9-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="93aa9-125">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="93aa9-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="93aa9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93aa9-126">None</span></span> | <span data-ttu-id="93aa9-127">Excluir um objeto **countryNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="93aa9-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93aa9-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93aa9-128">Properties</span></span>

| <span data-ttu-id="93aa9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93aa9-129">Property</span></span>     | <span data-ttu-id="93aa9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="93aa9-130">Type</span></span>        | <span data-ttu-id="93aa9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="93aa9-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="93aa9-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="93aa9-132">countriesAndRegions</span></span>|<span data-ttu-id="93aa9-133">Coleção String</span><span class="sxs-lookup"><span data-stu-id="93aa9-133">String collection</span></span>|<span data-ttu-id="93aa9-134">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="93aa9-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="93aa9-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93aa9-135">createdDateTime</span></span>|<span data-ttu-id="93aa9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93aa9-136">DateTimeOffset</span></span>|<span data-ttu-id="93aa9-137">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="93aa9-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93aa9-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="93aa9-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="93aa9-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93aa9-139">Read-only.</span></span> <span data-ttu-id="93aa9-140">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="93aa9-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="93aa9-141">displayName</span><span class="sxs-lookup"><span data-stu-id="93aa9-141">displayName</span></span>|<span data-ttu-id="93aa9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93aa9-142">String</span></span>|<span data-ttu-id="93aa9-143">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="93aa9-143">Human-readable name of the location.</span></span> <span data-ttu-id="93aa9-144">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="93aa9-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="93aa9-145">id</span><span class="sxs-lookup"><span data-stu-id="93aa9-145">id</span></span>|<span data-ttu-id="93aa9-146">String</span><span class="sxs-lookup"><span data-stu-id="93aa9-146">String</span></span>|<span data-ttu-id="93aa9-147">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="93aa9-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="93aa9-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93aa9-148">Read-only.</span></span> <span data-ttu-id="93aa9-149">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="93aa9-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="93aa9-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="93aa9-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="93aa9-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="93aa9-151">Boolean</span></span>|<span data-ttu-id="93aa9-152">True se endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="93aa9-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="93aa9-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93aa9-153">modifiedDateTime</span></span>|<span data-ttu-id="93aa9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93aa9-154">DateTimeOffset</span></span>|<span data-ttu-id="93aa9-155">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="93aa9-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93aa9-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="93aa9-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="93aa9-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93aa9-157">Read-only.</span></span> <span data-ttu-id="93aa9-158">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="93aa9-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="93aa9-159">Relações</span><span class="sxs-lookup"><span data-stu-id="93aa9-159">Relationships</span></span>

<span data-ttu-id="93aa9-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93aa9-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93aa9-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93aa9-161">JSON representation</span></span>

<span data-ttu-id="93aa9-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93aa9-162">The following is a JSON representation of the resource.</span></span>

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
