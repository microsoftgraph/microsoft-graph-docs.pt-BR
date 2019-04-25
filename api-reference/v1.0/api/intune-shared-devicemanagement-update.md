---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c96877d25476ede3cee6ce407c1df84f08448a9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576941"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="49b28-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="49b28-103">Update deviceManagement</span></span>

> <span data-ttu-id="49b28-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49b28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49b28-105">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="49b28-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49b28-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49b28-106">Prerequisites</span></span>
<span data-ttu-id="49b28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49b28-109">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="49b28-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="49b28-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49b28-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="49b28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49b28-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="49b28-112">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="49b28-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="49b28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-114">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="49b28-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="49b28-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-116">&nbsp;&nbsp; Registro corporativo</span><span class="sxs-lookup"><span data-stu-id="49b28-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="49b28-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="49b28-118">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="49b28-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="49b28-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-120">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="49b28-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="49b28-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-122">&nbsp;&nbsp; Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="49b28-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="49b28-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-124">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="49b28-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="49b28-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-126">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="49b28-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="49b28-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-128">&nbsp;&nbsp; Controle de acesso baseado em função</span><span class="sxs-lookup"><span data-stu-id="49b28-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="49b28-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-130">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="49b28-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="49b28-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-132">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="49b28-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="49b28-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-134">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="49b28-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="49b28-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-136">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="49b28-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="49b28-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b28-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="49b28-138">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49b28-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49b28-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49b28-139">Not supported.</span></span>|
| <span data-ttu-id="49b28-140">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49b28-140">Application</span></span> | <span data-ttu-id="49b28-141">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49b28-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49b28-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49b28-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="49b28-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49b28-143">Request headers</span></span>
|<span data-ttu-id="49b28-144">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49b28-144">Header</span></span>|<span data-ttu-id="49b28-145">Valor</span><span class="sxs-lookup"><span data-stu-id="49b28-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49b28-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="49b28-146">Authorization</span></span>|<span data-ttu-id="49b28-147">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49b28-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49b28-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49b28-148">Accept</span></span>|<span data-ttu-id="49b28-149">application/json</span><span class="sxs-lookup"><span data-stu-id="49b28-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b28-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49b28-150">Request body</span></span>
<span data-ttu-id="49b28-151">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="49b28-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="49b28-152">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="49b28-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="49b28-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49b28-153">Property</span></span>|<span data-ttu-id="49b28-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="49b28-154">Type</span></span>|<span data-ttu-id="49b28-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b28-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49b28-156">id</span><span class="sxs-lookup"><span data-stu-id="49b28-156">id</span></span>|<span data-ttu-id="49b28-157">String</span><span class="sxs-lookup"><span data-stu-id="49b28-157">String</span></span>|<span data-ttu-id="49b28-158">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="49b28-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="49b28-159">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="49b28-159">**Device configuration**</span></span>|
|<span data-ttu-id="49b28-160">settings</span><span class="sxs-lookup"><span data-stu-id="49b28-160">settings</span></span>|[<span data-ttu-id="49b28-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="49b28-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="49b28-162">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="49b28-162">Account level settings.</span></span>|
|<span data-ttu-id="49b28-163">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="49b28-163">**Device management**</span></span>|
|<span data-ttu-id="49b28-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="49b28-164">subscriptionState</span></span>|[<span data-ttu-id="49b28-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="49b28-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="49b28-166">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="49b28-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="49b28-167">Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="49b28-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="49b28-168">**Integração**</span><span class="sxs-lookup"><span data-stu-id="49b28-168">**Onboarding**</span></span>|
|<span data-ttu-id="49b28-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="49b28-169">intuneBrand</span></span>|[<span data-ttu-id="49b28-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="49b28-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="49b28-171">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="49b28-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="49b28-172">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="49b28-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="49b28-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b28-173">Response</span></span>
<span data-ttu-id="49b28-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49b28-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b28-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49b28-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="49b28-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49b28-176">Request</span></span>
<span data-ttu-id="49b28-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49b28-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49b28-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b28-178">Response</span></span>

<span data-ttu-id="49b28-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49b28-179">Here is an example of the response.</span></span> <span data-ttu-id="49b28-180">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="49b28-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49b28-181">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="49b28-181">Returned properties vary according to workflow and context.</span></span>

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



