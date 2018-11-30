---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
ms.openlocfilehash: 0cd886e594e58dec3486af6d447969f1610c84fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006089"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="13b60-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="13b60-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="13b60-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13b60-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13b60-105">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="13b60-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="13b60-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="13b60-106">Methods</span></span>
|<span data-ttu-id="13b60-107">Método</span><span class="sxs-lookup"><span data-stu-id="13b60-107">Method</span></span>|<span data-ttu-id="13b60-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13b60-108">Return Type</span></span>|<span data-ttu-id="13b60-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13b60-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13b60-110">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="13b60-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="13b60-111">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="13b60-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="13b60-112">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="13b60-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="13b60-113">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="13b60-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="13b60-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="13b60-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="13b60-115">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="13b60-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="13b60-116">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="13b60-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="13b60-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13b60-117">None</span></span>|<span data-ttu-id="13b60-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="13b60-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="13b60-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13b60-119">Properties</span></span>
|<span data-ttu-id="13b60-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13b60-120">Property</span></span>|<span data-ttu-id="13b60-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="13b60-121">Type</span></span>|<span data-ttu-id="13b60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="13b60-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b60-123">displayName</span><span class="sxs-lookup"><span data-stu-id="13b60-123">displayName</span></span>|<span data-ttu-id="13b60-124">String</span><span class="sxs-lookup"><span data-stu-id="13b60-124">String</span></span>|<span data-ttu-id="13b60-125">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="13b60-125">Policy display name.</span></span>|
|<span data-ttu-id="13b60-126">descrição</span><span class="sxs-lookup"><span data-stu-id="13b60-126">description</span></span>|<span data-ttu-id="13b60-127">String</span><span class="sxs-lookup"><span data-stu-id="13b60-127">String</span></span>|<span data-ttu-id="13b60-128">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="13b60-128">The policy's description.</span></span>|
|<span data-ttu-id="13b60-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13b60-129">createdDateTime</span></span>|<span data-ttu-id="13b60-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13b60-130">DateTimeOffset</span></span>|<span data-ttu-id="13b60-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="13b60-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="13b60-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13b60-132">lastModifiedDateTime</span></span>|<span data-ttu-id="13b60-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13b60-133">DateTimeOffset</span></span>|<span data-ttu-id="13b60-134">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="13b60-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="13b60-135">id</span><span class="sxs-lookup"><span data-stu-id="13b60-135">id</span></span>|<span data-ttu-id="13b60-136">String</span><span class="sxs-lookup"><span data-stu-id="13b60-136">String</span></span>|<span data-ttu-id="13b60-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="13b60-137">Key of the entity.</span></span>|
|<span data-ttu-id="13b60-138">version</span><span class="sxs-lookup"><span data-stu-id="13b60-138">version</span></span>|<span data-ttu-id="13b60-139">String</span><span class="sxs-lookup"><span data-stu-id="13b60-139">String</span></span>|<span data-ttu-id="13b60-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="13b60-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b60-141">Relações</span><span class="sxs-lookup"><span data-stu-id="13b60-141">Relationships</span></span>
<span data-ttu-id="13b60-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13b60-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13b60-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13b60-143">JSON Representation</span></span>
<span data-ttu-id="13b60-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13b60-144">Here is a JSON representation of the resource.</span></span>
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



