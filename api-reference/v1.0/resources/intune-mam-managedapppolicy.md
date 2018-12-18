---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
ms.openlocfilehash: b1efe085bc2fc43804049ff4b091e10c458b9a98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310546"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="bdb41-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bdb41-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="bdb41-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bdb41-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdb41-105">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="bdb41-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="bdb41-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdb41-106">Methods</span></span>
|<span data-ttu-id="bdb41-107">Método</span><span class="sxs-lookup"><span data-stu-id="bdb41-107">Method</span></span>|<span data-ttu-id="bdb41-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdb41-108">Return Type</span></span>|<span data-ttu-id="bdb41-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdb41-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bdb41-110">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="bdb41-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="bdb41-111">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bdb41-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bdb41-112">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bdb41-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="bdb41-113">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bdb41-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="bdb41-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bdb41-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="bdb41-115">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bdb41-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="bdb41-116">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="bdb41-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="bdb41-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdb41-117">None</span></span>|<span data-ttu-id="bdb41-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bdb41-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bdb41-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdb41-119">Properties</span></span>
|<span data-ttu-id="bdb41-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdb41-120">Property</span></span>|<span data-ttu-id="bdb41-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdb41-121">Type</span></span>|<span data-ttu-id="bdb41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdb41-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb41-123">displayName</span><span class="sxs-lookup"><span data-stu-id="bdb41-123">displayName</span></span>|<span data-ttu-id="bdb41-124">String</span><span class="sxs-lookup"><span data-stu-id="bdb41-124">String</span></span>|<span data-ttu-id="bdb41-125">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="bdb41-125">Policy display name.</span></span>|
|<span data-ttu-id="bdb41-126">descrição</span><span class="sxs-lookup"><span data-stu-id="bdb41-126">description</span></span>|<span data-ttu-id="bdb41-127">String</span><span class="sxs-lookup"><span data-stu-id="bdb41-127">String</span></span>|<span data-ttu-id="bdb41-128">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="bdb41-128">The policy's description.</span></span>|
|<span data-ttu-id="bdb41-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdb41-129">createdDateTime</span></span>|<span data-ttu-id="bdb41-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdb41-130">DateTimeOffset</span></span>|<span data-ttu-id="bdb41-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="bdb41-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="bdb41-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdb41-132">lastModifiedDateTime</span></span>|<span data-ttu-id="bdb41-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdb41-133">DateTimeOffset</span></span>|<span data-ttu-id="bdb41-134">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="bdb41-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="bdb41-135">id</span><span class="sxs-lookup"><span data-stu-id="bdb41-135">id</span></span>|<span data-ttu-id="bdb41-136">String</span><span class="sxs-lookup"><span data-stu-id="bdb41-136">String</span></span>|<span data-ttu-id="bdb41-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdb41-137">Key of the entity.</span></span>|
|<span data-ttu-id="bdb41-138">version</span><span class="sxs-lookup"><span data-stu-id="bdb41-138">version</span></span>|<span data-ttu-id="bdb41-139">String</span><span class="sxs-lookup"><span data-stu-id="bdb41-139">String</span></span>|<span data-ttu-id="bdb41-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdb41-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdb41-141">Relações</span><span class="sxs-lookup"><span data-stu-id="bdb41-141">Relationships</span></span>
<span data-ttu-id="bdb41-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdb41-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdb41-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdb41-143">JSON Representation</span></span>
<span data-ttu-id="bdb41-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdb41-144">Here is a JSON representation of the resource.</span></span>
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



