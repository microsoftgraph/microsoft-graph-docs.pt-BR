---
title: Obter managedAppPolicyDeploymentSummary
description: Ler propriedades e relações do objeto managedAppPolicyDeploymentSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4452de0e4e68f74c515df0be0b6b4c85ed738cb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904360"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="81297-103">Obter managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="81297-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="81297-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81297-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81297-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81297-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81297-106">Ler propriedades e relações do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="81297-106">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81297-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81297-107">Prerequisites</span></span>
<span data-ttu-id="81297-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81297-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81297-110">Permission type</span></span>|<span data-ttu-id="81297-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81297-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81297-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81297-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81297-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81297-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81297-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81297-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81297-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81297-115">Not supported.</span></span>|
|<span data-ttu-id="81297-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81297-116">Application</span></span>|<span data-ttu-id="81297-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81297-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81297-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81297-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81297-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81297-119">Optional query parameters</span></span>
<span data-ttu-id="81297-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81297-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81297-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-121">Request headers</span></span>
|<span data-ttu-id="81297-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81297-122">Header</span></span>|<span data-ttu-id="81297-123">Valor</span><span class="sxs-lookup"><span data-stu-id="81297-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81297-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="81297-124">Authorization</span></span>|<span data-ttu-id="81297-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81297-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81297-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81297-126">Accept</span></span>|<span data-ttu-id="81297-127">application/json</span><span class="sxs-lookup"><span data-stu-id="81297-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81297-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-128">Request body</span></span>
<span data-ttu-id="81297-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81297-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81297-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="81297-130">Response</span></span>
<span data-ttu-id="81297-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81297-131">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81297-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81297-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="81297-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-133">Request</span></span>
<span data-ttu-id="81297-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81297-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="81297-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="81297-135">Response</span></span>
<span data-ttu-id="81297-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81297-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```




