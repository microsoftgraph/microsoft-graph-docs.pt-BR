---
title: Listar importedWindowsAutopilotDeviceIdentities
description: Lista as propriedades e relações de objetos importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d3a91bcac93fe9d754d86db735793467b995315
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094621"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="4a820-103">Listar importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="4a820-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="4a820-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a820-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a820-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a820-106">Lista as propriedades e relações de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="4a820-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a820-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a820-107">Prerequisites</span></span>
<span data-ttu-id="4a820-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a820-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a820-110">Permission type</span></span>|<span data-ttu-id="4a820-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a820-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a820-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a820-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a820-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a820-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4a820-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a820-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a820-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a820-115">Not supported.</span></span>|
|<span data-ttu-id="4a820-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a820-116">Application</span></span>|<span data-ttu-id="4a820-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a820-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a820-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a820-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4a820-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a820-119">Request headers</span></span>
|<span data-ttu-id="4a820-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a820-120">Header</span></span>|<span data-ttu-id="4a820-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4a820-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a820-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a820-122">Authorization</span></span>|<span data-ttu-id="4a820-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a820-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a820-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a820-124">Accept</span></span>|<span data-ttu-id="4a820-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a820-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a820-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a820-126">Request body</span></span>
<span data-ttu-id="4a820-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a820-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a820-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a820-128">Response</span></span>
<span data-ttu-id="4a820-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a820-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a820-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a820-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a820-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a820-131">Request</span></span>
<span data-ttu-id="4a820-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a820-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="4a820-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a820-133">Response</span></span>
<span data-ttu-id="4a820-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a820-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      }
    }
  ]
}
```









