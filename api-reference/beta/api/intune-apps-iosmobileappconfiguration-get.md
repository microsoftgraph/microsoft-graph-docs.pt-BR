---
title: Obter iosMobileAppConfiguration
description: Lê propriedades e relações do objeto iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52ca4947c28a839b9c4a10acbf48ebac3ad09afe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700301"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="eb449-103">Obter iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb449-103">Get iosMobileAppConfiguration</span></span>

<span data-ttu-id="eb449-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb449-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb449-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb449-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb449-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb449-107">Lê propriedades e relações do objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb449-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb449-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb449-108">Prerequisites</span></span>
<span data-ttu-id="eb449-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb449-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb449-111">Permission type</span></span>|<span data-ttu-id="eb449-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb449-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb449-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb449-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb449-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb449-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb449-116">Not supported.</span></span>|
|<span data-ttu-id="eb449-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb449-117">Application</span></span>|<span data-ttu-id="eb449-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb449-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb449-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb449-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb449-120">Optional query parameters</span></span>
<span data-ttu-id="eb449-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb449-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb449-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb449-122">Request headers</span></span>
|<span data-ttu-id="eb449-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb449-123">Header</span></span>|<span data-ttu-id="eb449-124">Valor</span><span class="sxs-lookup"><span data-stu-id="eb449-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb449-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb449-125">Authorization</span></span>|<span data-ttu-id="eb449-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb449-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb449-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb449-127">Accept</span></span>|<span data-ttu-id="eb449-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eb449-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb449-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb449-129">Request body</span></span>
<span data-ttu-id="eb449-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb449-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb449-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb449-131">Response</span></span>
<span data-ttu-id="eb449-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e objeto [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb449-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb449-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb449-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb449-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb449-134">Request</span></span>
<span data-ttu-id="eb449-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb449-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="eb449-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb449-136">Response</span></span>
<span data-ttu-id="eb449-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb449-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





