---
title: Listar iosMobileAppConfigurations
description: Lista propriedades e relações dos objetos iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f93dbcec40f7d4aee62750f4b0bc24ecf201df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949665"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="df0f3-103">Listar iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="df0f3-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="df0f3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df0f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df0f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df0f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df0f3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df0f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df0f3-107">Lista propriedades e relações dos objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df0f3-107">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df0f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df0f3-108">Prerequisites</span></span>
<span data-ttu-id="df0f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df0f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df0f3-111">Permission type</span></span>|<span data-ttu-id="df0f3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df0f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0f3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df0f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df0f3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="df0f3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="df0f3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df0f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df0f3-116">Not supported.</span></span>|
|<span data-ttu-id="df0f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df0f3-117">Application</span></span>|<span data-ttu-id="df0f3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df0f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df0f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df0f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df0f3-120">Request headers</span></span>
|<span data-ttu-id="df0f3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df0f3-121">Header</span></span>|<span data-ttu-id="df0f3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df0f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df0f3-123">Authorization</span></span>|<span data-ttu-id="df0f3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df0f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0f3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df0f3-125">Accept</span></span>|<span data-ttu-id="df0f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df0f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0f3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df0f3-127">Request body</span></span>
<span data-ttu-id="df0f3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df0f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df0f3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0f3-129">Response</span></span>
<span data-ttu-id="df0f3-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df0f3-130">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0f3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df0f3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="df0f3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df0f3-132">Request</span></span>
<span data-ttu-id="df0f3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df0f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="df0f3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0f3-134">Response</span></span>
<span data-ttu-id="df0f3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df0f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
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
  ]
}
```





