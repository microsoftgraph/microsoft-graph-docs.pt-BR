---
title: Obter importedWindowsAutopilotDeviceIdentity
description: Lê as propriedades e relações do objeto importedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca3d5ee5b5fe43534acbd1d9627e17c59e7f71cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513410"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e1908-103">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e1908-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="e1908-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1908-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1908-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1908-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1908-106">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e1908-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1908-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1908-107">Prerequisites</span></span>
<span data-ttu-id="e1908-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1908-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1908-110">Permission type</span></span>|<span data-ttu-id="e1908-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1908-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1908-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1908-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1908-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1908-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e1908-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1908-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1908-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1908-115">Not supported.</span></span>|
|<span data-ttu-id="e1908-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1908-116">Application</span></span>|<span data-ttu-id="e1908-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1908-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1908-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1908-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1908-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1908-119">Optional query parameters</span></span>
<span data-ttu-id="e1908-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1908-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1908-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1908-121">Request headers</span></span>
|<span data-ttu-id="e1908-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1908-122">Header</span></span>|<span data-ttu-id="e1908-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e1908-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1908-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1908-124">Authorization</span></span>|<span data-ttu-id="e1908-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1908-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1908-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1908-126">Accept</span></span>|<span data-ttu-id="e1908-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1908-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1908-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1908-128">Request body</span></span>
<span data-ttu-id="e1908-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1908-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1908-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1908-130">Response</span></span>
<span data-ttu-id="e1908-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1908-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1908-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1908-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1908-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1908-133">Request</span></span>
<span data-ttu-id="e1908-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1908-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="e1908-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1908-135">Response</span></span>
<span data-ttu-id="e1908-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1908-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
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
}
```




