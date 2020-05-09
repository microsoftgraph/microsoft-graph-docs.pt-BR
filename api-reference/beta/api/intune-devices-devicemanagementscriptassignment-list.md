---
title: Listar deviceManagementScriptAssignments
description: Listar Propriedades e relações dos objetos deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 133676783e26ede198494f5539cf9e40f744054c
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176579"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="a818c-103">Listar deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="a818c-103">List deviceManagementScriptAssignments</span></span>

<span data-ttu-id="a818c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a818c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a818c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a818c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a818c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a818c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a818c-107">Listar Propriedades e relações dos objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a818c-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a818c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a818c-108">Prerequisites</span></span>
<span data-ttu-id="a818c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a818c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a818c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a818c-111">Permission type</span></span>|<span data-ttu-id="a818c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a818c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a818c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a818c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a818c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a818c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a818c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a818c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a818c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a818c-116">Not supported.</span></span>|
|<span data-ttu-id="a818c-117">Application</span><span class="sxs-lookup"><span data-stu-id="a818c-117">Application</span></span>|<span data-ttu-id="a818c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a818c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a818c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a818c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a818c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a818c-120">Request headers</span></span>
|<span data-ttu-id="a818c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a818c-121">Header</span></span>|<span data-ttu-id="a818c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a818c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a818c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a818c-123">Authorization</span></span>|<span data-ttu-id="a818c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a818c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a818c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a818c-125">Accept</span></span>|<span data-ttu-id="a818c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a818c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a818c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a818c-127">Request body</span></span>
<span data-ttu-id="a818c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a818c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a818c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a818c-129">Response</span></span>
<span data-ttu-id="a818c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a818c-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a818c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a818c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a818c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a818c-132">Request</span></span>
<span data-ttu-id="a818c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a818c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="a818c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a818c-134">Response</span></span>
<span data-ttu-id="a818c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a818c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



