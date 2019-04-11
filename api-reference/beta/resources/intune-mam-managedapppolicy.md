---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 610012b216a0fe924af3cd4f08fb3928e504454b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798856"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="f2028-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="f2028-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="f2028-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2028-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2028-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2028-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2028-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="f2028-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="f2028-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2028-107">Methods</span></span>
|<span data-ttu-id="f2028-108">Método</span><span class="sxs-lookup"><span data-stu-id="f2028-108">Method</span></span>|<span data-ttu-id="f2028-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2028-109">Return Type</span></span>|<span data-ttu-id="f2028-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2028-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2028-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="f2028-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="f2028-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f2028-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f2028-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f2028-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="f2028-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="f2028-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="f2028-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="f2028-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="f2028-116">Ler propriedades e relações do objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f2028-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="f2028-117">ação targetApps</span><span class="sxs-lookup"><span data-stu-id="f2028-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="f2028-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f2028-118">None</span></span>|<span data-ttu-id="f2028-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2028-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f2028-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2028-120">Properties</span></span>
|<span data-ttu-id="f2028-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2028-121">Property</span></span>|<span data-ttu-id="f2028-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2028-122">Type</span></span>|<span data-ttu-id="f2028-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2028-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2028-124">displayName</span><span class="sxs-lookup"><span data-stu-id="f2028-124">displayName</span></span>|<span data-ttu-id="f2028-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2028-125">String</span></span>|<span data-ttu-id="f2028-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="f2028-126">Policy display name.</span></span>|
|<span data-ttu-id="f2028-127">description</span><span class="sxs-lookup"><span data-stu-id="f2028-127">description</span></span>|<span data-ttu-id="f2028-128">String</span><span class="sxs-lookup"><span data-stu-id="f2028-128">String</span></span>|<span data-ttu-id="f2028-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="f2028-129">The policy's description.</span></span>|
|<span data-ttu-id="f2028-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2028-130">createdDateTime</span></span>|<span data-ttu-id="f2028-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2028-131">DateTimeOffset</span></span>|<span data-ttu-id="f2028-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="f2028-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="f2028-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2028-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f2028-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2028-134">DateTimeOffset</span></span>|<span data-ttu-id="f2028-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="f2028-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="f2028-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2028-136">roleScopeTagIds</span></span>|<span data-ttu-id="f2028-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f2028-137">String collection</span></span>|<span data-ttu-id="f2028-138">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f2028-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="f2028-139">id</span><span class="sxs-lookup"><span data-stu-id="f2028-139">id</span></span>|<span data-ttu-id="f2028-140">String</span><span class="sxs-lookup"><span data-stu-id="f2028-140">String</span></span>|<span data-ttu-id="f2028-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2028-141">Key of the entity.</span></span>|
|<span data-ttu-id="f2028-142">versão</span><span class="sxs-lookup"><span data-stu-id="f2028-142">version</span></span>|<span data-ttu-id="f2028-143">String</span><span class="sxs-lookup"><span data-stu-id="f2028-143">String</span></span>|<span data-ttu-id="f2028-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2028-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2028-145">Relações</span><span class="sxs-lookup"><span data-stu-id="f2028-145">Relationships</span></span>
<span data-ttu-id="f2028-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f2028-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2028-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2028-147">JSON Representation</span></span>
<span data-ttu-id="f2028-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2028-148">Here is a JSON representation of the resource.</span></span>
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





