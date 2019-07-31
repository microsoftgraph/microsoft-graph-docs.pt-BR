---
title: função getManagementConditionStatementExpressionString
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b6b8a6e5496e82479abdc1d55aa1a0e567ea546
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990299"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="5a42a-103">função getManagementConditionStatementExpressionString</span><span class="sxs-lookup"><span data-stu-id="5a42a-103">getManagementConditionStatementExpressionString function</span></span>

> <span data-ttu-id="5a42a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a42a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a42a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a42a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a42a-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5a42a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a42a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a42a-107">Prerequisites</span></span>
<span data-ttu-id="5a42a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a42a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a42a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a42a-110">Permission type</span></span>|<span data-ttu-id="5a42a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a42a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a42a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a42a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a42a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a42a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a42a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a42a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a42a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a42a-115">Not supported.</span></span>|
|<span data-ttu-id="5a42a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a42a-116">Application</span></span>|<span data-ttu-id="5a42a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a42a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a42a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a42a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="5a42a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a42a-119">Request headers</span></span>
|<span data-ttu-id="5a42a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a42a-120">Header</span></span>|<span data-ttu-id="5a42a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5a42a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a42a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a42a-122">Authorization</span></span>|<span data-ttu-id="5a42a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a42a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a42a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a42a-124">Accept</span></span>|<span data-ttu-id="5a42a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a42a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a42a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a42a-126">Request body</span></span>
<span data-ttu-id="5a42a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a42a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a42a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a42a-128">Response</span></span>
<span data-ttu-id="5a42a-129">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a42a-129">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a42a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a42a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a42a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a42a-131">Request</span></span>
<span data-ttu-id="5a42a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a42a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="5a42a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a42a-133">Response</span></span>
<span data-ttu-id="5a42a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a42a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





