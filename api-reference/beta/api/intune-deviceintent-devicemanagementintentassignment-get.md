---
title: Obter deviceManagementIntentAssignment
description: Leia as propriedades e as relações do objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5df05efed01dc16457d737699237cd6f110846cb
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792566"
---
# <a name="get-devicemanagementintentassignment"></a><span data-ttu-id="92128-103">Obter deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="92128-103">Get deviceManagementIntentAssignment</span></span>

<span data-ttu-id="92128-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92128-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92128-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92128-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92128-107">Leia as propriedades e as relações do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="92128-107">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92128-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92128-108">Prerequisites</span></span>
<span data-ttu-id="92128-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="92128-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92128-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92128-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92128-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92128-111">Permission type</span></span>|<span data-ttu-id="92128-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92128-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92128-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92128-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92128-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92128-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92128-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92128-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92128-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92128-116">Not supported.</span></span>|
|<span data-ttu-id="92128-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92128-117">Application</span></span>|<span data-ttu-id="92128-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92128-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92128-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92128-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92128-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92128-120">Optional query parameters</span></span>
<span data-ttu-id="92128-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92128-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92128-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92128-122">Request headers</span></span>
|<span data-ttu-id="92128-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92128-123">Header</span></span>|<span data-ttu-id="92128-124">Valor</span><span class="sxs-lookup"><span data-stu-id="92128-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92128-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="92128-125">Authorization</span></span>|<span data-ttu-id="92128-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92128-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92128-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92128-127">Accept</span></span>|<span data-ttu-id="92128-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92128-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92128-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92128-129">Request body</span></span>
<span data-ttu-id="92128-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92128-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92128-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92128-131">Response</span></span>
<span data-ttu-id="92128-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92128-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92128-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92128-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="92128-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92128-134">Request</span></span>
<span data-ttu-id="92128-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92128-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

### <a name="response"></a><span data-ttu-id="92128-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92128-136">Response</span></span>
<span data-ttu-id="92128-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="92128-137">Here is an example of the response.</span></span> <span data-ttu-id="92128-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="92128-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="92128-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="92128-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
    "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```



