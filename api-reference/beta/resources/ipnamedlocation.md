---
title: tipo de recurso ipNamedLocation
description: Representa um local nomeado do Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2d08de5438e85ce18cb9a78da0213a9b07fa104
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917563"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="0b388-104">tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="0b388-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b388-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b388-106">Representa um local nomeado do Azure Active Directory definido por intervalos de IP.</span><span class="sxs-lookup"><span data-stu-id="0b388-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="0b388-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="0b388-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="0b388-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0b388-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0b388-109">Methods</span><span class="sxs-lookup"><span data-stu-id="0b388-109">Methods</span></span>

| <span data-ttu-id="0b388-110">Método</span><span class="sxs-lookup"><span data-stu-id="0b388-110">Method</span></span>       | <span data-ttu-id="0b388-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b388-111">Return Type</span></span> | <span data-ttu-id="0b388-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b388-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0b388-113">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="0b388-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0b388-114">coleção [ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0b388-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="0b388-115">Obtenha todos os objetos **ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="0b388-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0b388-116">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="0b388-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="0b388-118">Criar um novo objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="0b388-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0b388-119">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="0b388-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0b388-121">Leia as propriedades e os relacionamentos de um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="0b388-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0b388-122">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="0b388-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0b388-124">Atualize um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="0b388-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0b388-125">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0b388-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="0b388-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b388-126">None</span></span> | <span data-ttu-id="0b388-127">Excluir um objeto **ipNamedLocation** .</span><span class="sxs-lookup"><span data-stu-id="0b388-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b388-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b388-128">Properties</span></span>

| <span data-ttu-id="0b388-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b388-129">Property</span></span>     | <span data-ttu-id="0b388-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b388-130">Type</span></span>        | <span data-ttu-id="0b388-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b388-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b388-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b388-132">createdDateTime</span></span>|<span data-ttu-id="0b388-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b388-133">DateTimeOffset</span></span>|<span data-ttu-id="0b388-134">O tipo TIMESTAMP representa data e hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0b388-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b388-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0b388-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0b388-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b388-136">Read-only.</span></span> <span data-ttu-id="0b388-137">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0b388-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0b388-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0b388-138">displayName</span></span>|<span data-ttu-id="0b388-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b388-139">String</span></span>|<span data-ttu-id="0b388-140">Nome legível do local.</span><span class="sxs-lookup"><span data-stu-id="0b388-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0b388-141">id</span><span class="sxs-lookup"><span data-stu-id="0b388-141">id</span></span>|<span data-ttu-id="0b388-142">String</span><span class="sxs-lookup"><span data-stu-id="0b388-142">String</span></span>|<span data-ttu-id="0b388-143">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="0b388-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0b388-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b388-144">Read-only.</span></span> <span data-ttu-id="0b388-145">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0b388-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0b388-146">Intervalos</span><span class="sxs-lookup"><span data-stu-id="0b388-146">ipRanges</span></span>|<span data-ttu-id="0b388-147">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0b388-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="0b388-148">Lista de intervalos de endereços IP no formato CIDR do IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 permitido da IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="0b388-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="0b388-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="0b388-149">isTrusted</span></span>|<span data-ttu-id="0b388-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b388-150">Boolean</span></span>|<span data-ttu-id="0b388-151">True se esse local é explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="0b388-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="0b388-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b388-152">modifiedDateTime</span></span>|<span data-ttu-id="0b388-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b388-153">DateTimeOffset</span></span>|<span data-ttu-id="0b388-154">O tipo TIMESTAMP representa data e hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0b388-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b388-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0b388-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0b388-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b388-156">Read-only.</span></span> <span data-ttu-id="0b388-157">Herdado de [namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0b388-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b388-158">Relações</span><span class="sxs-lookup"><span data-stu-id="0b388-158">Relationships</span></span>

<span data-ttu-id="0b388-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b388-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b388-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b388-160">JSON representation</span></span>

<span data-ttu-id="0b388-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b388-161">The following is a JSON representation of the resource.</span></span>

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
