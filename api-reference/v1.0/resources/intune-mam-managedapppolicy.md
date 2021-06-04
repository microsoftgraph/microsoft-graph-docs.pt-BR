---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61fedfab47ee44d187d2de81c0699885c4af06f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752774"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="5b70b-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5b70b-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="5b70b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b70b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b70b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b70b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b70b-106">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="5b70b-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="5b70b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5b70b-107">Methods</span></span>
|<span data-ttu-id="5b70b-108">Método</span><span class="sxs-lookup"><span data-stu-id="5b70b-108">Method</span></span>|<span data-ttu-id="5b70b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b70b-109">Return Type</span></span>|<span data-ttu-id="5b70b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b70b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b70b-111">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="5b70b-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="5b70b-112">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5b70b-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5b70b-113">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b70b-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="5b70b-114">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5b70b-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="5b70b-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5b70b-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="5b70b-116">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b70b-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="5b70b-117">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="5b70b-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="5b70b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b70b-118">None</span></span>|<span data-ttu-id="5b70b-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b70b-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5b70b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b70b-120">Properties</span></span>
|<span data-ttu-id="5b70b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b70b-121">Property</span></span>|<span data-ttu-id="5b70b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b70b-122">Type</span></span>|<span data-ttu-id="5b70b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b70b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b70b-124">displayName</span><span class="sxs-lookup"><span data-stu-id="5b70b-124">displayName</span></span>|<span data-ttu-id="5b70b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b70b-125">String</span></span>|<span data-ttu-id="5b70b-126">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="5b70b-126">Policy display name.</span></span>|
|<span data-ttu-id="5b70b-127">descrição</span><span class="sxs-lookup"><span data-stu-id="5b70b-127">description</span></span>|<span data-ttu-id="5b70b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b70b-128">String</span></span>|<span data-ttu-id="5b70b-129">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="5b70b-129">The policy's description.</span></span>|
|<span data-ttu-id="5b70b-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b70b-130">createdDateTime</span></span>|<span data-ttu-id="5b70b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b70b-131">DateTimeOffset</span></span>|<span data-ttu-id="5b70b-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="5b70b-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="5b70b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b70b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5b70b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b70b-134">DateTimeOffset</span></span>|<span data-ttu-id="5b70b-135">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="5b70b-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="5b70b-136">id</span><span class="sxs-lookup"><span data-stu-id="5b70b-136">id</span></span>|<span data-ttu-id="5b70b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b70b-137">String</span></span>|<span data-ttu-id="5b70b-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b70b-138">Key of the entity.</span></span>|
|<span data-ttu-id="5b70b-139">versão</span><span class="sxs-lookup"><span data-stu-id="5b70b-139">version</span></span>|<span data-ttu-id="5b70b-140">String</span><span class="sxs-lookup"><span data-stu-id="5b70b-140">String</span></span>|<span data-ttu-id="5b70b-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b70b-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b70b-142">Relações</span><span class="sxs-lookup"><span data-stu-id="5b70b-142">Relationships</span></span>
<span data-ttu-id="5b70b-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5b70b-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b70b-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b70b-144">JSON Representation</span></span>
<span data-ttu-id="5b70b-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b70b-145">Here is a JSON representation of the resource.</span></span>
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




