---
title: função getManagementConditionsForPlatform
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4573b2aa54dd33dd1da8bcd8112b2d419843ca4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905417"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="d5008-103">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="d5008-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="d5008-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5008-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5008-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5008-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5008-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d5008-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5008-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5008-107">Prerequisites</span></span>
<span data-ttu-id="d5008-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5008-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5008-110">Permission type</span></span>|<span data-ttu-id="d5008-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5008-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5008-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5008-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5008-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5008-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5008-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5008-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5008-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5008-115">Not supported.</span></span>|
|<span data-ttu-id="d5008-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5008-116">Application</span></span>|<span data-ttu-id="d5008-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5008-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5008-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5008-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="d5008-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5008-119">Request headers</span></span>
|<span data-ttu-id="d5008-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5008-120">Header</span></span>|<span data-ttu-id="d5008-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d5008-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5008-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5008-122">Authorization</span></span>|<span data-ttu-id="d5008-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5008-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5008-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5008-124">Accept</span></span>|<span data-ttu-id="d5008-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5008-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5008-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5008-126">Request body</span></span>
<span data-ttu-id="d5008-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d5008-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d5008-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d5008-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5008-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5008-129">Property</span></span>|<span data-ttu-id="d5008-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5008-130">Type</span></span>|<span data-ttu-id="d5008-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5008-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5008-132">platform</span><span class="sxs-lookup"><span data-stu-id="d5008-132">platform</span></span>|[<span data-ttu-id="d5008-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d5008-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d5008-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d5008-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5008-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5008-135">Response</span></span>
<span data-ttu-id="d5008-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5008-136">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5008-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5008-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5008-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5008-138">Request</span></span>
<span data-ttu-id="d5008-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5008-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d5008-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5008-140">Response</span></span>
<span data-ttu-id="d5008-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5008-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
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
  ]
}
```




