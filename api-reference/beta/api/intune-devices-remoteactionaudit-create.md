---
title: Criar remoteActionAudit
description: Criar um novo objeto remoteActionAudit.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb062127fc744f7612c0b81464f5de77436ceaeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468632"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="35f23-103">Criar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="35f23-103">Create remoteActionAudit</span></span>

<span data-ttu-id="35f23-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35f23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35f23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35f23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35f23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35f23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f23-107">Criar um novo objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="35f23-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f23-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35f23-108">Prerequisites</span></span>
<span data-ttu-id="35f23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35f23-111">Permission type</span></span>|<span data-ttu-id="35f23-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35f23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35f23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35f23-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f23-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="35f23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35f23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35f23-116">Not supported.</span></span>|
|<span data-ttu-id="35f23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35f23-117">Application</span></span>|<span data-ttu-id="35f23-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f23-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35f23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="35f23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35f23-120">Request headers</span></span>
|<span data-ttu-id="35f23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35f23-121">Header</span></span>|<span data-ttu-id="35f23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35f23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35f23-123">Authorization</span></span>|<span data-ttu-id="35f23-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35f23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f23-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35f23-125">Accept</span></span>|<span data-ttu-id="35f23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35f23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35f23-127">Request body</span></span>
<span data-ttu-id="35f23-128">No corpo da solicitação, forneça uma representação JSON do objeto remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="35f23-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="35f23-129">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="35f23-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="35f23-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35f23-130">Property</span></span>|<span data-ttu-id="35f23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35f23-131">Type</span></span>|<span data-ttu-id="35f23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35f23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f23-133">id</span><span class="sxs-lookup"><span data-stu-id="35f23-133">id</span></span>|<span data-ttu-id="35f23-134">String</span><span class="sxs-lookup"><span data-stu-id="35f23-134">String</span></span>|<span data-ttu-id="35f23-135">ID de relatório.</span><span class="sxs-lookup"><span data-stu-id="35f23-135">Report Id.</span></span>|
|<span data-ttu-id="35f23-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="35f23-136">deviceDisplayName</span></span>|<span data-ttu-id="35f23-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35f23-137">String</span></span>|<span data-ttu-id="35f23-138">Nome do dispositivo do Intune.</span><span class="sxs-lookup"><span data-stu-id="35f23-138">Intune device name.</span></span>|
|<span data-ttu-id="35f23-139">userName</span><span class="sxs-lookup"><span data-stu-id="35f23-139">userName</span></span>|<span data-ttu-id="35f23-140">String</span><span class="sxs-lookup"><span data-stu-id="35f23-140">String</span></span>|<span data-ttu-id="35f23-141">\[\] preterido use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="35f23-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="35f23-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="35f23-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="35f23-143">String</span><span class="sxs-lookup"><span data-stu-id="35f23-143">String</span></span>|<span data-ttu-id="35f23-144">O formato de usuário que iniciou a ação do dispositivo é UPN.</span><span class="sxs-lookup"><span data-stu-id="35f23-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="35f23-145">ação</span><span class="sxs-lookup"><span data-stu-id="35f23-145">action</span></span>|[<span data-ttu-id="35f23-146">remoteaction</span><span class="sxs-lookup"><span data-stu-id="35f23-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="35f23-147">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="35f23-147">The action name.</span></span> <span data-ttu-id="35f23-148">Os valores possíveis são `unknown`: `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock` `enableLostMode` `disableLostMode`,,, `locateDevice`, `rebootNow`, `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`,,, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey`,,,, `setDeviceName`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="35f23-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="35f23-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="35f23-149">requestDateTime</span></span>|<span data-ttu-id="35f23-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f23-150">DateTimeOffset</span></span>|<span data-ttu-id="35f23-151">Hora em que a ação foi emitida, dada em UTC.</span><span class="sxs-lookup"><span data-stu-id="35f23-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="35f23-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="35f23-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="35f23-153">String</span><span class="sxs-lookup"><span data-stu-id="35f23-153">String</span></span>|<span data-ttu-id="35f23-154">UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35f23-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="35f23-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="35f23-155">deviceIMEI</span></span>|<span data-ttu-id="35f23-156">String</span><span class="sxs-lookup"><span data-stu-id="35f23-156">String</span></span>|<span data-ttu-id="35f23-157">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35f23-157">IMEI of the device.</span></span>|
|<span data-ttu-id="35f23-158">actionState</span><span class="sxs-lookup"><span data-stu-id="35f23-158">actionState</span></span>|[<span data-ttu-id="35f23-159">actionState</span><span class="sxs-lookup"><span data-stu-id="35f23-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="35f23-160">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="35f23-160">Action state.</span></span> <span data-ttu-id="35f23-161">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="35f23-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="35f23-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="35f23-162">managedDeviceId</span></span>|<span data-ttu-id="35f23-163">String</span><span class="sxs-lookup"><span data-stu-id="35f23-163">String</span></span>|<span data-ttu-id="35f23-164">Destino de ação.</span><span class="sxs-lookup"><span data-stu-id="35f23-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="35f23-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="35f23-165">Response</span></span>
<span data-ttu-id="35f23-166">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35f23-166">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f23-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35f23-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f23-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35f23-168">Request</span></span>
<span data-ttu-id="35f23-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f23-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35f23-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="35f23-170">Response</span></span>
<span data-ttu-id="35f23-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35f23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





