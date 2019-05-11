---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aee308b24d136d7f8ee774fd8a5e41daf33e492e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940719"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="50068-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="50068-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="50068-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50068-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50068-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50068-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50068-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="50068-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="50068-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="50068-107">Methods</span></span>
|<span data-ttu-id="50068-108">Método</span><span class="sxs-lookup"><span data-stu-id="50068-108">Method</span></span>|<span data-ttu-id="50068-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50068-109">Return Type</span></span>|<span data-ttu-id="50068-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50068-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50068-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="50068-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="50068-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50068-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="50068-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="50068-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="50068-114">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="50068-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="50068-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="50068-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="50068-116">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="50068-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="50068-117">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="50068-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="50068-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50068-118">None</span></span>|<span data-ttu-id="50068-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50068-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="50068-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50068-120">Properties</span></span>
|<span data-ttu-id="50068-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50068-121">Property</span></span>|<span data-ttu-id="50068-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="50068-122">Type</span></span>|<span data-ttu-id="50068-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="50068-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50068-124">displayName</span><span class="sxs-lookup"><span data-stu-id="50068-124">displayName</span></span>|<span data-ttu-id="50068-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50068-125">String</span></span>|<span data-ttu-id="50068-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="50068-126">Policy display name.</span></span>|
|<span data-ttu-id="50068-127">description</span><span class="sxs-lookup"><span data-stu-id="50068-127">description</span></span>|<span data-ttu-id="50068-128">String</span><span class="sxs-lookup"><span data-stu-id="50068-128">String</span></span>|<span data-ttu-id="50068-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="50068-129">The policy's description.</span></span>|
|<span data-ttu-id="50068-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50068-130">createdDateTime</span></span>|<span data-ttu-id="50068-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50068-131">DateTimeOffset</span></span>|<span data-ttu-id="50068-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="50068-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="50068-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50068-133">lastModifiedDateTime</span></span>|<span data-ttu-id="50068-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50068-134">DateTimeOffset</span></span>|<span data-ttu-id="50068-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="50068-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="50068-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50068-136">roleScopeTagIds</span></span>|<span data-ttu-id="50068-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="50068-137">String collection</span></span>|<span data-ttu-id="50068-138">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="50068-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="50068-139">id</span><span class="sxs-lookup"><span data-stu-id="50068-139">id</span></span>|<span data-ttu-id="50068-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50068-140">String</span></span>|<span data-ttu-id="50068-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50068-141">Key of the entity.</span></span>|
|<span data-ttu-id="50068-142">versão</span><span class="sxs-lookup"><span data-stu-id="50068-142">version</span></span>|<span data-ttu-id="50068-143">String</span><span class="sxs-lookup"><span data-stu-id="50068-143">String</span></span>|<span data-ttu-id="50068-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="50068-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50068-145">Relações</span><span class="sxs-lookup"><span data-stu-id="50068-145">Relationships</span></span>
<span data-ttu-id="50068-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50068-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50068-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50068-147">JSON Representation</span></span>
<span data-ttu-id="50068-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50068-148">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```




