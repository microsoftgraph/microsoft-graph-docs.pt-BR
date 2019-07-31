---
title: Acessar deviceComplianceSettingState
description: Leia as propriedades e as relações do objeto deviceComplianceSettingState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7eb88bbbe71f2c39fc5feea69b277aaf99ee1c4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949563"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="cf596-103">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="cf596-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="cf596-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf596-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf596-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf596-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf596-106">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="cf596-106">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf596-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf596-107">Prerequisites</span></span>
<span data-ttu-id="cf596-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf596-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf596-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf596-110">Permission type</span></span>|<span data-ttu-id="cf596-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf596-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf596-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf596-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf596-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf596-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf596-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf596-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf596-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf596-115">Not supported.</span></span>|
|<span data-ttu-id="cf596-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf596-116">Application</span></span>|<span data-ttu-id="cf596-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf596-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf596-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf596-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf596-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf596-119">Optional query parameters</span></span>
<span data-ttu-id="cf596-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf596-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf596-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf596-121">Request headers</span></span>
|<span data-ttu-id="cf596-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf596-122">Header</span></span>|<span data-ttu-id="cf596-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cf596-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf596-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf596-124">Authorization</span></span>|<span data-ttu-id="cf596-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf596-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf596-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf596-126">Accept</span></span>|<span data-ttu-id="cf596-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf596-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf596-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf596-128">Request body</span></span>
<span data-ttu-id="cf596-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf596-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf596-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf596-130">Response</span></span>
<span data-ttu-id="cf596-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf596-131">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf596-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf596-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf596-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf596-133">Request</span></span>
<span data-ttu-id="cf596-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf596-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="cf596-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf596-135">Response</span></span>
<span data-ttu-id="cf596-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf596-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "platformType": "windowsRT",
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





