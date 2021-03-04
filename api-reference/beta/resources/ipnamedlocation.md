---
title: Tipo de recurso ipNamedLocation
description: Representa um local nomeado pelo Azure Active Directory definido por intervalos IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7dafb55a861325c89b11c0118813f759423f3d69
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444158"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="3aa2d-104">Tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="3aa2d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa2d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aa2d-106">Representa um local nomeado pelo Azure Active Directory definido por intervalos IP.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="3aa2d-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="3aa2d-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3aa2d-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3aa2d-109">Methods</span><span class="sxs-lookup"><span data-stu-id="3aa2d-109">Methods</span></span>

| <span data-ttu-id="3aa2d-110">Método</span><span class="sxs-lookup"><span data-stu-id="3aa2d-110">Method</span></span>       | <span data-ttu-id="3aa2d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3aa2d-111">Return Type</span></span> | <span data-ttu-id="3aa2d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aa2d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3aa2d-113">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="3aa2d-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="3aa2d-114">[Coleção ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3aa2d-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="3aa2d-115">Obter todos os **objetos ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="3aa2d-116">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="3aa2d-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="3aa2d-118">Crie um novo **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="3aa2d-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3aa2d-119">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="3aa2d-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="3aa2d-121">Leia as propriedades e as relações de um **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="3aa2d-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3aa2d-122">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="3aa2d-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="3aa2d-124">Atualize um **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="3aa2d-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3aa2d-125">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="3aa2d-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="3aa2d-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="3aa2d-126">None</span></span> | <span data-ttu-id="3aa2d-127">**Exclua um objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="3aa2d-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3aa2d-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3aa2d-128">Properties</span></span>

| <span data-ttu-id="3aa2d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aa2d-129">Property</span></span>     | <span data-ttu-id="3aa2d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aa2d-130">Type</span></span>        | <span data-ttu-id="3aa2d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aa2d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3aa2d-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3aa2d-132">createdDateTime</span></span>|<span data-ttu-id="3aa2d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aa2d-133">DateTimeOffset</span></span>|<span data-ttu-id="3aa2d-134">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3aa2d-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3aa2d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-136">Read-only.</span></span> <span data-ttu-id="3aa2d-137">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3aa2d-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3aa2d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3aa2d-138">displayName</span></span>|<span data-ttu-id="3aa2d-139">String</span><span class="sxs-lookup"><span data-stu-id="3aa2d-139">String</span></span>|<span data-ttu-id="3aa2d-140">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="3aa2d-141">id</span><span class="sxs-lookup"><span data-stu-id="3aa2d-141">id</span></span>|<span data-ttu-id="3aa2d-142">String</span><span class="sxs-lookup"><span data-stu-id="3aa2d-142">String</span></span>|<span data-ttu-id="3aa2d-143">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="3aa2d-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-144">Read-only.</span></span> <span data-ttu-id="3aa2d-145">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3aa2d-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3aa2d-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="3aa2d-146">ipRanges</span></span>|<span data-ttu-id="3aa2d-147">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3aa2d-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="3aa2d-148">Lista de intervalos de endereços IP no formato CIDR IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 acessível do IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="3aa2d-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="3aa2d-149">isTrusted</span></span>|<span data-ttu-id="3aa2d-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="3aa2d-150">Boolean</span></span>|<span data-ttu-id="3aa2d-151">True se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="3aa2d-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3aa2d-152">modifiedDateTime</span></span>|<span data-ttu-id="3aa2d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aa2d-153">DateTimeOffset</span></span>|<span data-ttu-id="3aa2d-154">O tipo Timestamp representa a última data e hora modificadas do local usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3aa2d-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3aa2d-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-156">Read-only.</span></span> <span data-ttu-id="3aa2d-157">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3aa2d-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aa2d-158">Relações</span><span class="sxs-lookup"><span data-stu-id="3aa2d-158">Relationships</span></span>

<span data-ttu-id="3aa2d-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3aa2d-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aa2d-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3aa2d-160">JSON representation</span></span>

<span data-ttu-id="3aa2d-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3aa2d-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
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


