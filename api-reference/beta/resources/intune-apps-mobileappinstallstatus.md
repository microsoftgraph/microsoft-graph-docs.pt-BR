---
title: tipo de recurso de mobileAppInstallStatus
description: Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cac5c94f0669f784bf4cdd020448e40799d53915
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982607"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="e4490-103">tipo de recurso de mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="e4490-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4490-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4490-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4490-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4490-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e4490-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4490-107">Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4490-107">Contains properties for the installation state of a mobile app for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="e4490-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e4490-108">Methods</span></span>
|<span data-ttu-id="e4490-109">Método</span><span class="sxs-lookup"><span data-stu-id="e4490-109">Method</span></span>|<span data-ttu-id="e4490-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e4490-110">Return Type</span></span>|<span data-ttu-id="e4490-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4490-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4490-112">Lista mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="e4490-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="e4490-113">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e4490-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e4490-114">Lista as propriedades e os relacionamentos dos objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e4490-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="e4490-115">Obter mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="e4490-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e4490-117">Leia as propriedades e os relacionamentos do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e4490-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e4490-118">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="e4490-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e4490-120">Crie um novo objeto de [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e4490-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="e4490-121">Excluir mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="e4490-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4490-122">None</span></span>|<span data-ttu-id="e4490-123">Exclui um [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e4490-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="e4490-124">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="e4490-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e4490-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="e4490-126">Atualize as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e4490-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4490-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4490-127">Properties</span></span>
|<span data-ttu-id="e4490-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4490-128">Property</span></span>|<span data-ttu-id="e4490-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4490-129">Type</span></span>|<span data-ttu-id="e4490-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4490-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4490-131">id</span><span class="sxs-lookup"><span data-stu-id="e4490-131">id</span></span>|<span data-ttu-id="e4490-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-132">String</span></span>|<span data-ttu-id="e4490-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e4490-133">Key of the entity.</span></span>|
|<span data-ttu-id="e4490-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="e4490-134">deviceName</span></span>|<span data-ttu-id="e4490-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-135">String</span></span>|<span data-ttu-id="e4490-136">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e4490-136">Device name</span></span>|
|<span data-ttu-id="e4490-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="e4490-137">deviceId</span></span>|<span data-ttu-id="e4490-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-138">String</span></span>|<span data-ttu-id="e4490-139">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e4490-139">Device ID</span></span>|
|<span data-ttu-id="e4490-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e4490-140">lastSyncDateTime</span></span>|<span data-ttu-id="e4490-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4490-141">DateTimeOffset</span></span>|<span data-ttu-id="e4490-142">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="e4490-142">Last sync date time</span></span>|
|<span data-ttu-id="e4490-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="e4490-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="e4490-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e4490-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e4490-145">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4490-145">The install state of the app.</span></span> <span data-ttu-id="e4490-146">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e4490-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e4490-147">installState</span><span class="sxs-lookup"><span data-stu-id="e4490-147">installState</span></span>|[<span data-ttu-id="e4490-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e4490-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e4490-149">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4490-149">The install state of the app.</span></span> <span data-ttu-id="e4490-150">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e4490-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e4490-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e4490-151">installStateDetail</span></span>|[<span data-ttu-id="e4490-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e4490-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e4490-153">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4490-153">The install state detail of the app.</span></span> <span data-ttu-id="e4490-154">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e4490-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e4490-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="e4490-155">errorCode</span></span>|<span data-ttu-id="e4490-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e4490-156">Int32</span></span>|<span data-ttu-id="e4490-157">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="e4490-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="e4490-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="e4490-158">osVersion</span></span>|<span data-ttu-id="e4490-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-159">String</span></span>|<span data-ttu-id="e4490-160">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e4490-160">OS Version</span></span>|
|<span data-ttu-id="e4490-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="e4490-161">osDescription</span></span>|<span data-ttu-id="e4490-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-162">String</span></span>|<span data-ttu-id="e4490-163">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e4490-163">OS Description</span></span>|
|<span data-ttu-id="e4490-164">userName</span><span class="sxs-lookup"><span data-stu-id="e4490-164">userName</span></span>|<span data-ttu-id="e4490-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-165">String</span></span>|<span data-ttu-id="e4490-166">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e4490-166">Device User Name</span></span>|
|<span data-ttu-id="e4490-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e4490-167">userPrincipalName</span></span>|<span data-ttu-id="e4490-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-168">String</span></span>|<span data-ttu-id="e4490-169">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e4490-169">User Principal Name</span></span>|
|<span data-ttu-id="e4490-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e4490-170">displayVersion</span></span>|<span data-ttu-id="e4490-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4490-171">String</span></span>|<span data-ttu-id="e4490-172">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4490-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4490-173">Relações</span><span class="sxs-lookup"><span data-stu-id="e4490-173">Relationships</span></span>
|<span data-ttu-id="e4490-174">Relação</span><span class="sxs-lookup"><span data-stu-id="e4490-174">Relationship</span></span>|<span data-ttu-id="e4490-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4490-175">Type</span></span>|<span data-ttu-id="e4490-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4490-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4490-177">app</span><span class="sxs-lookup"><span data-stu-id="e4490-177">app</span></span>|[<span data-ttu-id="e4490-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e4490-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e4490-179">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e4490-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4490-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4490-180">JSON Representation</span></span>
<span data-ttu-id="e4490-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4490-181">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```





