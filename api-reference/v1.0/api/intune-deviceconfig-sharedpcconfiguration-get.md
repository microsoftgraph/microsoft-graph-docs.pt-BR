---
title: Acessar sharedPCConfiguration
description: Leia as propriedades e relações do objeto sharedPCConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed5091c48248af42782b50bb324f8e7d2ee46c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514239"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="b43ee-103">Acessar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="b43ee-103">Get sharedPCConfiguration</span></span>

<span data-ttu-id="b43ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b43ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b43ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b43ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b43ee-106">Leia as propriedades e relações do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b43ee-106">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b43ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b43ee-107">Prerequisites</span></span>
<span data-ttu-id="b43ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b43ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b43ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b43ee-110">Permission type</span></span>|<span data-ttu-id="b43ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b43ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b43ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b43ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b43ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b43ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b43ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b43ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b43ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b43ee-115">Not supported.</span></span>|
|<span data-ttu-id="b43ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b43ee-116">Application</span></span>|<span data-ttu-id="b43ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b43ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b43ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b43ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b43ee-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b43ee-119">Optional query parameters</span></span>
<span data-ttu-id="b43ee-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b43ee-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b43ee-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b43ee-121">Request headers</span></span>
|<span data-ttu-id="b43ee-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b43ee-122">Header</span></span>|<span data-ttu-id="b43ee-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b43ee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b43ee-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b43ee-124">Authorization</span></span>|<span data-ttu-id="b43ee-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b43ee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b43ee-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b43ee-126">Accept</span></span>|<span data-ttu-id="b43ee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b43ee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b43ee-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b43ee-128">Request body</span></span>
<span data-ttu-id="b43ee-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b43ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b43ee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b43ee-130">Response</span></span>
<span data-ttu-id="b43ee-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b43ee-131">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b43ee-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b43ee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b43ee-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b43ee-133">Request</span></span>
<span data-ttu-id="b43ee-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b43ee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b43ee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b43ee-135">Response</span></span>
<span data-ttu-id="b43ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b43ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




