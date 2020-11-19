---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e19b62fe5b947487a71b5df359a567fe03dce21
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302520"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="413c2-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="413c2-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="413c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="413c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="413c2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="413c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="413c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="413c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="413c2-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="413c2-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="413c2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="413c2-108">Methods</span></span>
|<span data-ttu-id="413c2-109">Método</span><span class="sxs-lookup"><span data-stu-id="413c2-109">Method</span></span>|<span data-ttu-id="413c2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="413c2-110">Return Type</span></span>|<span data-ttu-id="413c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="413c2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="413c2-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="413c2-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="413c2-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="413c2-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="413c2-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="413c2-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="413c2-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="413c2-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="413c2-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="413c2-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="413c2-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="413c2-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="413c2-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="413c2-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="413c2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="413c2-119">None</span></span>|<span data-ttu-id="413c2-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="413c2-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="413c2-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413c2-121">Properties</span></span>
|<span data-ttu-id="413c2-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413c2-122">Property</span></span>|<span data-ttu-id="413c2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="413c2-123">Type</span></span>|<span data-ttu-id="413c2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="413c2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="413c2-125">displayName</span><span class="sxs-lookup"><span data-stu-id="413c2-125">displayName</span></span>|<span data-ttu-id="413c2-126">String</span><span class="sxs-lookup"><span data-stu-id="413c2-126">String</span></span>|<span data-ttu-id="413c2-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="413c2-127">Policy display name.</span></span>|
|<span data-ttu-id="413c2-128">description</span><span class="sxs-lookup"><span data-stu-id="413c2-128">description</span></span>|<span data-ttu-id="413c2-129">String</span><span class="sxs-lookup"><span data-stu-id="413c2-129">String</span></span>|<span data-ttu-id="413c2-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="413c2-130">The policy's description.</span></span>|
|<span data-ttu-id="413c2-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="413c2-131">createdDateTime</span></span>|<span data-ttu-id="413c2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413c2-132">DateTimeOffset</span></span>|<span data-ttu-id="413c2-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="413c2-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="413c2-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="413c2-134">lastModifiedDateTime</span></span>|<span data-ttu-id="413c2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413c2-135">DateTimeOffset</span></span>|<span data-ttu-id="413c2-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="413c2-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="413c2-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="413c2-137">roleScopeTagIds</span></span>|<span data-ttu-id="413c2-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="413c2-138">String collection</span></span>|<span data-ttu-id="413c2-139">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="413c2-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="413c2-140">id</span><span class="sxs-lookup"><span data-stu-id="413c2-140">id</span></span>|<span data-ttu-id="413c2-141">String</span><span class="sxs-lookup"><span data-stu-id="413c2-141">String</span></span>|<span data-ttu-id="413c2-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="413c2-142">Key of the entity.</span></span>|
|<span data-ttu-id="413c2-143">versão</span><span class="sxs-lookup"><span data-stu-id="413c2-143">version</span></span>|<span data-ttu-id="413c2-144">String</span><span class="sxs-lookup"><span data-stu-id="413c2-144">String</span></span>|<span data-ttu-id="413c2-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="413c2-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="413c2-146">Relações</span><span class="sxs-lookup"><span data-stu-id="413c2-146">Relationships</span></span>
<span data-ttu-id="413c2-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="413c2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="413c2-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413c2-148">JSON Representation</span></span>
<span data-ttu-id="413c2-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413c2-149">Here is a JSON representation of the resource.</span></span>
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




