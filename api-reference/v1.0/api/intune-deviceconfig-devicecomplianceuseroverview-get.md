---
title: Acessar deviceComplianceUserOverview
description: Leia as propriedades e relações de objetos de deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d73dcdfe35b23f0cc04e2d03ac97124554a570f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255962"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="ed362-103">Acessar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ed362-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="ed362-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed362-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed362-105">Leia as propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-105">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed362-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed362-106">Prerequisites</span></span>
<span data-ttu-id="ed362-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed362-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed362-109">Permission type</span></span>|<span data-ttu-id="ed362-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed362-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed362-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed362-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed362-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed362-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ed362-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed362-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed362-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed362-114">Not supported.</span></span>|
|<span data-ttu-id="ed362-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed362-115">Application</span></span>|<span data-ttu-id="ed362-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed362-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed362-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed362-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed362-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed362-118">Optional query parameters</span></span>
<span data-ttu-id="ed362-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed362-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed362-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed362-120">Request headers</span></span>
|<span data-ttu-id="ed362-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed362-121">Header</span></span>|<span data-ttu-id="ed362-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed362-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed362-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed362-123">Authorization</span></span>|<span data-ttu-id="ed362-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed362-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed362-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed362-125">Accept</span></span>|<span data-ttu-id="ed362-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed362-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed362-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed362-127">Request body</span></span>
<span data-ttu-id="ed362-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed362-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed362-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed362-129">Response</span></span>
<span data-ttu-id="ed362-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed362-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed362-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed362-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed362-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed362-132">Request</span></span>
<span data-ttu-id="ed362-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed362-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="ed362-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed362-134">Response</span></span>
<span data-ttu-id="ed362-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed362-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



