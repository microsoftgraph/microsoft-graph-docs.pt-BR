---
title: ação de importação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10e34fb59732616e1396761ee3ccd2e34eba231f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532671"
---
# <a name="import-action"></a><span data-ttu-id="50805-103">ação de importação</span><span class="sxs-lookup"><span data-stu-id="50805-103">import action</span></span>

> <span data-ttu-id="50805-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50805-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50805-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50805-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50805-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50805-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50805-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50805-107">Prerequisites</span></span>
<span data-ttu-id="50805-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50805-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50805-110">Permission type</span></span>|<span data-ttu-id="50805-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50805-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50805-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50805-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50805-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50805-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50805-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50805-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50805-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50805-115">Not supported.</span></span>|
|<span data-ttu-id="50805-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50805-116">Application</span></span>|<span data-ttu-id="50805-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50805-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50805-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50805-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="50805-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50805-119">Request headers</span></span>
|<span data-ttu-id="50805-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50805-120">Header</span></span>|<span data-ttu-id="50805-121">Valor</span><span class="sxs-lookup"><span data-stu-id="50805-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50805-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="50805-122">Authorization</span></span>|<span data-ttu-id="50805-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50805-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50805-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50805-124">Accept</span></span>|<span data-ttu-id="50805-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50805-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50805-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50805-126">Request body</span></span>
<span data-ttu-id="50805-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="50805-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="50805-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="50805-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="50805-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50805-129">Property</span></span>|<span data-ttu-id="50805-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="50805-130">Type</span></span>|<span data-ttu-id="50805-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="50805-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50805-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="50805-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="50805-133">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="50805-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="50805-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50805-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="50805-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50805-135">Response</span></span>
<span data-ttu-id="50805-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50805-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50805-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50805-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="50805-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50805-138">Request</span></span>
<span data-ttu-id="50805-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50805-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 748

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="50805-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50805-140">Response</span></span>
<span data-ttu-id="50805-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50805-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 713

{
  "value": [
    {
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
      }
    }
  ]
}
```





