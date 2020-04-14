---
title: tipo de recurso mobileAppRelationshipState
description: Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 31c96fc196de529a15c5ce69f9587dcff21d0e99
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462572"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="a5b14-103">tipo de recurso mobileAppRelationshipState</span><span class="sxs-lookup"><span data-stu-id="a5b14-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="a5b14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5b14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5b14-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5b14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5b14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5b14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5b14-107">Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5b14-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="a5b14-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5b14-108">Properties</span></span>
|<span data-ttu-id="a5b14-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5b14-109">Property</span></span>|<span data-ttu-id="a5b14-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5b14-110">Type</span></span>|<span data-ttu-id="a5b14-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5b14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b14-112">sourceIds</span><span class="sxs-lookup"><span data-stu-id="a5b14-112">sourceIds</span></span>|<span data-ttu-id="a5b14-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5b14-113">String collection</span></span>|<span data-ttu-id="a5b14-114">O conjunto de IDs do aplicativo móvel de origem.</span><span class="sxs-lookup"><span data-stu-id="a5b14-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="a5b14-115">targetId</span><span class="sxs-lookup"><span data-stu-id="a5b14-115">targetId</span></span>|<span data-ttu-id="a5b14-116">String</span><span class="sxs-lookup"><span data-stu-id="a5b14-116">String</span></span>|<span data-ttu-id="a5b14-117">A ID do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="a5b14-117">The related target app's id.</span></span>|
|<span data-ttu-id="a5b14-118">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="a5b14-118">targetDisplayName</span></span>|<span data-ttu-id="a5b14-119">String</span><span class="sxs-lookup"><span data-stu-id="a5b14-119">String</span></span>|<span data-ttu-id="a5b14-120">O nome de exibição do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="a5b14-120">The related target app's display name.</span></span>|
|<span data-ttu-id="a5b14-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="a5b14-121">deviceId</span></span>|<span data-ttu-id="a5b14-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5b14-122">String</span></span>|<span data-ttu-id="a5b14-123">A ID de dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="a5b14-123">The corresponding device id.</span></span>|
|<span data-ttu-id="a5b14-124">installState</span><span class="sxs-lookup"><span data-stu-id="a5b14-124">installState</span></span>|[<span data-ttu-id="a5b14-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="a5b14-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="a5b14-126">O estado de instalação do aplicativo do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="a5b14-126">The install state of the app of target app.</span></span> <span data-ttu-id="a5b14-127">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a5b14-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="a5b14-128">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="a5b14-128">installStateDetail</span></span>|[<span data-ttu-id="a5b14-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="a5b14-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="a5b14-130">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a5b14-130">The install state detail of the app.</span></span> <span data-ttu-id="a5b14-131">Os valores possíveis são: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a5b14-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="a5b14-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="a5b14-132">errorCode</span></span>|<span data-ttu-id="a5b14-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b14-133">Int32</span></span>|<span data-ttu-id="a5b14-134">O código de erro para instalar ou desinstalar falhas do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="a5b14-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="a5b14-135">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a5b14-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="a5b14-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5b14-136">DateTimeOffset</span></span>|<span data-ttu-id="a5b14-137">O horário da última sincronização do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="a5b14-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5b14-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a5b14-138">Relationships</span></span>
<span data-ttu-id="a5b14-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5b14-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5b14-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5b14-140">JSON Representation</span></span>
<span data-ttu-id="a5b14-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5b14-141">Here is a JSON representation of the resource.</span></span>
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



