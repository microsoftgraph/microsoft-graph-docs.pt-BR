---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5e11c43d9e27d337c1810b93aae7b1eb577563b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399503"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="eacce-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="eacce-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="eacce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eacce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eacce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eacce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eacce-106">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="eacce-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eacce-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eacce-107">Prerequisites</span></span>
<span data-ttu-id="eacce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eacce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eacce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eacce-110">Permission type</span></span>|<span data-ttu-id="eacce-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eacce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eacce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eacce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eacce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eacce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eacce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eacce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eacce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eacce-115">Not supported.</span></span>|
|<span data-ttu-id="eacce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eacce-116">Application</span></span>|<span data-ttu-id="eacce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eacce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eacce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eacce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="eacce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eacce-119">Request headers</span></span>
|<span data-ttu-id="eacce-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eacce-120">Header</span></span>|<span data-ttu-id="eacce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eacce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eacce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eacce-122">Authorization</span></span>|<span data-ttu-id="eacce-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eacce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eacce-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eacce-124">Accept</span></span>|<span data-ttu-id="eacce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eacce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eacce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eacce-126">Request body</span></span>
<span data-ttu-id="eacce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eacce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eacce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eacce-128">Response</span></span>
<span data-ttu-id="eacce-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eacce-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eacce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eacce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eacce-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eacce-131">Request</span></span>
<span data-ttu-id="eacce-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eacce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="eacce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eacce-133">Response</span></span>
<span data-ttu-id="eacce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eacce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






