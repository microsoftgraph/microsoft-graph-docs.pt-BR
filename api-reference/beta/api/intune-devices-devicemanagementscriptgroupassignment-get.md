---
title: Obter deviceManagementScriptGroupAssignment
description: Leia as propriedades e as relações do objeto deviceManagementScriptGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c2edc45405a3a7146da68a7126ec74c35c44592
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087521"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="1dbcb-103">Obter deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1dbcb-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="1dbcb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dbcb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dbcb-106">Leia as propriedades e as relações do objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1dbcb-106">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dbcb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dbcb-107">Prerequisites</span></span>
<span data-ttu-id="1dbcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dbcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbcb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dbcb-110">Permission type</span></span>|<span data-ttu-id="1dbcb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dbcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbcb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dbcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dbcb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dbcb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1dbcb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dbcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbcb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-115">Not supported.</span></span>|
|<span data-ttu-id="1dbcb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dbcb-116">Application</span></span>|<span data-ttu-id="1dbcb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dbcb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbcb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dbcb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dbcb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1dbcb-119">Optional query parameters</span></span>
<span data-ttu-id="1dbcb-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dbcb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbcb-121">Request headers</span></span>
|<span data-ttu-id="1dbcb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dbcb-122">Header</span></span>|<span data-ttu-id="1dbcb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1dbcb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbcb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dbcb-124">Authorization</span></span>|<span data-ttu-id="1dbcb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbcb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dbcb-126">Accept</span></span>|<span data-ttu-id="1dbcb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbcb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbcb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbcb-128">Request body</span></span>
<span data-ttu-id="1dbcb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dbcb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dbcb-130">Response</span></span>
<span data-ttu-id="1dbcb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dbcb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dbcb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dbcb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dbcb-133">Request</span></span>
<span data-ttu-id="1dbcb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="1dbcb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dbcb-135">Response</span></span>
<span data-ttu-id="1dbcb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dbcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```






