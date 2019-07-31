---
title: Obter networkManagementCondition
description: Leia as propriedades e as relações do objeto networkManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d0f995f34727bf2b8930bb2d87147950461b1b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990117"
---
# <a name="get-networkmanagementcondition"></a><span data-ttu-id="52e3f-103">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="52e3f-103">Get networkManagementCondition</span></span>

> <span data-ttu-id="52e3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52e3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52e3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52e3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e3f-106">Leia as propriedades e as relações do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="52e3f-106">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52e3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52e3f-107">Prerequisites</span></span>
<span data-ttu-id="52e3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52e3f-110">Permission type</span></span>|<span data-ttu-id="52e3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52e3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52e3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52e3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52e3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52e3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52e3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e3f-115">Not supported.</span></span>|
|<span data-ttu-id="52e3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52e3f-116">Application</span></span>|<span data-ttu-id="52e3f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e3f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52e3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52e3f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52e3f-119">Optional query parameters</span></span>
<span data-ttu-id="52e3f-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52e3f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52e3f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52e3f-121">Request headers</span></span>
|<span data-ttu-id="52e3f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52e3f-122">Header</span></span>|<span data-ttu-id="52e3f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="52e3f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e3f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52e3f-124">Authorization</span></span>|<span data-ttu-id="52e3f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52e3f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e3f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52e3f-126">Accept</span></span>|<span data-ttu-id="52e3f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="52e3f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e3f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52e3f-128">Request body</span></span>
<span data-ttu-id="52e3f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52e3f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52e3f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e3f-130">Response</span></span>
<span data-ttu-id="52e3f-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52e3f-131">If successful, this method returns a `200 OK` response code and [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e3f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52e3f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="52e3f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52e3f-133">Request</span></span>
<span data-ttu-id="52e3f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52e3f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="52e3f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e3f-135">Response</span></span>
<span data-ttu-id="52e3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52e3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "value": {
    "@odata.type": "#microsoft.graph.networkManagementCondition",
    "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```





