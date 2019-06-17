---
title: Obter networkIPv6ConfigurationManagementCondition
description: Leia as propriedades e as relações do objeto networkIPv6ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6462bd66fda6de92a7f7a73f9d6407d39f948017
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984335"
---
# <a name="get-networkipv6configurationmanagementcondition"></a><span data-ttu-id="22ad8-103">Obter networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="22ad8-103">Get networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="22ad8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22ad8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ad8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22ad8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ad8-106">Leia as propriedades e as relações do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="22ad8-106">Read properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22ad8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22ad8-107">Prerequisites</span></span>
<span data-ttu-id="22ad8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ad8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22ad8-110">Permission type</span></span>|<span data-ttu-id="22ad8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22ad8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ad8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22ad8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22ad8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22ad8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22ad8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22ad8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ad8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ad8-115">Not supported.</span></span>|
|<span data-ttu-id="22ad8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22ad8-116">Application</span></span>|<span data-ttu-id="22ad8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ad8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22ad8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22ad8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22ad8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22ad8-119">Optional query parameters</span></span>
<span data-ttu-id="22ad8-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22ad8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22ad8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22ad8-121">Request headers</span></span>
|<span data-ttu-id="22ad8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22ad8-122">Header</span></span>|<span data-ttu-id="22ad8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="22ad8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22ad8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="22ad8-124">Authorization</span></span>|<span data-ttu-id="22ad8-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22ad8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22ad8-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22ad8-126">Accept</span></span>|<span data-ttu-id="22ad8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22ad8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ad8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22ad8-128">Request body</span></span>
<span data-ttu-id="22ad8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22ad8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22ad8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ad8-130">Response</span></span>
<span data-ttu-id="22ad8-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22ad8-131">If successful, this method returns a `200 OK` response code and [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ad8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22ad8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22ad8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22ad8-133">Request</span></span>
<span data-ttu-id="22ad8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22ad8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="22ad8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ad8-135">Response</span></span>
<span data-ttu-id="22ad8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22ad8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
    "id": "25811206-1206-2581-0612-812506128125",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV6Prefix": "Ip V6Prefix value",
    "ipV6Gateway": "Ip V6Gateway value",
    "ipV6DNSServerList": [
      "Ip V6DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





