---
title: ação de executeAction
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 8ab2749e694ac600c141e314018308efe34b4151
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305149"
---
# <a name="executeaction-action"></a><span data-ttu-id="82659-103">ação de executeAction</span><span class="sxs-lookup"><span data-stu-id="82659-103">executeAction action</span></span>

> <span data-ttu-id="82659-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82659-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82659-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82659-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82659-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82659-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82659-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82659-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82659-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82659-108">Prerequisites</span></span>
<span data-ttu-id="82659-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82659-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82659-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82659-111">Permission type</span></span>|<span data-ttu-id="82659-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82659-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82659-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82659-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82659-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="82659-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="82659-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82659-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82659-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82659-116">Not supported.</span></span>|
|<span data-ttu-id="82659-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82659-117">Application</span></span>|<span data-ttu-id="82659-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82659-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82659-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82659-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="82659-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82659-120">Request headers</span></span>
|<span data-ttu-id="82659-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82659-121">Header</span></span>|<span data-ttu-id="82659-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82659-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82659-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82659-123">Authorization</span></span>|<span data-ttu-id="82659-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82659-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82659-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82659-125">Accept</span></span>|<span data-ttu-id="82659-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82659-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82659-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82659-127">Request body</span></span>
<span data-ttu-id="82659-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="82659-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82659-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="82659-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82659-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82659-130">Property</span></span>|<span data-ttu-id="82659-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82659-131">Type</span></span>|<span data-ttu-id="82659-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82659-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82659-133">actionName</span><span class="sxs-lookup"><span data-stu-id="82659-133">actionName</span></span>|[<span data-ttu-id="82659-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="82659-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="82659-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82659-135">Not yet documented</span></span>|
|<span data-ttu-id="82659-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="82659-136">deviceIds</span></span>|<span data-ttu-id="82659-137">String collection</span><span class="sxs-lookup"><span data-stu-id="82659-137">String collection</span></span>|<span data-ttu-id="82659-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82659-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82659-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="82659-139">Response</span></span>
<span data-ttu-id="82659-140">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82659-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82659-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82659-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="82659-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82659-142">Request</span></span>
<span data-ttu-id="82659-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82659-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82659-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="82659-144">Response</span></span>
<span data-ttu-id="82659-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82659-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





