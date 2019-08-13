---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97c35f52182a82c2ddf2447e4d22935d8410826c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350913"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="921f0-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="921f0-103">Get deviceManagement</span></span>

> <span data-ttu-id="921f0-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="921f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="921f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="921f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="921f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="921f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921f0-107">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="921f0-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="921f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="921f0-108">Prerequisites</span></span>

<span data-ttu-id="921f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="921f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="921f0-111">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="921f0-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="921f0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="921f0-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="921f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="921f0-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="921f0-114">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="921f0-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="921f0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="921f0-116">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="921f0-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="921f0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="921f0-118">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="921f0-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="921f0-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="921f0-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="921f0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="921f0-122">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="921f0-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="921f0-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="921f0-124">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="921f0-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="921f0-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="921f0-126">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="921f0-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="921f0-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="921f0-128">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="921f0-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="921f0-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-130">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="921f0-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="921f0-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="921f0-132">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="921f0-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="921f0-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="921f0-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="921f0-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-136">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="921f0-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="921f0-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-138">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="921f0-138">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="921f0-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="921f0-140">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="921f0-140">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="921f0-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="921f0-142">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="921f0-142">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="921f0-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-144">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="921f0-144">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="921f0-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="921f0-146">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="921f0-146">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="921f0-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="921f0-148">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="921f0-148">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="921f0-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="921f0-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="921f0-150">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="921f0-150">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="921f0-151">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="921f0-151">Not supported.</span></span>|
| <span data-ttu-id="921f0-152">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="921f0-152">Application</span></span> | <span data-ttu-id="921f0-153">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="921f0-153">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="921f0-154">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="921f0-154">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="921f0-155">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="921f0-155">Optional query parameters</span></span>

<span data-ttu-id="921f0-156">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="921f0-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="921f0-157">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="921f0-157">Request headers</span></span>
|<span data-ttu-id="921f0-158">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="921f0-158">Header</span></span>|<span data-ttu-id="921f0-159">Valor</span><span class="sxs-lookup"><span data-stu-id="921f0-159">Value</span></span>|
|:---|:---|
|<span data-ttu-id="921f0-160">Autorização</span><span class="sxs-lookup"><span data-stu-id="921f0-160">Authorization</span></span>|<span data-ttu-id="921f0-161">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="921f0-161">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="921f0-162">Aceitar</span><span class="sxs-lookup"><span data-stu-id="921f0-162">Accept</span></span>|<span data-ttu-id="921f0-163">application/json</span><span class="sxs-lookup"><span data-stu-id="921f0-163">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="921f0-164">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="921f0-164">Request body</span></span>

<span data-ttu-id="921f0-165">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="921f0-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="921f0-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="921f0-166">Response</span></span>

<span data-ttu-id="921f0-167">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="921f0-167">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921f0-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="921f0-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="921f0-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="921f0-169">Request</span></span>

<span data-ttu-id="921f0-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="921f0-170">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="921f0-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="921f0-171">Response</span></span>

<span data-ttu-id="921f0-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="921f0-172">Here are example of the response.</span></span> 

<span data-ttu-id="921f0-173">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="921f0-173">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="921f0-174">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="921f0-174">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```






