---
title: Listar deviceManagementScriptAssignments
description: Listar Propriedades e relações dos objetos deviceManagementScriptAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5dd298e0f1724b3b0be15306229211bddc71ff5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945006"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="4cbef-103">Listar deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="4cbef-103">List deviceManagementScriptAssignments</span></span>

> <span data-ttu-id="4cbef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4cbef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cbef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4cbef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cbef-106">Listar Propriedades e relações dos objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4cbef-106">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cbef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4cbef-107">Prerequisites</span></span>
<span data-ttu-id="4cbef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cbef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cbef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cbef-110">Permission type</span></span>|<span data-ttu-id="4cbef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4cbef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cbef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cbef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cbef-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cbef-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4cbef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cbef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cbef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cbef-115">Not supported.</span></span>|
|<span data-ttu-id="4cbef-116">Application</span><span class="sxs-lookup"><span data-stu-id="4cbef-116">Application</span></span>|<span data-ttu-id="4cbef-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cbef-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cbef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cbef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4cbef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cbef-119">Request headers</span></span>
|<span data-ttu-id="4cbef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4cbef-120">Header</span></span>|<span data-ttu-id="4cbef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4cbef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cbef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cbef-122">Authorization</span></span>|<span data-ttu-id="4cbef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cbef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cbef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4cbef-124">Accept</span></span>|<span data-ttu-id="4cbef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cbef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cbef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cbef-126">Request body</span></span>
<span data-ttu-id="4cbef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cbef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cbef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cbef-128">Response</span></span>
<span data-ttu-id="4cbef-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cbef-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cbef-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cbef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cbef-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cbef-131">Request</span></span>
<span data-ttu-id="4cbef-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cbef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="4cbef-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cbef-133">Response</span></span>
<span data-ttu-id="4cbef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cbef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





