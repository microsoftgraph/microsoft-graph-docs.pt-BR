---
title: tipo de recurso de mobileAppInstallStatus
description: Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f9ee188190e834016e7dc919c6a2c672d5e22227
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422429"
---
# <a name="mobileappinstallstatus-resource-type"></a><span data-ttu-id="74c49-103">tipo de recurso de mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-103">mobileAppInstallStatus resource type</span></span>

> <span data-ttu-id="74c49-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="74c49-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="74c49-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="74c49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74c49-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="74c49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74c49-107">Contém propriedades para o estado de instalação de um aplicativo móvel para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74c49-107">Contains properties for the installation state of a mobile app for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="74c49-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="74c49-108">Methods</span></span>
|<span data-ttu-id="74c49-109">Método</span><span class="sxs-lookup"><span data-stu-id="74c49-109">Method</span></span>|<span data-ttu-id="74c49-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74c49-110">Return Type</span></span>|<span data-ttu-id="74c49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c49-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74c49-112">Lista mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="74c49-112">List mobileAppInstallStatuses</span></span>](../api/intune-apps-mobileappinstallstatus-list.md)|<span data-ttu-id="74c49-113">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="74c49-113">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="74c49-114">Lista as propriedades e os relacionamentos dos objetos [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="74c49-114">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="74c49-115">Obter mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-115">Get mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-get.md)|[<span data-ttu-id="74c49-116">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-116">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74c49-117">Leia as propriedades e os relacionamentos do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="74c49-117">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="74c49-118">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-118">Create mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-create.md)|[<span data-ttu-id="74c49-119">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-119">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74c49-120">Crie um novo objeto de [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="74c49-120">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="74c49-121">Excluir mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-121">Delete mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-delete.md)|<span data-ttu-id="74c49-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74c49-122">None</span></span>|<span data-ttu-id="74c49-123">Exclui um [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="74c49-123">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>|
|[<span data-ttu-id="74c49-124">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-124">Update mobileAppInstallStatus</span></span>](../api/intune-apps-mobileappinstallstatus-update.md)|[<span data-ttu-id="74c49-125">mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="74c49-125">mobileAppInstallStatus</span></span>](../resources/intune-apps-mobileappinstallstatus.md)|<span data-ttu-id="74c49-126">Atualize as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="74c49-126">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74c49-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74c49-127">Properties</span></span>
|<span data-ttu-id="74c49-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74c49-128">Property</span></span>|<span data-ttu-id="74c49-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c49-129">Type</span></span>|<span data-ttu-id="74c49-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74c49-131">id</span><span class="sxs-lookup"><span data-stu-id="74c49-131">id</span></span>|<span data-ttu-id="74c49-132">String</span><span class="sxs-lookup"><span data-stu-id="74c49-132">String</span></span>|<span data-ttu-id="74c49-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="74c49-133">Key of the entity.</span></span>|
|<span data-ttu-id="74c49-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="74c49-134">deviceName</span></span>|<span data-ttu-id="74c49-135">String</span><span class="sxs-lookup"><span data-stu-id="74c49-135">String</span></span>|<span data-ttu-id="74c49-136">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74c49-136">Device name</span></span>|
|<span data-ttu-id="74c49-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="74c49-137">deviceId</span></span>|<span data-ttu-id="74c49-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c49-138">String</span></span>|<span data-ttu-id="74c49-139">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74c49-139">Device ID</span></span>|
|<span data-ttu-id="74c49-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="74c49-140">lastSyncDateTime</span></span>|<span data-ttu-id="74c49-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74c49-141">DateTimeOffset</span></span>|<span data-ttu-id="74c49-142">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="74c49-142">Last sync date time</span></span>|
|<span data-ttu-id="74c49-143">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="74c49-143">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="74c49-144">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="74c49-144">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="74c49-145">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c49-145">The install state of the app.</span></span> <span data-ttu-id="74c49-146">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="74c49-146">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="74c49-147">installState</span><span class="sxs-lookup"><span data-stu-id="74c49-147">installState</span></span>|[<span data-ttu-id="74c49-148">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="74c49-148">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="74c49-149">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c49-149">The install state of the app.</span></span> <span data-ttu-id="74c49-150">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="74c49-150">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="74c49-151">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="74c49-151">installStateDetail</span></span>|[<span data-ttu-id="74c49-152">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="74c49-152">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="74c49-153">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c49-153">The install state detail of the app.</span></span> <span data-ttu-id="74c49-154">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="74c49-154">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="74c49-155">errorCode</span><span class="sxs-lookup"><span data-stu-id="74c49-155">errorCode</span></span>|<span data-ttu-id="74c49-156">Int32</span><span class="sxs-lookup"><span data-stu-id="74c49-156">Int32</span></span>|<span data-ttu-id="74c49-157">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="74c49-157">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="74c49-158">osVersion</span><span class="sxs-lookup"><span data-stu-id="74c49-158">osVersion</span></span>|<span data-ttu-id="74c49-159">String</span><span class="sxs-lookup"><span data-stu-id="74c49-159">String</span></span>|<span data-ttu-id="74c49-160">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="74c49-160">OS Version</span></span>|
|<span data-ttu-id="74c49-161">osDescription</span><span class="sxs-lookup"><span data-stu-id="74c49-161">osDescription</span></span>|<span data-ttu-id="74c49-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c49-162">String</span></span>|<span data-ttu-id="74c49-163">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="74c49-163">OS Description</span></span>|
|<span data-ttu-id="74c49-164">userName</span><span class="sxs-lookup"><span data-stu-id="74c49-164">userName</span></span>|<span data-ttu-id="74c49-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c49-165">String</span></span>|<span data-ttu-id="74c49-166">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74c49-166">Device User Name</span></span>|
|<span data-ttu-id="74c49-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74c49-167">userPrincipalName</span></span>|<span data-ttu-id="74c49-168">String</span><span class="sxs-lookup"><span data-stu-id="74c49-168">String</span></span>|<span data-ttu-id="74c49-169">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="74c49-169">User Principal Name</span></span>|
|<span data-ttu-id="74c49-170">displayVersion</span><span class="sxs-lookup"><span data-stu-id="74c49-170">displayVersion</span></span>|<span data-ttu-id="74c49-171">String</span><span class="sxs-lookup"><span data-stu-id="74c49-171">String</span></span>|<span data-ttu-id="74c49-172">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c49-172">Human readable version of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="74c49-173">Relações</span><span class="sxs-lookup"><span data-stu-id="74c49-173">Relationships</span></span>
|<span data-ttu-id="74c49-174">Relação</span><span class="sxs-lookup"><span data-stu-id="74c49-174">Relationship</span></span>|<span data-ttu-id="74c49-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c49-175">Type</span></span>|<span data-ttu-id="74c49-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c49-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74c49-177">app</span><span class="sxs-lookup"><span data-stu-id="74c49-177">app</span></span>|[<span data-ttu-id="74c49-178">mobileApp</span><span class="sxs-lookup"><span data-stu-id="74c49-178">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="74c49-179">O link de navegação para o aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="74c49-179">The navigation link to the mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74c49-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74c49-180">JSON Representation</span></span>
<span data-ttu-id="74c49-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74c49-181">Here is a JSON representation of the resource.</span></span>
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




