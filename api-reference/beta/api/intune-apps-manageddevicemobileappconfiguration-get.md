---
title: Obter managedDeviceMobileAppConfiguration
description: Ler propriedades e relações do objeto managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0c00c44092659e11409f3943fbc5ab5a1190973
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250545"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="03510-103">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="03510-103">Get managedDeviceMobileAppConfiguration</span></span>

<span data-ttu-id="03510-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03510-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03510-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03510-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03510-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03510-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03510-107">Ler propriedades e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03510-107">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03510-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03510-108">Prerequisites</span></span>
<span data-ttu-id="03510-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03510-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03510-111">Permission type</span></span>|<span data-ttu-id="03510-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03510-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03510-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03510-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="03510-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03510-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03510-116">Not supported.</span></span>|
|<span data-ttu-id="03510-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03510-117">Application</span></span>|<span data-ttu-id="03510-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03510-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03510-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03510-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03510-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03510-120">Optional query parameters</span></span>
<span data-ttu-id="03510-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03510-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03510-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03510-122">Request headers</span></span>
|<span data-ttu-id="03510-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03510-123">Header</span></span>|<span data-ttu-id="03510-124">Valor</span><span class="sxs-lookup"><span data-stu-id="03510-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03510-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="03510-125">Authorization</span></span>|<span data-ttu-id="03510-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03510-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03510-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03510-127">Accept</span></span>|<span data-ttu-id="03510-128">application/json</span><span class="sxs-lookup"><span data-stu-id="03510-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03510-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03510-129">Request body</span></span>
<span data-ttu-id="03510-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03510-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03510-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="03510-131">Response</span></span>
<span data-ttu-id="03510-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03510-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03510-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03510-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="03510-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03510-134">Request</span></span>
<span data-ttu-id="03510-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03510-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="03510-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="03510-136">Response</span></span>
<span data-ttu-id="03510-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




