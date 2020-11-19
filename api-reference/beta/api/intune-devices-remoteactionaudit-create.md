---
title: Criar remoteActionAudit
description: Criar um novo objeto remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4195b2d244295d670df64dfaa851bc744509fdd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234521"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="397fb-103">Criar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="397fb-103">Create remoteActionAudit</span></span>

<span data-ttu-id="397fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="397fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="397fb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="397fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="397fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="397fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="397fb-107">Criar um novo objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="397fb-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="397fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="397fb-108">Prerequisites</span></span>
<span data-ttu-id="397fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="397fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="397fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="397fb-111">Permission type</span></span>|<span data-ttu-id="397fb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="397fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="397fb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="397fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="397fb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="397fb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="397fb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="397fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="397fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="397fb-116">Not supported.</span></span>|
|<span data-ttu-id="397fb-117">Application</span><span class="sxs-lookup"><span data-stu-id="397fb-117">Application</span></span>|<span data-ttu-id="397fb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="397fb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="397fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="397fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="397fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="397fb-120">Request headers</span></span>
|<span data-ttu-id="397fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="397fb-121">Header</span></span>|<span data-ttu-id="397fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="397fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="397fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="397fb-123">Authorization</span></span>|<span data-ttu-id="397fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="397fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="397fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="397fb-125">Accept</span></span>|<span data-ttu-id="397fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="397fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="397fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="397fb-127">Request body</span></span>
<span data-ttu-id="397fb-128">No corpo da solicitação, forneça uma representação JSON do objeto remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="397fb-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="397fb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="397fb-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="397fb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="397fb-130">Property</span></span>|<span data-ttu-id="397fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="397fb-131">Type</span></span>|<span data-ttu-id="397fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="397fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397fb-133">id</span><span class="sxs-lookup"><span data-stu-id="397fb-133">id</span></span>|<span data-ttu-id="397fb-134">String</span><span class="sxs-lookup"><span data-stu-id="397fb-134">String</span></span>|<span data-ttu-id="397fb-135">ID de relatório.</span><span class="sxs-lookup"><span data-stu-id="397fb-135">Report Id.</span></span>|
|<span data-ttu-id="397fb-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="397fb-136">deviceDisplayName</span></span>|<span data-ttu-id="397fb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397fb-137">String</span></span>|<span data-ttu-id="397fb-138">Nome do dispositivo do Intune.</span><span class="sxs-lookup"><span data-stu-id="397fb-138">Intune device name.</span></span>|
|<span data-ttu-id="397fb-139">userName</span><span class="sxs-lookup"><span data-stu-id="397fb-139">userName</span></span>|<span data-ttu-id="397fb-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397fb-140">String</span></span>|<span data-ttu-id="397fb-141">\[preterido \] use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="397fb-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="397fb-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="397fb-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="397fb-143">String</span><span class="sxs-lookup"><span data-stu-id="397fb-143">String</span></span>|<span data-ttu-id="397fb-144">O formato de usuário que iniciou a ação do dispositivo é UPN.</span><span class="sxs-lookup"><span data-stu-id="397fb-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="397fb-145">ação</span><span class="sxs-lookup"><span data-stu-id="397fb-145">action</span></span>|[<span data-ttu-id="397fb-146">remoteaction</span><span class="sxs-lookup"><span data-stu-id="397fb-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="397fb-147">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="397fb-147">The action name.</span></span> <span data-ttu-id="397fb-148">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `unknown` `factoryReset` `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` , `fullScan` , `windowsDefenderUpdateSignatures` ,, `factoryResetKeepEnrollmentData` `updateDeviceAccount` , `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="397fb-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="397fb-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="397fb-149">requestDateTime</span></span>|<span data-ttu-id="397fb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="397fb-150">DateTimeOffset</span></span>|<span data-ttu-id="397fb-151">Hora em que a ação foi emitida, dada em UTC.</span><span class="sxs-lookup"><span data-stu-id="397fb-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="397fb-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="397fb-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="397fb-153">String</span><span class="sxs-lookup"><span data-stu-id="397fb-153">String</span></span>|<span data-ttu-id="397fb-154">UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="397fb-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="397fb-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="397fb-155">deviceIMEI</span></span>|<span data-ttu-id="397fb-156">String</span><span class="sxs-lookup"><span data-stu-id="397fb-156">String</span></span>|<span data-ttu-id="397fb-157">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="397fb-157">IMEI of the device.</span></span>|
|<span data-ttu-id="397fb-158">actionState</span><span class="sxs-lookup"><span data-stu-id="397fb-158">actionState</span></span>|[<span data-ttu-id="397fb-159">actionState</span><span class="sxs-lookup"><span data-stu-id="397fb-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="397fb-160">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="397fb-160">Action state.</span></span> <span data-ttu-id="397fb-161">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="397fb-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="397fb-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="397fb-162">managedDeviceId</span></span>|<span data-ttu-id="397fb-163">String</span><span class="sxs-lookup"><span data-stu-id="397fb-163">String</span></span>|<span data-ttu-id="397fb-164">Destino de ação.</span><span class="sxs-lookup"><span data-stu-id="397fb-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="397fb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="397fb-165">Response</span></span>
<span data-ttu-id="397fb-166">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="397fb-166">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="397fb-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="397fb-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="397fb-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="397fb-168">Request</span></span>
<span data-ttu-id="397fb-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="397fb-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="397fb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="397fb-170">Response</span></span>
<span data-ttu-id="397fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="397fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```




