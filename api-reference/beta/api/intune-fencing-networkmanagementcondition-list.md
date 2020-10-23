---
title: Listar networkManagementConditions
description: Listar Propriedades e relações dos objetos networkManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4730c34ba23becfc663686f4a62764c6cb922577
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728694"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="ebc7d-103">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="ebc7d-103">List networkManagementConditions</span></span>

<span data-ttu-id="ebc7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebc7d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebc7d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebc7d-107">Listar Propriedades e relações dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ebc7d-107">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebc7d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebc7d-108">Prerequisites</span></span>
<span data-ttu-id="ebc7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebc7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebc7d-111">Permission type</span></span>|<span data-ttu-id="ebc7d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebc7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebc7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebc7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebc7d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebc7d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ebc7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebc7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebc7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-116">Not supported.</span></span>|
|<span data-ttu-id="ebc7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc7d-117">Application</span></span>|<span data-ttu-id="ebc7d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebc7d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebc7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="ebc7d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc7d-120">Request headers</span></span>
|<span data-ttu-id="ebc7d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebc7d-121">Header</span></span>|<span data-ttu-id="ebc7d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebc7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebc7d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc7d-123">Authorization</span></span>|<span data-ttu-id="ebc7d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebc7d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebc7d-125">Accept</span></span>|<span data-ttu-id="ebc7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebc7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebc7d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc7d-127">Request body</span></span>
<span data-ttu-id="ebc7d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebc7d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc7d-129">Response</span></span>
<span data-ttu-id="ebc7d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-130">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebc7d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebc7d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebc7d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebc7d-132">Request</span></span>
<span data-ttu-id="ebc7d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="ebc7d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebc7d-134">Response</span></span>
<span data-ttu-id="ebc7d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebc7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





