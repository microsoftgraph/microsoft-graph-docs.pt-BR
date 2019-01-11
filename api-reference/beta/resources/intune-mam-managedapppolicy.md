---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cea81d492e708c1d21039c6286fe01e70a590b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840730"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="afc3f-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="afc3f-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="afc3f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="afc3f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afc3f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="afc3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afc3f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="afc3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afc3f-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="afc3f-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="afc3f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="afc3f-108">Methods</span></span>
|<span data-ttu-id="afc3f-109">Método</span><span class="sxs-lookup"><span data-stu-id="afc3f-109">Method</span></span>|<span data-ttu-id="afc3f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="afc3f-110">Return Type</span></span>|<span data-ttu-id="afc3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="afc3f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="afc3f-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="afc3f-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="afc3f-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afc3f-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="afc3f-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afc3f-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="afc3f-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="afc3f-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="afc3f-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="afc3f-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="afc3f-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afc3f-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="afc3f-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="afc3f-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="afc3f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afc3f-119">None</span></span>|<span data-ttu-id="afc3f-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="afc3f-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="afc3f-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afc3f-121">Properties</span></span>
|<span data-ttu-id="afc3f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afc3f-122">Property</span></span>|<span data-ttu-id="afc3f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="afc3f-123">Type</span></span>|<span data-ttu-id="afc3f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="afc3f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afc3f-125">displayName</span><span class="sxs-lookup"><span data-stu-id="afc3f-125">displayName</span></span>|<span data-ttu-id="afc3f-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afc3f-126">String</span></span>|<span data-ttu-id="afc3f-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="afc3f-127">Policy display name.</span></span>|
|<span data-ttu-id="afc3f-128">descrição</span><span class="sxs-lookup"><span data-stu-id="afc3f-128">description</span></span>|<span data-ttu-id="afc3f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afc3f-129">String</span></span>|<span data-ttu-id="afc3f-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="afc3f-130">The policy's description.</span></span>|
|<span data-ttu-id="afc3f-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afc3f-131">createdDateTime</span></span>|<span data-ttu-id="afc3f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afc3f-132">DateTimeOffset</span></span>|<span data-ttu-id="afc3f-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="afc3f-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="afc3f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afc3f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="afc3f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afc3f-135">DateTimeOffset</span></span>|<span data-ttu-id="afc3f-136">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="afc3f-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="afc3f-137">id</span><span class="sxs-lookup"><span data-stu-id="afc3f-137">id</span></span>|<span data-ttu-id="afc3f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afc3f-138">String</span></span>|<span data-ttu-id="afc3f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afc3f-139">Key of the entity.</span></span>|
|<span data-ttu-id="afc3f-140">version</span><span class="sxs-lookup"><span data-stu-id="afc3f-140">version</span></span>|<span data-ttu-id="afc3f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afc3f-141">String</span></span>|<span data-ttu-id="afc3f-142">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="afc3f-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afc3f-143">Relações</span><span class="sxs-lookup"><span data-stu-id="afc3f-143">Relationships</span></span>
<span data-ttu-id="afc3f-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afc3f-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afc3f-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afc3f-145">JSON Representation</span></span>
<span data-ttu-id="afc3f-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afc3f-146">Here is a JSON representation of the resource.</span></span>
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





