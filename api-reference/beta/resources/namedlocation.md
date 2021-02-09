---
title: Tipo de recurso namedLocation
description: Esta é a classe base que representa um local nomeado pelo Azure Active Directory. Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1e714bb949c79d65a1563fe51bb5e1f16d6d67c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156725"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="41078-104">Tipo de recurso namedLocation</span><span class="sxs-lookup"><span data-stu-id="41078-104">namedLocation resource type</span></span>

<span data-ttu-id="41078-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41078-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41078-106">Esta é a classe base que representa um local nomeado pelo Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="41078-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="41078-107">Locais nomeados são regras personalizadas que definem locais de rede que podem ser usados em uma política de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="41078-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="41078-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="41078-108">Methods</span></span>

| <span data-ttu-id="41078-109">Método</span><span class="sxs-lookup"><span data-stu-id="41078-109">Method</span></span>       | <span data-ttu-id="41078-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="41078-110">Return Type</span></span> | <span data-ttu-id="41078-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41078-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="41078-112">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="41078-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="41078-113">[Coleção namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="41078-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="41078-114">Obter todos os **objetos namedLocation** na organização.</span><span class="sxs-lookup"><span data-stu-id="41078-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="41078-115">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="41078-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="41078-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="41078-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="41078-117">Leia as propriedades e os relacionamentos de um **objeto namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="41078-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="41078-118">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="41078-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="41078-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="41078-119">None</span></span> | <span data-ttu-id="41078-120">**Exclua um objeto namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="41078-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41078-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41078-121">Properties</span></span>

| <span data-ttu-id="41078-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41078-122">Property</span></span>     | <span data-ttu-id="41078-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="41078-123">Type</span></span>        | <span data-ttu-id="41078-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="41078-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41078-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41078-125">createdDateTime</span></span>|<span data-ttu-id="41078-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41078-126">DateTimeOffset</span></span>|<span data-ttu-id="41078-127">O tipo Timestamp representa a data e a hora de criação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41078-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41078-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="41078-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="41078-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41078-129">Read-only.</span></span>|
|<span data-ttu-id="41078-130">displayName</span><span class="sxs-lookup"><span data-stu-id="41078-130">displayName</span></span>|<span data-ttu-id="41078-131">String</span><span class="sxs-lookup"><span data-stu-id="41078-131">String</span></span>|<span data-ttu-id="41078-132">Nome acessível para humanos do local.</span><span class="sxs-lookup"><span data-stu-id="41078-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="41078-133">id</span><span class="sxs-lookup"><span data-stu-id="41078-133">id</span></span>|<span data-ttu-id="41078-134">String</span><span class="sxs-lookup"><span data-stu-id="41078-134">String</span></span>|<span data-ttu-id="41078-135">Identificador de um objeto namedLocation.</span><span class="sxs-lookup"><span data-stu-id="41078-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="41078-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41078-136">Read-only.</span></span>|
|<span data-ttu-id="41078-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41078-137">modifiedDateTime</span></span>|<span data-ttu-id="41078-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41078-138">DateTimeOffset</span></span>|<span data-ttu-id="41078-139">O tipo Timestamp representa a data e a hora da última modificação do local usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="41078-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="41078-140">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="41078-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="41078-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41078-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41078-142">Relações</span><span class="sxs-lookup"><span data-stu-id="41078-142">Relationships</span></span>

<span data-ttu-id="41078-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41078-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41078-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41078-144">JSON representation</span></span>

<span data-ttu-id="41078-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41078-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


