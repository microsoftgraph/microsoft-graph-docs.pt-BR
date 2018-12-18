---
title: Obter networkIPv6ConfigurationManagementCondition
description: Leia as propriedades e os relacionamentos do objeto networkIPv6ConfigurationManagementCondition.
author: tfitzmac
ms.openlocfilehash: 4ca4417a66c869a65cc7ff3a6ed9700801452140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312779"
---
# <a name="get-networkipv6configurationmanagementcondition"></a><span data-ttu-id="34eaa-103">Obter networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="34eaa-103">Get networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="34eaa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34eaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34eaa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34eaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34eaa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="34eaa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34eaa-107">Leia as propriedades e os relacionamentos do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="34eaa-107">Read properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34eaa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34eaa-108">Prerequisites</span></span>
<span data-ttu-id="34eaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34eaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34eaa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34eaa-111">Permission type</span></span>|<span data-ttu-id="34eaa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34eaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34eaa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34eaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34eaa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34eaa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34eaa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34eaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34eaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34eaa-116">Not supported.</span></span>|
|<span data-ttu-id="34eaa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34eaa-117">Application</span></span>|<span data-ttu-id="34eaa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34eaa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34eaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34eaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34eaa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34eaa-120">Optional query parameters</span></span>
<span data-ttu-id="34eaa-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34eaa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34eaa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34eaa-122">Request headers</span></span>
|<span data-ttu-id="34eaa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34eaa-123">Header</span></span>|<span data-ttu-id="34eaa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="34eaa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34eaa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="34eaa-125">Authorization</span></span>|<span data-ttu-id="34eaa-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34eaa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34eaa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="34eaa-127">Accept</span></span>|<span data-ttu-id="34eaa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="34eaa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34eaa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34eaa-129">Request body</span></span>
<span data-ttu-id="34eaa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34eaa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34eaa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="34eaa-131">Response</span></span>
<span data-ttu-id="34eaa-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34eaa-132">If successful, this method returns a `200 OK` response code and [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34eaa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34eaa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="34eaa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34eaa-134">Request</span></span>
<span data-ttu-id="34eaa-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34eaa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="34eaa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="34eaa-136">Response</span></span>
<span data-ttu-id="34eaa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34eaa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





