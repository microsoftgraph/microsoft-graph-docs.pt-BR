---
title: tipo de recurso mobileAppRelationshipState
description: Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6013482fe69aa7a4ccf789c677ef448e0a277991
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993351"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="53e13-103">tipo de recurso mobileAppRelationshipState</span><span class="sxs-lookup"><span data-stu-id="53e13-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="53e13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53e13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53e13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e13-106">Descreve os detalhes de status da instalação do aplicativo filho no contexto de UPN e ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53e13-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="53e13-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53e13-107">Properties</span></span>
|<span data-ttu-id="53e13-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53e13-108">Property</span></span>|<span data-ttu-id="53e13-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53e13-109">Type</span></span>|<span data-ttu-id="53e13-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53e13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e13-111">sourceIds</span><span class="sxs-lookup"><span data-stu-id="53e13-111">sourceIds</span></span>|<span data-ttu-id="53e13-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53e13-112">String collection</span></span>|<span data-ttu-id="53e13-113">O conjunto de IDs do aplicativo móvel de origem.</span><span class="sxs-lookup"><span data-stu-id="53e13-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="53e13-114">targetId</span><span class="sxs-lookup"><span data-stu-id="53e13-114">targetId</span></span>|<span data-ttu-id="53e13-115">String</span><span class="sxs-lookup"><span data-stu-id="53e13-115">String</span></span>|<span data-ttu-id="53e13-116">A ID do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="53e13-116">The related target app's id.</span></span>|
|<span data-ttu-id="53e13-117">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="53e13-117">targetDisplayName</span></span>|<span data-ttu-id="53e13-118">String</span><span class="sxs-lookup"><span data-stu-id="53e13-118">String</span></span>|<span data-ttu-id="53e13-119">O nome de exibição do aplicativo de destino relacionado.</span><span class="sxs-lookup"><span data-stu-id="53e13-119">The related target app's display name.</span></span>|
|<span data-ttu-id="53e13-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="53e13-120">deviceId</span></span>|<span data-ttu-id="53e13-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53e13-121">String</span></span>|<span data-ttu-id="53e13-122">A ID de dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="53e13-122">The corresponding device id.</span></span>|
|<span data-ttu-id="53e13-123">installState</span><span class="sxs-lookup"><span data-stu-id="53e13-123">installState</span></span>|[<span data-ttu-id="53e13-124">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="53e13-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="53e13-125">O estado de instalação do aplicativo do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="53e13-125">The install state of the app of target app.</span></span> <span data-ttu-id="53e13-126">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="53e13-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="53e13-127">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="53e13-127">installStateDetail</span></span>|[<span data-ttu-id="53e13-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="53e13-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="53e13-129">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e13-129">The install state detail of the app.</span></span> <span data-ttu-id="53e13-130">Os valores possíveis são `noAdditionalDetails`: `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`,,, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet` ,,,,,,,, , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="53e13-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="53e13-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="53e13-131">errorCode</span></span>|<span data-ttu-id="53e13-132">Int32</span><span class="sxs-lookup"><span data-stu-id="53e13-132">Int32</span></span>|<span data-ttu-id="53e13-133">O código de erro para instalar ou desinstalar falhas do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="53e13-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="53e13-134">targetLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="53e13-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="53e13-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e13-135">DateTimeOffset</span></span>|<span data-ttu-id="53e13-136">O horário da última sincronização do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="53e13-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e13-137">Relações</span><span class="sxs-lookup"><span data-stu-id="53e13-137">Relationships</span></span>
<span data-ttu-id="53e13-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53e13-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e13-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53e13-139">JSON Representation</span></span>
<span data-ttu-id="53e13-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53e13-140">Here is a JSON representation of the resource.</span></span>
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





