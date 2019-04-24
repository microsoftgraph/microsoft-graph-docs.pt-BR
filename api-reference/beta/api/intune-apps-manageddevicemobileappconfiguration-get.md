---
title: Obter managedDeviceMobileAppConfiguration
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 943e4076e08f29c32d14feab6a5ed3bf07c55d73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32494977"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="da8ac-103">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="da8ac-103">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="da8ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da8ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da8ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da8ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da8ac-106">Ler propriedades e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da8ac-106">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da8ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da8ac-107">Prerequisites</span></span>
<span data-ttu-id="da8ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da8ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da8ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da8ac-110">Permission type</span></span>|<span data-ttu-id="da8ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da8ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da8ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da8ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da8ac-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da8ac-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da8ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da8ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da8ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da8ac-115">Not supported.</span></span>|
|<span data-ttu-id="da8ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da8ac-116">Application</span></span>|<span data-ttu-id="da8ac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da8ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da8ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da8ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da8ac-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da8ac-119">Optional query parameters</span></span>
<span data-ttu-id="da8ac-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da8ac-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da8ac-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da8ac-121">Request headers</span></span>
|<span data-ttu-id="da8ac-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da8ac-122">Header</span></span>|<span data-ttu-id="da8ac-123">Valor</span><span class="sxs-lookup"><span data-stu-id="da8ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da8ac-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="da8ac-124">Authorization</span></span>|<span data-ttu-id="da8ac-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da8ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da8ac-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da8ac-126">Accept</span></span>|<span data-ttu-id="da8ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="da8ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da8ac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da8ac-128">Request body</span></span>
<span data-ttu-id="da8ac-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da8ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da8ac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="da8ac-130">Response</span></span>
<span data-ttu-id="da8ac-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da8ac-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da8ac-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da8ac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="da8ac-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da8ac-133">Request</span></span>
<span data-ttu-id="da8ac-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da8ac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="da8ac-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da8ac-135">Response</span></span>
<span data-ttu-id="da8ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da8ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





