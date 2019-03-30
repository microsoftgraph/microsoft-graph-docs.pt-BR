---
title: Obter importedWindowsAutopilotDeviceIdentity
description: Lê as propriedades e relações do objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 459ba1a0673740b2f65147a198479ddc41ea99af
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989019"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="ff667-103">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ff667-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="ff667-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff667-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff667-105">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ff667-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff667-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff667-106">Prerequisites</span></span>
<span data-ttu-id="ff667-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff667-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff667-109">Permission type</span></span>|<span data-ttu-id="ff667-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff667-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff667-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff667-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff667-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff667-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ff667-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff667-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff667-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff667-114">Not supported.</span></span>|
|<span data-ttu-id="ff667-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff667-115">Application</span></span>|<span data-ttu-id="ff667-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff667-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff667-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff667-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff667-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff667-118">Optional query parameters</span></span>
<span data-ttu-id="ff667-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff667-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff667-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff667-120">Request headers</span></span>
|<span data-ttu-id="ff667-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff667-121">Header</span></span>|<span data-ttu-id="ff667-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff667-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff667-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff667-123">Authorization</span></span>|<span data-ttu-id="ff667-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff667-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff667-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff667-125">Accept</span></span>|<span data-ttu-id="ff667-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff667-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff667-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff667-127">Request body</span></span>
<span data-ttu-id="ff667-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff667-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff667-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff667-129">Response</span></span>
<span data-ttu-id="ff667-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff667-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff667-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff667-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff667-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff667-132">Request</span></span>
<span data-ttu-id="ff667-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff667-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="ff667-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff667-134">Response</span></span>
<span data-ttu-id="ff667-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff667-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



