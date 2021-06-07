---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações do objeto deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d0a16e26ea24560bb96f4987b2005f6c88d2080
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748394"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="2365b-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2365b-103">Get deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="2365b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2365b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2365b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2365b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2365b-106">Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2365b-106">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2365b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2365b-107">Prerequisites</span></span>
<span data-ttu-id="2365b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2365b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2365b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2365b-110">Permission type</span></span>|<span data-ttu-id="2365b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2365b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2365b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2365b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2365b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2365b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2365b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2365b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2365b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2365b-115">Not supported.</span></span>|
|<span data-ttu-id="2365b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2365b-116">Application</span></span>|<span data-ttu-id="2365b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2365b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2365b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2365b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2365b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2365b-119">Optional query parameters</span></span>
<span data-ttu-id="2365b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2365b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2365b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2365b-121">Request headers</span></span>
|<span data-ttu-id="2365b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2365b-122">Header</span></span>|<span data-ttu-id="2365b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2365b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2365b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2365b-124">Authorization</span></span>|<span data-ttu-id="2365b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2365b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2365b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2365b-126">Accept</span></span>|<span data-ttu-id="2365b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2365b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2365b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2365b-128">Request body</span></span>
<span data-ttu-id="2365b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2365b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2365b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2365b-130">Response</span></span>
<span data-ttu-id="2365b-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2365b-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2365b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2365b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2365b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2365b-133">Request</span></span>
<span data-ttu-id="2365b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2365b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="2365b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2365b-135">Response</span></span>
<span data-ttu-id="2365b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2365b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
    "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "platformType": "iOS",
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




