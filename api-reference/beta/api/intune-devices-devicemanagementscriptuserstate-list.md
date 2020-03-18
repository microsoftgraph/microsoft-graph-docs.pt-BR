---
title: Listar deviceManagementScriptUserStates
description: Listar Propriedades e relações dos objetos deviceManagementScriptUserState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42b294c50d823c33d4f6f88fddba3e41f4581f87
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814355"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="e41fd-103">Listar deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="e41fd-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="e41fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e41fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e41fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e41fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e41fd-106">Listar Propriedades e relações dos objetos [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e41fd-106">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e41fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e41fd-107">Prerequisites</span></span>
<span data-ttu-id="e41fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e41fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e41fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e41fd-110">Permission type</span></span>|<span data-ttu-id="e41fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e41fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e41fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e41fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e41fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e41fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e41fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e41fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e41fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e41fd-115">Not supported.</span></span>|
|<span data-ttu-id="e41fd-116">Application</span><span class="sxs-lookup"><span data-stu-id="e41fd-116">Application</span></span>|<span data-ttu-id="e41fd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e41fd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e41fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e41fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="e41fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e41fd-119">Request headers</span></span>
|<span data-ttu-id="e41fd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e41fd-120">Header</span></span>|<span data-ttu-id="e41fd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e41fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e41fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e41fd-122">Authorization</span></span>|<span data-ttu-id="e41fd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e41fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e41fd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e41fd-124">Accept</span></span>|<span data-ttu-id="e41fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e41fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e41fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e41fd-126">Request body</span></span>
<span data-ttu-id="e41fd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e41fd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e41fd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41fd-128">Response</span></span>
<span data-ttu-id="e41fd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e41fd-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e41fd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e41fd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e41fd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e41fd-131">Request</span></span>
<span data-ttu-id="e41fd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e41fd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="e41fd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e41fd-133">Response</span></span>
<span data-ttu-id="e41fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e41fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




