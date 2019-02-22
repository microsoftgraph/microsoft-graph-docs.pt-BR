---
title: Get deviceManagement
description: Ler propriedades e relações do objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a74718ee1f05b27c58b3515c29a0190428107314
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156494"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="e4194-103">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4194-103">Get deviceManagement</span></span>

> <span data-ttu-id="e4194-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4194-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4194-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4194-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4194-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4194-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4194-107">Ler propriedades e relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e4194-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4194-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4194-108">Prerequisites</span></span>

<span data-ttu-id="e4194-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4194-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

| <span data-ttu-id="e4194-111">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="e4194-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="e4194-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4194-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="e4194-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4194-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="e4194-114">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="e4194-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="e4194-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e4194-116">&nbsp;&nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="e4194-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="e4194-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e4194-118">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="e4194-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="e4194-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e4194-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e4194-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e4194-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e4194-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e4194-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e4194-124">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="e4194-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="e4194-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e4194-126">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="e4194-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="e4194-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-128">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="e4194-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="e4194-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e4194-130">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="e4194-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="e4194-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-132">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="e4194-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e4194-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="e4194-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="e4194-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="e4194-136">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="e4194-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="e4194-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e4194-138">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="e4194-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="e4194-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-140">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="e4194-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="e4194-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e4194-142">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e4194-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e4194-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e4194-144">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="e4194-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="e4194-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4194-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e4194-146">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4194-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4194-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4194-147">Not supported.</span></span>|
| <span data-ttu-id="e4194-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4194-148">Application</span></span> | <span data-ttu-id="e4194-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4194-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="e4194-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4194-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4194-151">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4194-151">Optional query parameters</span></span>

<span data-ttu-id="e4194-152">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4194-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4194-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4194-153">Request headers</span></span>
|<span data-ttu-id="e4194-154">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4194-154">Header</span></span>|<span data-ttu-id="e4194-155">Valor</span><span class="sxs-lookup"><span data-stu-id="e4194-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4194-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4194-156">Authorization</span></span>|<span data-ttu-id="e4194-157">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4194-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4194-158">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4194-158">Accept</span></span>|<span data-ttu-id="e4194-159">application/json</span><span class="sxs-lookup"><span data-stu-id="e4194-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4194-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4194-160">Request body</span></span>

<span data-ttu-id="e4194-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4194-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4194-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4194-162">Response</span></span>

<span data-ttu-id="e4194-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4194-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4194-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4194-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4194-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4194-165">Request</span></span>

<span data-ttu-id="e4194-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4194-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="e4194-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4194-167">Response</span></span>

<span data-ttu-id="e4194-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4194-168">Here are example of the response.</span></span> 

<span data-ttu-id="e4194-169">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="e4194-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="e4194-170">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="e4194-170">Properties appropriate for the workflow are returned.</span></span>

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



