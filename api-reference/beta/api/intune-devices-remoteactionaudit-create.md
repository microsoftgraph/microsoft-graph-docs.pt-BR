---
title: Criar remoteActionAudit
description: Crie um novo objeto de remoteActionAudit.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 47ba3de19ca5cdc9b01bb3b65eb8b04e75831d87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396879"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="fbbde-103">Criar remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fbbde-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="fbbde-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbbde-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbbde-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbbde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbbde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fbbde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbbde-107">Crie um novo objeto de [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="fbbde-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbbde-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbbde-108">Prerequisites</span></span>
<span data-ttu-id="fbbde-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbbde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fbbde-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbbde-111">Permission type</span></span>|<span data-ttu-id="fbbde-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbbde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbbde-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbbde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbbde-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbbde-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fbbde-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbbde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbbde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbbde-116">Not supported.</span></span>|
|<span data-ttu-id="fbbde-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbbde-117">Application</span></span>|<span data-ttu-id="fbbde-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbbde-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbbde-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbbde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="fbbde-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbbde-120">Request headers</span></span>
|<span data-ttu-id="fbbde-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbbde-121">Header</span></span>|<span data-ttu-id="fbbde-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbbde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbbde-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbbde-123">Authorization</span></span>|<span data-ttu-id="fbbde-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbbde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbbde-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbbde-125">Accept</span></span>|<span data-ttu-id="fbbde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbbde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbbde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbbde-127">Request body</span></span>
<span data-ttu-id="fbbde-128">No corpo da solicitação, fornece uma representação JSON para o objeto remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="fbbde-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="fbbde-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="fbbde-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="fbbde-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbbde-130">Property</span></span>|<span data-ttu-id="fbbde-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbbde-131">Type</span></span>|<span data-ttu-id="fbbde-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbbde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbbde-133">id</span><span class="sxs-lookup"><span data-stu-id="fbbde-133">id</span></span>|<span data-ttu-id="fbbde-134">String</span><span class="sxs-lookup"><span data-stu-id="fbbde-134">String</span></span>|<span data-ttu-id="fbbde-135">ID do relatório.</span><span class="sxs-lookup"><span data-stu-id="fbbde-135">Report Id.</span></span>|
|<span data-ttu-id="fbbde-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fbbde-136">deviceDisplayName</span></span>|<span data-ttu-id="fbbde-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbbde-137">String</span></span>|<span data-ttu-id="fbbde-138">Nome do dispositivo Intune.</span><span class="sxs-lookup"><span data-stu-id="fbbde-138">Intune device name.</span></span>|
|<span data-ttu-id="fbbde-139">userName</span><span class="sxs-lookup"><span data-stu-id="fbbde-139">userName</span></span>|<span data-ttu-id="fbbde-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbbde-140">String</span></span>|<span data-ttu-id="fbbde-141">\[preterido\] use InitiatedByUserPrincipalName em vez disso.</span><span class="sxs-lookup"><span data-stu-id="fbbde-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="fbbde-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fbbde-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="fbbde-143">String</span><span class="sxs-lookup"><span data-stu-id="fbbde-143">String</span></span>|<span data-ttu-id="fbbde-144">Usuário que iniciou a ação de dispositivo, formato é UPN.</span><span class="sxs-lookup"><span data-stu-id="fbbde-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="fbbde-145">action</span><span class="sxs-lookup"><span data-stu-id="fbbde-145">action</span></span>|[<span data-ttu-id="fbbde-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="fbbde-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="fbbde-147">O nome da ação.</span><span class="sxs-lookup"><span data-stu-id="fbbde-147">The action name.</span></span> <span data-ttu-id="fbbde-148">Os valores possíveis são: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="fbbde-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="fbbde-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="fbbde-149">requestDateTime</span></span>|<span data-ttu-id="fbbde-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbbde-150">DateTimeOffset</span></span>|<span data-ttu-id="fbbde-151">Tempo quando a ação foi emitida, dado em UTC.</span><span class="sxs-lookup"><span data-stu-id="fbbde-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="fbbde-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fbbde-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="fbbde-153">String</span><span class="sxs-lookup"><span data-stu-id="fbbde-153">String</span></span>|<span data-ttu-id="fbbde-154">Nome UPN do proprietário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbbde-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="fbbde-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="fbbde-155">deviceIMEI</span></span>|<span data-ttu-id="fbbde-156">String</span><span class="sxs-lookup"><span data-stu-id="fbbde-156">String</span></span>|<span data-ttu-id="fbbde-157">IMEI do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbbde-157">IMEI of the device.</span></span>|
|<span data-ttu-id="fbbde-158">actionState</span><span class="sxs-lookup"><span data-stu-id="fbbde-158">actionState</span></span>|[<span data-ttu-id="fbbde-159">actionState</span><span class="sxs-lookup"><span data-stu-id="fbbde-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fbbde-160">Estado de ação.</span><span class="sxs-lookup"><span data-stu-id="fbbde-160">Action state.</span></span> <span data-ttu-id="fbbde-161">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fbbde-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="fbbde-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbbde-162">Response</span></span>
<span data-ttu-id="fbbde-163">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbbde-163">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbbde-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbbde-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbbde-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbbde-165">Request</span></span>
<span data-ttu-id="fbbde-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbbde-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
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

### <a name="response"></a><span data-ttu-id="fbbde-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbbde-167">Response</span></span>
<span data-ttu-id="fbbde-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbbde-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




