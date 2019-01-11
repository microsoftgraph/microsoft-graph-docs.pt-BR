---
title: Acessar deviceComplianceUserOverview
description: Leia as propriedades e relações de objetos de deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f36401ba5e1a5928658da175d679a258230aa3df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814886"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="529be-103">Acessar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="529be-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="529be-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="529be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="529be-105">Leia as propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="529be-105">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="529be-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="529be-106">Prerequisites</span></span>
<span data-ttu-id="529be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="529be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="529be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="529be-109">Permission type</span></span>|<span data-ttu-id="529be-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="529be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="529be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="529be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="529be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="529be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="529be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="529be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="529be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="529be-114">Not supported.</span></span>|
|<span data-ttu-id="529be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="529be-115">Application</span></span>|<span data-ttu-id="529be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="529be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="529be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="529be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="529be-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="529be-118">Optional query parameters</span></span>
<span data-ttu-id="529be-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="529be-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="529be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="529be-120">Request headers</span></span>
|<span data-ttu-id="529be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="529be-121">Header</span></span>|<span data-ttu-id="529be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="529be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="529be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="529be-123">Authorization</span></span>|<span data-ttu-id="529be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="529be-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="529be-125">Accept</span></span>|<span data-ttu-id="529be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="529be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="529be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="529be-127">Request body</span></span>
<span data-ttu-id="529be-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="529be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="529be-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="529be-129">Response</span></span>
<span data-ttu-id="529be-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="529be-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="529be-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="529be-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="529be-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="529be-132">Request</span></span>
<span data-ttu-id="529be-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="529be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="529be-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="529be-134">Response</span></span>
<span data-ttu-id="529be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="529be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



