---
title: Tipo de recurso remoteActionAudit
description: Relatório de ações remotas iniciadas nos dispositivos pertencentes a um determinado locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d1d9e7a340db9cc176b2ebc11bfcb4e7bd5f8de
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611878"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="a9412-103">Tipo de recurso remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-103">remoteActionAudit resource type</span></span>

<span data-ttu-id="a9412-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9412-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9412-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9412-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9412-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9412-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9412-107">Relatório de ações remotas iniciadas nos dispositivos pertencentes a um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="a9412-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="a9412-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a9412-108">Methods</span></span>
|<span data-ttu-id="a9412-109">Método</span><span class="sxs-lookup"><span data-stu-id="a9412-109">Method</span></span>|<span data-ttu-id="a9412-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a9412-110">Return Type</span></span>|<span data-ttu-id="a9412-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9412-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a9412-112">Listar remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="a9412-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="a9412-113">[Coleção remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a9412-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="a9412-114">Listar propriedades e relações dos [objetos remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a9412-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="a9412-115">Obter remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="a9412-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a9412-117">Leia propriedades e relações do [objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a9412-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="a9412-118">Criar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="a9412-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a9412-120">Crie um novo [objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a9412-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="a9412-121">Excluir remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="a9412-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9412-122">None</span></span>|<span data-ttu-id="a9412-123">Exclui um [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="a9412-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="a9412-124">Atualizar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="a9412-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a9412-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="a9412-126">Atualize as propriedades de [um objeto remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="a9412-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9412-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9412-127">Properties</span></span>
|<span data-ttu-id="a9412-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9412-128">Property</span></span>|<span data-ttu-id="a9412-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9412-129">Type</span></span>|<span data-ttu-id="a9412-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9412-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9412-131">id</span><span class="sxs-lookup"><span data-stu-id="a9412-131">id</span></span>|<span data-ttu-id="a9412-132">String</span><span class="sxs-lookup"><span data-stu-id="a9412-132">String</span></span>|<span data-ttu-id="a9412-133">ID do relatório.</span><span class="sxs-lookup"><span data-stu-id="a9412-133">Report Id.</span></span>|
|<span data-ttu-id="a9412-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9412-134">deviceDisplayName</span></span>|<span data-ttu-id="a9412-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9412-135">String</span></span>|<span data-ttu-id="a9412-136">Nome do dispositivo do Intune.</span><span class="sxs-lookup"><span data-stu-id="a9412-136">Intune device name.</span></span>|
|<span data-ttu-id="a9412-137">userName</span><span class="sxs-lookup"><span data-stu-id="a9412-137">userName</span></span>|<span data-ttu-id="a9412-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9412-138">String</span></span>|<span data-ttu-id="a9412-139">\[preterido \] Use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="a9412-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="a9412-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9412-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="a9412-141">String</span><span class="sxs-lookup"><span data-stu-id="a9412-141">String</span></span>|<span data-ttu-id="a9412-142">Usuário que iniciou a ação do dispositivo, o formato é UPN.</span><span class="sxs-lookup"><span data-stu-id="a9412-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="a9412-143">ação</span><span class="sxs-lookup"><span data-stu-id="a9412-143">action</span></span>|[<span data-ttu-id="a9412-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="a9412-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="a9412-145">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="a9412-145">The action name.</span></span> <span data-ttu-id="a9412-146">Os valores possíveis são: `unknown` , , , , , , , , `factoryReset` `removeCompanyData` , `resetPasscode` `remoteLock` , `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` , `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName`</span><span class="sxs-lookup"><span data-stu-id="a9412-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="a9412-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="a9412-147">requestDateTime</span></span>|<span data-ttu-id="a9412-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9412-148">DateTimeOffset</span></span>|<span data-ttu-id="a9412-149">Hora em que a ação foi emitida, dada em UTC.</span><span class="sxs-lookup"><span data-stu-id="a9412-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="a9412-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9412-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="a9412-151">String</span><span class="sxs-lookup"><span data-stu-id="a9412-151">String</span></span>|<span data-ttu-id="a9412-152">Upn do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9412-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="a9412-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="a9412-153">deviceIMEI</span></span>|<span data-ttu-id="a9412-154">String</span><span class="sxs-lookup"><span data-stu-id="a9412-154">String</span></span>|<span data-ttu-id="a9412-155">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9412-155">IMEI of the device.</span></span>|
|<span data-ttu-id="a9412-156">actionState</span><span class="sxs-lookup"><span data-stu-id="a9412-156">actionState</span></span>|[<span data-ttu-id="a9412-157">actionState</span><span class="sxs-lookup"><span data-stu-id="a9412-157">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a9412-158">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="a9412-158">Action state.</span></span> <span data-ttu-id="a9412-159">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a9412-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a9412-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9412-160">managedDeviceId</span></span>|<span data-ttu-id="a9412-161">String</span><span class="sxs-lookup"><span data-stu-id="a9412-161">String</span></span>|<span data-ttu-id="a9412-162">Destino da ação.</span><span class="sxs-lookup"><span data-stu-id="a9412-162">Action target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9412-163">Relações</span><span class="sxs-lookup"><span data-stu-id="a9412-163">Relationships</span></span>
<span data-ttu-id="a9412-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9412-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9412-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9412-165">JSON Representation</span></span>
<span data-ttu-id="a9412-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9412-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String",
  "managedDeviceId": "String"
}
```




