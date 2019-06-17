---
title: Obter importedWindowsAutopilotDeviceIdentity
description: Lê as propriedades e relações do objeto importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c349cbe092d638c113031d6499ff6c0615bfee9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981752"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="882e3-103">Obter importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="882e3-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="882e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="882e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="882e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="882e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="882e3-106">Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="882e3-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="882e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="882e3-107">Prerequisites</span></span>
<span data-ttu-id="882e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="882e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="882e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="882e3-110">Permission type</span></span>|<span data-ttu-id="882e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="882e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="882e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="882e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="882e3-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="882e3-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="882e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="882e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="882e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="882e3-115">Not supported.</span></span>|
|<span data-ttu-id="882e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="882e3-116">Application</span></span>|<span data-ttu-id="882e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="882e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="882e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="882e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="882e3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="882e3-119">Optional query parameters</span></span>
<span data-ttu-id="882e3-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="882e3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="882e3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="882e3-121">Request headers</span></span>
|<span data-ttu-id="882e3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="882e3-122">Header</span></span>|<span data-ttu-id="882e3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="882e3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="882e3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="882e3-124">Authorization</span></span>|<span data-ttu-id="882e3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="882e3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="882e3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="882e3-126">Accept</span></span>|<span data-ttu-id="882e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="882e3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="882e3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="882e3-128">Request body</span></span>
<span data-ttu-id="882e3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="882e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="882e3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="882e3-130">Response</span></span>
<span data-ttu-id="882e3-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="882e3-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="882e3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="882e3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="882e3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="882e3-133">Request</span></span>
<span data-ttu-id="882e3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="882e3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="882e3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="882e3-135">Response</span></span>
<span data-ttu-id="882e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="882e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "importId": "Import Id value",
    "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
    "state": {
      "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
      "deviceImportStatus": "pending",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceErrorCode": 15,
      "deviceErrorName": "Device Error Name value"
    },
    "assignedUserPrincipalName": "Assigned User Principal Name value"
  }
}
```





