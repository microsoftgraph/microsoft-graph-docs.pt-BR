---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a745012db7de61a781fa29daf7f11a3cb6fbcac3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455451"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="d5436-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="d5436-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="d5436-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5436-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5436-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5436-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5436-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5436-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5436-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d5436-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5436-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5436-108">Prerequisites</span></span>
<span data-ttu-id="d5436-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5436-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5436-111">Permission type</span></span>|<span data-ttu-id="d5436-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5436-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5436-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5436-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5436-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5436-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5436-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5436-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5436-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5436-116">Not supported.</span></span>|
|<span data-ttu-id="d5436-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5436-117">Application</span></span>|<span data-ttu-id="d5436-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5436-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5436-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5436-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="d5436-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5436-120">Request headers</span></span>
|<span data-ttu-id="d5436-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5436-121">Header</span></span>|<span data-ttu-id="d5436-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5436-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5436-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5436-123">Authorization</span></span>|<span data-ttu-id="d5436-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5436-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5436-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5436-125">Accept</span></span>|<span data-ttu-id="d5436-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5436-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5436-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5436-127">Request body</span></span>
<span data-ttu-id="d5436-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d5436-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d5436-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d5436-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5436-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5436-130">Property</span></span>|<span data-ttu-id="d5436-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5436-131">Type</span></span>|<span data-ttu-id="d5436-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5436-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5436-133">platform</span><span class="sxs-lookup"><span data-stu-id="d5436-133">platform</span></span>|[<span data-ttu-id="d5436-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d5436-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d5436-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d5436-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5436-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5436-136">Response</span></span>
<span data-ttu-id="d5436-137">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5436-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5436-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5436-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5436-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5436-139">Request</span></span>
<span data-ttu-id="d5436-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5436-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d5436-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5436-141">Response</span></span>
<span data-ttu-id="d5436-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5436-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementConditionStatement",
      "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "expression": {
        "@odata.type": "microsoft.graph.managementConditionExpression"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```



