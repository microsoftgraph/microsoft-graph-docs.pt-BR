---
title: Get iosDeviceFeaturesConfiguration
description: Ler propriedades e relações do objeto iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ac30dc6205074f99aaf5c9269159178b0563910
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514554"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="8cd5e-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cd5e-103">Get iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="8cd5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cd5e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd5e-106">Ler propriedades e relações do objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cd5e-106">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cd5e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cd5e-107">Prerequisites</span></span>
<span data-ttu-id="8cd5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd5e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cd5e-110">Permission type</span></span>|<span data-ttu-id="8cd5e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cd5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cd5e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cd5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd5e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cd5e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8cd5e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cd5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cd5e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-115">Not supported.</span></span>|
|<span data-ttu-id="8cd5e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cd5e-116">Application</span></span>|<span data-ttu-id="8cd5e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cd5e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cd5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cd5e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8cd5e-119">Optional query parameters</span></span>
<span data-ttu-id="8cd5e-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cd5e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cd5e-121">Request headers</span></span>
|<span data-ttu-id="8cd5e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cd5e-122">Header</span></span>|<span data-ttu-id="8cd5e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8cd5e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cd5e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cd5e-124">Authorization</span></span>|<span data-ttu-id="8cd5e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cd5e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cd5e-126">Accept</span></span>|<span data-ttu-id="8cd5e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8cd5e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cd5e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cd5e-128">Request body</span></span>
<span data-ttu-id="8cd5e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd5e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cd5e-130">Response</span></span>
<span data-ttu-id="8cd5e-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-131">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cd5e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cd5e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cd5e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cd5e-133">Request</span></span>
<span data-ttu-id="8cd5e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8cd5e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cd5e-135">Response</span></span>
<span data-ttu-id="8cd5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cd5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "assetTagTemplate": "Asset Tag Template value",
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ]
  }
}
```




