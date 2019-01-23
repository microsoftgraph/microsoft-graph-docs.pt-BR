---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6bc4a7bbc4bc0dc85da8759ad95162712b1deb13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422975"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="7b9f3-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="7b9f3-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="7b9f3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b9f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b9f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b9f3-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="7b9f3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b9f3-108">Methods</span></span>
|<span data-ttu-id="7b9f3-109">Método</span><span class="sxs-lookup"><span data-stu-id="7b9f3-109">Method</span></span>|<span data-ttu-id="7b9f3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b9f3-110">Return Type</span></span>|<span data-ttu-id="7b9f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b9f3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b9f3-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="7b9f3-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="7b9f3-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7b9f3-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="7b9f3-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7b9f3-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="7b9f3-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="7b9f3-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="7b9f3-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="7b9f3-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="7b9f3-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7b9f3-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="7b9f3-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="7b9f3-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="7b9f3-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b9f3-119">None</span></span>|<span data-ttu-id="7b9f3-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7b9f3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7b9f3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b9f3-121">Properties</span></span>
|<span data-ttu-id="7b9f3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b9f3-122">Property</span></span>|<span data-ttu-id="7b9f3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b9f3-123">Type</span></span>|<span data-ttu-id="7b9f3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b9f3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b9f3-125">displayName</span><span class="sxs-lookup"><span data-stu-id="7b9f3-125">displayName</span></span>|<span data-ttu-id="7b9f3-126">String</span><span class="sxs-lookup"><span data-stu-id="7b9f3-126">String</span></span>|<span data-ttu-id="7b9f3-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-127">Policy display name.</span></span>|
|<span data-ttu-id="7b9f3-128">descrição</span><span class="sxs-lookup"><span data-stu-id="7b9f3-128">description</span></span>|<span data-ttu-id="7b9f3-129">String</span><span class="sxs-lookup"><span data-stu-id="7b9f3-129">String</span></span>|<span data-ttu-id="7b9f3-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-130">The policy's description.</span></span>|
|<span data-ttu-id="7b9f3-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9f3-131">createdDateTime</span></span>|<span data-ttu-id="7b9f3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b9f3-132">DateTimeOffset</span></span>|<span data-ttu-id="7b9f3-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="7b9f3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9f3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="7b9f3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b9f3-135">DateTimeOffset</span></span>|<span data-ttu-id="7b9f3-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="7b9f3-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b9f3-137">roleScopeTagIds</span></span>|<span data-ttu-id="7b9f3-138">String collection</span><span class="sxs-lookup"><span data-stu-id="7b9f3-138">String collection</span></span>|<span data-ttu-id="7b9f3-139">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="7b9f3-140">id</span><span class="sxs-lookup"><span data-stu-id="7b9f3-140">id</span></span>|<span data-ttu-id="7b9f3-141">String</span><span class="sxs-lookup"><span data-stu-id="7b9f3-141">String</span></span>|<span data-ttu-id="7b9f3-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-142">Key of the entity.</span></span>|
|<span data-ttu-id="7b9f3-143">version</span><span class="sxs-lookup"><span data-stu-id="7b9f3-143">version</span></span>|<span data-ttu-id="7b9f3-144">String</span><span class="sxs-lookup"><span data-stu-id="7b9f3-144">String</span></span>|<span data-ttu-id="7b9f3-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b9f3-146">Relações</span><span class="sxs-lookup"><span data-stu-id="7b9f3-146">Relationships</span></span>
<span data-ttu-id="7b9f3-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b9f3-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b9f3-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b9f3-148">JSON Representation</span></span>
<span data-ttu-id="7b9f3-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b9f3-149">Here is a JSON representation of the resource.</span></span>
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




