---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd1b057616f106e169390e2aeb547480f7656a25
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696563"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="89979-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="89979-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="89979-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89979-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89979-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89979-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89979-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89979-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89979-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89979-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89979-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89979-108">Prerequisites</span></span>
<span data-ttu-id="89979-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89979-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89979-111">Permission type</span></span>|<span data-ttu-id="89979-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89979-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89979-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89979-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89979-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89979-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89979-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89979-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89979-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89979-116">Not supported.</span></span>|
|<span data-ttu-id="89979-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89979-117">Application</span></span>|<span data-ttu-id="89979-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89979-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89979-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89979-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="89979-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89979-120">Request headers</span></span>
|<span data-ttu-id="89979-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89979-121">Header</span></span>|<span data-ttu-id="89979-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89979-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89979-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89979-123">Authorization</span></span>|<span data-ttu-id="89979-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89979-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89979-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89979-125">Accept</span></span>|<span data-ttu-id="89979-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89979-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89979-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89979-127">Request body</span></span>
<span data-ttu-id="89979-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="89979-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="89979-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="89979-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="89979-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89979-130">Property</span></span>|<span data-ttu-id="89979-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89979-131">Type</span></span>|<span data-ttu-id="89979-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89979-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89979-133">plataforma</span><span class="sxs-lookup"><span data-stu-id="89979-133">platform</span></span>|[<span data-ttu-id="89979-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="89979-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="89979-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89979-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89979-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="89979-136">Response</span></span>
<span data-ttu-id="89979-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89979-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89979-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89979-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="89979-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89979-139">Request</span></span>
<span data-ttu-id="89979-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89979-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="89979-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="89979-141">Response</span></span>
<span data-ttu-id="89979-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89979-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

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
        "@odata.type": "microsoft.graph.managementConditionExpressionString",
        "value": "Value value"
      },
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





