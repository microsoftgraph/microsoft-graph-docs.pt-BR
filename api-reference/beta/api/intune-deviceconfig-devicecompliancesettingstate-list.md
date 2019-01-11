---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dfddb77cf258074df20496d9def43f38a013a81
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873854"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="373fb-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="373fb-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="373fb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="373fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="373fb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="373fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="373fb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="373fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="373fb-107">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="373fb-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="373fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="373fb-108">Prerequisites</span></span>
<span data-ttu-id="373fb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="373fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="373fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="373fb-111">Permission type</span></span>|<span data-ttu-id="373fb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="373fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="373fb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="373fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="373fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="373fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="373fb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="373fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="373fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="373fb-116">Not supported.</span></span>|
|<span data-ttu-id="373fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="373fb-117">Application</span></span>|<span data-ttu-id="373fb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="373fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="373fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="373fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="373fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="373fb-120">Request headers</span></span>
|<span data-ttu-id="373fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="373fb-121">Header</span></span>|<span data-ttu-id="373fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="373fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="373fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="373fb-123">Authorization</span></span>|<span data-ttu-id="373fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="373fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="373fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="373fb-125">Accept</span></span>|<span data-ttu-id="373fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="373fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="373fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="373fb-127">Request body</span></span>
<span data-ttu-id="373fb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="373fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="373fb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="373fb-129">Response</span></span>
<span data-ttu-id="373fb-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="373fb-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="373fb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="373fb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="373fb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="373fb-132">Request</span></span>
<span data-ttu-id="373fb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="373fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="373fb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="373fb-134">Response</span></span>
<span data-ttu-id="373fb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="373fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
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
  ]
}
```





