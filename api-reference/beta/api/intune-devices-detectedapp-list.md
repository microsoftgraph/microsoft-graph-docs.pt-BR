---
title: Listar detectedApps
description: Listar propriedades e relações dos objetos detectedApp.
ms.openlocfilehash: 1e485f8fe0bb02818c8e5ed55b8ddd7da86379ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038775"
---
# <a name="list-detectedapps"></a><span data-ttu-id="e5438-103">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="e5438-103">List detectedApps</span></span>

> <span data-ttu-id="e5438-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5438-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5438-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5438-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5438-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e5438-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5438-107">Listar propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5438-107">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5438-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5438-108">Prerequisites</span></span>
<span data-ttu-id="e5438-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5438-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5438-111">Permission type</span></span>|<span data-ttu-id="e5438-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5438-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5438-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5438-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5438-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e5438-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5438-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5438-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5438-116">Not supported.</span></span>|
|<span data-ttu-id="e5438-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5438-117">Application</span></span>|<span data-ttu-id="e5438-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5438-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5438-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5438-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="e5438-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5438-120">Request headers</span></span>
|<span data-ttu-id="e5438-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5438-121">Header</span></span>|<span data-ttu-id="e5438-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5438-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5438-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5438-123">Authorization</span></span>|<span data-ttu-id="e5438-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5438-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5438-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5438-125">Accept</span></span>|<span data-ttu-id="e5438-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5438-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5438-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5438-127">Request body</span></span>
<span data-ttu-id="e5438-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5438-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5438-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5438-129">Response</span></span>
<span data-ttu-id="e5438-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5438-130">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5438-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5438-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5438-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5438-132">Request</span></span>
<span data-ttu-id="e5438-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5438-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="e5438-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5438-134">Response</span></span>
<span data-ttu-id="e5438-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5438-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```





