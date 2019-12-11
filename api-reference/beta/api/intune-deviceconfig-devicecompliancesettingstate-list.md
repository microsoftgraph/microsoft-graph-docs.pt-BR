---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11b144741b01b1baac3a7749f2cfbcd601de9974
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949550"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="86989-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="86989-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="86989-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86989-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86989-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86989-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86989-106">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="86989-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86989-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86989-107">Prerequisites</span></span>
<span data-ttu-id="86989-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86989-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86989-110">Permission type</span></span>|<span data-ttu-id="86989-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86989-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86989-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86989-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86989-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86989-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="86989-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86989-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86989-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86989-115">Not supported.</span></span>|
|<span data-ttu-id="86989-116">Application</span><span class="sxs-lookup"><span data-stu-id="86989-116">Application</span></span>|<span data-ttu-id="86989-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86989-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86989-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86989-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="86989-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86989-119">Request headers</span></span>
|<span data-ttu-id="86989-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86989-120">Header</span></span>|<span data-ttu-id="86989-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86989-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86989-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86989-122">Authorization</span></span>|<span data-ttu-id="86989-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86989-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86989-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86989-124">Accept</span></span>|<span data-ttu-id="86989-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86989-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86989-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86989-126">Request body</span></span>
<span data-ttu-id="86989-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86989-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86989-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86989-128">Response</span></span>
<span data-ttu-id="86989-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86989-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86989-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86989-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86989-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86989-131">Request</span></span>
<span data-ttu-id="86989-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86989-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="86989-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="86989-133">Response</span></span>
<span data-ttu-id="86989-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86989-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





