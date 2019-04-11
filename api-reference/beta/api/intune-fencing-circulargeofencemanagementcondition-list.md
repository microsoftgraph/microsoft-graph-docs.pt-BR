---
title: Listar circularGeofenceManagementConditions
description: Listar Propriedades e relações dos objetos circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c3d0652a9bc4bad843313f21e837c1d5b2cdba4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805555"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="d38eb-103">Listar circularGeofenceManagementConditions</span><span class="sxs-lookup"><span data-stu-id="d38eb-103">List circularGeofenceManagementConditions</span></span>

> <span data-ttu-id="d38eb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d38eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d38eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d38eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d38eb-106">Listar Propriedades e relações dos objetos [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d38eb-106">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d38eb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d38eb-107">Prerequisites</span></span>
<span data-ttu-id="d38eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d38eb-110">Permission type</span></span>|<span data-ttu-id="d38eb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d38eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d38eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d38eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d38eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d38eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d38eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d38eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d38eb-115">Not supported.</span></span>|
|<span data-ttu-id="d38eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d38eb-116">Application</span></span>|<span data-ttu-id="d38eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d38eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d38eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d38eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="d38eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d38eb-119">Request headers</span></span>
|<span data-ttu-id="d38eb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d38eb-120">Header</span></span>|<span data-ttu-id="d38eb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d38eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d38eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d38eb-122">Authorization</span></span>|<span data-ttu-id="d38eb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d38eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d38eb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d38eb-124">Accept</span></span>|<span data-ttu-id="d38eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d38eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d38eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d38eb-126">Request body</span></span>
<span data-ttu-id="d38eb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d38eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d38eb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d38eb-128">Response</span></span>
<span data-ttu-id="d38eb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d38eb-129">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38eb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d38eb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d38eb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d38eb-131">Request</span></span>
<span data-ttu-id="d38eb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d38eb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="d38eb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d38eb-133">Response</span></span>
<span data-ttu-id="d38eb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d38eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
    {
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
  ]
}
```





