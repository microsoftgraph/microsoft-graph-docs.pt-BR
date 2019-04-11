---
title: Atualizar remoteActionAudit
description: Atualiza as propriedades de um objeto remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfae09fc5dd7e90e2109a5a858a25b062922df1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802545"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="3104e-103">Atualizar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="3104e-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="3104e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3104e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3104e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3104e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3104e-106">Atualiza as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="3104e-106">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3104e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3104e-107">Prerequisites</span></span>
<span data-ttu-id="3104e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3104e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3104e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3104e-110">Permission type</span></span>|<span data-ttu-id="3104e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3104e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3104e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3104e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3104e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3104e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3104e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3104e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3104e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3104e-115">Not supported.</span></span>|
|<span data-ttu-id="3104e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3104e-116">Application</span></span>|<span data-ttu-id="3104e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3104e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3104e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3104e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="3104e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3104e-119">Request headers</span></span>
|<span data-ttu-id="3104e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3104e-120">Header</span></span>|<span data-ttu-id="3104e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3104e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3104e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3104e-122">Authorization</span></span>|<span data-ttu-id="3104e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3104e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3104e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3104e-124">Accept</span></span>|<span data-ttu-id="3104e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3104e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3104e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3104e-126">Request body</span></span>
<span data-ttu-id="3104e-127">No corpo da solicitação, forneça uma representação JSON do objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="3104e-127">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="3104e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="3104e-128">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="3104e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3104e-129">Property</span></span>|<span data-ttu-id="3104e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3104e-130">Type</span></span>|<span data-ttu-id="3104e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3104e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3104e-132">id</span><span class="sxs-lookup"><span data-stu-id="3104e-132">id</span></span>|<span data-ttu-id="3104e-133">String</span><span class="sxs-lookup"><span data-stu-id="3104e-133">String</span></span>|<span data-ttu-id="3104e-134">ID de relatório.</span><span class="sxs-lookup"><span data-stu-id="3104e-134">Report Id.</span></span>|
|<span data-ttu-id="3104e-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3104e-135">deviceDisplayName</span></span>|<span data-ttu-id="3104e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3104e-136">String</span></span>|<span data-ttu-id="3104e-137">Nome do dispositivo do Intune.</span><span class="sxs-lookup"><span data-stu-id="3104e-137">Intune device name.</span></span>|
|<span data-ttu-id="3104e-138">userName</span><span class="sxs-lookup"><span data-stu-id="3104e-138">userName</span></span>|<span data-ttu-id="3104e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3104e-139">String</span></span>|<span data-ttu-id="3104e-140">\[\] preterido use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="3104e-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="3104e-141">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3104e-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="3104e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3104e-142">String</span></span>|<span data-ttu-id="3104e-143">O formato de usuário que iniciou a ação do dispositivo é UPN.</span><span class="sxs-lookup"><span data-stu-id="3104e-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="3104e-144">action</span><span class="sxs-lookup"><span data-stu-id="3104e-144">action</span></span>|[<span data-ttu-id="3104e-145">remoteaction</span><span class="sxs-lookup"><span data-stu-id="3104e-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="3104e-146">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="3104e-146">The action name.</span></span> <span data-ttu-id="3104e-147">Os valores possíveis são `unknown`: `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`,,, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` ,,,,,,,, .</span><span class="sxs-lookup"><span data-stu-id="3104e-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="3104e-148">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="3104e-148">requestDateTime</span></span>|<span data-ttu-id="3104e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3104e-149">DateTimeOffset</span></span>|<span data-ttu-id="3104e-150">Hora em que a ação foi emitida, dada em UTC.</span><span class="sxs-lookup"><span data-stu-id="3104e-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="3104e-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3104e-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="3104e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3104e-152">String</span></span>|<span data-ttu-id="3104e-153">UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3104e-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="3104e-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="3104e-154">deviceIMEI</span></span>|<span data-ttu-id="3104e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3104e-155">String</span></span>|<span data-ttu-id="3104e-156">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3104e-156">IMEI of the device.</span></span>|
|<span data-ttu-id="3104e-157">actionState</span><span class="sxs-lookup"><span data-stu-id="3104e-157">actionState</span></span>|[<span data-ttu-id="3104e-158">actionState</span><span class="sxs-lookup"><span data-stu-id="3104e-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3104e-159">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="3104e-159">Action state.</span></span> <span data-ttu-id="3104e-160">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3104e-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="3104e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3104e-161">Response</span></span>
<span data-ttu-id="3104e-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3104e-162">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3104e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3104e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3104e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3104e-164">Request</span></span>
<span data-ttu-id="3104e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3104e-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a><span data-ttu-id="3104e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3104e-166">Response</span></span>
<span data-ttu-id="3104e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3104e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

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
  "actionState": "pending"
}
```





