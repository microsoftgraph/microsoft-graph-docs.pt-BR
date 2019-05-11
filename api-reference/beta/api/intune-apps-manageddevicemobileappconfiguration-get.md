---
title: Obter managedDeviceMobileAppConfiguration
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f644e378ef723bd80d3aa33c49b02fdc3474534b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935696"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="e9802-103">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9802-103">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="e9802-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9802-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9802-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9802-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9802-106">Ler propriedades e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9802-106">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9802-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9802-107">Prerequisites</span></span>
<span data-ttu-id="e9802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9802-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9802-110">Permission type</span></span>|<span data-ttu-id="e9802-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9802-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9802-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9802-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9802-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9802-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e9802-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9802-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9802-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9802-115">Not supported.</span></span>|
|<span data-ttu-id="e9802-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9802-116">Application</span></span>|<span data-ttu-id="e9802-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9802-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9802-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9802-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9802-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9802-119">Optional query parameters</span></span>
<span data-ttu-id="e9802-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9802-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9802-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9802-121">Request headers</span></span>
|<span data-ttu-id="e9802-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9802-122">Header</span></span>|<span data-ttu-id="e9802-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e9802-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9802-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9802-124">Authorization</span></span>|<span data-ttu-id="e9802-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9802-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9802-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9802-126">Accept</span></span>|<span data-ttu-id="e9802-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9802-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9802-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9802-128">Request body</span></span>
<span data-ttu-id="e9802-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9802-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9802-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9802-130">Response</span></span>
<span data-ttu-id="e9802-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9802-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9802-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9802-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9802-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9802-133">Request</span></span>
<span data-ttu-id="e9802-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9802-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9802-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9802-135">Response</span></span>
<span data-ttu-id="e9802-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9802-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




