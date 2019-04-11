---
title: Obter circularGeofenceManagementCondition
description: Leia as propriedades e as relações do objeto circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 183a63ebb715938fcce63ab3bd8edadacf552a2d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772591"
---
# <a name="get-circulargeofencemanagementcondition"></a><span data-ttu-id="84ad6-103">Obter circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="84ad6-103">Get circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="84ad6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84ad6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ad6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84ad6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ad6-106">Leia as propriedades e as relações do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="84ad6-106">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ad6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84ad6-107">Prerequisites</span></span>
<span data-ttu-id="84ad6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84ad6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84ad6-110">Permission type</span></span>|<span data-ttu-id="84ad6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84ad6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ad6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84ad6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84ad6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ad6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84ad6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84ad6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ad6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84ad6-115">Not supported.</span></span>|
|<span data-ttu-id="84ad6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84ad6-116">Application</span></span>|<span data-ttu-id="84ad6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84ad6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ad6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84ad6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84ad6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84ad6-119">Optional query parameters</span></span>
<span data-ttu-id="84ad6-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84ad6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84ad6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84ad6-121">Request headers</span></span>
|<span data-ttu-id="84ad6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84ad6-122">Header</span></span>|<span data-ttu-id="84ad6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="84ad6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ad6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="84ad6-124">Authorization</span></span>|<span data-ttu-id="84ad6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84ad6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ad6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84ad6-126">Accept</span></span>|<span data-ttu-id="84ad6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84ad6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ad6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84ad6-128">Request body</span></span>
<span data-ttu-id="84ad6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84ad6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84ad6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ad6-130">Response</span></span>
<span data-ttu-id="84ad6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84ad6-131">If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ad6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84ad6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="84ad6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84ad6-133">Request</span></span>
<span data-ttu-id="84ad6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84ad6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="84ad6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ad6-135">Response</span></span>
<span data-ttu-id="84ad6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84ad6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": {
    "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
    "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
  }
}
```





