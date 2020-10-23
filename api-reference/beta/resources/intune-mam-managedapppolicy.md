---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 140e9541cf6719c5348e6ed06e713f5c3e0757b3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726350"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="54648-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="54648-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="54648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54648-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54648-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54648-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54648-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54648-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54648-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="54648-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="54648-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="54648-108">Methods</span></span>
|<span data-ttu-id="54648-109">Método</span><span class="sxs-lookup"><span data-stu-id="54648-109">Method</span></span>|<span data-ttu-id="54648-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="54648-110">Return Type</span></span>|<span data-ttu-id="54648-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="54648-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54648-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="54648-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="54648-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54648-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="54648-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54648-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="54648-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="54648-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="54648-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="54648-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="54648-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54648-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="54648-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="54648-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="54648-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54648-119">None</span></span>|<span data-ttu-id="54648-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54648-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="54648-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54648-121">Properties</span></span>
|<span data-ttu-id="54648-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54648-122">Property</span></span>|<span data-ttu-id="54648-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="54648-123">Type</span></span>|<span data-ttu-id="54648-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="54648-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54648-125">displayName</span><span class="sxs-lookup"><span data-stu-id="54648-125">displayName</span></span>|<span data-ttu-id="54648-126">String</span><span class="sxs-lookup"><span data-stu-id="54648-126">String</span></span>|<span data-ttu-id="54648-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="54648-127">Policy display name.</span></span>|
|<span data-ttu-id="54648-128">description</span><span class="sxs-lookup"><span data-stu-id="54648-128">description</span></span>|<span data-ttu-id="54648-129">String</span><span class="sxs-lookup"><span data-stu-id="54648-129">String</span></span>|<span data-ttu-id="54648-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="54648-130">The policy's description.</span></span>|
|<span data-ttu-id="54648-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54648-131">createdDateTime</span></span>|<span data-ttu-id="54648-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54648-132">DateTimeOffset</span></span>|<span data-ttu-id="54648-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="54648-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="54648-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54648-134">lastModifiedDateTime</span></span>|<span data-ttu-id="54648-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54648-135">DateTimeOffset</span></span>|<span data-ttu-id="54648-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="54648-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="54648-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54648-137">roleScopeTagIds</span></span>|<span data-ttu-id="54648-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54648-138">String collection</span></span>|<span data-ttu-id="54648-139">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="54648-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="54648-140">id</span><span class="sxs-lookup"><span data-stu-id="54648-140">id</span></span>|<span data-ttu-id="54648-141">String</span><span class="sxs-lookup"><span data-stu-id="54648-141">String</span></span>|<span data-ttu-id="54648-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54648-142">Key of the entity.</span></span>|
|<span data-ttu-id="54648-143">versão</span><span class="sxs-lookup"><span data-stu-id="54648-143">version</span></span>|<span data-ttu-id="54648-144">String</span><span class="sxs-lookup"><span data-stu-id="54648-144">String</span></span>|<span data-ttu-id="54648-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="54648-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54648-146">Relações</span><span class="sxs-lookup"><span data-stu-id="54648-146">Relationships</span></span>
<span data-ttu-id="54648-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54648-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54648-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54648-148">JSON Representation</span></span>
<span data-ttu-id="54648-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54648-149">Here is a JSON representation of the resource.</span></span>
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





