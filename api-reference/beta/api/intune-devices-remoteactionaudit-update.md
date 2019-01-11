---
title: Atualizar remoteActionAudit
description: Atualize as propriedades de um objeto remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 147f526218e70c788bdb3c60312e1ebe8591b125
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886944"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="a60e6-103">Atualizar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a60e6-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="a60e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a60e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a60e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a60e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a60e6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a60e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a60e6-107">Atualize as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="a60e6-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a60e6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a60e6-108">Prerequisites</span></span>
<span data-ttu-id="a60e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a60e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a60e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a60e6-111">Permission type</span></span>|<span data-ttu-id="a60e6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a60e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a60e6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a60e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a60e6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a60e6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a60e6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a60e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a60e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a60e6-116">Not supported.</span></span>|
|<span data-ttu-id="a60e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a60e6-117">Application</span></span>|<span data-ttu-id="a60e6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a60e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a60e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a60e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="a60e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a60e6-120">Request headers</span></span>
|<span data-ttu-id="a60e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a60e6-121">Header</span></span>|<span data-ttu-id="a60e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a60e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a60e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a60e6-123">Authorization</span></span>|<span data-ttu-id="a60e6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a60e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a60e6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a60e6-125">Accept</span></span>|<span data-ttu-id="a60e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a60e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a60e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a60e6-127">Request body</span></span>
<span data-ttu-id="a60e6-128">No corpo da solicitação, fornece uma representação JSON para o objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="a60e6-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="a60e6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="a60e6-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="a60e6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a60e6-130">Property</span></span>|<span data-ttu-id="a60e6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a60e6-131">Type</span></span>|<span data-ttu-id="a60e6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a60e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60e6-133">id</span><span class="sxs-lookup"><span data-stu-id="a60e6-133">id</span></span>|<span data-ttu-id="a60e6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-134">String</span></span>|<span data-ttu-id="a60e6-135">ID do relatório.</span><span class="sxs-lookup"><span data-stu-id="a60e6-135">Report Id.</span></span>|
|<span data-ttu-id="a60e6-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a60e6-136">deviceDisplayName</span></span>|<span data-ttu-id="a60e6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-137">String</span></span>|<span data-ttu-id="a60e6-138">Nome do dispositivo Intune.</span><span class="sxs-lookup"><span data-stu-id="a60e6-138">Intune device name.</span></span>|
|<span data-ttu-id="a60e6-139">userName</span><span class="sxs-lookup"><span data-stu-id="a60e6-139">userName</span></span>|<span data-ttu-id="a60e6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-140">String</span></span>|<span data-ttu-id="a60e6-141">\[preterido\] use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="a60e6-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="a60e6-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a60e6-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="a60e6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-143">String</span></span>|<span data-ttu-id="a60e6-144">Usuário que iniciou a ação de dispositivo, formato é UPN.</span><span class="sxs-lookup"><span data-stu-id="a60e6-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="a60e6-145">action</span><span class="sxs-lookup"><span data-stu-id="a60e6-145">action</span></span>|[<span data-ttu-id="a60e6-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="a60e6-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="a60e6-147">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="a60e6-147">The action name.</span></span> <span data-ttu-id="a60e6-148">Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="a60e6-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="a60e6-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="a60e6-149">requestDateTime</span></span>|<span data-ttu-id="a60e6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a60e6-150">DateTimeOffset</span></span>|<span data-ttu-id="a60e6-151">Tempo quando a ação foi emitida, dado em UTC.</span><span class="sxs-lookup"><span data-stu-id="a60e6-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="a60e6-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a60e6-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="a60e6-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-153">String</span></span>|<span data-ttu-id="a60e6-154">Nome UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a60e6-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="a60e6-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="a60e6-155">deviceIMEI</span></span>|<span data-ttu-id="a60e6-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60e6-156">String</span></span>|<span data-ttu-id="a60e6-157">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a60e6-157">IMEI of the device.</span></span>|
|<span data-ttu-id="a60e6-158">actionState</span><span class="sxs-lookup"><span data-stu-id="a60e6-158">actionState</span></span>|[<span data-ttu-id="a60e6-159">actionState</span><span class="sxs-lookup"><span data-stu-id="a60e6-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a60e6-160">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="a60e6-160">Action state.</span></span> <span data-ttu-id="a60e6-161">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a60e6-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="a60e6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a60e6-162">Response</span></span>
<span data-ttu-id="a60e6-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a60e6-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a60e6-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a60e6-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="a60e6-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a60e6-165">Request</span></span>
<span data-ttu-id="a60e6-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a60e6-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 399

{
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

### <a name="response"></a><span data-ttu-id="a60e6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a60e6-167">Response</span></span>
<span data-ttu-id="a60e6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a60e6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





