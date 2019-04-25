---
title: função getManagementConditionsForPlatform
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22bd8bad354477df3528a82e811b38ad817e49d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532027"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="d63ba-103">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="d63ba-103">getManagementConditionsForPlatform function</span></span>

> <span data-ttu-id="d63ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d63ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d63ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d63ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d63ba-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d63ba-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d63ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d63ba-107">Prerequisites</span></span>
<span data-ttu-id="d63ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d63ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d63ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d63ba-110">Permission type</span></span>|<span data-ttu-id="d63ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d63ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d63ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d63ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d63ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d63ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d63ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d63ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d63ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d63ba-115">Not supported.</span></span>|
|<span data-ttu-id="d63ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d63ba-116">Application</span></span>|<span data-ttu-id="d63ba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d63ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d63ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d63ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="d63ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d63ba-119">Request headers</span></span>
|<span data-ttu-id="d63ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d63ba-120">Header</span></span>|<span data-ttu-id="d63ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d63ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d63ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d63ba-122">Authorization</span></span>|<span data-ttu-id="d63ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d63ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d63ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d63ba-124">Accept</span></span>|<span data-ttu-id="d63ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d63ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d63ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d63ba-126">Request body</span></span>
<span data-ttu-id="d63ba-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d63ba-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d63ba-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d63ba-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d63ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d63ba-129">Property</span></span>|<span data-ttu-id="d63ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d63ba-130">Type</span></span>|<span data-ttu-id="d63ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d63ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63ba-132">platform</span><span class="sxs-lookup"><span data-stu-id="d63ba-132">platform</span></span>|[<span data-ttu-id="d63ba-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d63ba-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d63ba-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d63ba-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d63ba-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63ba-135">Response</span></span>
<span data-ttu-id="d63ba-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d63ba-136">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d63ba-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d63ba-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d63ba-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d63ba-138">Request</span></span>
<span data-ttu-id="d63ba-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d63ba-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d63ba-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63ba-140">Response</span></span>
<span data-ttu-id="d63ba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d63ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





