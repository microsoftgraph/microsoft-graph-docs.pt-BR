---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09563eeced6f557df2c2e40f126623f974cea2d7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976502"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="1a4ce-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1a4ce-103">Get deviceManagement</span></span>

> <span data-ttu-id="1a4ce-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a4ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a4ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a4ce-107">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1a4ce-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a4ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a4ce-108">Prerequisites</span></span>

<span data-ttu-id="1a4ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a4ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a4ce-111">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="1a4ce-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="1a4ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a4ce-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="1a4ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a4ce-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="1a4ce-114">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="1a4ce-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="1a4ce-116">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="1a4ce-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="1a4ce-118">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="1a4ce-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1a4ce-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="1a4ce-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1a4ce-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="1a4ce-124">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="1a4ce-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="1a4ce-126">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="1a4ce-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-128">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="1a4ce-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="1a4ce-130">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="1a4ce-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-132">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1a4ce-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="1a4ce-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="1a4ce-136">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="1a4ce-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="1a4ce-138">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="1a4ce-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-140">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="1a4ce-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="1a4ce-142">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1a4ce-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="1a4ce-144">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="1a4ce-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="1a4ce-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a4ce-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="1a4ce-146">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a4ce-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a4ce-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-147">Not supported.</span></span>|
| <span data-ttu-id="1a4ce-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a4ce-148">Application</span></span> | <span data-ttu-id="1a4ce-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="1a4ce-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a4ce-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a4ce-151">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a4ce-151">Optional query parameters</span></span>

<span data-ttu-id="1a4ce-152">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a4ce-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ce-153">Request headers</span></span>
|<span data-ttu-id="1a4ce-154">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a4ce-154">Header</span></span>|<span data-ttu-id="1a4ce-155">Valor</span><span class="sxs-lookup"><span data-stu-id="1a4ce-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a4ce-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a4ce-156">Authorization</span></span>|<span data-ttu-id="1a4ce-157">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a4ce-158">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a4ce-158">Accept</span></span>|<span data-ttu-id="1a4ce-159">application/json</span><span class="sxs-lookup"><span data-stu-id="1a4ce-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a4ce-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ce-160">Request body</span></span>

<span data-ttu-id="1a4ce-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a4ce-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4ce-162">Response</span></span>

<span data-ttu-id="1a4ce-163">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a4ce-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a4ce-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a4ce-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ce-165">Request</span></span>

<span data-ttu-id="1a4ce-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="1a4ce-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4ce-167">Response</span></span>

<span data-ttu-id="1a4ce-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-168">Here are example of the response.</span></span> 

<span data-ttu-id="1a4ce-169">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="1a4ce-170">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="1a4ce-170">Properties appropriate for the workflow are returned.</span></span>

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



