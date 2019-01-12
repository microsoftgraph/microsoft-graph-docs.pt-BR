---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações do objeto deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bbff377d832a569cbfa22feb3d28fdc0bf975857
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974207"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="eceb2-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="eceb2-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="eceb2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eceb2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eceb2-105">Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="eceb2-105">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eceb2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eceb2-106">Prerequisites</span></span>
<span data-ttu-id="eceb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eceb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eceb2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eceb2-109">Permission type</span></span>|<span data-ttu-id="eceb2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eceb2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eceb2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eceb2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eceb2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eceb2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eceb2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eceb2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eceb2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eceb2-114">Not supported.</span></span>|
|<span data-ttu-id="eceb2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eceb2-115">Application</span></span>|<span data-ttu-id="eceb2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eceb2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eceb2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eceb2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eceb2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eceb2-118">Optional query parameters</span></span>
<span data-ttu-id="eceb2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eceb2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eceb2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eceb2-120">Request headers</span></span>
|<span data-ttu-id="eceb2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eceb2-121">Header</span></span>|<span data-ttu-id="eceb2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eceb2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eceb2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eceb2-123">Authorization</span></span>|<span data-ttu-id="eceb2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eceb2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eceb2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eceb2-125">Accept</span></span>|<span data-ttu-id="eceb2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eceb2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eceb2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eceb2-127">Request body</span></span>
<span data-ttu-id="eceb2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eceb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eceb2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eceb2-129">Response</span></span>
<span data-ttu-id="eceb2-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eceb2-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eceb2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eceb2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="eceb2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eceb2-132">Request</span></span>
<span data-ttu-id="eceb2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eceb2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="eceb2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eceb2-134">Response</span></span>
<span data-ttu-id="eceb2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eceb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



