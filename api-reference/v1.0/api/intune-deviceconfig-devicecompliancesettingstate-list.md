---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
ms.openlocfilehash: 4ad3cc5d8bbbd9d143208dba7812ee4170084e43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004885"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="89c1b-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="89c1b-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="89c1b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89c1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89c1b-105">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="89c1b-105">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89c1b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89c1b-106">Prerequisites</span></span>
<span data-ttu-id="89c1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89c1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89c1b-109">Permission type</span></span>|<span data-ttu-id="89c1b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89c1b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89c1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89c1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89c1b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89c1b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89c1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89c1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89c1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89c1b-114">Not supported.</span></span>|
|<span data-ttu-id="89c1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89c1b-115">Application</span></span>|<span data-ttu-id="89c1b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89c1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89c1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89c1b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="89c1b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89c1b-118">Request headers</span></span>
|<span data-ttu-id="89c1b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89c1b-119">Header</span></span>|<span data-ttu-id="89c1b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="89c1b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89c1b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="89c1b-121">Authorization</span></span>|<span data-ttu-id="89c1b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89c1b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89c1b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="89c1b-123">Accept</span></span>|<span data-ttu-id="89c1b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89c1b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89c1b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89c1b-125">Request body</span></span>
<span data-ttu-id="89c1b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89c1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89c1b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c1b-127">Response</span></span>
<span data-ttu-id="89c1b-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89c1b-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89c1b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89c1b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="89c1b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89c1b-130">Request</span></span>
<span data-ttu-id="89c1b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89c1b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="89c1b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c1b-132">Response</span></span>
<span data-ttu-id="89c1b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89c1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
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
  ]
}
```



