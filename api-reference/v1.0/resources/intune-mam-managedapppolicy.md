---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8eec128ba38343683698deef64dfc78b41fc84d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025251"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="fdca4-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fdca4-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="fdca4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdca4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdca4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdca4-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="fdca4-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="fdca4-107">Methods</span><span class="sxs-lookup"><span data-stu-id="fdca4-107">Methods</span></span>
|<span data-ttu-id="fdca4-108">Método</span><span class="sxs-lookup"><span data-stu-id="fdca4-108">Method</span></span>|<span data-ttu-id="fdca4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fdca4-109">Return Type</span></span>|<span data-ttu-id="fdca4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdca4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fdca4-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="fdca4-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="fdca4-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fdca4-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="fdca4-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fdca4-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="fdca4-114">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fdca4-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="fdca4-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fdca4-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="fdca4-116">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fdca4-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="fdca4-117">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="fdca4-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="fdca4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdca4-118">None</span></span>|<span data-ttu-id="fdca4-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdca4-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fdca4-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdca4-120">Properties</span></span>
|<span data-ttu-id="fdca4-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdca4-121">Property</span></span>|<span data-ttu-id="fdca4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdca4-122">Type</span></span>|<span data-ttu-id="fdca4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdca4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdca4-124">displayName</span><span class="sxs-lookup"><span data-stu-id="fdca4-124">displayName</span></span>|<span data-ttu-id="fdca4-125">String</span><span class="sxs-lookup"><span data-stu-id="fdca4-125">String</span></span>|<span data-ttu-id="fdca4-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="fdca4-126">Policy display name.</span></span>|
|<span data-ttu-id="fdca4-127">description</span><span class="sxs-lookup"><span data-stu-id="fdca4-127">description</span></span>|<span data-ttu-id="fdca4-128">String</span><span class="sxs-lookup"><span data-stu-id="fdca4-128">String</span></span>|<span data-ttu-id="fdca4-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="fdca4-129">The policy's description.</span></span>|
|<span data-ttu-id="fdca4-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdca4-130">createdDateTime</span></span>|<span data-ttu-id="fdca4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdca4-131">DateTimeOffset</span></span>|<span data-ttu-id="fdca4-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="fdca4-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="fdca4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdca4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fdca4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdca4-134">DateTimeOffset</span></span>|<span data-ttu-id="fdca4-135">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="fdca4-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="fdca4-136">id</span><span class="sxs-lookup"><span data-stu-id="fdca4-136">id</span></span>|<span data-ttu-id="fdca4-137">String</span><span class="sxs-lookup"><span data-stu-id="fdca4-137">String</span></span>|<span data-ttu-id="fdca4-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fdca4-138">Key of the entity.</span></span>|
|<span data-ttu-id="fdca4-139">versão</span><span class="sxs-lookup"><span data-stu-id="fdca4-139">version</span></span>|<span data-ttu-id="fdca4-140">String</span><span class="sxs-lookup"><span data-stu-id="fdca4-140">String</span></span>|<span data-ttu-id="fdca4-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="fdca4-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdca4-142">Relações</span><span class="sxs-lookup"><span data-stu-id="fdca4-142">Relationships</span></span>
<span data-ttu-id="fdca4-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdca4-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdca4-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdca4-144">JSON Representation</span></span>
<span data-ttu-id="fdca4-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdca4-145">Here is a JSON representation of the resource.</span></span>
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









