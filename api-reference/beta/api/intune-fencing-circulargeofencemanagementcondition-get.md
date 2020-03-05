---
title: Obter circularGeofenceManagementCondition
description: Leia as propriedades e as relações do objeto circularGeofenceManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20437615fccb34a82a232e82a6b90e1a1c2163cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465951"
---
# <a name="get-circulargeofencemanagementcondition"></a><span data-ttu-id="5d9ce-103">Obter circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="5d9ce-103">Get circularGeofenceManagementCondition</span></span>

<span data-ttu-id="5d9ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5d9ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d9ce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d9ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d9ce-107">Leia as propriedades e as relações do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5d9ce-107">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d9ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d9ce-108">Prerequisites</span></span>
<span data-ttu-id="5d9ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d9ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d9ce-111">Permission type</span></span>|<span data-ttu-id="5d9ce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d9ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d9ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d9ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d9ce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d9ce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5d9ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d9ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d9ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-116">Not supported.</span></span>|
|<span data-ttu-id="5d9ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d9ce-117">Application</span></span>|<span data-ttu-id="5d9ce-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d9ce-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d9ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d9ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d9ce-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d9ce-120">Optional query parameters</span></span>
<span data-ttu-id="5d9ce-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d9ce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d9ce-122">Request headers</span></span>
|<span data-ttu-id="5d9ce-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d9ce-123">Header</span></span>|<span data-ttu-id="5d9ce-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5d9ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d9ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d9ce-125">Authorization</span></span>|<span data-ttu-id="5d9ce-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d9ce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d9ce-127">Accept</span></span>|<span data-ttu-id="5d9ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5d9ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d9ce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d9ce-129">Request body</span></span>
<span data-ttu-id="5d9ce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d9ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d9ce-131">Response</span></span>
<span data-ttu-id="5d9ce-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-132">If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d9ce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d9ce-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d9ce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d9ce-134">Request</span></span>
<span data-ttu-id="5d9ce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="5d9ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d9ce-136">Response</span></span>
<span data-ttu-id="5d9ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d9ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





