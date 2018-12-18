---
title: função autopilotDeviceStream
description: Crie uma solicitação de carregamento com fluxo de dispositivo piloto automático nela.
author: tfitzmac
ms.openlocfilehash: 6de8f8620ec5f4e189701a51644c55417118b868
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350852"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="12fcb-103">função autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="12fcb-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="12fcb-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="12fcb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12fcb-105">Crie uma solicitação de carregamento com fluxo de dispositivo piloto automático nela.</span><span class="sxs-lookup"><span data-stu-id="12fcb-105">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12fcb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12fcb-106">Prerequisites</span></span>
<span data-ttu-id="12fcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fcb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12fcb-109">Permission type</span></span>|<span data-ttu-id="12fcb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12fcb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fcb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12fcb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12fcb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fcb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12fcb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12fcb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fcb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fcb-114">Not supported.</span></span>|
|<span data-ttu-id="12fcb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12fcb-115">Application</span></span>|<span data-ttu-id="12fcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fcb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fcb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12fcb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="12fcb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12fcb-118">Request headers</span></span>
|<span data-ttu-id="12fcb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12fcb-119">Header</span></span>|<span data-ttu-id="12fcb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="12fcb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="12fcb-121">Authorization</span></span>|<span data-ttu-id="12fcb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12fcb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fcb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="12fcb-123">Accept</span></span>|<span data-ttu-id="12fcb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12fcb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fcb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12fcb-125">Request body</span></span>
<span data-ttu-id="12fcb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12fcb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12fcb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fcb-127">Response</span></span>
<span data-ttu-id="12fcb-128">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12fcb-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fcb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12fcb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="12fcb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12fcb-130">Request</span></span>
<span data-ttu-id="12fcb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12fcb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="12fcb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fcb-132">Response</span></span>
<span data-ttu-id="12fcb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12fcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



