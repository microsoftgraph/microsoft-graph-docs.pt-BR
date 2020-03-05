---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55045faa017c852b812c04b2565269773090ee2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448379"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="e984d-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e984d-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="e984d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e984d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e984d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e984d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e984d-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="e984d-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="e984d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e984d-107">Methods</span></span>
|<span data-ttu-id="e984d-108">Método</span><span class="sxs-lookup"><span data-stu-id="e984d-108">Method</span></span>|<span data-ttu-id="e984d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e984d-109">Return Type</span></span>|<span data-ttu-id="e984d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e984d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e984d-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="e984d-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="e984d-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e984d-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e984d-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e984d-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="e984d-114">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e984d-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="e984d-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e984d-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="e984d-116">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e984d-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="e984d-117">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="e984d-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="e984d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e984d-118">None</span></span>|<span data-ttu-id="e984d-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e984d-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e984d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e984d-120">Properties</span></span>
|<span data-ttu-id="e984d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e984d-121">Property</span></span>|<span data-ttu-id="e984d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e984d-122">Type</span></span>|<span data-ttu-id="e984d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e984d-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e984d-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e984d-124">displayName</span></span>|<span data-ttu-id="e984d-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e984d-125">String</span></span>|<span data-ttu-id="e984d-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="e984d-126">Policy display name.</span></span>|
|<span data-ttu-id="e984d-127">description</span><span class="sxs-lookup"><span data-stu-id="e984d-127">description</span></span>|<span data-ttu-id="e984d-128">String</span><span class="sxs-lookup"><span data-stu-id="e984d-128">String</span></span>|<span data-ttu-id="e984d-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="e984d-129">The policy's description.</span></span>|
|<span data-ttu-id="e984d-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e984d-130">createdDateTime</span></span>|<span data-ttu-id="e984d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e984d-131">DateTimeOffset</span></span>|<span data-ttu-id="e984d-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="e984d-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="e984d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e984d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e984d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e984d-134">DateTimeOffset</span></span>|<span data-ttu-id="e984d-135">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="e984d-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="e984d-136">id</span><span class="sxs-lookup"><span data-stu-id="e984d-136">id</span></span>|<span data-ttu-id="e984d-137">String</span><span class="sxs-lookup"><span data-stu-id="e984d-137">String</span></span>|<span data-ttu-id="e984d-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e984d-138">Key of the entity.</span></span>|
|<span data-ttu-id="e984d-139">versão</span><span class="sxs-lookup"><span data-stu-id="e984d-139">version</span></span>|<span data-ttu-id="e984d-140">String</span><span class="sxs-lookup"><span data-stu-id="e984d-140">String</span></span>|<span data-ttu-id="e984d-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="e984d-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e984d-142">Relações</span><span class="sxs-lookup"><span data-stu-id="e984d-142">Relationships</span></span>
<span data-ttu-id="e984d-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e984d-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e984d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e984d-144">JSON Representation</span></span>
<span data-ttu-id="e984d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e984d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```




