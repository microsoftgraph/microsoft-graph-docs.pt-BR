---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
ms.openlocfilehash: d971f99c4f081d5b40179d406f6a50acf5812e4f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313458"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="09c9a-103">Tipo de recurso managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="09c9a-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="09c9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09c9a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09c9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09c9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09c9a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="09c9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09c9a-107">O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.</span><span class="sxs-lookup"><span data-stu-id="09c9a-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="09c9a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="09c9a-108">Methods</span></span>
|<span data-ttu-id="09c9a-109">Método</span><span class="sxs-lookup"><span data-stu-id="09c9a-109">Method</span></span>|<span data-ttu-id="09c9a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09c9a-110">Return Type</span></span>|<span data-ttu-id="09c9a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="09c9a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09c9a-112">Listar managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="09c9a-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="09c9a-113">Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="09c9a-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="09c9a-114">Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09c9a-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="09c9a-115">Obter managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="09c9a-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="09c9a-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="09c9a-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="09c9a-117">Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="09c9a-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="09c9a-118">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="09c9a-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="09c9a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09c9a-119">None</span></span>|<span data-ttu-id="09c9a-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="09c9a-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="09c9a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09c9a-121">Properties</span></span>
|<span data-ttu-id="09c9a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09c9a-122">Property</span></span>|<span data-ttu-id="09c9a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="09c9a-123">Type</span></span>|<span data-ttu-id="09c9a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="09c9a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09c9a-125">displayName</span><span class="sxs-lookup"><span data-stu-id="09c9a-125">displayName</span></span>|<span data-ttu-id="09c9a-126">String</span><span class="sxs-lookup"><span data-stu-id="09c9a-126">String</span></span>|<span data-ttu-id="09c9a-127">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="09c9a-127">Policy display name.</span></span>|
|<span data-ttu-id="09c9a-128">descrição</span><span class="sxs-lookup"><span data-stu-id="09c9a-128">description</span></span>|<span data-ttu-id="09c9a-129">String</span><span class="sxs-lookup"><span data-stu-id="09c9a-129">String</span></span>|<span data-ttu-id="09c9a-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="09c9a-130">The policy's description.</span></span>|
|<span data-ttu-id="09c9a-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09c9a-131">createdDateTime</span></span>|<span data-ttu-id="09c9a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09c9a-132">DateTimeOffset</span></span>|<span data-ttu-id="09c9a-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="09c9a-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="09c9a-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09c9a-134">lastModifiedDateTime</span></span>|<span data-ttu-id="09c9a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09c9a-135">DateTimeOffset</span></span>|<span data-ttu-id="09c9a-136">Última hora em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="09c9a-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="09c9a-137">id</span><span class="sxs-lookup"><span data-stu-id="09c9a-137">id</span></span>|<span data-ttu-id="09c9a-138">String</span><span class="sxs-lookup"><span data-stu-id="09c9a-138">String</span></span>|<span data-ttu-id="09c9a-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="09c9a-139">Key of the entity.</span></span>|
|<span data-ttu-id="09c9a-140">version</span><span class="sxs-lookup"><span data-stu-id="09c9a-140">version</span></span>|<span data-ttu-id="09c9a-141">String</span><span class="sxs-lookup"><span data-stu-id="09c9a-141">String</span></span>|<span data-ttu-id="09c9a-142">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="09c9a-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09c9a-143">Relações</span><span class="sxs-lookup"><span data-stu-id="09c9a-143">Relationships</span></span>
<span data-ttu-id="09c9a-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09c9a-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09c9a-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09c9a-145">JSON Representation</span></span>
<span data-ttu-id="09c9a-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09c9a-146">Here is a JSON representation of the resource.</span></span>
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





