---
title: Listar importedWindowsAutopilotDeviceIdentityUploads
description: Listar Propriedades e relações dos objetos importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82fcb17b23f820c998aa119c018cdb5c16b418ee
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807655"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="21559-103">Listar importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="21559-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="21559-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21559-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21559-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21559-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21559-106">Listar Propriedades e relações dos objetos [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="21559-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21559-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21559-107">Prerequisites</span></span>
<span data-ttu-id="21559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21559-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21559-110">Permission type</span></span>|<span data-ttu-id="21559-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21559-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21559-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21559-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21559-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21559-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21559-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21559-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21559-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21559-115">Not supported.</span></span>|
|<span data-ttu-id="21559-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21559-116">Application</span></span>|<span data-ttu-id="21559-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21559-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21559-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21559-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="21559-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21559-119">Request headers</span></span>
|<span data-ttu-id="21559-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21559-120">Header</span></span>|<span data-ttu-id="21559-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21559-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21559-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21559-122">Authorization</span></span>|<span data-ttu-id="21559-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21559-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21559-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21559-124">Accept</span></span>|<span data-ttu-id="21559-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21559-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21559-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21559-126">Request body</span></span>
<span data-ttu-id="21559-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21559-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21559-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21559-128">Response</span></span>
<span data-ttu-id="21559-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21559-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21559-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21559-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="21559-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21559-131">Request</span></span>
<span data-ttu-id="21559-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21559-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="21559-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21559-133">Response</span></span>
<span data-ttu-id="21559-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21559-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```





