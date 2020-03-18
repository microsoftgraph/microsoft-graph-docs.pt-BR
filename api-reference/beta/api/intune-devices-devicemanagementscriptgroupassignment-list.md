---
title: Listar deviceManagementScriptGroupAssignments
description: Listar Propriedades e relações dos objetos deviceManagementScriptGroupAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f9b0722bfea44751c267378d0e6a40af3896c1f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814404"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="5f238-103">Listar deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="5f238-103">List deviceManagementScriptGroupAssignments</span></span>

> <span data-ttu-id="5f238-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f238-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f238-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f238-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f238-106">Listar Propriedades e relações dos objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5f238-106">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f238-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f238-107">Prerequisites</span></span>
<span data-ttu-id="5f238-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f238-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f238-110">Permission type</span></span>|<span data-ttu-id="5f238-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f238-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f238-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f238-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f238-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f238-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5f238-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f238-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f238-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f238-115">Not supported.</span></span>|
|<span data-ttu-id="5f238-116">Application</span><span class="sxs-lookup"><span data-stu-id="5f238-116">Application</span></span>|<span data-ttu-id="5f238-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f238-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f238-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f238-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="5f238-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f238-119">Request headers</span></span>
|<span data-ttu-id="5f238-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f238-120">Header</span></span>|<span data-ttu-id="5f238-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f238-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f238-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f238-122">Authorization</span></span>|<span data-ttu-id="5f238-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f238-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f238-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f238-124">Accept</span></span>|<span data-ttu-id="5f238-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f238-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f238-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f238-126">Request body</span></span>
<span data-ttu-id="5f238-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f238-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f238-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f238-128">Response</span></span>
<span data-ttu-id="5f238-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f238-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f238-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f238-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f238-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f238-131">Request</span></span>
<span data-ttu-id="5f238-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f238-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="5f238-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f238-133">Response</span></span>
<span data-ttu-id="5f238-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f238-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```




