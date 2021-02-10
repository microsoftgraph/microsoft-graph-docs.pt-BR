---
title: Tipo de recurso ipNamedLocation
description: Representa um local nomeado pelo Azure Active Directory definido por intervalos de IP. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5f76d5bb27a17ec0cc642479f3808dfbc8a45f66
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159392"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="50827-104">Tipo de recurso ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="50827-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50827-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50827-106">Representa um local nomeado pelo Azure Active Directory definido por intervalos de IP.</span><span class="sxs-lookup"><span data-stu-id="50827-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="50827-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="50827-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="50827-108">Herda de [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="50827-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="50827-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="50827-109">Methods</span></span>

| <span data-ttu-id="50827-110">Método</span><span class="sxs-lookup"><span data-stu-id="50827-110">Method</span></span>       | <span data-ttu-id="50827-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50827-111">Return Type</span></span> | <span data-ttu-id="50827-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="50827-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="50827-113">Listar ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="50827-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="50827-114">[coleção ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="50827-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="50827-115">Obter todos os **objetos ipNamedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="50827-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="50827-116">Criar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="50827-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="50827-118">Criar um novo **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="50827-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="50827-119">Get ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="50827-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="50827-121">Leia as propriedades e os relacionamentos de um **objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="50827-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="50827-122">Atualizar ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="50827-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="50827-124">Atualize **um objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="50827-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="50827-125">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="50827-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="50827-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50827-126">None</span></span> | <span data-ttu-id="50827-127">**Exclua um objeto ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="50827-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="50827-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50827-128">Properties</span></span>

| <span data-ttu-id="50827-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50827-129">Property</span></span>     | <span data-ttu-id="50827-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50827-130">Type</span></span>        | <span data-ttu-id="50827-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50827-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50827-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50827-132">createdDateTime</span></span>|<span data-ttu-id="50827-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50827-133">DateTimeOffset</span></span>|<span data-ttu-id="50827-134">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="50827-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="50827-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="50827-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="50827-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50827-136">Read-only.</span></span> <span data-ttu-id="50827-137">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="50827-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="50827-138">displayName</span><span class="sxs-lookup"><span data-stu-id="50827-138">displayName</span></span>|<span data-ttu-id="50827-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50827-139">String</span></span>|<span data-ttu-id="50827-140">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="50827-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="50827-141">id</span><span class="sxs-lookup"><span data-stu-id="50827-141">id</span></span>|<span data-ttu-id="50827-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50827-142">String</span></span>|<span data-ttu-id="50827-143">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="50827-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="50827-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50827-144">Read-only.</span></span> <span data-ttu-id="50827-145">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="50827-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="50827-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="50827-146">ipRanges</span></span>|<span data-ttu-id="50827-147">Coleção [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="50827-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="50827-148">Lista de intervalos de endereços IP no formato CIDR IPv4 (por exemplo, 1.2.3.4/32) ou qualquer formato IPv6 acessível do IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="50827-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="50827-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="50827-149">isTrusted</span></span>|<span data-ttu-id="50827-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="50827-150">Boolean</span></span>|<span data-ttu-id="50827-151">True se esse local for explicitamente confiável.</span><span class="sxs-lookup"><span data-stu-id="50827-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="50827-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50827-152">modifiedDateTime</span></span>|<span data-ttu-id="50827-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50827-153">DateTimeOffset</span></span>|<span data-ttu-id="50827-154">O tipo Timestamp representa a data e a hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="50827-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="50827-155">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="50827-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="50827-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50827-156">Read-only.</span></span> <span data-ttu-id="50827-157">Herdado [de namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="50827-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="50827-158">Relações</span><span class="sxs-lookup"><span data-stu-id="50827-158">Relationships</span></span>

<span data-ttu-id="50827-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50827-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50827-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50827-160">JSON representation</span></span>

<span data-ttu-id="50827-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50827-161">The following is a JSON representation of the resource.</span></span>

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

