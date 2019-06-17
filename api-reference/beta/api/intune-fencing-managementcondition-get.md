---
title: Obter managementCondition
description: Leia as propriedades e as relações do objeto managementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8313fadf643b20103c12f5d97e826ff998ec109b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984125"
---
# <a name="get-managementcondition"></a><span data-ttu-id="2020d-103">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="2020d-103">Get managementCondition</span></span>

> <span data-ttu-id="2020d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2020d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2020d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2020d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2020d-106">Leia as propriedades e as relações do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="2020d-106">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2020d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2020d-107">Prerequisites</span></span>
<span data-ttu-id="2020d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2020d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2020d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2020d-110">Permission type</span></span>|<span data-ttu-id="2020d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2020d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2020d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2020d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2020d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2020d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2020d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2020d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2020d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2020d-115">Not supported.</span></span>|
|<span data-ttu-id="2020d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2020d-116">Application</span></span>|<span data-ttu-id="2020d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2020d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2020d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2020d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2020d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2020d-119">Optional query parameters</span></span>
<span data-ttu-id="2020d-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2020d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2020d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-121">Request headers</span></span>
|<span data-ttu-id="2020d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2020d-122">Header</span></span>|<span data-ttu-id="2020d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2020d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2020d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2020d-124">Authorization</span></span>|<span data-ttu-id="2020d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2020d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2020d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2020d-126">Accept</span></span>|<span data-ttu-id="2020d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2020d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2020d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-128">Request body</span></span>
<span data-ttu-id="2020d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2020d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2020d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2020d-130">Response</span></span>
<span data-ttu-id="2020d-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2020d-131">If successful, this method returns a `200 OK` response code and [managementCondition](../resources/intune-fencing-managementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2020d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2020d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2020d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-133">Request</span></span>
<span data-ttu-id="2020d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2020d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="2020d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2020d-135">Response</span></span>
<span data-ttu-id="2020d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2020d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 468

{
  "value": {
    "@odata.type": "#microsoft.graph.managementCondition",
    "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
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





