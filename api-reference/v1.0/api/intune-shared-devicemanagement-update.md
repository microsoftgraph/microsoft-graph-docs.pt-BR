---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
ms.openlocfilehash: f63e9b717f912e255abccedf809772590eb44d1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004626"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="64bea-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="64bea-103">Update deviceManagement</span></span>

> <span data-ttu-id="64bea-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="64bea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64bea-105">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="64bea-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64bea-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64bea-106">Prerequisites</span></span>
<span data-ttu-id="64bea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64bea-109">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="64bea-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="64bea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64bea-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="64bea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64bea-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="64bea-112">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="64bea-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="64bea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-114">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="64bea-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="64bea-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-116">&nbsp;&nbsp; Inscrição corporativa</span><span class="sxs-lookup"><span data-stu-id="64bea-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="64bea-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="64bea-118">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="64bea-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="64bea-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-120">&nbsp;&nbsp; Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="64bea-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="64bea-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-122">&nbsp;&nbsp; Proteção de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="64bea-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="64bea-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-124">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="64bea-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="64bea-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-126">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="64bea-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="64bea-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-128">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="64bea-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="64bea-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-130">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="64bea-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="64bea-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-132">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="64bea-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="64bea-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-134">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="64bea-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="64bea-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-136">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="64bea-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="64bea-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bea-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="64bea-138">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64bea-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64bea-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64bea-139">Not supported.</span></span>|
| <span data-ttu-id="64bea-140">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64bea-140">Application</span></span> | <span data-ttu-id="64bea-141">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64bea-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64bea-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64bea-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="64bea-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64bea-143">Request headers</span></span>
|<span data-ttu-id="64bea-144">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64bea-144">Header</span></span>|<span data-ttu-id="64bea-145">Valor</span><span class="sxs-lookup"><span data-stu-id="64bea-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64bea-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="64bea-146">Authorization</span></span>|<span data-ttu-id="64bea-147">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64bea-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64bea-148">Accept</span><span class="sxs-lookup"><span data-stu-id="64bea-148">Accept</span></span>|<span data-ttu-id="64bea-149">application/json</span><span class="sxs-lookup"><span data-stu-id="64bea-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64bea-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64bea-150">Request body</span></span>
<span data-ttu-id="64bea-151">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="64bea-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="64bea-152">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="64bea-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="64bea-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64bea-153">Property</span></span>|<span data-ttu-id="64bea-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="64bea-154">Type</span></span>|<span data-ttu-id="64bea-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="64bea-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64bea-156">id</span><span class="sxs-lookup"><span data-stu-id="64bea-156">id</span></span>|<span data-ttu-id="64bea-157">String</span><span class="sxs-lookup"><span data-stu-id="64bea-157">String</span></span>|<span data-ttu-id="64bea-158">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="64bea-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="64bea-159">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="64bea-159">**Device configuration**</span></span>|
|<span data-ttu-id="64bea-160">configurações</span><span class="sxs-lookup"><span data-stu-id="64bea-160">settings</span></span>|[<span data-ttu-id="64bea-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="64bea-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="64bea-162">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="64bea-162">Account level settings.</span></span>|
|<span data-ttu-id="64bea-163">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="64bea-163">**Device management**</span></span>|
|<span data-ttu-id="64bea-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="64bea-164">subscriptionState</span></span>|[<span data-ttu-id="64bea-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="64bea-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="64bea-166">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="64bea-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="64bea-167">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="64bea-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="64bea-168">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="64bea-168">**Onboarding**</span></span>|
|<span data-ttu-id="64bea-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="64bea-169">intuneBrand</span></span>|[<span data-ttu-id="64bea-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="64bea-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="64bea-171">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="64bea-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="64bea-172">Suporte de propriedade de corpo de solicitação varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="64bea-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="64bea-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="64bea-173">Response</span></span>
<span data-ttu-id="64bea-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64bea-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64bea-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64bea-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="64bea-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64bea-176">Request</span></span>
<span data-ttu-id="64bea-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64bea-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64bea-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="64bea-178">Response</span></span>

<span data-ttu-id="64bea-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64bea-179">Here is an example of the response.</span></span> <span data-ttu-id="64bea-180">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="64bea-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="64bea-181">Propriedades retornadas variam de acordo com o fluxo de trabalho e contexto.</span><span class="sxs-lookup"><span data-stu-id="64bea-181">Returned properties vary according to workflow and context.</span></span>

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



