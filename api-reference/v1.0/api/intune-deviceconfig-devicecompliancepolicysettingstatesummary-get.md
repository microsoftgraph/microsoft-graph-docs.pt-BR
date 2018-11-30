---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações do objeto deviceCompliancePolicySettingStateSummary.
ms.openlocfilehash: f8a4e819cdbaf1986b2f99d48a6822f4da6bf10b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003404"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="4ad79-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4ad79-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="4ad79-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad79-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ad79-105">Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4ad79-105">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ad79-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ad79-106">Prerequisites</span></span>
<span data-ttu-id="4ad79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ad79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ad79-109">Permission type</span></span>|<span data-ttu-id="4ad79-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ad79-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ad79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ad79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ad79-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ad79-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ad79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ad79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ad79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ad79-114">Not supported.</span></span>|
|<span data-ttu-id="4ad79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ad79-115">Application</span></span>|<span data-ttu-id="4ad79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ad79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ad79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad79-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ad79-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ad79-118">Optional query parameters</span></span>
<span data-ttu-id="4ad79-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ad79-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ad79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad79-120">Request headers</span></span>
|<span data-ttu-id="4ad79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ad79-121">Header</span></span>|<span data-ttu-id="4ad79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ad79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ad79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ad79-123">Authorization</span></span>|<span data-ttu-id="4ad79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ad79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ad79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ad79-125">Accept</span></span>|<span data-ttu-id="4ad79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ad79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ad79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad79-127">Request body</span></span>
<span data-ttu-id="4ad79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ad79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ad79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ad79-129">Response</span></span>
<span data-ttu-id="4ad79-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ad79-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ad79-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ad79-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ad79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad79-132">Request</span></span>
<span data-ttu-id="4ad79-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ad79-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="4ad79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ad79-134">Response</span></span>
<span data-ttu-id="4ad79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ad79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



