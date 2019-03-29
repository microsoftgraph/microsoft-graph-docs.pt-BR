---
title: Obter importedWindowsAutopilotDeviceIdentityUpload
description: Leia as propriedades e as relações do objeto importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cb9962e4b1328c75558c9ff77b6dabe2f86c4de
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958372"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="a64af-103">Obter importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="a64af-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="a64af-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a64af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a64af-105">Leia as propriedades e as relações do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="a64af-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a64af-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a64af-106">Prerequisites</span></span>
<span data-ttu-id="a64af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a64af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a64af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a64af-109">Permission type</span></span>|<span data-ttu-id="a64af-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a64af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a64af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a64af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a64af-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a64af-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a64af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a64af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a64af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a64af-114">Not supported.</span></span>|
|<span data-ttu-id="a64af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a64af-115">Application</span></span>|<span data-ttu-id="a64af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a64af-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a64af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a64af-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a64af-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a64af-118">Optional query parameters</span></span>
<span data-ttu-id="a64af-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a64af-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a64af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-120">Request headers</span></span>
|<span data-ttu-id="a64af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a64af-121">Header</span></span>|<span data-ttu-id="a64af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a64af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a64af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a64af-123">Authorization</span></span>|<span data-ttu-id="a64af-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a64af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a64af-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a64af-125">Accept</span></span>|<span data-ttu-id="a64af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a64af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a64af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-127">Request body</span></span>
<span data-ttu-id="a64af-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a64af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a64af-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64af-129">Response</span></span>
<span data-ttu-id="a64af-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a64af-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64af-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a64af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a64af-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a64af-132">Request</span></span>
<span data-ttu-id="a64af-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a64af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="a64af-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a64af-134">Response</span></span>
<span data-ttu-id="a64af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a64af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



