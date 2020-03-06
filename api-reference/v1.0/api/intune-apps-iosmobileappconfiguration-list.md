---
title: Listar iosMobileAppConfigurations
description: Lista propriedades e relações dos objetos iosMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3945a1dffe57358df1dbab61dfd401a38e2dd4e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516564"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="afe54-103">Listar iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="afe54-103">List iosMobileAppConfigurations</span></span>

<span data-ttu-id="afe54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afe54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afe54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afe54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afe54-106">Lista propriedades e relações dos objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="afe54-106">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afe54-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afe54-107">Prerequisites</span></span>
<span data-ttu-id="afe54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afe54-110">Permission type</span></span>|<span data-ttu-id="afe54-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afe54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afe54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afe54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afe54-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="afe54-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="afe54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afe54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afe54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afe54-115">Not supported.</span></span>|
|<span data-ttu-id="afe54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afe54-116">Application</span></span>|<span data-ttu-id="afe54-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afe54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afe54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afe54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="afe54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afe54-119">Request headers</span></span>
|<span data-ttu-id="afe54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afe54-120">Header</span></span>|<span data-ttu-id="afe54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="afe54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afe54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="afe54-122">Authorization</span></span>|<span data-ttu-id="afe54-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afe54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afe54-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afe54-124">Accept</span></span>|<span data-ttu-id="afe54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afe54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afe54-126">Request body</span></span>
<span data-ttu-id="afe54-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afe54-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afe54-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="afe54-128">Response</span></span>
<span data-ttu-id="afe54-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afe54-129">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afe54-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afe54-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="afe54-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afe54-131">Request</span></span>
<span data-ttu-id="afe54-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afe54-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="afe54-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="afe54-133">Response</span></span>
<span data-ttu-id="afe54-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afe54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
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
  ]
}
```




