---
title: Obter managedAppPolicyDeploymentSummary
description: Ler propriedades e relações do objeto managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1645ae6ee487a2e8507f73eebc95269781e6d039
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852231"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="5c186-103">Obter managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="5c186-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="5c186-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5c186-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c186-105">Ler propriedades e relações do objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5c186-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c186-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c186-106">Prerequisites</span></span>
<span data-ttu-id="5c186-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c186-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c186-109">Permission type</span></span>|<span data-ttu-id="5c186-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c186-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c186-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c186-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c186-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c186-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5c186-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c186-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c186-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c186-114">Not supported.</span></span>|
|<span data-ttu-id="5c186-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c186-115">Application</span></span>|<span data-ttu-id="5c186-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c186-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c186-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c186-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="5c186-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c186-118">Optional query parameters</span></span>
<span data-ttu-id="5c186-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c186-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c186-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c186-120">Request headers</span></span>
|<span data-ttu-id="5c186-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c186-121">Header</span></span>|<span data-ttu-id="5c186-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c186-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c186-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c186-123">Authorization</span></span>|<span data-ttu-id="5c186-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c186-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c186-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c186-125">Accept</span></span>|<span data-ttu-id="5c186-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c186-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c186-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c186-127">Request body</span></span>
<span data-ttu-id="5c186-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c186-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c186-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c186-129">Response</span></span>
<span data-ttu-id="5c186-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c186-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c186-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c186-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c186-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c186-132">Request</span></span>
<span data-ttu-id="5c186-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c186-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="5c186-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c186-134">Response</span></span>
<span data-ttu-id="5c186-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c186-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



