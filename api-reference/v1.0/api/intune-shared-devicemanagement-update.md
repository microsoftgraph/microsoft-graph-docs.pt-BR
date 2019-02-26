---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c96877d25476ede3cee6ce407c1df84f08448a9a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253054"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="e250a-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e250a-103">Update deviceManagement</span></span>

> <span data-ttu-id="e250a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e250a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e250a-105">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e250a-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e250a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e250a-106">Prerequisites</span></span>
<span data-ttu-id="e250a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e250a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e250a-109">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="e250a-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="e250a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e250a-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="e250a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e250a-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="e250a-112">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="e250a-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="e250a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-114">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="e250a-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="e250a-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-116">&nbsp;&nbsp; Registro corporativo</span><span class="sxs-lookup"><span data-stu-id="e250a-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="e250a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="e250a-118">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e250a-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="e250a-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-120">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e250a-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="e250a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-122">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="e250a-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="e250a-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-124">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="e250a-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="e250a-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-126">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="e250a-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="e250a-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-128">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="e250a-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="e250a-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-130">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="e250a-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="e250a-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-132">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="e250a-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="e250a-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-134">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e250a-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e250a-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-136">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="e250a-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="e250a-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e250a-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e250a-138">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e250a-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e250a-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e250a-139">Not supported.</span></span>|
| <span data-ttu-id="e250a-140">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e250a-140">Application</span></span> | <span data-ttu-id="e250a-141">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e250a-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e250a-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e250a-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="e250a-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e250a-143">Request headers</span></span>
|<span data-ttu-id="e250a-144">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e250a-144">Header</span></span>|<span data-ttu-id="e250a-145">Valor</span><span class="sxs-lookup"><span data-stu-id="e250a-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e250a-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="e250a-146">Authorization</span></span>|<span data-ttu-id="e250a-147">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e250a-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e250a-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e250a-148">Accept</span></span>|<span data-ttu-id="e250a-149">application/json</span><span class="sxs-lookup"><span data-stu-id="e250a-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e250a-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e250a-150">Request body</span></span>
<span data-ttu-id="e250a-151">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e250a-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="e250a-152">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e250a-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="e250a-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e250a-153">Property</span></span>|<span data-ttu-id="e250a-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="e250a-154">Type</span></span>|<span data-ttu-id="e250a-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="e250a-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e250a-156">id</span><span class="sxs-lookup"><span data-stu-id="e250a-156">id</span></span>|<span data-ttu-id="e250a-157">String</span><span class="sxs-lookup"><span data-stu-id="e250a-157">String</span></span>|<span data-ttu-id="e250a-158">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e250a-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="e250a-159">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e250a-159">**Device configuration**</span></span>|
|<span data-ttu-id="e250a-160">settings</span><span class="sxs-lookup"><span data-stu-id="e250a-160">settings</span></span>|[<span data-ttu-id="e250a-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e250a-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="e250a-162">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="e250a-162">Account level settings.</span></span>|
|<span data-ttu-id="e250a-163">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="e250a-163">**Device management**</span></span>|
|<span data-ttu-id="e250a-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="e250a-164">subscriptionState</span></span>|[<span data-ttu-id="e250a-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="e250a-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="e250a-166">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="e250a-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="e250a-167">Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="e250a-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="e250a-168">**Integração**</span><span class="sxs-lookup"><span data-stu-id="e250a-168">**Onboarding**</span></span>|
|<span data-ttu-id="e250a-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="e250a-169">intuneBrand</span></span>|[<span data-ttu-id="e250a-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="e250a-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="e250a-171">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="e250a-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="e250a-172">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="e250a-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="e250a-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e250a-173">Response</span></span>
<span data-ttu-id="e250a-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e250a-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e250a-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e250a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e250a-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e250a-176">Request</span></span>
<span data-ttu-id="e250a-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e250a-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e250a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="e250a-178">Response</span></span>

<span data-ttu-id="e250a-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e250a-179">Here is an example of the response.</span></span> <span data-ttu-id="e250a-180">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e250a-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e250a-181">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="e250a-181">Returned properties vary according to workflow and context.</span></span>

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



