---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações do objeto deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e3d6dad0eee4f01041c7ed731ed6d6fe61ce5c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292125"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="c16bf-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c16bf-103">Get deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="c16bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c16bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c16bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c16bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c16bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c16bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c16bf-107">Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c16bf-107">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c16bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c16bf-108">Prerequisites</span></span>
<span data-ttu-id="c16bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c16bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c16bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c16bf-111">Permission type</span></span>|<span data-ttu-id="c16bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c16bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c16bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c16bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c16bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c16bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c16bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c16bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c16bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c16bf-116">Not supported.</span></span>|
|<span data-ttu-id="c16bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c16bf-117">Application</span></span>|<span data-ttu-id="c16bf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c16bf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c16bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c16bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c16bf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c16bf-120">Optional query parameters</span></span>
<span data-ttu-id="c16bf-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c16bf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c16bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c16bf-122">Request headers</span></span>
|<span data-ttu-id="c16bf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c16bf-123">Header</span></span>|<span data-ttu-id="c16bf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c16bf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c16bf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c16bf-125">Authorization</span></span>|<span data-ttu-id="c16bf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c16bf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c16bf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c16bf-127">Accept</span></span>|<span data-ttu-id="c16bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c16bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c16bf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c16bf-129">Request body</span></span>
<span data-ttu-id="c16bf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c16bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c16bf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c16bf-131">Response</span></span>
<span data-ttu-id="c16bf-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c16bf-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c16bf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c16bf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c16bf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c16bf-134">Request</span></span>
<span data-ttu-id="c16bf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c16bf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="c16bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c16bf-136">Response</span></span>
<span data-ttu-id="c16bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c16bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
    "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "platformType": "androidForWork",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```




