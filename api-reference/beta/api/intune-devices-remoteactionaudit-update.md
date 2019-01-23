---
title: Atualizar remoteActionAudit
description: Atualize as propriedades de um objeto remoteActionAudit.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6078b3f6fd5236bd0e6e1a51f5f52cbf69a59c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396186"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="f4060-103">Atualizar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f4060-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="f4060-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4060-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4060-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4060-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4060-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f4060-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4060-107">Atualize as propriedades de um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="f4060-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4060-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4060-108">Prerequisites</span></span>
<span data-ttu-id="f4060-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4060-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4060-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4060-111">Permission type</span></span>|<span data-ttu-id="f4060-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4060-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4060-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4060-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4060-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4060-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4060-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4060-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4060-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4060-116">Not supported.</span></span>|
|<span data-ttu-id="f4060-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4060-117">Application</span></span>|<span data-ttu-id="f4060-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4060-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4060-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4060-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="f4060-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4060-120">Request headers</span></span>
|<span data-ttu-id="f4060-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4060-121">Header</span></span>|<span data-ttu-id="f4060-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4060-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4060-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4060-123">Authorization</span></span>|<span data-ttu-id="f4060-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4060-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4060-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4060-125">Accept</span></span>|<span data-ttu-id="f4060-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4060-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4060-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4060-127">Request body</span></span>
<span data-ttu-id="f4060-128">No corpo da solicitação, fornece uma representação JSON para o objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="f4060-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="f4060-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="f4060-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="f4060-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4060-130">Property</span></span>|<span data-ttu-id="f4060-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4060-131">Type</span></span>|<span data-ttu-id="f4060-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4060-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4060-133">id</span><span class="sxs-lookup"><span data-stu-id="f4060-133">id</span></span>|<span data-ttu-id="f4060-134">String</span><span class="sxs-lookup"><span data-stu-id="f4060-134">String</span></span>|<span data-ttu-id="f4060-135">ID do relatório.</span><span class="sxs-lookup"><span data-stu-id="f4060-135">Report Id.</span></span>|
|<span data-ttu-id="f4060-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4060-136">deviceDisplayName</span></span>|<span data-ttu-id="f4060-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4060-137">String</span></span>|<span data-ttu-id="f4060-138">Nome do dispositivo Intune.</span><span class="sxs-lookup"><span data-stu-id="f4060-138">Intune device name.</span></span>|
|<span data-ttu-id="f4060-139">userName</span><span class="sxs-lookup"><span data-stu-id="f4060-139">userName</span></span>|<span data-ttu-id="f4060-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4060-140">String</span></span>|<span data-ttu-id="f4060-141">\[preterido\] use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f4060-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="f4060-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4060-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="f4060-143">String</span><span class="sxs-lookup"><span data-stu-id="f4060-143">String</span></span>|<span data-ttu-id="f4060-144">Usuário que iniciou a ação de dispositivo, formato é UPN.</span><span class="sxs-lookup"><span data-stu-id="f4060-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="f4060-145">action</span><span class="sxs-lookup"><span data-stu-id="f4060-145">action</span></span>|[<span data-ttu-id="f4060-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="f4060-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="f4060-147">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="f4060-147">The action name.</span></span> <span data-ttu-id="f4060-148">Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="f4060-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="f4060-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="f4060-149">requestDateTime</span></span>|<span data-ttu-id="f4060-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4060-150">DateTimeOffset</span></span>|<span data-ttu-id="f4060-151">Tempo quando a ação foi emitida, dado em UTC.</span><span class="sxs-lookup"><span data-stu-id="f4060-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="f4060-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4060-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="f4060-153">String</span><span class="sxs-lookup"><span data-stu-id="f4060-153">String</span></span>|<span data-ttu-id="f4060-154">Nome UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4060-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="f4060-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="f4060-155">deviceIMEI</span></span>|<span data-ttu-id="f4060-156">String</span><span class="sxs-lookup"><span data-stu-id="f4060-156">String</span></span>|<span data-ttu-id="f4060-157">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4060-157">IMEI of the device.</span></span>|
|<span data-ttu-id="f4060-158">actionState</span><span class="sxs-lookup"><span data-stu-id="f4060-158">actionState</span></span>|[<span data-ttu-id="f4060-159">actionState</span><span class="sxs-lookup"><span data-stu-id="f4060-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f4060-160">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="f4060-160">Action state.</span></span> <span data-ttu-id="f4060-161">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f4060-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4060-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4060-162">Response</span></span>
<span data-ttu-id="f4060-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4060-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4060-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4060-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4060-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4060-165">Request</span></span>
<span data-ttu-id="f4060-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4060-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4060-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4060-167">Response</span></span>
<span data-ttu-id="f4060-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4060-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




