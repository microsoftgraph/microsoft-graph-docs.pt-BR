---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 928cadc0fe14c60799dd017120c20f5f6355b815
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354081"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="fa99e-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="fa99e-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="fa99e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa99e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa99e-105">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="fa99e-105">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa99e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa99e-106">Prerequisites</span></span>
<span data-ttu-id="fa99e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa99e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa99e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa99e-109">Permission type</span></span>|<span data-ttu-id="fa99e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa99e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa99e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa99e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa99e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa99e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa99e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa99e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa99e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa99e-114">Not supported.</span></span>|
|<span data-ttu-id="fa99e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa99e-115">Application</span></span>|<span data-ttu-id="fa99e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa99e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa99e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa99e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="fa99e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa99e-118">Request headers</span></span>
|<span data-ttu-id="fa99e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa99e-119">Header</span></span>|<span data-ttu-id="fa99e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fa99e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa99e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa99e-121">Authorization</span></span>|<span data-ttu-id="fa99e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa99e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa99e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa99e-123">Accept</span></span>|<span data-ttu-id="fa99e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa99e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa99e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa99e-125">Request body</span></span>
<span data-ttu-id="fa99e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa99e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa99e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa99e-127">Response</span></span>
<span data-ttu-id="fa99e-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa99e-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa99e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa99e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa99e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa99e-130">Request</span></span>
<span data-ttu-id="fa99e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa99e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="fa99e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa99e-132">Response</span></span>
<span data-ttu-id="fa99e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa99e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




