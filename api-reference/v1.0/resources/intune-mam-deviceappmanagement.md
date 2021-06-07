---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton de gerenciamento de aplicativos do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8906e96a0218360bbe78d1c08dd4d8767568775
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751775"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="1a4b3-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1a4b3-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="1a4b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a4b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a4b3-106">Entidade singleton de gerenciamento de aplicativos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-106">Device app management singleton entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1a4b3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a4b3-107">Methods</span></span>
|<span data-ttu-id="1a4b3-108">Método</span><span class="sxs-lookup"><span data-stu-id="1a4b3-108">Method</span></span>|<span data-ttu-id="1a4b3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a4b3-109">Return Type</span></span>|<span data-ttu-id="1a4b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4b3-110">Description</span></span>|
|:---|:---|:---|

## <a name="properties"></a><span data-ttu-id="1a4b3-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a4b3-111">Properties</span></span>
|<span data-ttu-id="1a4b3-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a4b3-112">Property</span></span>|<span data-ttu-id="1a4b3-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a4b3-113">Type</span></span>|<span data-ttu-id="1a4b3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4b3-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a4b3-115">id</span><span class="sxs-lookup"><span data-stu-id="1a4b3-115">id</span></span>|<span data-ttu-id="1a4b3-116">String</span><span class="sxs-lookup"><span data-stu-id="1a4b3-116">String</span></span>|<span data-ttu-id="1a4b3-117">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-117">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a4b3-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1a4b3-118">Relationships</span></span>
|<span data-ttu-id="1a4b3-119">Relação</span><span class="sxs-lookup"><span data-stu-id="1a4b3-119">Relationship</span></span>|<span data-ttu-id="1a4b3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a4b3-120">Type</span></span>|<span data-ttu-id="1a4b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4b3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a4b3-122">managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="1a4b3-122">managedAppPolicies</span></span>|<span data-ttu-id="1a4b3-123">Coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-123">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="1a4b3-124">Políticas de aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-124">Managed app policies.</span></span>|
|<span data-ttu-id="1a4b3-125">iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="1a4b3-125">iosManagedAppProtections</span></span>|<span data-ttu-id="1a4b3-126">Coleção [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-126">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) collection</span></span>|<span data-ttu-id="1a4b3-127">Políticas de aplicativos gerenciados para iOS.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-127">iOS managed app policies.</span></span>|
|<span data-ttu-id="1a4b3-128">androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="1a4b3-128">androidManagedAppProtections</span></span>|<span data-ttu-id="1a4b3-129">Coleção [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-129">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) collection</span></span>|<span data-ttu-id="1a4b3-130">Políticas de aplicativos gerenciados para Android.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-130">Android managed app policies.</span></span>|
|<span data-ttu-id="1a4b3-131">defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="1a4b3-131">defaultManagedAppProtections</span></span>|<span data-ttu-id="1a4b3-132">Coleção [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-132">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) collection</span></span>|<span data-ttu-id="1a4b3-133">Políticas de aplicativos gerenciados padrão.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-133">Default managed app policies.</span></span>|
|<span data-ttu-id="1a4b3-134">targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a4b3-134">targetedManagedAppConfigurations</span></span>|<span data-ttu-id="1a4b3-135">Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-135">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="1a4b3-136">Configurações de aplicativos gerenciados direcionadas.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-136">Targeted managed app configurations.</span></span>|
|<span data-ttu-id="1a4b3-137">mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="1a4b3-137">mdmWindowsInformationProtectionPolicies</span></span>|<span data-ttu-id="1a4b3-138">Coleção [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-138">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="1a4b3-139">Proteção de informações do Windows para aplicativos em execução em dispositivos que estão registrados no MDM.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-139">Windows information protection for apps running on devices which are MDM enrolled.</span></span>|
|<span data-ttu-id="1a4b3-140">windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="1a4b3-140">windowsInformationProtectionPolicies</span></span>|<span data-ttu-id="1a4b3-141">Coleção [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-141">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="1a4b3-142">Proteção de informações do Windows para aplicativos em execução em dispositivos que não estão registrados no MDM.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-142">Windows information protection for apps running on devices which are not MDM enrolled.</span></span>|
|<span data-ttu-id="1a4b3-143">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="1a4b3-143">managedAppRegistrations</span></span>|<span data-ttu-id="1a4b3-144">Coleção [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-144">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="1a4b3-145">Os registros de aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-145">The managed app registrations.</span></span>|
|<span data-ttu-id="1a4b3-146">managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="1a4b3-146">managedAppStatuses</span></span>|<span data-ttu-id="1a4b3-147">Coleção [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1a4b3-147">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="1a4b3-148">Os status de aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-148">The managed app statuses.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a4b3-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a4b3-149">JSON Representation</span></span>
<span data-ttu-id="1a4b3-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a4b3-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




