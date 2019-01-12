---
title: Obter iosMobileAppConfiguration
description: Lê propriedades e relações do objeto iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa28947d3eb3eceb2726676a75351e08d58cd5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911774"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="767ae-103">Obter iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="767ae-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="767ae-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="767ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="767ae-105">Lê propriedades e relações do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="767ae-105">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="767ae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="767ae-106">Prerequisites</span></span>
<span data-ttu-id="767ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="767ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="767ae-109">Permission type</span></span>|<span data-ttu-id="767ae-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="767ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="767ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="767ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="767ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="767ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="767ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767ae-114">Not supported.</span></span>|
|<span data-ttu-id="767ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="767ae-115">Application</span></span>|<span data-ttu-id="767ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="767ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="767ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="767ae-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="767ae-118">Optional query parameters</span></span>
<span data-ttu-id="767ae-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="767ae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="767ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="767ae-120">Request headers</span></span>
|<span data-ttu-id="767ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="767ae-121">Header</span></span>|<span data-ttu-id="767ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="767ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="767ae-123">Authorization</span></span>|<span data-ttu-id="767ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="767ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="767ae-125">Accept</span></span>|<span data-ttu-id="767ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="767ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="767ae-127">Request body</span></span>
<span data-ttu-id="767ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="767ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="767ae-129">Response</span></span>
<span data-ttu-id="767ae-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="767ae-130">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767ae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="767ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="767ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="767ae-132">Request</span></span>
<span data-ttu-id="767ae-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="767ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="767ae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="767ae-134">Response</span></span>
<span data-ttu-id="767ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="767ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
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



