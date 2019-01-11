---
title: ação de executeAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a95d9dd38c317f83e53c0c4bca98a379602df8db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812548"
---
# <a name="executeaction-action"></a><span data-ttu-id="fdfbb-103">ação de executeAction</span><span class="sxs-lookup"><span data-stu-id="fdfbb-103">executeAction action</span></span>

> <span data-ttu-id="fdfbb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdfbb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdfbb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdfbb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdfbb-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdfbb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdfbb-108">Prerequisites</span></span>
<span data-ttu-id="fdfbb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdfbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdfbb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdfbb-111">Permission type</span></span>|<span data-ttu-id="fdfbb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdfbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdfbb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdfbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdfbb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fdfbb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fdfbb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdfbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdfbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-116">Not supported.</span></span>|
|<span data-ttu-id="fdfbb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdfbb-117">Application</span></span>|<span data-ttu-id="fdfbb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdfbb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdfbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="fdfbb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdfbb-120">Request headers</span></span>
|<span data-ttu-id="fdfbb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdfbb-121">Header</span></span>|<span data-ttu-id="fdfbb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdfbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdfbb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdfbb-123">Authorization</span></span>|<span data-ttu-id="fdfbb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdfbb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdfbb-125">Accept</span></span>|<span data-ttu-id="fdfbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdfbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdfbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdfbb-127">Request body</span></span>
<span data-ttu-id="fdfbb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fdfbb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fdfbb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdfbb-130">Property</span></span>|<span data-ttu-id="fdfbb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdfbb-131">Type</span></span>|<span data-ttu-id="fdfbb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdfbb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdfbb-133">actionName</span><span class="sxs-lookup"><span data-stu-id="fdfbb-133">actionName</span></span>|[<span data-ttu-id="fdfbb-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="fdfbb-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="fdfbb-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdfbb-135">Not yet documented</span></span>|
|<span data-ttu-id="fdfbb-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="fdfbb-136">deviceIds</span></span>|<span data-ttu-id="fdfbb-137">String collection</span><span class="sxs-lookup"><span data-stu-id="fdfbb-137">String collection</span></span>|<span data-ttu-id="fdfbb-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdfbb-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fdfbb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdfbb-139">Response</span></span>
<span data-ttu-id="fdfbb-140">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdfbb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdfbb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdfbb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdfbb-142">Request</span></span>
<span data-ttu-id="fdfbb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdfbb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdfbb-144">Response</span></span>
<span data-ttu-id="fdfbb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdfbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





