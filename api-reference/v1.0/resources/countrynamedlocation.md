---
title: Tipo de recurso countryNamedLocation
description: Representa uma Azure Active Directory nome definida por países e regiões. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 531942e5026e2fc3d4d9ed3311d9130275d5a853
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443162"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="dd7df-104">Tipo de recurso countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="dd7df-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd7df-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd7df-106">Representa uma Azure Active Directory nome definida por países e regiões.</span><span class="sxs-lookup"><span data-stu-id="dd7df-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="dd7df-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="dd7df-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="dd7df-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="dd7df-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="dd7df-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd7df-109">Methods</span></span>

| <span data-ttu-id="dd7df-110">Método</span><span class="sxs-lookup"><span data-stu-id="dd7df-110">Method</span></span>       | <span data-ttu-id="dd7df-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd7df-111">Return Type</span></span> | <span data-ttu-id="dd7df-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd7df-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd7df-113">Listar countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="dd7df-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="dd7df-114">[coleção countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="dd7df-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="dd7df-115">Obter todos os **objetos countryNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="dd7df-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="dd7df-116">Criar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="dd7df-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="dd7df-118">Crie um novo **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="dd7df-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="dd7df-119">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="dd7df-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="dd7df-121">Leia as propriedades e as relações de um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="dd7df-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="dd7df-122">Atualizar countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="dd7df-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="dd7df-124">Atualize um **objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="dd7df-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="dd7df-125">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="dd7df-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="dd7df-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd7df-126">None</span></span> | <span data-ttu-id="dd7df-127">Exclua **um objeto countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="dd7df-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd7df-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd7df-128">Properties</span></span>

| <span data-ttu-id="dd7df-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd7df-129">Property</span></span>     | <span data-ttu-id="dd7df-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd7df-130">Type</span></span>        | <span data-ttu-id="dd7df-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd7df-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd7df-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="dd7df-132">countriesAndRegions</span></span>|<span data-ttu-id="dd7df-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7df-133">String collection</span></span>|<span data-ttu-id="dd7df-134">Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="dd7df-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="dd7df-135">countryLookupMethod</span><span class="sxs-lookup"><span data-stu-id="dd7df-135">countryLookupMethod</span></span>|<span data-ttu-id="dd7df-136">countryLookupMethodType</span><span class="sxs-lookup"><span data-stu-id="dd7df-136">countryLookupMethodType</span></span>|<span data-ttu-id="dd7df-137">Determina em qual método é usado para decidir em qual país o usuário está localizado.</span><span class="sxs-lookup"><span data-stu-id="dd7df-137">Determines what method is used to decide which country the user is located in.</span></span> <span data-ttu-id="dd7df-138">Os valores possíveis são: `clientIpAddress` e `authenticatorAppGps`.</span><span class="sxs-lookup"><span data-stu-id="dd7df-138">Possible values are `clientIpAddress` and `authenticatorAppGps`.</span></span>|
|<span data-ttu-id="dd7df-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7df-139">createdDateTime</span></span>|<span data-ttu-id="dd7df-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7df-140">DateTimeOffset</span></span>|<span data-ttu-id="dd7df-141">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd7df-141">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd7df-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dd7df-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="dd7df-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd7df-143">Read-only.</span></span> <span data-ttu-id="dd7df-144">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="dd7df-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="dd7df-145">displayName</span><span class="sxs-lookup"><span data-stu-id="dd7df-145">displayName</span></span>|<span data-ttu-id="dd7df-146">String</span><span class="sxs-lookup"><span data-stu-id="dd7df-146">String</span></span>|<span data-ttu-id="dd7df-147">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="dd7df-147">Human-readable name of the location.</span></span> <span data-ttu-id="dd7df-148">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="dd7df-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="dd7df-149">id</span><span class="sxs-lookup"><span data-stu-id="dd7df-149">id</span></span>|<span data-ttu-id="dd7df-150">String</span><span class="sxs-lookup"><span data-stu-id="dd7df-150">String</span></span>|<span data-ttu-id="dd7df-151">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="dd7df-151">Identifier of a namedLocation object.</span></span> <span data-ttu-id="dd7df-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd7df-152">Read-only.</span></span> <span data-ttu-id="dd7df-153">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="dd7df-153">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="dd7df-154">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="dd7df-154">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="dd7df-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd7df-155">Boolean</span></span>|<span data-ttu-id="dd7df-156">True se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.</span><span class="sxs-lookup"><span data-stu-id="dd7df-156">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="dd7df-157">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7df-157">modifiedDateTime</span></span>|<span data-ttu-id="dd7df-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7df-158">DateTimeOffset</span></span>|<span data-ttu-id="dd7df-159">O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd7df-159">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd7df-160">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dd7df-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="dd7df-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd7df-161">Read-only.</span></span> <span data-ttu-id="dd7df-162">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="dd7df-162">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd7df-163">Relações</span><span class="sxs-lookup"><span data-stu-id="dd7df-163">Relationships</span></span>

<span data-ttu-id="dd7df-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd7df-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd7df-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd7df-165">JSON representation</span></span>

<span data-ttu-id="dd7df-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd7df-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "countryLookupMethod": "String",
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
