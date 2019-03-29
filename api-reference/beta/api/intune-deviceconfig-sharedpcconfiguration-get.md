---
title: Acessar sharedPCConfiguration
description: Leia as propriedades e relações do objeto sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 585c2b74687104c331af1895bbda50a40e2c57f4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967304"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="3cc3d-103">Acessar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cc3d-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="3cc3d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cc3d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cc3d-106">Leia as propriedades e relações do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cc3d-106">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cc3d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3cc3d-107">Prerequisites</span></span>
<span data-ttu-id="3cc3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc3d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cc3d-110">Permission type</span></span>|<span data-ttu-id="3cc3d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3cc3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cc3d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cc3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cc3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cc3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3cc3d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cc3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cc3d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-115">Not supported.</span></span>|
|<span data-ttu-id="3cc3d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cc3d-116">Application</span></span>|<span data-ttu-id="3cc3d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cc3d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cc3d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3cc3d-119">Optional query parameters</span></span>
<span data-ttu-id="3cc3d-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cc3d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc3d-121">Request headers</span></span>
|<span data-ttu-id="3cc3d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cc3d-122">Header</span></span>|<span data-ttu-id="3cc3d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3cc3d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cc3d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cc3d-124">Authorization</span></span>|<span data-ttu-id="3cc3d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cc3d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3cc3d-126">Accept</span></span>|<span data-ttu-id="3cc3d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3cc3d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cc3d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc3d-128">Request body</span></span>
<span data-ttu-id="3cc3d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cc3d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc3d-130">Response</span></span>
<span data-ttu-id="3cc3d-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-131">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cc3d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cc3d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cc3d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cc3d-133">Request</span></span>
<span data-ttu-id="3cc3d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3cc3d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cc3d-135">Response</span></span>
<span data-ttu-id="3cc3d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cc3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedPCConfiguration",
    "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "allowedAccounts": "guest",
    "localStorage": "enabled",
    "allowLocalStorage": true,
    "setAccountManager": "enabled",
    "disableAccountManager": true,
    "setEduPolicies": "enabled",
    "disableEduPolicies": true,
    "setPowerPolicies": "enabled",
    "disablePowerPolicies": true,
    "signInOnResume": "enabled",
    "disableSignInOnResume": true,
    "enabled": true,
    "idleTimeBeforeSleepInSeconds": 12,
    "kioskAppDisplayName": "Kiosk App Display Name value",
    "kioskAppUserModelId": "Kiosk App User Model Id value",
    "maintenanceStartTime": "11:59:24.7240000",
    "fastFirstSignIn": "enabled"
  }
}
```




