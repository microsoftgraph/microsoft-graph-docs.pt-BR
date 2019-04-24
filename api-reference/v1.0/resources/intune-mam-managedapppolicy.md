---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465339"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="cae63-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cae63-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="cae63-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cae63-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cae63-105">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="cae63-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="cae63-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cae63-106">Methods</span></span>
|<span data-ttu-id="cae63-107">Método</span><span class="sxs-lookup"><span data-stu-id="cae63-107">Method</span></span>|<span data-ttu-id="cae63-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cae63-108">Return Type</span></span>|<span data-ttu-id="cae63-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae63-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cae63-110">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="cae63-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="cae63-111">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cae63-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cae63-112">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae63-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="cae63-113">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cae63-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="cae63-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cae63-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="cae63-115">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cae63-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="cae63-116">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="cae63-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="cae63-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cae63-117">None</span></span>|<span data-ttu-id="cae63-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cae63-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cae63-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cae63-119">Properties</span></span>
|<span data-ttu-id="cae63-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cae63-120">Property</span></span>|<span data-ttu-id="cae63-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cae63-121">Type</span></span>|<span data-ttu-id="cae63-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae63-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae63-123">displayName</span><span class="sxs-lookup"><span data-stu-id="cae63-123">displayName</span></span>|<span data-ttu-id="cae63-124">String</span><span class="sxs-lookup"><span data-stu-id="cae63-124">String</span></span>|<span data-ttu-id="cae63-125">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="cae63-125">Policy display name.</span></span>|
|<span data-ttu-id="cae63-126">description</span><span class="sxs-lookup"><span data-stu-id="cae63-126">description</span></span>|<span data-ttu-id="cae63-127">String</span><span class="sxs-lookup"><span data-stu-id="cae63-127">String</span></span>|<span data-ttu-id="cae63-128">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="cae63-128">The policy's description.</span></span>|
|<span data-ttu-id="cae63-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cae63-129">createdDateTime</span></span>|<span data-ttu-id="cae63-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae63-130">DateTimeOffset</span></span>|<span data-ttu-id="cae63-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="cae63-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="cae63-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cae63-132">lastModifiedDateTime</span></span>|<span data-ttu-id="cae63-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae63-133">DateTimeOffset</span></span>|<span data-ttu-id="cae63-134">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="cae63-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="cae63-135">id</span><span class="sxs-lookup"><span data-stu-id="cae63-135">id</span></span>|<span data-ttu-id="cae63-136">String</span><span class="sxs-lookup"><span data-stu-id="cae63-136">String</span></span>|<span data-ttu-id="cae63-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cae63-137">Key of the entity.</span></span>|
|<span data-ttu-id="cae63-138">versão</span><span class="sxs-lookup"><span data-stu-id="cae63-138">version</span></span>|<span data-ttu-id="cae63-139">String</span><span class="sxs-lookup"><span data-stu-id="cae63-139">String</span></span>|<span data-ttu-id="cae63-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="cae63-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae63-141">Relações</span><span class="sxs-lookup"><span data-stu-id="cae63-141">Relationships</span></span>
<span data-ttu-id="cae63-142">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cae63-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cae63-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cae63-143">JSON Representation</span></span>
<span data-ttu-id="cae63-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cae63-144">Here is a JSON representation of the resource.</span></span>
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



