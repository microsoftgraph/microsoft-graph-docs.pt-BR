---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
ms.openlocfilehash: ab87690e611effa239a8471612dbb201ea6b75b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037188"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="61a94-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="61a94-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="61a94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61a94-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61a94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61a94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61a94-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61a94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61a94-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="61a94-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="61a94-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="61a94-108">Methods</span></span>
|<span data-ttu-id="61a94-109">Método</span><span class="sxs-lookup"><span data-stu-id="61a94-109">Method</span></span>|<span data-ttu-id="61a94-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61a94-110">Return Type</span></span>|<span data-ttu-id="61a94-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61a94-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61a94-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="61a94-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="61a94-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="61a94-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="61a94-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="61a94-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="61a94-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="61a94-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="61a94-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="61a94-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="61a94-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="61a94-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="61a94-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="61a94-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="61a94-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61a94-119">None</span></span>|<span data-ttu-id="61a94-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61a94-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="61a94-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61a94-121">Properties</span></span>
|<span data-ttu-id="61a94-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61a94-122">Property</span></span>|<span data-ttu-id="61a94-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="61a94-123">Type</span></span>|<span data-ttu-id="61a94-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="61a94-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61a94-125">displayName</span><span class="sxs-lookup"><span data-stu-id="61a94-125">displayName</span></span>|<span data-ttu-id="61a94-126">String</span><span class="sxs-lookup"><span data-stu-id="61a94-126">String</span></span>|<span data-ttu-id="61a94-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="61a94-127">Policy display name.</span></span>|
|<span data-ttu-id="61a94-128">descrição</span><span class="sxs-lookup"><span data-stu-id="61a94-128">description</span></span>|<span data-ttu-id="61a94-129">String</span><span class="sxs-lookup"><span data-stu-id="61a94-129">String</span></span>|<span data-ttu-id="61a94-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="61a94-130">The policy's description.</span></span>|
|<span data-ttu-id="61a94-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61a94-131">createdDateTime</span></span>|<span data-ttu-id="61a94-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61a94-132">DateTimeOffset</span></span>|<span data-ttu-id="61a94-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="61a94-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="61a94-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61a94-134">lastModifiedDateTime</span></span>|<span data-ttu-id="61a94-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61a94-135">DateTimeOffset</span></span>|<span data-ttu-id="61a94-136">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="61a94-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="61a94-137">id</span><span class="sxs-lookup"><span data-stu-id="61a94-137">id</span></span>|<span data-ttu-id="61a94-138">String</span><span class="sxs-lookup"><span data-stu-id="61a94-138">String</span></span>|<span data-ttu-id="61a94-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61a94-139">Key of the entity.</span></span>|
|<span data-ttu-id="61a94-140">version</span><span class="sxs-lookup"><span data-stu-id="61a94-140">version</span></span>|<span data-ttu-id="61a94-141">String</span><span class="sxs-lookup"><span data-stu-id="61a94-141">String</span></span>|<span data-ttu-id="61a94-142">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="61a94-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61a94-143">Relações</span><span class="sxs-lookup"><span data-stu-id="61a94-143">Relationships</span></span>
<span data-ttu-id="61a94-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61a94-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61a94-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61a94-145">JSON Representation</span></span>
<span data-ttu-id="61a94-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61a94-146">Here is a JSON representation of the resource.</span></span>
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





