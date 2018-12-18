---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 6589cb380f5ea639b27cb4d3e2258b0bc9f1516f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321935"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="fef49-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="fef49-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="fef49-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fef49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fef49-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fef49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fef49-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fef49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fef49-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fef49-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fef49-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fef49-108">Prerequisites</span></span>
<span data-ttu-id="fef49-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef49-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fef49-111">Permission type</span></span>|<span data-ttu-id="fef49-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fef49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef49-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fef49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fef49-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fef49-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fef49-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fef49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fef49-116">Not supported.</span></span>|
|<span data-ttu-id="fef49-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fef49-117">Application</span></span>|<span data-ttu-id="fef49-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fef49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fef49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="fef49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fef49-120">Request headers</span></span>
|<span data-ttu-id="fef49-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fef49-121">Header</span></span>|<span data-ttu-id="fef49-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fef49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef49-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fef49-123">Authorization</span></span>|<span data-ttu-id="fef49-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fef49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fef49-125">Accept</span></span>|<span data-ttu-id="fef49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fef49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef49-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fef49-127">Request body</span></span>
<span data-ttu-id="fef49-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="fef49-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fef49-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="fef49-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fef49-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fef49-130">Property</span></span>|<span data-ttu-id="fef49-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fef49-131">Type</span></span>|<span data-ttu-id="fef49-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fef49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef49-133">platform</span><span class="sxs-lookup"><span data-stu-id="fef49-133">platform</span></span>|[<span data-ttu-id="fef49-134">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="fef49-134">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="fef49-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fef49-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fef49-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fef49-136">Response</span></span>
<span data-ttu-id="fef49-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fef49-137">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef49-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fef49-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fef49-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fef49-139">Request</span></span>
<span data-ttu-id="fef49-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fef49-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fef49-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fef49-141">Response</span></span>
<span data-ttu-id="fef49-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fef49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





