---
title: função getManagementConditionStatementExpressionString
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: cde3e5b3c4867d2b3b0156fce550896b0748c8e1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354541"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="a9583-103">função getManagementConditionStatementExpressionString</span><span class="sxs-lookup"><span data-stu-id="a9583-103">getManagementConditionStatementExpressionString function</span></span>

> <span data-ttu-id="a9583-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9583-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9583-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9583-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9583-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a9583-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9583-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a9583-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9583-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9583-108">Prerequisites</span></span>
<span data-ttu-id="a9583-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9583-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9583-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9583-111">Permission type</span></span>|<span data-ttu-id="a9583-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9583-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9583-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9583-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9583-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9583-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a9583-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9583-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9583-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9583-116">Not supported.</span></span>|
|<span data-ttu-id="a9583-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9583-117">Application</span></span>|<span data-ttu-id="a9583-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9583-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9583-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9583-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="a9583-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9583-120">Request headers</span></span>
|<span data-ttu-id="a9583-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9583-121">Header</span></span>|<span data-ttu-id="a9583-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9583-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9583-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9583-123">Authorization</span></span>|<span data-ttu-id="a9583-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9583-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9583-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9583-125">Accept</span></span>|<span data-ttu-id="a9583-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9583-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9583-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9583-127">Request body</span></span>
<span data-ttu-id="a9583-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9583-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9583-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9583-129">Response</span></span>
<span data-ttu-id="a9583-130">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9583-130">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9583-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9583-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9583-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9583-132">Request</span></span>
<span data-ttu-id="a9583-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9583-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="a9583-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9583-134">Response</span></span>
<span data-ttu-id="a9583-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9583-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





