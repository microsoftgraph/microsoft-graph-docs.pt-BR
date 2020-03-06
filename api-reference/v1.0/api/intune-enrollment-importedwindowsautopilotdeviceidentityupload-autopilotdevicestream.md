---
title: função autopilotDeviceStream
description: Crie uma solicitação de upload com o fluxo de dispositivo do AutoPilot nele.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f87e35744d2a4ba434f45984066a32d4f420d8f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513389"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="853ff-103">função autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="853ff-103">autopilotDeviceStream function</span></span>

<span data-ttu-id="853ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="853ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="853ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="853ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="853ff-106">Crie uma solicitação de upload com o fluxo de dispositivo do AutoPilot nele.</span><span class="sxs-lookup"><span data-stu-id="853ff-106">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="853ff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="853ff-107">Prerequisites</span></span>
<span data-ttu-id="853ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="853ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="853ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="853ff-110">Permission type</span></span>|<span data-ttu-id="853ff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="853ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="853ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="853ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="853ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="853ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="853ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="853ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="853ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="853ff-115">Not supported.</span></span>|
|<span data-ttu-id="853ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="853ff-116">Application</span></span>|<span data-ttu-id="853ff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="853ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="853ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="853ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="853ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="853ff-119">Request headers</span></span>
|<span data-ttu-id="853ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="853ff-120">Header</span></span>|<span data-ttu-id="853ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="853ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="853ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="853ff-122">Authorization</span></span>|<span data-ttu-id="853ff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="853ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="853ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="853ff-124">Accept</span></span>|<span data-ttu-id="853ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="853ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="853ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="853ff-126">Request body</span></span>
<span data-ttu-id="853ff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="853ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="853ff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="853ff-128">Response</span></span>
<span data-ttu-id="853ff-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="853ff-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="853ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="853ff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="853ff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="853ff-131">Request</span></span>
<span data-ttu-id="853ff-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="853ff-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="853ff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="853ff-133">Response</span></span>
<span data-ttu-id="853ff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="853ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```




