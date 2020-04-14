---
title: Obter deviceHealthScriptAssignment
description: Leia as propriedades e as relações do objeto deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 003c286b3f068d05e25de7e3b10ba210613075cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426204"
---
# <a name="get-devicehealthscriptassignment"></a><span data-ttu-id="58303-103">Obter deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="58303-103">Get deviceHealthScriptAssignment</span></span>

<span data-ttu-id="58303-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58303-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58303-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58303-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58303-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58303-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58303-107">Leia as propriedades e as relações do objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="58303-107">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58303-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58303-108">Prerequisites</span></span>
<span data-ttu-id="58303-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58303-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58303-111">Permission type</span></span>|<span data-ttu-id="58303-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58303-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58303-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58303-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58303-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58303-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="58303-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58303-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58303-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58303-116">Not supported.</span></span>|
|<span data-ttu-id="58303-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58303-117">Application</span></span>|<span data-ttu-id="58303-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58303-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58303-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58303-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58303-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58303-120">Optional query parameters</span></span>
<span data-ttu-id="58303-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58303-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58303-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58303-122">Request headers</span></span>
|<span data-ttu-id="58303-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58303-123">Header</span></span>|<span data-ttu-id="58303-124">Valor</span><span class="sxs-lookup"><span data-stu-id="58303-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58303-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="58303-125">Authorization</span></span>|<span data-ttu-id="58303-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58303-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58303-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58303-127">Accept</span></span>|<span data-ttu-id="58303-128">application/json</span><span class="sxs-lookup"><span data-stu-id="58303-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58303-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58303-129">Request body</span></span>
<span data-ttu-id="58303-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58303-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58303-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="58303-131">Response</span></span>
<span data-ttu-id="58303-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58303-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58303-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58303-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="58303-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58303-134">Request</span></span>
<span data-ttu-id="58303-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58303-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="58303-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="58303-136">Response</span></span>
<span data-ttu-id="58303-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58303-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
    "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "runRemediationScript": true,
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    }
  }
}
```



