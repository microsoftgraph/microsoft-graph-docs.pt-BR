---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57fddece1d8059e46121f23596180636c5765913
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463818"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="690ab-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="690ab-103">Update deviceManagement</span></span>

<span data-ttu-id="690ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="690ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="690ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="690ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="690ab-106">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="690ab-106">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="690ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="690ab-107">Prerequisites</span></span>
<span data-ttu-id="690ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="690ab-110">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="690ab-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="690ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="690ab-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="690ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="690ab-112">Delegated (work or school account)</span></span> |
| <span data-ttu-id="690ab-113">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="690ab-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="690ab-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-115">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="690ab-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="690ab-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-117">&nbsp;&nbsp; Registro corporativo</span><span class="sxs-lookup"><span data-stu-id="690ab-117">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="690ab-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="690ab-119">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="690ab-119">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="690ab-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-121">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="690ab-121">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="690ab-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-123">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="690ab-123">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="690ab-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-125">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="690ab-125">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="690ab-126">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-126">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-127">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="690ab-127">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="690ab-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-129">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="690ab-129">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="690ab-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-130">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-131">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="690ab-131">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="690ab-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-133">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="690ab-133">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="690ab-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-135">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="690ab-135">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="690ab-136">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-136">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-137">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="690ab-137">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="690ab-138">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690ab-138">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="690ab-139">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="690ab-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="690ab-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690ab-140">Not supported.</span></span>|
| <span data-ttu-id="690ab-141">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="690ab-141">Application</span></span> | <span data-ttu-id="690ab-142">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690ab-142">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="690ab-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="690ab-143">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="690ab-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="690ab-144">Request headers</span></span>
|<span data-ttu-id="690ab-145">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="690ab-145">Header</span></span>|<span data-ttu-id="690ab-146">Valor</span><span class="sxs-lookup"><span data-stu-id="690ab-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="690ab-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="690ab-147">Authorization</span></span>|<span data-ttu-id="690ab-148">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="690ab-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="690ab-149">Aceitar</span><span class="sxs-lookup"><span data-stu-id="690ab-149">Accept</span></span>|<span data-ttu-id="690ab-150">application/json</span><span class="sxs-lookup"><span data-stu-id="690ab-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="690ab-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="690ab-151">Request body</span></span>
<span data-ttu-id="690ab-152">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="690ab-152">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="690ab-153">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="690ab-153">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="690ab-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="690ab-154">Property</span></span>|<span data-ttu-id="690ab-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="690ab-155">Type</span></span>|<span data-ttu-id="690ab-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="690ab-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="690ab-157">id</span><span class="sxs-lookup"><span data-stu-id="690ab-157">id</span></span>|<span data-ttu-id="690ab-158">String</span><span class="sxs-lookup"><span data-stu-id="690ab-158">String</span></span>|<span data-ttu-id="690ab-159">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="690ab-159">Unique Identifier for the device</span></span>|
|<span data-ttu-id="690ab-160">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="690ab-160">**Device configuration**</span></span>|
|<span data-ttu-id="690ab-161">settings</span><span class="sxs-lookup"><span data-stu-id="690ab-161">settings</span></span>|[<span data-ttu-id="690ab-162">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="690ab-162">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="690ab-163">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="690ab-163">Account level settings.</span></span>|
|<span data-ttu-id="690ab-164">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="690ab-164">**Device management**</span></span>|
|<span data-ttu-id="690ab-165">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="690ab-165">subscriptionState</span></span>|[<span data-ttu-id="690ab-166">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="690ab-166">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="690ab-167">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="690ab-167">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="690ab-168">Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="690ab-168">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="690ab-169">**Integração**</span><span class="sxs-lookup"><span data-stu-id="690ab-169">**Onboarding**</span></span>|
|<span data-ttu-id="690ab-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="690ab-170">intuneBrand</span></span>|[<span data-ttu-id="690ab-171">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="690ab-171">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="690ab-172">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="690ab-172">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="690ab-173">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="690ab-173">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="690ab-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="690ab-174">Response</span></span>
<span data-ttu-id="690ab-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="690ab-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="690ab-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="690ab-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="690ab-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="690ab-177">Request</span></span>
<span data-ttu-id="690ab-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="690ab-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="690ab-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="690ab-179">Response</span></span>

<span data-ttu-id="690ab-180">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="690ab-180">Here is an example of the response.</span></span> <span data-ttu-id="690ab-181">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="690ab-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="690ab-182">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="690ab-182">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```






