---
title: Tipo de recurso countryNamedLocation
description: Representa um Azure Active Directory nomeado local definido por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c01811ce3940c77a3586196db7b5d2fdf82ebbbb
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491030"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="eb664-104">Tipo de recurso countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="eb664-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb664-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb664-106">Representa um Azure Active Directory nomeado local definido por países e regiões.</span><span class="sxs-lookup"><span data-stu-id="eb664-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="eb664-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="eb664-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="eb664-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="eb664-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb664-109">Methods</span></span>

| <span data-ttu-id="eb664-110">Método</span><span class="sxs-lookup"><span data-stu-id="eb664-110">Method</span></span>       | <span data-ttu-id="eb664-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb664-111">Return Type</span></span> | <span data-ttu-id="eb664-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb664-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb664-113">Listar countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="eb664-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="eb664-114">[coleção countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="eb664-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="eb664-115">Obter todos os **objetos countryNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="eb664-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="eb664-116">Criar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="eb664-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="eb664-118">Crie um novo **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="eb664-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb664-119">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="eb664-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="eb664-121">Leia as propriedades e as relações de um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="eb664-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb664-122">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="eb664-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="eb664-124">Atualize um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="eb664-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="eb664-125">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="eb664-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="eb664-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb664-126">None</span></span> | <span data-ttu-id="eb664-127">Exclua **um objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="eb664-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb664-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb664-128">Properties</span></span>

| <span data-ttu-id="eb664-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb664-129">Property</span></span>     | <span data-ttu-id="eb664-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb664-130">Type</span></span>        | <span data-ttu-id="eb664-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb664-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb664-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb664-132">countriesAndRegions</span></span>|<span data-ttu-id="eb664-133">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb664-133">String collection</span></span>|<span data-ttu-id="eb664-134">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="eb664-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="eb664-135">countryLookupMethod</span><span class="sxs-lookup"><span data-stu-id="eb664-135">countryLookupMethod</span></span>|<span data-ttu-id="eb664-136">countryLookupMethodType</span><span class="sxs-lookup"><span data-stu-id="eb664-136">countryLookupMethodType</span></span>|<span data-ttu-id="eb664-137">Determina em qual método é usado para decidir em qual país o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="eb664-137">Determines what method is used to decide which country the user is located in.</span></span> <span data-ttu-id="eb664-138">Os valores possíveis são: `clientIpAddress` e `authenticatorAppGps`.</span><span class="sxs-lookup"><span data-stu-id="eb664-138">Possible values are `clientIpAddress` and `authenticatorAppGps`.</span></span>|
|<span data-ttu-id="eb664-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb664-139">createdDateTime</span></span>|<span data-ttu-id="eb664-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb664-140">DateTimeOffset</span></span>|<span data-ttu-id="eb664-141">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eb664-141">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb664-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eb664-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="eb664-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb664-143">Read-only.</span></span> <span data-ttu-id="eb664-144">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="eb664-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb664-145">displayName</span><span class="sxs-lookup"><span data-stu-id="eb664-145">displayName</span></span>|<span data-ttu-id="eb664-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb664-146">String</span></span>|<span data-ttu-id="eb664-147">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="eb664-147">Human-readable name of the location.</span></span> <span data-ttu-id="eb664-148">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="eb664-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb664-149">id</span><span class="sxs-lookup"><span data-stu-id="eb664-149">id</span></span>|<span data-ttu-id="eb664-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb664-150">String</span></span>|<span data-ttu-id="eb664-151">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="eb664-151">Identifier of a namedLocation object.</span></span> <span data-ttu-id="eb664-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb664-152">Read-only.</span></span> <span data-ttu-id="eb664-153">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="eb664-153">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="eb664-154">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="eb664-154">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="eb664-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb664-155">Boolean</span></span>|<span data-ttu-id="eb664-156">True se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="eb664-156">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="eb664-157">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb664-157">modifiedDateTime</span></span>|<span data-ttu-id="eb664-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb664-158">DateTimeOffset</span></span>|<span data-ttu-id="eb664-159">O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eb664-159">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb664-160">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eb664-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="eb664-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb664-161">Read-only.</span></span> <span data-ttu-id="eb664-162">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="eb664-162">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|


## <a name="relationships"></a><span data-ttu-id="eb664-163">Relações</span><span class="sxs-lookup"><span data-stu-id="eb664-163">Relationships</span></span>

<span data-ttu-id="eb664-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb664-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb664-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb664-165">JSON representation</span></span>

<span data-ttu-id="eb664-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb664-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "countryLookupMethod": "countryLookedupMethodType",
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


