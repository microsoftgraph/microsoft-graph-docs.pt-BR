---
title: Tipo de recurso tenantGroup
description: Representa um grupo lógico de locatários gerenciados.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2ab0d97afff68dca7d76b1ad6c4e461ad6af6233
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401993"
---
# <a name="tenantgroup-resource-type"></a><span data-ttu-id="cc28d-103">Tipo de recurso tenantGroup</span><span class="sxs-lookup"><span data-stu-id="cc28d-103">tenantGroup resource type</span></span>

<span data-ttu-id="cc28d-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cc28d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc28d-105">Representa um grupo lógico de locatários gerenciados.</span><span class="sxs-lookup"><span data-stu-id="cc28d-105">Represents a logical group of managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="cc28d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc28d-106">Methods</span></span>
|<span data-ttu-id="cc28d-107">Método</span><span class="sxs-lookup"><span data-stu-id="cc28d-107">Method</span></span>|<span data-ttu-id="cc28d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc28d-108">Return type</span></span>|<span data-ttu-id="cc28d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc28d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc28d-110">Listar tenantGroups</span><span class="sxs-lookup"><span data-stu-id="cc28d-110">List tenantGroups</span></span>](../api/managedtenants-managedtenant-list-tenantgroups.md)|<span data-ttu-id="cc28d-111">[coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cc28d-111">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="cc28d-112">Obter uma lista dos objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cc28d-112">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="cc28d-113">Obter tenantGroup</span><span class="sxs-lookup"><span data-stu-id="cc28d-113">Get tenantGroup</span></span>](../api/managedtenants-tenantgroup-get.md)|[<span data-ttu-id="cc28d-114">microsoft.graph.managedTenants.tenantGroup</span><span class="sxs-lookup"><span data-stu-id="cc28d-114">microsoft.graph.managedTenants.tenantGroup</span></span>](../resources/managedtenants-tenantgroup.md)|<span data-ttu-id="cc28d-115">Leia as propriedades e as relações de um [objeto tenantGroup.](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cc28d-115">Read the properties and relationships of a [tenantGroup](../resources/managedtenants-tenantgroup.md) object.</span></span>|
|[<span data-ttu-id="cc28d-116">tenantSearch</span><span class="sxs-lookup"><span data-stu-id="cc28d-116">tenantSearch</span></span>](../api/managedtenants-tenantgroup-tenantsearch.md)|<span data-ttu-id="cc28d-117">[coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cc28d-117">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="cc28d-118">Pesquisa o locatário gerenciado específico entre grupos de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-118">Searches for the specific managed tenant across tenant groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc28d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc28d-119">Properties</span></span>
|<span data-ttu-id="cc28d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc28d-120">Property</span></span>|<span data-ttu-id="cc28d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc28d-121">Type</span></span>|<span data-ttu-id="cc28d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc28d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc28d-123">allTenantsIncluded</span><span class="sxs-lookup"><span data-stu-id="cc28d-123">allTenantsIncluded</span></span>|<span data-ttu-id="cc28d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc28d-124">Boolean</span></span>|<span data-ttu-id="cc28d-125">Um sinalizador indicando se todos os locatários gerenciados estão incluídos no grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-125">A flag indicating whether all managed tenant are included in the tenant group.</span></span> <span data-ttu-id="cc28d-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc28d-126">Required.</span></span> <span data-ttu-id="cc28d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-127">Read-only.</span></span>|
|<span data-ttu-id="cc28d-128">displayName</span><span class="sxs-lookup"><span data-stu-id="cc28d-128">displayName</span></span>|<span data-ttu-id="cc28d-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc28d-129">String</span></span>|<span data-ttu-id="cc28d-130">O nome de exibição do grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-130">The display name for the tenant group.</span></span> <span data-ttu-id="cc28d-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc28d-131">Optional.</span></span> <span data-ttu-id="cc28d-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-132">Read-only.</span></span>|
|<span data-ttu-id="cc28d-133">id</span><span class="sxs-lookup"><span data-stu-id="cc28d-133">id</span></span>|<span data-ttu-id="cc28d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc28d-134">String</span></span>|<span data-ttu-id="cc28d-135">O identificador exclusivo do grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-135">The unique identifier for the tenant group.</span></span> <span data-ttu-id="cc28d-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc28d-136">Required.</span></span> <span data-ttu-id="cc28d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-137">Read-only.</span></span>|
|<span data-ttu-id="cc28d-138">managementActions</span><span class="sxs-lookup"><span data-stu-id="cc28d-138">managementActions</span></span>|<span data-ttu-id="cc28d-139">[coleção microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md)</span><span class="sxs-lookup"><span data-stu-id="cc28d-139">[microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md) collection</span></span>|<span data-ttu-id="cc28d-140">O conjunto de ações de gerenciamento associadas ao grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-140">The collection of management action associated with the tenant group.</span></span> <span data-ttu-id="cc28d-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc28d-141">Optional.</span></span> <span data-ttu-id="cc28d-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-142">Read-only.</span></span>|
|<span data-ttu-id="cc28d-143">managementIntents</span><span class="sxs-lookup"><span data-stu-id="cc28d-143">managementIntents</span></span>|<span data-ttu-id="cc28d-144">[coleção microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cc28d-144">[microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md) collection</span></span>|<span data-ttu-id="cc28d-145">A coleção de intenções de gerenciamento associadas ao grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-145">The collection of management intents associated with the tenant group.</span></span> <span data-ttu-id="cc28d-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc28d-146">Optional.</span></span> <span data-ttu-id="cc28d-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-147">Read-only.</span></span>|
|<span data-ttu-id="cc28d-148">tenantIds</span><span class="sxs-lookup"><span data-stu-id="cc28d-148">tenantIds</span></span>|<span data-ttu-id="cc28d-149">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc28d-149">String collection</span></span>|<span data-ttu-id="cc28d-150">A coleção de identificadores de locatários gerenciados inclui no grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="cc28d-150">The collection of managed tenant identifiers include in the tenant group.</span></span> <span data-ttu-id="cc28d-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc28d-151">Optional.</span></span> <span data-ttu-id="cc28d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc28d-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc28d-153">Relações</span><span class="sxs-lookup"><span data-stu-id="cc28d-153">Relationships</span></span>
<span data-ttu-id="cc28d-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc28d-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc28d-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc28d-155">JSON representation</span></span>
<span data-ttu-id="cc28d-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc28d-156">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```
