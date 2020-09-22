---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eebc919315bc6faadc4ef5acd887124bbd4223d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056216"
---
# <a name="assign-action"></a><span data-ttu-id="6f9d0-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="6f9d0-103">assign action</span></span>

<span data-ttu-id="6f9d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f9d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f9d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f9d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f9d0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6f9d0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f9d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f9d0-108">Prerequisites</span></span>
<span data-ttu-id="6f9d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f9d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f9d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f9d0-111">Permission type</span></span>|<span data-ttu-id="6f9d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f9d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f9d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f9d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f9d0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f9d0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f9d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f9d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f9d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-116">Not supported.</span></span>|
|<span data-ttu-id="6f9d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f9d0-117">Application</span></span>|<span data-ttu-id="6f9d0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f9d0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f9d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f9d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="6f9d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f9d0-120">Request headers</span></span>
|<span data-ttu-id="6f9d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f9d0-121">Header</span></span>|<span data-ttu-id="6f9d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f9d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f9d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f9d0-123">Authorization</span></span>|<span data-ttu-id="6f9d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f9d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f9d0-125">Accept</span></span>|<span data-ttu-id="6f9d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f9d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f9d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f9d0-127">Request body</span></span>
<span data-ttu-id="6f9d0-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f9d0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f9d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f9d0-130">Property</span></span>|<span data-ttu-id="6f9d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f9d0-131">Type</span></span>|<span data-ttu-id="6f9d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f9d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9d0-133">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="6f9d0-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="6f9d0-134">coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6f9d0-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="6f9d0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6f9d0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f9d0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f9d0-136">Response</span></span>
<span data-ttu-id="6f9d0-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6f9d0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f9d0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f9d0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f9d0-139">Request</span></span>
<span data-ttu-id="6f9d0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 688

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6f9d0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f9d0-141">Response</span></span>
<span data-ttu-id="6f9d0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f9d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






