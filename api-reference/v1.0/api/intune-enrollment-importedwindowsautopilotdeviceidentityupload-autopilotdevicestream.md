---
title: função autopilotDeviceStream
description: Crie uma solicitação de upload com o fluxo de dispositivo do AutoPilot nele.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df3cd9c7deff70d7cc81f3016d1d08e62c277608
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253712"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="97d62-103">função autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="97d62-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="97d62-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97d62-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d62-105">Crie uma solicitação de upload com o fluxo de dispositivo do AutoPilot nele.</span><span class="sxs-lookup"><span data-stu-id="97d62-105">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97d62-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97d62-106">Prerequisites</span></span>
<span data-ttu-id="97d62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97d62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97d62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97d62-109">Permission type</span></span>|<span data-ttu-id="97d62-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97d62-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97d62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97d62-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d62-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97d62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97d62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d62-114">Not supported.</span></span>|
|<span data-ttu-id="97d62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97d62-115">Application</span></span>|<span data-ttu-id="97d62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d62-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97d62-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="97d62-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97d62-118">Request headers</span></span>
|<span data-ttu-id="97d62-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97d62-119">Header</span></span>|<span data-ttu-id="97d62-120">Valor</span><span class="sxs-lookup"><span data-stu-id="97d62-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97d62-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="97d62-121">Authorization</span></span>|<span data-ttu-id="97d62-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97d62-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97d62-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97d62-123">Accept</span></span>|<span data-ttu-id="97d62-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97d62-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d62-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97d62-125">Request body</span></span>
<span data-ttu-id="97d62-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97d62-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d62-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d62-127">Response</span></span>
<span data-ttu-id="97d62-128">Se tiver êxito, esta função retornará um código de resposta `200 OK` e uma Cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d62-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d62-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97d62-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d62-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97d62-130">Request</span></span>
<span data-ttu-id="97d62-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97d62-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="97d62-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d62-132">Response</span></span>
<span data-ttu-id="97d62-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97d62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



