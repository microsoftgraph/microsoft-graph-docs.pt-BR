---
title: Listar deviceManagementScriptUserStates
description: Listar Propriedades e relações dos objetos deviceManagementScriptUserState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d16a8c54a0fc099ef173db8e72ecbed5a11f3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465444"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="62d16-103">Listar deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="62d16-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="62d16-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62d16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62d16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d16-106">Listar Propriedades e relações dos objetos [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="62d16-106">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62d16-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62d16-107">Prerequisites</span></span>
<span data-ttu-id="62d16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62d16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62d16-110">Permission type</span></span>|<span data-ttu-id="62d16-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62d16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62d16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62d16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62d16-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="62d16-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="62d16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62d16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62d16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d16-115">Not supported.</span></span>|
|<span data-ttu-id="62d16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62d16-116">Application</span></span>|<span data-ttu-id="62d16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62d16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62d16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62d16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="62d16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62d16-119">Request headers</span></span>
|<span data-ttu-id="62d16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62d16-120">Header</span></span>|<span data-ttu-id="62d16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="62d16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62d16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="62d16-122">Authorization</span></span>|<span data-ttu-id="62d16-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62d16-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62d16-124">Accept</span></span>|<span data-ttu-id="62d16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62d16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62d16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62d16-126">Request body</span></span>
<span data-ttu-id="62d16-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62d16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62d16-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d16-128">Response</span></span>
<span data-ttu-id="62d16-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62d16-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d16-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62d16-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="62d16-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62d16-131">Request</span></span>
<span data-ttu-id="62d16-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62d16-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="62d16-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="62d16-133">Response</span></span>
<span data-ttu-id="62d16-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62d16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





