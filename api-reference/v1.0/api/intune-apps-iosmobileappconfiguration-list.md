---
title: Listar iosMobileAppConfigurations
description: Lista propriedades e relações dos objetos iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4af324de29c6ecaceb6a2f13da86d8337a008cdd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822327"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="8cb19-103">Listar iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8cb19-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="8cb19-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8cb19-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cb19-105">Lista propriedades e relações dos objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cb19-105">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cb19-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cb19-106">Prerequisites</span></span>
<span data-ttu-id="8cb19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cb19-109">Permission type</span></span>|<span data-ttu-id="8cb19-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cb19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cb19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cb19-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cb19-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8cb19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cb19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cb19-114">Not supported.</span></span>|
|<span data-ttu-id="8cb19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cb19-115">Application</span></span>|<span data-ttu-id="8cb19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cb19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cb19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8cb19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb19-118">Request headers</span></span>
|<span data-ttu-id="8cb19-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cb19-119">Header</span></span>|<span data-ttu-id="8cb19-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8cb19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cb19-121">Authorization</span></span>|<span data-ttu-id="8cb19-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cb19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb19-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cb19-123">Accept</span></span>|<span data-ttu-id="8cb19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb19-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb19-125">Request body</span></span>
<span data-ttu-id="8cb19-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cb19-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cb19-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb19-127">Response</span></span>
<span data-ttu-id="8cb19-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cb19-128">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb19-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cb19-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cb19-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb19-130">Request</span></span>
<span data-ttu-id="8cb19-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cb19-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="8cb19-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb19-132">Response</span></span>
<span data-ttu-id="8cb19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cb19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



