---
title: Obter importedWindowsAutopilotDeviceIdentityUpload
description: Leia as propriedades e os relacionamentos do objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 369a1dadd706efc05db6029ab912e964f98bc620
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837034"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="6edac-103">Obter importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="6edac-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="6edac-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6edac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6edac-105">Leia as propriedades e os relacionamentos do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="6edac-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6edac-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6edac-106">Prerequisites</span></span>
<span data-ttu-id="6edac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6edac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6edac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6edac-109">Permission type</span></span>|<span data-ttu-id="6edac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6edac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6edac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6edac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6edac-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6edac-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6edac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6edac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6edac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6edac-114">Not supported.</span></span>|
|<span data-ttu-id="6edac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6edac-115">Application</span></span>|<span data-ttu-id="6edac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6edac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6edac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6edac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6edac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6edac-118">Optional query parameters</span></span>
<span data-ttu-id="6edac-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6edac-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6edac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6edac-120">Request headers</span></span>
|<span data-ttu-id="6edac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6edac-121">Header</span></span>|<span data-ttu-id="6edac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6edac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6edac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6edac-123">Authorization</span></span>|<span data-ttu-id="6edac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6edac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6edac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6edac-125">Accept</span></span>|<span data-ttu-id="6edac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6edac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6edac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6edac-127">Request body</span></span>
<span data-ttu-id="6edac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6edac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6edac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6edac-129">Response</span></span>
<span data-ttu-id="6edac-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6edac-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6edac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6edac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6edac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6edac-132">Request</span></span>
<span data-ttu-id="6edac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6edac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="6edac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6edac-134">Response</span></span>
<span data-ttu-id="6edac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6edac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
    "id": "8d639524-9524-8d63-2495-638d2495638d",
    "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
    "status": "pending"
  }
}
```



