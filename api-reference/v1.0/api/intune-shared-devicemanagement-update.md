---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f265c4e8665d607b1bed87e7c61949131877fa99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019114"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="0f88e-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="0f88e-103">Update deviceManagement</span></span>

<span data-ttu-id="0f88e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f88e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f88e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f88e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f88e-106">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0f88e-106">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f88e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f88e-107">Prerequisites</span></span>
<span data-ttu-id="0f88e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f88e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f88e-110">&nbsp;Tipo &nbsp; de permissão (por &nbsp; fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="0f88e-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="0f88e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f88e-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="0f88e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f88e-112">Delegated (work or school account)</span></span> |
| <span data-ttu-id="0f88e-113">&nbsp;&nbsp;Auditoria</span><span class="sxs-lookup"><span data-stu-id="0f88e-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="0f88e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-115">&nbsp;&nbsp;Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="0f88e-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="0f88e-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-117">&nbsp;&nbsp;Registro corporativo</span><span class="sxs-lookup"><span data-stu-id="0f88e-117">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="0f88e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="0f88e-119">&nbsp;&nbsp;Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0f88e-119">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="0f88e-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-121">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0f88e-121">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="0f88e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-123">&nbsp;&nbsp;Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="0f88e-123">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="0f88e-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-125">&nbsp;&nbsp;Notificação</span><span class="sxs-lookup"><span data-stu-id="0f88e-125">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="0f88e-126">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-126">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-127">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="0f88e-127">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0f88e-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-129">&nbsp;&nbsp;Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="0f88e-129">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="0f88e-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-130">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-131">&nbsp;&nbsp;Assistência remota</span><span class="sxs-lookup"><span data-stu-id="0f88e-131">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="0f88e-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-133">&nbsp;&nbsp;Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="0f88e-133">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="0f88e-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-135">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="0f88e-135">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="0f88e-136">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-136">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-137">&nbsp;&nbsp;Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="0f88e-137">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="0f88e-138">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f88e-138">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0f88e-139">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f88e-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f88e-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f88e-140">Not supported.</span></span>|
| <span data-ttu-id="0f88e-141">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f88e-141">Application</span></span> | <span data-ttu-id="0f88e-142">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f88e-142">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f88e-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f88e-143">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="0f88e-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f88e-144">Request headers</span></span>
|<span data-ttu-id="0f88e-145">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f88e-145">Header</span></span>|<span data-ttu-id="0f88e-146">Valor</span><span class="sxs-lookup"><span data-stu-id="0f88e-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f88e-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f88e-147">Authorization</span></span>|<span data-ttu-id="0f88e-148">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f88e-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f88e-149">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f88e-149">Accept</span></span>|<span data-ttu-id="0f88e-150">application/json</span><span class="sxs-lookup"><span data-stu-id="0f88e-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f88e-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f88e-151">Request body</span></span>
<span data-ttu-id="0f88e-152">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0f88e-152">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="0f88e-153">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0f88e-153">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="0f88e-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f88e-154">Property</span></span>|<span data-ttu-id="0f88e-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f88e-155">Type</span></span>|<span data-ttu-id="0f88e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f88e-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f88e-157">id</span><span class="sxs-lookup"><span data-stu-id="0f88e-157">id</span></span>|<span data-ttu-id="0f88e-158">String</span><span class="sxs-lookup"><span data-stu-id="0f88e-158">String</span></span>|<span data-ttu-id="0f88e-159">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0f88e-159">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0f88e-160">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0f88e-160">**Device configuration**</span></span>|
|<span data-ttu-id="0f88e-161">settings</span><span class="sxs-lookup"><span data-stu-id="0f88e-161">settings</span></span>|[<span data-ttu-id="0f88e-162">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="0f88e-162">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="0f88e-163">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="0f88e-163">Account level settings.</span></span>|
|<span data-ttu-id="0f88e-164">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="0f88e-164">**Device management**</span></span>|
|<span data-ttu-id="0f88e-165">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="0f88e-165">subscriptionState</span></span>|[<span data-ttu-id="0f88e-166">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="0f88e-166">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="0f88e-167">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="0f88e-167">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="0f88e-168">Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="0f88e-168">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="0f88e-169">**Integração**</span><span class="sxs-lookup"><span data-stu-id="0f88e-169">**Onboarding**</span></span>|
|<span data-ttu-id="0f88e-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="0f88e-170">intuneBrand</span></span>|[<span data-ttu-id="0f88e-171">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="0f88e-171">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="0f88e-172">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="0f88e-172">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="0f88e-173">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="0f88e-173">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="0f88e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f88e-174">Response</span></span>
<span data-ttu-id="0f88e-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f88e-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f88e-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f88e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f88e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f88e-177">Request</span></span>
<span data-ttu-id="0f88e-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f88e-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f88e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f88e-179">Response</span></span>

<span data-ttu-id="0f88e-180">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f88e-180">Here is an example of the response.</span></span> <span data-ttu-id="0f88e-181">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0f88e-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0f88e-182">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="0f88e-182">Returned properties vary according to workflow and context.</span></span>

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









