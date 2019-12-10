---
title: função getManagementConditionStatementsForPlatform
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2920ff9752dcf388b80e91486df3a3e7e17c83f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943414"
---
# <a name="getmanagementconditionstatementsforplatform-function"></a><span data-ttu-id="57609-103">função getManagementConditionStatementsForPlatform</span><span class="sxs-lookup"><span data-stu-id="57609-103">getManagementConditionStatementsForPlatform function</span></span>

> <span data-ttu-id="57609-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57609-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57609-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57609-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57609-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57609-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57609-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57609-107">Prerequisites</span></span>
<span data-ttu-id="57609-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57609-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57609-110">Permission type</span></span>|<span data-ttu-id="57609-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57609-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57609-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57609-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57609-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57609-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57609-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57609-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57609-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57609-115">Not supported.</span></span>|
|<span data-ttu-id="57609-116">Application</span><span class="sxs-lookup"><span data-stu-id="57609-116">Application</span></span>|<span data-ttu-id="57609-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57609-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57609-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57609-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/getManagementConditionStatementsForPlatform
```

## <a name="request-headers"></a><span data-ttu-id="57609-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57609-119">Request headers</span></span>
|<span data-ttu-id="57609-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57609-120">Header</span></span>|<span data-ttu-id="57609-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57609-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57609-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57609-122">Authorization</span></span>|<span data-ttu-id="57609-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57609-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57609-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57609-124">Accept</span></span>|<span data-ttu-id="57609-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57609-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57609-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57609-126">Request body</span></span>
<span data-ttu-id="57609-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="57609-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="57609-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="57609-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="57609-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57609-129">Property</span></span>|<span data-ttu-id="57609-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="57609-130">Type</span></span>|<span data-ttu-id="57609-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="57609-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57609-132">platform</span><span class="sxs-lookup"><span data-stu-id="57609-132">platform</span></span>|[<span data-ttu-id="57609-133">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="57609-133">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="57609-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57609-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="57609-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="57609-135">Response</span></span>
<span data-ttu-id="57609-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57609-136">If successful, this function returns a `200 OK` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57609-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57609-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="57609-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57609-138">Request</span></span>
<span data-ttu-id="57609-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57609-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/getManagementConditionStatementsForPlatform(platform='parameterValue')
```

### <a name="response"></a><span data-ttu-id="57609-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="57609-140">Response</span></span>
<span data-ttu-id="57609-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57609-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





