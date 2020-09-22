---
title: tipo de recurso ipNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 37e5f46bf4806e402dcb527745c58c381945160a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988965"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="c3d6a-104">tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="c3d6a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3d6a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3d6a-106">Representa um local nomeado do Azure Active Directory definido por intervalos de IP.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="c3d6a-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="c3d6a-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="c3d6a-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c3d6a-109">Methods</span><span class="sxs-lookup"><span data-stu-id="c3d6a-109">Methods</span></span>

| <span data-ttu-id="c3d6a-110">Método</span><span class="sxs-lookup"><span data-stu-id="c3d6a-110">Method</span></span>       | <span data-ttu-id="c3d6a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3d6a-111">Return Type</span></span> | <span data-ttu-id="c3d6a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3d6a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c3d6a-113">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="c3d6a-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="c3d6a-114">coleção [ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="c3d6a-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="c3d6a-115">Obtenha todos os objetos **ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="c3d6a-116">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="c3d6a-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="c3d6a-118">Criar um novo objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="c3d6a-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="c3d6a-119">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="c3d6a-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="c3d6a-121">Leia as propriedades e os relacionamentos de um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="c3d6a-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="c3d6a-122">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="c3d6a-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="c3d6a-124">Atualize um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="c3d6a-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="c3d6a-125">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c3d6a-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="c3d6a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3d6a-126">None</span></span> | <span data-ttu-id="c3d6a-127">Excluir um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="c3d6a-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3d6a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3d6a-128">Properties</span></span>

| <span data-ttu-id="c3d6a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3d6a-129">Property</span></span>     | <span data-ttu-id="c3d6a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3d6a-130">Type</span></span>        | <span data-ttu-id="c3d6a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3d6a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3d6a-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3d6a-132">createdDateTime</span></span>|<span data-ttu-id="c3d6a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3d6a-133">DateTimeOffset</span></span>|<span data-ttu-id="c3d6a-134">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c3d6a-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c3d6a-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-136">Read-only.</span></span> <span data-ttu-id="c3d6a-137">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="c3d6a-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="c3d6a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c3d6a-138">displayName</span></span>|<span data-ttu-id="c3d6a-139">String</span><span class="sxs-lookup"><span data-stu-id="c3d6a-139">String</span></span>|<span data-ttu-id="c3d6a-140">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="c3d6a-141">id</span><span class="sxs-lookup"><span data-stu-id="c3d6a-141">id</span></span>|<span data-ttu-id="c3d6a-142">String</span><span class="sxs-lookup"><span data-stu-id="c3d6a-142">String</span></span>|<span data-ttu-id="c3d6a-143">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="c3d6a-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-144">Read-only.</span></span> <span data-ttu-id="c3d6a-145">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="c3d6a-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="c3d6a-146">Intervalos</span><span class="sxs-lookup"><span data-stu-id="c3d6a-146">ipRanges</span></span>|<span data-ttu-id="c3d6a-147">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c3d6a-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="c3d6a-148">Lista de intervalos de endereços IP no formato CIDR do IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="c3d6a-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="c3d6a-149">isTrusted</span></span>|<span data-ttu-id="c3d6a-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3d6a-150">Boolean</span></span>|<span data-ttu-id="c3d6a-151">True se esse local é explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="c3d6a-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3d6a-152">modifiedDateTime</span></span>|<span data-ttu-id="c3d6a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3d6a-153">DateTimeOffset</span></span>|<span data-ttu-id="c3d6a-154">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c3d6a-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c3d6a-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-156">Read-only.</span></span> <span data-ttu-id="c3d6a-157">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="c3d6a-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3d6a-158">Relações</span><span class="sxs-lookup"><span data-stu-id="c3d6a-158">Relationships</span></span>

<span data-ttu-id="c3d6a-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3d6a-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3d6a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3d6a-160">JSON representation</span></span>

<span data-ttu-id="c3d6a-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3d6a-161">The following is a JSON representation of the resource.</span></span>

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


