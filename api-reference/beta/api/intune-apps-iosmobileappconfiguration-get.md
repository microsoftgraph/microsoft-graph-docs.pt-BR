---
title: Obter iosMobileAppConfiguration
description: Lê propriedades e relações do objeto iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a6ce81342e0a70a700b6a9057b41ff161437636
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960696"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="3bbca-103">Obter iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bbca-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3bbca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bbca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bbca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bbca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bbca-106">Lê propriedades e relações do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bbca-106">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bbca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bbca-107">Prerequisites</span></span>
<span data-ttu-id="3bbca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bbca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bbca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bbca-110">Permission type</span></span>|<span data-ttu-id="3bbca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3bbca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bbca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bbca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3bbca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bbca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3bbca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bbca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bbca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bbca-115">Not supported.</span></span>|
|<span data-ttu-id="3bbca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bbca-116">Application</span></span>|<span data-ttu-id="3bbca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bbca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bbca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bbca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bbca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bbca-119">Optional query parameters</span></span>
<span data-ttu-id="3bbca-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bbca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bbca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbca-121">Request headers</span></span>
|<span data-ttu-id="3bbca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bbca-122">Header</span></span>|<span data-ttu-id="3bbca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3bbca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bbca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bbca-124">Authorization</span></span>|<span data-ttu-id="3bbca-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bbca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bbca-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bbca-126">Accept</span></span>|<span data-ttu-id="3bbca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3bbca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bbca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbca-128">Request body</span></span>
<span data-ttu-id="3bbca-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bbca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bbca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbca-130">Response</span></span>
<span data-ttu-id="3bbca-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bbca-131">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bbca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bbca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bbca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbca-133">Request</span></span>
<span data-ttu-id="3bbca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bbca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3bbca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbca-135">Response</span></span>
<span data-ttu-id="3bbca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bbca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
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
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```




