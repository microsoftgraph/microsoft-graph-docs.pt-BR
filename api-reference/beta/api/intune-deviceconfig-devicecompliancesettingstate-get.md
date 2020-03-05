---
title: Acessar deviceComplianceSettingState
description: Leia as propriedades e as relações do objeto deviceComplianceSettingState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cece71873aec04c6765d8bc444406da495366b2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443143"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="c2746-103">Acessar deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="c2746-103">Get deviceComplianceSettingState</span></span>

<span data-ttu-id="c2746-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2746-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2746-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2746-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2746-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2746-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2746-107">Leia as propriedades e as relações do objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="c2746-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2746-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c2746-108">Prerequisites</span></span>
<span data-ttu-id="c2746-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2746-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2746-111">Permission type</span></span>|<span data-ttu-id="c2746-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c2746-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2746-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2746-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2746-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2746-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2746-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2746-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2746-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2746-116">Not supported.</span></span>|
|<span data-ttu-id="c2746-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2746-117">Application</span></span>|<span data-ttu-id="c2746-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2746-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2746-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2746-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2746-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2746-120">Optional query parameters</span></span>
<span data-ttu-id="c2746-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2746-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2746-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2746-122">Request headers</span></span>
|<span data-ttu-id="c2746-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2746-123">Header</span></span>|<span data-ttu-id="c2746-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c2746-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2746-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2746-125">Authorization</span></span>|<span data-ttu-id="c2746-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2746-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2746-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c2746-127">Accept</span></span>|<span data-ttu-id="c2746-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2746-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2746-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2746-129">Request body</span></span>
<span data-ttu-id="c2746-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2746-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2746-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2746-131">Response</span></span>
<span data-ttu-id="c2746-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2746-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2746-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2746-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2746-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2746-134">Request</span></span>
<span data-ttu-id="c2746-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2746-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="c2746-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2746-136">Response</span></span>
<span data-ttu-id="c2746-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2746-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





