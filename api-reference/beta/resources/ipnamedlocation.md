---
title: tipo de recurso ipNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10bdafb9894d822f345bb6fb23174fa7f7deee4c
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653815"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="ee842-104">tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-104">ipNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee842-105">Representa um local nomeado do Azure Active Directory definido por intervalos de IP.</span><span class="sxs-lookup"><span data-stu-id="ee842-105">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="ee842-106">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="ee842-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="ee842-107">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="ee842-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ee842-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee842-108">Methods</span></span>

| <span data-ttu-id="ee842-109">Método</span><span class="sxs-lookup"><span data-stu-id="ee842-109">Method</span></span>       | <span data-ttu-id="ee842-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee842-110">Return Type</span></span> | <span data-ttu-id="ee842-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee842-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ee842-112">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="ee842-112">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="ee842-113">coleção [ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="ee842-113">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="ee842-114">Obtenha todos os objetos **ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="ee842-114">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="ee842-115">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-115">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="ee842-116">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-116">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="ee842-117">Criar um novo objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="ee842-117">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="ee842-118">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-118">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="ee842-119">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-119">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="ee842-120">Leia as propriedades e os relacionamentos de um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="ee842-120">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="ee842-121">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-121">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="ee842-122">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-122">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="ee842-123">Atualize um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="ee842-123">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="ee842-124">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="ee842-124">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="ee842-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee842-125">None</span></span> | <span data-ttu-id="ee842-126">Excluir um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="ee842-126">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ee842-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee842-127">Properties</span></span>

| <span data-ttu-id="ee842-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee842-128">Property</span></span>     | <span data-ttu-id="ee842-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee842-129">Type</span></span>        | <span data-ttu-id="ee842-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee842-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee842-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee842-131">createdDateTime</span></span>|<span data-ttu-id="ee842-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee842-132">DateTimeOffset</span></span>|<span data-ttu-id="ee842-133">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ee842-133">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee842-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ee842-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ee842-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee842-135">Read-only.</span></span> <span data-ttu-id="ee842-136">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="ee842-136">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="ee842-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee842-137">displayName</span></span>|<span data-ttu-id="ee842-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee842-138">String</span></span>|<span data-ttu-id="ee842-139">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="ee842-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="ee842-140">id</span><span class="sxs-lookup"><span data-stu-id="ee842-140">id</span></span>|<span data-ttu-id="ee842-141">String</span><span class="sxs-lookup"><span data-stu-id="ee842-141">String</span></span>|<span data-ttu-id="ee842-142">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="ee842-142">Identifier of a namedLocation object.</span></span> <span data-ttu-id="ee842-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee842-143">Read-only.</span></span> <span data-ttu-id="ee842-144">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="ee842-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="ee842-145">Intervalos</span><span class="sxs-lookup"><span data-stu-id="ee842-145">ipRanges</span></span>|<span data-ttu-id="ee842-146">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ee842-146">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="ee842-147">Lista de intervalos de endereços IP no formato CIDR do IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="ee842-147">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="ee842-148">isTrusted</span><span class="sxs-lookup"><span data-stu-id="ee842-148">isTrusted</span></span>|<span data-ttu-id="ee842-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee842-149">Boolean</span></span>|<span data-ttu-id="ee842-150">True se esse local é explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="ee842-150">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="ee842-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee842-151">modifiedDateTime</span></span>|<span data-ttu-id="ee842-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee842-152">DateTimeOffset</span></span>|<span data-ttu-id="ee842-153">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ee842-153">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee842-154">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ee842-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ee842-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee842-155">Read-only.</span></span> <span data-ttu-id="ee842-156">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="ee842-156">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee842-157">Relações</span><span class="sxs-lookup"><span data-stu-id="ee842-157">Relationships</span></span>

<span data-ttu-id="ee842-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee842-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee842-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee842-159">JSON representation</span></span>

<span data-ttu-id="ee842-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee842-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation",
  "baseType": ""
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
