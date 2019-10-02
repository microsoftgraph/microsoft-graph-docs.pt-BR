---
title: Acessar deviceComplianceSettingState
description: Leia as propriedades e as relações do objeto deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9e4a92166d1d2660042c002c58b93642622c12d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354095"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="6e6ba-103">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="6e6ba-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="6e6ba-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e6ba-105">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="6e6ba-105">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e6ba-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e6ba-106">Prerequisites</span></span>
<span data-ttu-id="6e6ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e6ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e6ba-109">Permission type</span></span>|<span data-ttu-id="6e6ba-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e6ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e6ba-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e6ba-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e6ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e6ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-114">Not supported.</span></span>|
|<span data-ttu-id="6e6ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e6ba-115">Application</span></span>|<span data-ttu-id="6e6ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e6ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e6ba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e6ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e6ba-118">Optional query parameters</span></span>
<span data-ttu-id="6e6ba-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e6ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6ba-120">Request headers</span></span>
|<span data-ttu-id="6e6ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e6ba-121">Header</span></span>|<span data-ttu-id="6e6ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e6ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e6ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e6ba-123">Authorization</span></span>|<span data-ttu-id="6e6ba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e6ba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e6ba-125">Accept</span></span>|<span data-ttu-id="6e6ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e6ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e6ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6ba-127">Request body</span></span>
<span data-ttu-id="6e6ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e6ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e6ba-129">Response</span></span>
<span data-ttu-id="6e6ba-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-130">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e6ba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e6ba-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e6ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6ba-132">Request</span></span>
<span data-ttu-id="6e6ba-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="6e6ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e6ba-134">Response</span></span>
<span data-ttu-id="6e6ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e6ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```




