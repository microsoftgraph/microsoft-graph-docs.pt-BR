---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b502364cdcc461601b8790955bb93710be336e24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030267"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2fd2e-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2fd2e-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="2fd2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fd2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fd2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fd2e-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="2fd2e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2fd2e-108">Methods</span></span>
|<span data-ttu-id="2fd2e-109">Método</span><span class="sxs-lookup"><span data-stu-id="2fd2e-109">Method</span></span>|<span data-ttu-id="2fd2e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2fd2e-110">Return Type</span></span>|<span data-ttu-id="2fd2e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd2e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fd2e-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="2fd2e-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2fd2e-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fd2e-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2fd2e-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2fd2e-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2fd2e-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2fd2e-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2fd2e-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2fd2e-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2fd2e-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2fd2e-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2fd2e-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="2fd2e-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2fd2e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd2e-119">None</span></span>|<span data-ttu-id="2fd2e-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fd2e-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2fd2e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fd2e-121">Properties</span></span>
|<span data-ttu-id="2fd2e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd2e-122">Property</span></span>|<span data-ttu-id="2fd2e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd2e-123">Type</span></span>|<span data-ttu-id="2fd2e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd2e-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd2e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="2fd2e-125">displayName</span></span>|<span data-ttu-id="2fd2e-126">String</span><span class="sxs-lookup"><span data-stu-id="2fd2e-126">String</span></span>|<span data-ttu-id="2fd2e-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-127">Policy display name.</span></span>|
|<span data-ttu-id="2fd2e-128">description</span><span class="sxs-lookup"><span data-stu-id="2fd2e-128">description</span></span>|<span data-ttu-id="2fd2e-129">String</span><span class="sxs-lookup"><span data-stu-id="2fd2e-129">String</span></span>|<span data-ttu-id="2fd2e-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-130">The policy's description.</span></span>|
|<span data-ttu-id="2fd2e-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd2e-131">createdDateTime</span></span>|<span data-ttu-id="2fd2e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd2e-132">DateTimeOffset</span></span>|<span data-ttu-id="2fd2e-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2fd2e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd2e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="2fd2e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd2e-135">DateTimeOffset</span></span>|<span data-ttu-id="2fd2e-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2fd2e-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fd2e-137">roleScopeTagIds</span></span>|<span data-ttu-id="2fd2e-138">Coleção String</span><span class="sxs-lookup"><span data-stu-id="2fd2e-138">String collection</span></span>|<span data-ttu-id="2fd2e-139">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="2fd2e-140">id</span><span class="sxs-lookup"><span data-stu-id="2fd2e-140">id</span></span>|<span data-ttu-id="2fd2e-141">String</span><span class="sxs-lookup"><span data-stu-id="2fd2e-141">String</span></span>|<span data-ttu-id="2fd2e-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-142">Key of the entity.</span></span>|
|<span data-ttu-id="2fd2e-143">versão</span><span class="sxs-lookup"><span data-stu-id="2fd2e-143">version</span></span>|<span data-ttu-id="2fd2e-144">String</span><span class="sxs-lookup"><span data-stu-id="2fd2e-144">String</span></span>|<span data-ttu-id="2fd2e-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fd2e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="2fd2e-146">Relationships</span></span>
<span data-ttu-id="2fd2e-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd2e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fd2e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fd2e-148">JSON Representation</span></span>
<span data-ttu-id="2fd2e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fd2e-149">Here is a JSON representation of the resource.</span></span>
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






