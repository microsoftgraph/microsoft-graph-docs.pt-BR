---
title: Listar sharedPCConfigurations
description: Listar propriedades e relações dos objetos sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 254b3a4a6a10afaa1cd528ba6527185e49b1d415
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914616"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="13a1c-103">Listar sharedPCConfigurations</span><span class="sxs-lookup"><span data-stu-id="13a1c-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="13a1c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13a1c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13a1c-105">Listar propriedades e relações dos objetos [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13a1c-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13a1c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13a1c-106">Prerequisites</span></span>
<span data-ttu-id="13a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13a1c-109">Permission type</span></span>|<span data-ttu-id="13a1c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13a1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13a1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13a1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13a1c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="13a1c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="13a1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13a1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a1c-114">Not supported.</span></span>|
|<span data-ttu-id="13a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13a1c-115">Application</span></span>|<span data-ttu-id="13a1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13a1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13a1c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13a1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1c-118">Request headers</span></span>
|<span data-ttu-id="13a1c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13a1c-119">Header</span></span>|<span data-ttu-id="13a1c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="13a1c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13a1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13a1c-121">Authorization</span></span>|<span data-ttu-id="13a1c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13a1c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13a1c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13a1c-123">Accept</span></span>|<span data-ttu-id="13a1c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13a1c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a1c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1c-125">Request body</span></span>
<span data-ttu-id="13a1c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13a1c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a1c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a1c-127">Response</span></span>
<span data-ttu-id="13a1c-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13a1c-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a1c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13a1c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="13a1c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1c-130">Request</span></span>
<span data-ttu-id="13a1c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13a1c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="13a1c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a1c-132">Response</span></span>
<span data-ttu-id="13a1c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13a1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1165

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedPCConfiguration",
      "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountManagerPolicy": {
        "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
        "accountDeletionPolicy": "diskSpaceThreshold",
        "cacheAccountsAboveDiskFreePercentage": 4,
        "inactiveThresholdDays": 5,
        "removeAccountsBelowDiskFreePercentage": 5
      },
      "allowedAccounts": "domain",
      "allowLocalStorage": true,
      "disableAccountManager": true,
      "disableEduPolicies": true,
      "disablePowerPolicies": true,
      "disableSignInOnResume": true,
      "enabled": true,
      "idleTimeBeforeSleepInSeconds": 12,
      "kioskAppDisplayName": "Kiosk App Display Name value",
      "kioskAppUserModelId": "Kiosk App User Model Id value",
      "maintenanceStartTime": "11:59:24.7240000"
    }
  ]
}
```



