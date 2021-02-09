---
title: Tipo de recurso ipNamedLocation
description: Representa um local nomeado pelo Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b63452ca6eefb9ad3a0d4b3f860fb1a8d41638fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158398"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="0f4bb-104">Tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="0f4bb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4bb-106">Representa um local nomeado pelo Azure Active Directory definido por intervalos de IP.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="0f4bb-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="0f4bb-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0f4bb-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0f4bb-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f4bb-109">Methods</span></span>

| <span data-ttu-id="0f4bb-110">Método</span><span class="sxs-lookup"><span data-stu-id="0f4bb-110">Method</span></span>       | <span data-ttu-id="0f4bb-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f4bb-111">Return Type</span></span> | <span data-ttu-id="0f4bb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4bb-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0f4bb-113">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="0f4bb-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0f4bb-114">[Coleção ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0f4bb-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="0f4bb-115">Obter todos os **objetos ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0f4bb-116">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="0f4bb-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="0f4bb-118">Criar um novo **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="0f4bb-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0f4bb-119">Get ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="0f4bb-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0f4bb-121">Leia as propriedades e os relacionamentos de um **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="0f4bb-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0f4bb-122">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="0f4bb-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="0f4bb-124">Atualize **um objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="0f4bb-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="0f4bb-125">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0f4bb-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="0f4bb-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0f4bb-126">None</span></span> | <span data-ttu-id="0f4bb-127">**Exclua um objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="0f4bb-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f4bb-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f4bb-128">Properties</span></span>

| <span data-ttu-id="0f4bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f4bb-129">Property</span></span>     | <span data-ttu-id="0f4bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f4bb-130">Type</span></span>        | <span data-ttu-id="0f4bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4bb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f4bb-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f4bb-132">createdDateTime</span></span>|<span data-ttu-id="0f4bb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4bb-133">DateTimeOffset</span></span>|<span data-ttu-id="0f4bb-134">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f4bb-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0f4bb-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-136">Read-only.</span></span> <span data-ttu-id="0f4bb-137">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0f4bb-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0f4bb-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0f4bb-138">displayName</span></span>|<span data-ttu-id="0f4bb-139">String</span><span class="sxs-lookup"><span data-stu-id="0f4bb-139">String</span></span>|<span data-ttu-id="0f4bb-140">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0f4bb-141">id</span><span class="sxs-lookup"><span data-stu-id="0f4bb-141">id</span></span>|<span data-ttu-id="0f4bb-142">String</span><span class="sxs-lookup"><span data-stu-id="0f4bb-142">String</span></span>|<span data-ttu-id="0f4bb-143">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0f4bb-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-144">Read-only.</span></span> <span data-ttu-id="0f4bb-145">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0f4bb-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="0f4bb-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="0f4bb-146">ipRanges</span></span>|<span data-ttu-id="0f4bb-147">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0f4bb-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="0f4bb-148">Lista de intervalos de endereços IP no formato CIDR IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 acessível do IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="0f4bb-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="0f4bb-149">isTrusted</span></span>|<span data-ttu-id="0f4bb-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f4bb-150">Boolean</span></span>|<span data-ttu-id="0f4bb-151">True se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="0f4bb-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f4bb-152">modifiedDateTime</span></span>|<span data-ttu-id="0f4bb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4bb-153">DateTimeOffset</span></span>|<span data-ttu-id="0f4bb-154">O tipo Timestamp representa a data e a hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f4bb-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0f4bb-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-156">Read-only.</span></span> <span data-ttu-id="0f4bb-157">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="0f4bb-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4bb-158">Relações</span><span class="sxs-lookup"><span data-stu-id="0f4bb-158">Relationships</span></span>

<span data-ttu-id="0f4bb-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f4bb-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f4bb-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f4bb-160">JSON representation</span></span>

<span data-ttu-id="0f4bb-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f4bb-161">The following is a JSON representation of the resource.</span></span>

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


