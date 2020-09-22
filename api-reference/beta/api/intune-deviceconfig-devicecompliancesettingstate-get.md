---
title: Acessar deviceComplianceSettingState
description: Leia as propriedades e as relações do objeto deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00dcde4f66032564e3f762baa53f6bae04f33c99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011673"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="22060-103">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="22060-103">Get deviceComplianceSettingState</span></span>

<span data-ttu-id="22060-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="22060-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22060-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22060-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22060-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22060-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22060-107">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="22060-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22060-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22060-108">Prerequisites</span></span>
<span data-ttu-id="22060-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22060-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22060-111">Permission type</span></span>|<span data-ttu-id="22060-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22060-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22060-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22060-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22060-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22060-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22060-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22060-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22060-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22060-116">Not supported.</span></span>|
|<span data-ttu-id="22060-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22060-117">Application</span></span>|<span data-ttu-id="22060-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22060-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22060-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22060-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22060-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22060-120">Optional query parameters</span></span>
<span data-ttu-id="22060-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22060-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22060-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22060-122">Request headers</span></span>
|<span data-ttu-id="22060-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22060-123">Header</span></span>|<span data-ttu-id="22060-124">Valor</span><span class="sxs-lookup"><span data-stu-id="22060-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22060-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22060-125">Authorization</span></span>|<span data-ttu-id="22060-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22060-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22060-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22060-127">Accept</span></span>|<span data-ttu-id="22060-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22060-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22060-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22060-129">Request body</span></span>
<span data-ttu-id="22060-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22060-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22060-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22060-131">Response</span></span>
<span data-ttu-id="22060-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22060-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22060-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22060-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22060-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22060-134">Request</span></span>
<span data-ttu-id="22060-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22060-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="22060-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22060-136">Response</span></span>
<span data-ttu-id="22060-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22060-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






