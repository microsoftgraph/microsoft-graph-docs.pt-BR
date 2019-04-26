---
title: Acessar sharedPCConfiguration
description: Leia as propriedades e relações do objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d3e89306a715749dbcf08da6d118a0de7eabfd2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558353"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="7a488-103">Acessar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a488-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="7a488-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a488-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a488-105">Leia as propriedades e relações do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a488-105">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a488-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a488-106">Prerequisites</span></span>
<span data-ttu-id="7a488-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a488-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a488-109">Permission type</span></span>|<span data-ttu-id="7a488-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a488-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a488-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a488-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a488-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a488-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a488-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a488-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a488-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a488-114">Not supported.</span></span>|
|<span data-ttu-id="7a488-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a488-115">Application</span></span>|<span data-ttu-id="7a488-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a488-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a488-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a488-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a488-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a488-118">Optional query parameters</span></span>
<span data-ttu-id="7a488-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a488-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a488-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a488-120">Request headers</span></span>
|<span data-ttu-id="7a488-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a488-121">Header</span></span>|<span data-ttu-id="7a488-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a488-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a488-123">Authorization</span></span>|<span data-ttu-id="7a488-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a488-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a488-125">Accept</span></span>|<span data-ttu-id="7a488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a488-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a488-127">Request body</span></span>
<span data-ttu-id="7a488-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a488-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a488-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a488-129">Response</span></span>
<span data-ttu-id="7a488-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a488-130">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a488-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a488-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a488-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a488-132">Request</span></span>
<span data-ttu-id="7a488-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a488-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7a488-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a488-134">Response</span></span>
<span data-ttu-id="7a488-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
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
}
```



