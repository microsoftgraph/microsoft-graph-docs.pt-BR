---
title: Obter importedWindowsAutopilotDeviceIdentity
description: Lê as propriedades e relações do objeto importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
ms.openlocfilehash: 0f9d1c80fae8144dc37110345f9162e3c006f9fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309356"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="775fc-103">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="775fc-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="775fc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="775fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="775fc-105">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="775fc-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="775fc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="775fc-106">Prerequisites</span></span>
<span data-ttu-id="775fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="775fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="775fc-109">Permission type</span></span>|<span data-ttu-id="775fc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="775fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="775fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="775fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="775fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="775fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="775fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="775fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="775fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775fc-114">Not supported.</span></span>|
|<span data-ttu-id="775fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="775fc-115">Application</span></span>|<span data-ttu-id="775fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="775fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="775fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="775fc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="775fc-118">Optional query parameters</span></span>
<span data-ttu-id="775fc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="775fc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="775fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="775fc-120">Request headers</span></span>
|<span data-ttu-id="775fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="775fc-121">Header</span></span>|<span data-ttu-id="775fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="775fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="775fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="775fc-123">Authorization</span></span>|<span data-ttu-id="775fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="775fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="775fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="775fc-125">Accept</span></span>|<span data-ttu-id="775fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="775fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="775fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="775fc-127">Request body</span></span>
<span data-ttu-id="775fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="775fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="775fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="775fc-129">Response</span></span>
<span data-ttu-id="775fc-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="775fc-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="775fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="775fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="775fc-132">Request</span></span>
<span data-ttu-id="775fc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="775fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="775fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="775fc-134">Response</span></span>
<span data-ttu-id="775fc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="775fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



