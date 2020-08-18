---
title: tipo de recurso mobileAppRelationshipState
description: Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: daca7e69b70ccfecef181dd0bdd4eb381f010d87
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792699"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="00946-103">tipo de recurso mobileAppRelationshipState</span><span class="sxs-lookup"><span data-stu-id="00946-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="00946-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00946-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00946-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00946-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00946-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00946-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00946-107">Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00946-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="00946-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00946-108">Properties</span></span>
|<span data-ttu-id="00946-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00946-109">Property</span></span>|<span data-ttu-id="00946-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="00946-110">Type</span></span>|<span data-ttu-id="00946-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="00946-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00946-112">sourceIds</span><span class="sxs-lookup"><span data-stu-id="00946-112">sourceIds</span></span>|<span data-ttu-id="00946-113">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00946-113">String collection</span></span>|<span data-ttu-id="00946-114">O conjunto de IDs do aplicativo móvel de origem.</span><span class="sxs-lookup"><span data-stu-id="00946-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="00946-115">targetId</span><span class="sxs-lookup"><span data-stu-id="00946-115">targetId</span></span>|<span data-ttu-id="00946-116">String</span><span class="sxs-lookup"><span data-stu-id="00946-116">String</span></span>|<span data-ttu-id="00946-117">A ID do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="00946-117">The related target app's id.</span></span>|
|<span data-ttu-id="00946-118">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="00946-118">targetDisplayName</span></span>|<span data-ttu-id="00946-119">String</span><span class="sxs-lookup"><span data-stu-id="00946-119">String</span></span>|<span data-ttu-id="00946-120">O nome de exibição do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="00946-120">The related target app's display name.</span></span>|
|<span data-ttu-id="00946-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="00946-121">deviceId</span></span>|<span data-ttu-id="00946-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00946-122">String</span></span>|<span data-ttu-id="00946-123">A ID de dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="00946-123">The corresponding device id.</span></span>|
|<span data-ttu-id="00946-124">installState</span><span class="sxs-lookup"><span data-stu-id="00946-124">installState</span></span>|[<span data-ttu-id="00946-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="00946-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="00946-126">O estado de instalação do aplicativo do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="00946-126">The install state of the app of target app.</span></span> <span data-ttu-id="00946-127">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="00946-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="00946-128">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="00946-128">installStateDetail</span></span>|[<span data-ttu-id="00946-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="00946-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="00946-130">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00946-130">The install state detail of the app.</span></span> <span data-ttu-id="00946-131">Os valores possíveis são:,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` , `powerShellScriptRequirementNotMet` , `registryRequirementNotMet` , `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="00946-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="00946-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="00946-132">errorCode</span></span>|<span data-ttu-id="00946-133">Int32</span><span class="sxs-lookup"><span data-stu-id="00946-133">Int32</span></span>|<span data-ttu-id="00946-134">O código de erro para instalar ou desinstalar falhas do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="00946-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="00946-135">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="00946-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="00946-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00946-136">DateTimeOffset</span></span>|<span data-ttu-id="00946-137">O horário da última sincronização do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="00946-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00946-138">Relações</span><span class="sxs-lookup"><span data-stu-id="00946-138">Relationships</span></span>
<span data-ttu-id="00946-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00946-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00946-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00946-140">JSON Representation</span></span>
<span data-ttu-id="00946-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00946-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```



