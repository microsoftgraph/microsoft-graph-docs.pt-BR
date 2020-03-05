---
title: função getManagementConditionStatementExpressionString
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9522b9c18b3bdea9690bfeb62fa6b60c511adab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465741"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="fdcdf-103">função getManagementConditionStatementExpressionString</span><span class="sxs-lookup"><span data-stu-id="fdcdf-103">getManagementConditionStatementExpressionString function</span></span>

<span data-ttu-id="fdcdf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fdcdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdcdf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdcdf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdcdf-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fdcdf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdcdf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdcdf-108">Prerequisites</span></span>
<span data-ttu-id="fdcdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdcdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdcdf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdcdf-111">Permission type</span></span>|<span data-ttu-id="fdcdf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdcdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdcdf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdcdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdcdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdcdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fdcdf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdcdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdcdf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-116">Not supported.</span></span>|
|<span data-ttu-id="fdcdf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdcdf-117">Application</span></span>|<span data-ttu-id="fdcdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdcdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdcdf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdcdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="fdcdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcdf-120">Request headers</span></span>
|<span data-ttu-id="fdcdf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdcdf-121">Header</span></span>|<span data-ttu-id="fdcdf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdcdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdcdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdcdf-123">Authorization</span></span>|<span data-ttu-id="fdcdf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdcdf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdcdf-125">Accept</span></span>|<span data-ttu-id="fdcdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdcdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdcdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcdf-127">Request body</span></span>
<span data-ttu-id="fdcdf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdcdf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdcdf-129">Response</span></span>
<span data-ttu-id="fdcdf-130">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-130">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdcdf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdcdf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdcdf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcdf-132">Request</span></span>
<span data-ttu-id="fdcdf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="fdcdf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdcdf-134">Response</span></span>
<span data-ttu-id="fdcdf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdcdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "value": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  }
}
```





