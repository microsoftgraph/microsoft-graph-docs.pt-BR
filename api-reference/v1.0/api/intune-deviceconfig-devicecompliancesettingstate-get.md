---
title: Acessar deviceComplianceSettingState
description: Leia as propriedades e as relações do objeto deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c804f03218ad7a0cb5385bb4ca73dc12d83460f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980359"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="df544-103">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="df544-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="df544-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df544-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df544-105">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="df544-105">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df544-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df544-106">Prerequisites</span></span>
<span data-ttu-id="df544-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df544-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df544-109">Permission type</span></span>|<span data-ttu-id="df544-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df544-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df544-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df544-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df544-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df544-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df544-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df544-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df544-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df544-114">Not supported.</span></span>|
|<span data-ttu-id="df544-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df544-115">Application</span></span>|<span data-ttu-id="df544-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df544-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df544-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df544-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df544-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df544-118">Optional query parameters</span></span>
<span data-ttu-id="df544-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df544-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df544-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df544-120">Request headers</span></span>
|<span data-ttu-id="df544-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df544-121">Header</span></span>|<span data-ttu-id="df544-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df544-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df544-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df544-123">Authorization</span></span>|<span data-ttu-id="df544-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df544-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df544-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df544-125">Accept</span></span>|<span data-ttu-id="df544-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df544-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df544-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df544-127">Request body</span></span>
<span data-ttu-id="df544-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df544-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df544-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="df544-129">Response</span></span>
<span data-ttu-id="df544-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df544-130">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df544-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df544-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df544-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df544-132">Request</span></span>
<span data-ttu-id="df544-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df544-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="df544-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df544-134">Response</span></span>
<span data-ttu-id="df544-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df544-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



