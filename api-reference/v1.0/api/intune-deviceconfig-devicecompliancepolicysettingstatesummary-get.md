---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações do objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd0c93fba3af78e2b63e5b4d82cf6d719e03658a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263739"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d1c01-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="d1c01-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="d1c01-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1c01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c01-105">Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d1c01-105">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1c01-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1c01-106">Prerequisites</span></span>
<span data-ttu-id="d1c01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d1c01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d1c01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1c01-109">Permission type</span></span>|<span data-ttu-id="d1c01-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1c01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1c01-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1c01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c01-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1c01-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d1c01-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1c01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1c01-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1c01-114">Not supported.</span></span>|
|<span data-ttu-id="d1c01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1c01-115">Application</span></span>|<span data-ttu-id="d1c01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1c01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1c01-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1c01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1c01-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1c01-118">Optional query parameters</span></span>
<span data-ttu-id="d1c01-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c01-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1c01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c01-120">Request headers</span></span>
|<span data-ttu-id="d1c01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1c01-121">Header</span></span>|<span data-ttu-id="d1c01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1c01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1c01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1c01-123">Authorization</span></span>|<span data-ttu-id="d1c01-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1c01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1c01-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1c01-125">Accept</span></span>|<span data-ttu-id="d1c01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c01-127">Request body</span></span>
<span data-ttu-id="d1c01-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1c01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1c01-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c01-129">Response</span></span>
<span data-ttu-id="d1c01-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c01-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c01-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1c01-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c01-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c01-132">Request</span></span>
<span data-ttu-id="d1c01-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1c01-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="d1c01-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c01-134">Response</span></span>
<span data-ttu-id="d1c01-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1c01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



