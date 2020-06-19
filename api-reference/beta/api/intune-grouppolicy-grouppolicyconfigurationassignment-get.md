---
title: Obter groupPolicyConfigurationAssignment
description: Leia as propriedades e as relações do objeto groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 735577cdce7a0c24b1152d88a53f8e557c65393f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791977"
---
# <a name="get-grouppolicyconfigurationassignment"></a><span data-ttu-id="7d3c8-103">Obter groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7d3c8-103">Get groupPolicyConfigurationAssignment</span></span>

<span data-ttu-id="7d3c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d3c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d3c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d3c8-107">Leia as propriedades e as relações do objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7d3c8-107">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d3c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d3c8-108">Prerequisites</span></span>
<span data-ttu-id="7d3c8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7d3c8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3c8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d3c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d3c8-111">Permission type</span></span>|<span data-ttu-id="7d3c8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d3c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d3c8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d3c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d3c8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d3c8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7d3c8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d3c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d3c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-116">Not supported.</span></span>|
|<span data-ttu-id="7d3c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d3c8-117">Application</span></span>|<span data-ttu-id="7d3c8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d3c8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d3c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d3c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d3c8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d3c8-120">Optional query parameters</span></span>
<span data-ttu-id="7d3c8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d3c8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3c8-122">Request headers</span></span>
|<span data-ttu-id="7d3c8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d3c8-123">Header</span></span>|<span data-ttu-id="7d3c8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7d3c8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d3c8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d3c8-125">Authorization</span></span>|<span data-ttu-id="7d3c8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d3c8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d3c8-127">Accept</span></span>|<span data-ttu-id="7d3c8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d3c8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d3c8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3c8-129">Request body</span></span>
<span data-ttu-id="7d3c8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d3c8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d3c8-131">Response</span></span>
<span data-ttu-id="7d3c8-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-132">If successful, this method returns a `200 OK` response code and [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d3c8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d3c8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d3c8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3c8-134">Request</span></span>
<span data-ttu-id="7d3c8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7d3c8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d3c8-136">Response</span></span>
<span data-ttu-id="7d3c8-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-137">Here is an example of the response.</span></span> <span data-ttu-id="7d3c8-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7d3c8-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7d3c8-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 477

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
    "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```



