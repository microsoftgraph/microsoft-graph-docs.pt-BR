---
title: Obter iosMobileAppConfiguration
description: Lê propriedades e relações do objeto iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07b51e1ec6cb51d0a577c0dec5643fdac99525fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843523"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="e7c05-103">Obter iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7c05-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="e7c05-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7c05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7c05-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7c05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c05-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e7c05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7c05-107">Lê propriedades e relações do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7c05-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7c05-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7c05-108">Prerequisites</span></span>
<span data-ttu-id="e7c05-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c05-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7c05-111">Permission type</span></span>|<span data-ttu-id="e7c05-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7c05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c05-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7c05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e7c05-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7c05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7c05-116">Not supported.</span></span>|
|<span data-ttu-id="e7c05-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7c05-117">Application</span></span>|<span data-ttu-id="e7c05-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7c05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7c05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7c05-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7c05-120">Optional query parameters</span></span>
<span data-ttu-id="e7c05-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7c05-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e7c05-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c05-122">Request headers</span></span>
|<span data-ttu-id="e7c05-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7c05-123">Header</span></span>|<span data-ttu-id="e7c05-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e7c05-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c05-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7c05-125">Authorization</span></span>|<span data-ttu-id="e7c05-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7c05-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c05-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7c05-127">Accept</span></span>|<span data-ttu-id="e7c05-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c05-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c05-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c05-129">Request body</span></span>
<span data-ttu-id="e7c05-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7c05-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7c05-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c05-131">Response</span></span>
<span data-ttu-id="e7c05-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7c05-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c05-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7c05-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7c05-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c05-134">Request</span></span>
<span data-ttu-id="e7c05-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7c05-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e7c05-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c05-136">Response</span></span>
<span data-ttu-id="e7c05-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7c05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





