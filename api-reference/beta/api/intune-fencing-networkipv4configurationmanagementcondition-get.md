---
title: Obter networkIPv4ConfigurationManagementCondition
description: Leia as propriedades e as relações do objeto networkIPv4ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04287dbf3e7ea75c8fc9503ede895821eb906f5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355413"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="9b392-103">Obter networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9b392-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="9b392-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b392-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b392-106">Leia as propriedades e as relações do objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="9b392-106">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b392-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b392-107">Prerequisites</span></span>
<span data-ttu-id="9b392-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b392-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b392-110">Permission type</span></span>|<span data-ttu-id="9b392-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b392-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b392-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b392-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b392-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b392-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b392-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b392-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b392-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b392-115">Not supported.</span></span>|
|<span data-ttu-id="9b392-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b392-116">Application</span></span>|<span data-ttu-id="9b392-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b392-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b392-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b392-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b392-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b392-119">Optional query parameters</span></span>
<span data-ttu-id="9b392-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b392-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b392-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b392-121">Request headers</span></span>
|<span data-ttu-id="9b392-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b392-122">Header</span></span>|<span data-ttu-id="9b392-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9b392-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b392-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b392-124">Authorization</span></span>|<span data-ttu-id="9b392-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b392-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b392-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b392-126">Accept</span></span>|<span data-ttu-id="9b392-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9b392-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b392-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b392-128">Request body</span></span>
<span data-ttu-id="9b392-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b392-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b392-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b392-130">Response</span></span>
<span data-ttu-id="9b392-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b392-131">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b392-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b392-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b392-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b392-133">Request</span></span>
<span data-ttu-id="9b392-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b392-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="9b392-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b392-135">Response</span></span>
<span data-ttu-id="9b392-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b392-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV4Prefix": "Ip V4Prefix value",
    "ipV4Gateway": "Ip V4Gateway value",
    "ipV4DHCPServer": "Ip V4DHCPServer value",
    "ipV4DNSServerList": [
      "Ip V4DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```






