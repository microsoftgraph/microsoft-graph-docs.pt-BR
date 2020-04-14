---
title: Listar circularGeofenceManagementConditions
description: Listar Propriedades e relações dos objetos circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14ab47410658484fda0898f74534ff0ae29fe009
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453966"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="4673b-103">Listar circularGeofenceManagementConditions</span><span class="sxs-lookup"><span data-stu-id="4673b-103">List circularGeofenceManagementConditions</span></span>

<span data-ttu-id="4673b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4673b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4673b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4673b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4673b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4673b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4673b-107">Listar Propriedades e relações dos objetos [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="4673b-107">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4673b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4673b-108">Prerequisites</span></span>
<span data-ttu-id="4673b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4673b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4673b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4673b-111">Permission type</span></span>|<span data-ttu-id="4673b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4673b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4673b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4673b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4673b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4673b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4673b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4673b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4673b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4673b-116">Not supported.</span></span>|
|<span data-ttu-id="4673b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4673b-117">Application</span></span>|<span data-ttu-id="4673b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4673b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4673b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4673b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4673b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4673b-120">Request headers</span></span>
|<span data-ttu-id="4673b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4673b-121">Header</span></span>|<span data-ttu-id="4673b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4673b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4673b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4673b-123">Authorization</span></span>|<span data-ttu-id="4673b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4673b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4673b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4673b-125">Accept</span></span>|<span data-ttu-id="4673b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4673b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4673b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4673b-127">Request body</span></span>
<span data-ttu-id="4673b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4673b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4673b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4673b-129">Response</span></span>
<span data-ttu-id="4673b-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4673b-130">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4673b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4673b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4673b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4673b-132">Request</span></span>
<span data-ttu-id="4673b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4673b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="4673b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4673b-134">Response</span></span>
<span data-ttu-id="4673b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4673b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



