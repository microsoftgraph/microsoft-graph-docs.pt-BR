---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adf74d54775811e80a3f203708130409d2f8e820
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309167"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="dabc4-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="dabc4-103">getManagementConditionStatementsForPlatform function</span></span>

<span data-ttu-id="dabc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dabc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dabc4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dabc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dabc4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dabc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dabc4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dabc4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dabc4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dabc4-108">Prerequisites</span></span>
<span data-ttu-id="dabc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dabc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dabc4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dabc4-111">Permission type</span></span>|<span data-ttu-id="dabc4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dabc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dabc4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dabc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dabc4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dabc4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dabc4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dabc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dabc4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dabc4-116">Not supported.</span></span>|
|<span data-ttu-id="dabc4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dabc4-117">Application</span></span>|<span data-ttu-id="dabc4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dabc4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dabc4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dabc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="dabc4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dabc4-120">Request headers</span></span>
|<span data-ttu-id="dabc4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dabc4-121">Header</span></span>|<span data-ttu-id="dabc4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dabc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dabc4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dabc4-123">Authorization</span></span>|<span data-ttu-id="dabc4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dabc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dabc4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dabc4-125">Accept</span></span>|<span data-ttu-id="dabc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dabc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dabc4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dabc4-127">Request body</span></span>
<span data-ttu-id="dabc4-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="dabc4-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="dabc4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="dabc4-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="dabc4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dabc4-130">Property</span></span>|<span data-ttu-id="dabc4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dabc4-131">Type</span></span>|<span data-ttu-id="dabc4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dabc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dabc4-133">plataforma</span><span class="sxs-lookup"><span data-stu-id="dabc4-133">platform</span></span>|[<span data-ttu-id="dabc4-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="dabc4-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="dabc4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dabc4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dabc4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dabc4-136">Response</span></span>
<span data-ttu-id="dabc4-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dabc4-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dabc4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dabc4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dabc4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dabc4-139">Request</span></span>
<span data-ttu-id="dabc4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dabc4-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="dabc4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dabc4-141">Response</span></span>
<span data-ttu-id="dabc4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dabc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




