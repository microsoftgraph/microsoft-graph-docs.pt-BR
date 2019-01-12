---
title: ação de executeAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23d34a999fdc874126fee527c7c62b32d859d953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912992"
---
# <a name="executeaction-action"></a><span data-ttu-id="9d721-103">ação de executeAction</span><span class="sxs-lookup"><span data-stu-id="9d721-103">executeAction action</span></span>

> <span data-ttu-id="9d721-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d721-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d721-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d721-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d721-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9d721-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d721-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9d721-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d721-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d721-108">Prerequisites</span></span>
<span data-ttu-id="9d721-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d721-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d721-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d721-111">Permission type</span></span>|<span data-ttu-id="9d721-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d721-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d721-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d721-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d721-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9d721-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9d721-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d721-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d721-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d721-116">Not supported.</span></span>|
|<span data-ttu-id="9d721-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d721-117">Application</span></span>|<span data-ttu-id="9d721-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d721-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d721-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d721-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="9d721-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d721-120">Request headers</span></span>
|<span data-ttu-id="9d721-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d721-121">Header</span></span>|<span data-ttu-id="9d721-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d721-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d721-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d721-123">Authorization</span></span>|<span data-ttu-id="9d721-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d721-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d721-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d721-125">Accept</span></span>|<span data-ttu-id="9d721-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d721-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d721-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d721-127">Request body</span></span>
<span data-ttu-id="9d721-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9d721-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9d721-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9d721-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9d721-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d721-130">Property</span></span>|<span data-ttu-id="9d721-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d721-131">Type</span></span>|<span data-ttu-id="9d721-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d721-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d721-133">actionName</span><span class="sxs-lookup"><span data-stu-id="9d721-133">actionName</span></span>|[<span data-ttu-id="9d721-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="9d721-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="9d721-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9d721-135">Not yet documented</span></span>|
|<span data-ttu-id="9d721-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="9d721-136">deviceIds</span></span>|<span data-ttu-id="9d721-137">String collection</span><span class="sxs-lookup"><span data-stu-id="9d721-137">String collection</span></span>|<span data-ttu-id="9d721-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9d721-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9d721-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d721-139">Response</span></span>
<span data-ttu-id="9d721-140">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d721-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d721-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d721-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d721-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d721-142">Request</span></span>
<span data-ttu-id="9d721-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d721-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9d721-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d721-144">Response</span></span>
<span data-ttu-id="9d721-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d721-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```





