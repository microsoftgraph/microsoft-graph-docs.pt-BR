---
title: tipo de recurso de remoteActionAudit
description: Relatório de ações remotos iniciadas nos dispositivos que pertencem a um determinado inquilino.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7624610ed35a583e0ec11582caa1dccda5ce4ce7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840807"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="19d15-103">tipo de recurso de remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="19d15-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19d15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19d15-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19d15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19d15-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19d15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19d15-107">Relatório de ações remotos iniciadas nos dispositivos que pertencem a um determinado inquilino.</span><span class="sxs-lookup"><span data-stu-id="19d15-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="19d15-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="19d15-108">Methods</span></span>
|<span data-ttu-id="19d15-109">Método</span><span class="sxs-lookup"><span data-stu-id="19d15-109">Method</span></span>|<span data-ttu-id="19d15-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="19d15-110">Return Type</span></span>|<span data-ttu-id="19d15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19d15-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19d15-112">Lista remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="19d15-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="19d15-113">coleção [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="19d15-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="19d15-114">Lista as propriedades e os relacionamentos dos objetos [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="19d15-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="19d15-115">Obter remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="19d15-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19d15-117">Leia as propriedades e os relacionamentos do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="19d15-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="19d15-118">Criar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="19d15-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19d15-120">Crie um novo objeto de [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="19d15-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="19d15-121">Excluir remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="19d15-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19d15-122">None</span></span>|<span data-ttu-id="19d15-123">Exclui um [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="19d15-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="19d15-124">Atualizar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="19d15-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="19d15-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="19d15-126">Atualize as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="19d15-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19d15-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19d15-127">Properties</span></span>
|<span data-ttu-id="19d15-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19d15-128">Property</span></span>|<span data-ttu-id="19d15-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="19d15-129">Type</span></span>|<span data-ttu-id="19d15-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="19d15-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d15-131">id</span><span class="sxs-lookup"><span data-stu-id="19d15-131">id</span></span>|<span data-ttu-id="19d15-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-132">String</span></span>|<span data-ttu-id="19d15-133">ID do relatório.</span><span class="sxs-lookup"><span data-stu-id="19d15-133">Report Id.</span></span>|
|<span data-ttu-id="19d15-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="19d15-134">deviceDisplayName</span></span>|<span data-ttu-id="19d15-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-135">String</span></span>|<span data-ttu-id="19d15-136">Nome do dispositivo Intune.</span><span class="sxs-lookup"><span data-stu-id="19d15-136">Intune device name.</span></span>|
|<span data-ttu-id="19d15-137">userName</span><span class="sxs-lookup"><span data-stu-id="19d15-137">userName</span></span>|<span data-ttu-id="19d15-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-138">String</span></span>|<span data-ttu-id="19d15-139">\[preterido\] use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="19d15-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="19d15-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19d15-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="19d15-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-141">String</span></span>|<span data-ttu-id="19d15-142">Usuário que iniciou a ação de dispositivo, formato é UPN.</span><span class="sxs-lookup"><span data-stu-id="19d15-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="19d15-143">action</span><span class="sxs-lookup"><span data-stu-id="19d15-143">action</span></span>|[<span data-ttu-id="19d15-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="19d15-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="19d15-145">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="19d15-145">The action name.</span></span> <span data-ttu-id="19d15-146">Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="19d15-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="19d15-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="19d15-147">requestDateTime</span></span>|<span data-ttu-id="19d15-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19d15-148">DateTimeOffset</span></span>|<span data-ttu-id="19d15-149">Tempo quando a ação foi emitida, dado em UTC.</span><span class="sxs-lookup"><span data-stu-id="19d15-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="19d15-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19d15-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="19d15-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-151">String</span></span>|<span data-ttu-id="19d15-152">Nome UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19d15-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="19d15-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="19d15-153">deviceIMEI</span></span>|<span data-ttu-id="19d15-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19d15-154">String</span></span>|<span data-ttu-id="19d15-155">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19d15-155">IMEI of the device.</span></span>|
|<span data-ttu-id="19d15-156">actionState</span><span class="sxs-lookup"><span data-stu-id="19d15-156">actionState</span></span>|[<span data-ttu-id="19d15-157">actionState</span><span class="sxs-lookup"><span data-stu-id="19d15-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="19d15-158">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="19d15-158">Action state.</span></span> <span data-ttu-id="19d15-159">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="19d15-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d15-160">Relações</span><span class="sxs-lookup"><span data-stu-id="19d15-160">Relationships</span></span>
<span data-ttu-id="19d15-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19d15-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19d15-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19d15-162">JSON Representation</span></span>
<span data-ttu-id="19d15-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19d15-163">Here is a JSON representation of the resource.</span></span>
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
  "actionState": "String"
}
```





