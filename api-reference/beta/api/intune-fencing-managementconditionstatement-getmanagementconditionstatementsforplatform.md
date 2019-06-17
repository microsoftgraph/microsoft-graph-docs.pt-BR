---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6562830cbbaa57f6009e1c864eb3f99a4044869a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984216"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="5f910-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="5f910-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="5f910-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f910-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f910-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f910-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f910-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f910-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f910-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f910-107">Prerequisites</span></span>
<span data-ttu-id="5f910-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f910-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f910-110">Permission type</span></span>|<span data-ttu-id="5f910-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f910-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f910-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f910-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f910-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f910-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f910-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f910-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f910-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f910-115">Not supported.</span></span>|
|<span data-ttu-id="5f910-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f910-116">Application</span></span>|<span data-ttu-id="5f910-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f910-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f910-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f910-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="5f910-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f910-119">Request headers</span></span>
|<span data-ttu-id="5f910-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f910-120">Header</span></span>|<span data-ttu-id="5f910-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f910-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f910-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f910-122">Authorization</span></span>|<span data-ttu-id="5f910-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f910-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f910-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f910-124">Accept</span></span>|<span data-ttu-id="5f910-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f910-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f910-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f910-126">Request body</span></span>
<span data-ttu-id="5f910-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="5f910-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5f910-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="5f910-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5f910-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f910-129">Property</span></span>|<span data-ttu-id="5f910-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f910-130">Type</span></span>|<span data-ttu-id="5f910-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f910-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f910-132">platform</span><span class="sxs-lookup"><span data-stu-id="5f910-132">platform</span></span>|[<span data-ttu-id="5f910-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="5f910-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="5f910-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f910-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5f910-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f910-135">Response</span></span>
<span data-ttu-id="5f910-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f910-136">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f910-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f910-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f910-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f910-138">Request</span></span>
<span data-ttu-id="5f910-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f910-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5f910-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f910-140">Response</span></span>
<span data-ttu-id="5f910-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f910-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





