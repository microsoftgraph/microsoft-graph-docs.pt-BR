---
title: Listar deviceManagementScriptGroupAssignments
description: Listar Propriedades e relações dos objetos deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a795b92095fe53d616c73ee6db8b58b1afd65dbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469290"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="46264-103">Listar deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="46264-103">List deviceManagementScriptGroupAssignments</span></span>

<span data-ttu-id="46264-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="46264-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46264-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46264-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46264-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46264-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46264-107">Listar Propriedades e relações dos objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="46264-107">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46264-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46264-108">Prerequisites</span></span>
<span data-ttu-id="46264-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46264-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46264-111">Permission type</span></span>|<span data-ttu-id="46264-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46264-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46264-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46264-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46264-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46264-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="46264-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46264-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46264-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46264-116">Not supported.</span></span>|
|<span data-ttu-id="46264-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46264-117">Application</span></span>|<span data-ttu-id="46264-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46264-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46264-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46264-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="46264-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46264-120">Request headers</span></span>
|<span data-ttu-id="46264-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46264-121">Header</span></span>|<span data-ttu-id="46264-122">Valor</span><span class="sxs-lookup"><span data-stu-id="46264-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46264-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46264-123">Authorization</span></span>|<span data-ttu-id="46264-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46264-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46264-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46264-125">Accept</span></span>|<span data-ttu-id="46264-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46264-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46264-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46264-127">Request body</span></span>
<span data-ttu-id="46264-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46264-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46264-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46264-129">Response</span></span>
<span data-ttu-id="46264-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46264-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46264-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46264-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="46264-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46264-132">Request</span></span>
<span data-ttu-id="46264-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46264-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="46264-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46264-134">Response</span></span>
<span data-ttu-id="46264-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46264-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





