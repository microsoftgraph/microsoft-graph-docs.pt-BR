---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c050415fc9402bdeb064ca6426bfe291e790940b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994745"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2917f-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2917f-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2917f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2917f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2917f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2917f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2917f-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="2917f-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="2917f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2917f-107">Methods</span></span>
|<span data-ttu-id="2917f-108">Método</span><span class="sxs-lookup"><span data-stu-id="2917f-108">Method</span></span>|<span data-ttu-id="2917f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2917f-109">Return Type</span></span>|<span data-ttu-id="2917f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2917f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2917f-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="2917f-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2917f-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2917f-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2917f-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2917f-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2917f-114">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2917f-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2917f-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2917f-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2917f-116">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2917f-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2917f-117">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="2917f-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2917f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2917f-118">None</span></span>|<span data-ttu-id="2917f-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2917f-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2917f-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2917f-120">Properties</span></span>
|<span data-ttu-id="2917f-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2917f-121">Property</span></span>|<span data-ttu-id="2917f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2917f-122">Type</span></span>|<span data-ttu-id="2917f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2917f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2917f-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2917f-124">displayName</span></span>|<span data-ttu-id="2917f-125">String</span><span class="sxs-lookup"><span data-stu-id="2917f-125">String</span></span>|<span data-ttu-id="2917f-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="2917f-126">Policy display name.</span></span>|
|<span data-ttu-id="2917f-127">descrição</span><span class="sxs-lookup"><span data-stu-id="2917f-127">description</span></span>|<span data-ttu-id="2917f-128">String</span><span class="sxs-lookup"><span data-stu-id="2917f-128">String</span></span>|<span data-ttu-id="2917f-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2917f-129">The policy's description.</span></span>|
|<span data-ttu-id="2917f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2917f-130">createdDateTime</span></span>|<span data-ttu-id="2917f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2917f-131">DateTimeOffset</span></span>|<span data-ttu-id="2917f-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="2917f-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2917f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2917f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2917f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2917f-134">DateTimeOffset</span></span>|<span data-ttu-id="2917f-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="2917f-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2917f-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2917f-136">roleScopeTagIds</span></span>|<span data-ttu-id="2917f-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2917f-137">String collection</span></span>|<span data-ttu-id="2917f-138">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2917f-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="2917f-139">id</span><span class="sxs-lookup"><span data-stu-id="2917f-139">id</span></span>|<span data-ttu-id="2917f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2917f-140">String</span></span>|<span data-ttu-id="2917f-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2917f-141">Key of the entity.</span></span>|
|<span data-ttu-id="2917f-142">versão</span><span class="sxs-lookup"><span data-stu-id="2917f-142">version</span></span>|<span data-ttu-id="2917f-143">String</span><span class="sxs-lookup"><span data-stu-id="2917f-143">String</span></span>|<span data-ttu-id="2917f-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="2917f-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2917f-145">Relações</span><span class="sxs-lookup"><span data-stu-id="2917f-145">Relationships</span></span>
<span data-ttu-id="2917f-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2917f-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2917f-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2917f-147">JSON Representation</span></span>
<span data-ttu-id="2917f-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2917f-148">Here is a JSON representation of the resource.</span></span>
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





