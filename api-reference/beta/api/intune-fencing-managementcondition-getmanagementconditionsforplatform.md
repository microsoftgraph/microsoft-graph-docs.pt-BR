---
title: função getManagementConditionsForPlatform
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d63e0c3f3775b2b9999d364fcc79dad6adedf98f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465825"
---
# <a name="getmanagementconditionsforplatform-function"></a><span data-ttu-id="4a557-103">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="4a557-103">getManagementConditionsForPlatform function</span></span>

<span data-ttu-id="4a557-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a557-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a557-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a557-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a557-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a557-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a557-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a557-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a557-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a557-108">Prerequisites</span></span>
<span data-ttu-id="4a557-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a557-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a557-111">Permission type</span></span>|<span data-ttu-id="4a557-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a557-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a557-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a557-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a557-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a557-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a557-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a557-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a557-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a557-116">Not supported.</span></span>|
|<span data-ttu-id="4a557-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a557-117">Application</span></span>|<span data-ttu-id="4a557-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a557-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a557-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a557-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/getManagementConditionsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/getManagementConditionsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="4a557-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a557-120">Request headers</span></span>
|<span data-ttu-id="4a557-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a557-121">Header</span></span>|<span data-ttu-id="4a557-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a557-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a557-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a557-123">Authorization</span></span>|<span data-ttu-id="4a557-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a557-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a557-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a557-125">Accept</span></span>|<span data-ttu-id="4a557-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a557-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a557-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a557-127">Request body</span></span>
<span data-ttu-id="4a557-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4a557-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4a557-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4a557-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4a557-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a557-130">Property</span></span>|<span data-ttu-id="4a557-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a557-131">Type</span></span>|<span data-ttu-id="4a557-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a557-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a557-133">platform</span><span class="sxs-lookup"><span data-stu-id="4a557-133">platform</span></span>|[<span data-ttu-id="4a557-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="4a557-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="4a557-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a557-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a557-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a557-136">Response</span></span>
<span data-ttu-id="4a557-137">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a557-137">If successful, this function returns a `200 OK` response code and a [managementCondition](../resources/intune-fencing-managementcondition.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a557-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a557-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a557-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a557-139">Request</span></span>
<span data-ttu-id="4a557-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a557-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/getManagementConditionsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4a557-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a557-141">Response</span></span>
<span data-ttu-id="4a557-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a557-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





