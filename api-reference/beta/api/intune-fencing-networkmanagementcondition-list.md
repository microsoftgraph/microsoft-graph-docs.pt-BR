---
title: Listar networkManagementConditions
description: Listar Propriedades e relações dos objetos networkManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c93776671fc059dfeefdec1a9b6687edaa0eac6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905228"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="6bebd-103">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="6bebd-103">List networkManagementConditions</span></span>

> <span data-ttu-id="6bebd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bebd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bebd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bebd-106">Listar Propriedades e relações dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="6bebd-106">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bebd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bebd-107">Prerequisites</span></span>
<span data-ttu-id="6bebd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bebd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bebd-110">Permission type</span></span>|<span data-ttu-id="6bebd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bebd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bebd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bebd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6bebd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bebd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6bebd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bebd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bebd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bebd-115">Not supported.</span></span>|
|<span data-ttu-id="6bebd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bebd-116">Application</span></span>|<span data-ttu-id="6bebd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bebd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bebd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bebd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="6bebd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bebd-119">Request headers</span></span>
|<span data-ttu-id="6bebd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bebd-120">Header</span></span>|<span data-ttu-id="6bebd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6bebd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bebd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bebd-122">Authorization</span></span>|<span data-ttu-id="6bebd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bebd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bebd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bebd-124">Accept</span></span>|<span data-ttu-id="6bebd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6bebd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bebd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bebd-126">Request body</span></span>
<span data-ttu-id="6bebd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bebd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bebd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bebd-128">Response</span></span>
<span data-ttu-id="6bebd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bebd-129">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bebd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bebd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bebd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bebd-131">Request</span></span>
<span data-ttu-id="6bebd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bebd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="6bebd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bebd-133">Response</span></span>
<span data-ttu-id="6bebd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bebd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
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
  ]
}
```




