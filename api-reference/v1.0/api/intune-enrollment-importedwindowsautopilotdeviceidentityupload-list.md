---
title: Listar importedWindowsAutopilotDeviceIdentityUploads
description: Listar Propriedades e relações dos objetos importedWindowsAutopilotDeviceIdentityUpload.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e45f340cc1ce23e08a56418f583a64758ebcaf4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364036"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="05dc0-103">Listar importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="05dc0-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="05dc0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05dc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05dc0-105">Listar Propriedades e relações dos objetos [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="05dc0-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05dc0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05dc0-106">Prerequisites</span></span>
<span data-ttu-id="05dc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05dc0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05dc0-109">Permission type</span></span>|<span data-ttu-id="05dc0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05dc0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05dc0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05dc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05dc0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="05dc0-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="05dc0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05dc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05dc0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05dc0-114">Not supported.</span></span>|
|<span data-ttu-id="05dc0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05dc0-115">Application</span></span>|<span data-ttu-id="05dc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05dc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05dc0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05dc0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="05dc0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05dc0-118">Request headers</span></span>
|<span data-ttu-id="05dc0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05dc0-119">Header</span></span>|<span data-ttu-id="05dc0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="05dc0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05dc0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05dc0-121">Authorization</span></span>|<span data-ttu-id="05dc0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05dc0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05dc0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05dc0-123">Accept</span></span>|<span data-ttu-id="05dc0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05dc0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05dc0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05dc0-125">Request body</span></span>
<span data-ttu-id="05dc0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05dc0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05dc0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="05dc0-127">Response</span></span>
<span data-ttu-id="05dc0-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05dc0-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05dc0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05dc0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="05dc0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05dc0-130">Request</span></span>
<span data-ttu-id="05dc0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05dc0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="05dc0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="05dc0-132">Response</span></span>
<span data-ttu-id="05dc0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05dc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




