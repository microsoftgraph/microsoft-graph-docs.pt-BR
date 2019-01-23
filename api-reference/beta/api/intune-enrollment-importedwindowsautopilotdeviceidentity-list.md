---
title: Listar importedWindowsAutopilotDeviceIdentities
description: Lista as propriedades e relações de objetos importedWindowsAutopilotDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62ac9c96f1815b32353651de5d5530785eda2456
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418110"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="f9f73-103">Listar importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="f9f73-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="f9f73-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9f73-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9f73-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9f73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9f73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f9f73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9f73-107">Lista as propriedades e relações de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f9f73-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9f73-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9f73-108">Prerequisites</span></span>
<span data-ttu-id="f9f73-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9f73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9f73-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f73-111">Permission type</span></span>|<span data-ttu-id="f9f73-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9f73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f73-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9f73-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9f73-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f9f73-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f73-116">Not supported.</span></span>|
|<span data-ttu-id="f9f73-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f73-117">Application</span></span>|<span data-ttu-id="f9f73-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f73-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="f9f73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f73-120">Request headers</span></span>
|<span data-ttu-id="f9f73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9f73-121">Header</span></span>|<span data-ttu-id="f9f73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9f73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f73-123">Authorization</span></span>|<span data-ttu-id="f9f73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f73-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9f73-125">Accept</span></span>|<span data-ttu-id="f9f73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f73-127">Request body</span></span>
<span data-ttu-id="f9f73-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9f73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9f73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f73-129">Response</span></span>
<span data-ttu-id="f9f73-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f73-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f73-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9f73-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9f73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f73-132">Request</span></span>
<span data-ttu-id="f9f73-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="f9f73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f73-134">Response</span></span>
<span data-ttu-id="f9f73-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9f73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




