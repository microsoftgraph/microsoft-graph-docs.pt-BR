---
title: Listar importedWindowsAutopilotDeviceIdentities
description: Lista as propriedades e relações de objetos importedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7b077021809dbd0927a48c8c940b29498792222
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364127"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="cbd61-103">Listar importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="cbd61-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="cbd61-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbd61-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbd61-105">Lista as propriedades e relações de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="cbd61-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbd61-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbd61-106">Prerequisites</span></span>
<span data-ttu-id="cbd61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbd61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbd61-109">Permission type</span></span>|<span data-ttu-id="cbd61-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbd61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbd61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbd61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbd61-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbd61-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cbd61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbd61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbd61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbd61-114">Not supported.</span></span>|
|<span data-ttu-id="cbd61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbd61-115">Application</span></span>|<span data-ttu-id="cbd61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbd61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbd61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbd61-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="cbd61-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd61-118">Request headers</span></span>
|<span data-ttu-id="cbd61-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbd61-119">Header</span></span>|<span data-ttu-id="cbd61-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cbd61-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbd61-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbd61-121">Authorization</span></span>|<span data-ttu-id="cbd61-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbd61-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbd61-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbd61-123">Accept</span></span>|<span data-ttu-id="cbd61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbd61-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbd61-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd61-125">Request body</span></span>
<span data-ttu-id="cbd61-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbd61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd61-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd61-127">Response</span></span>
<span data-ttu-id="cbd61-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbd61-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbd61-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbd61-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbd61-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd61-130">Request</span></span>
<span data-ttu-id="cbd61-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbd61-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="cbd61-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd61-132">Response</span></span>
<span data-ttu-id="cbd61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbd61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




