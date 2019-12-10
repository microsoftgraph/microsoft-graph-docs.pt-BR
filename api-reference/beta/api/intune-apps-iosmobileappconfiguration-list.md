---
title: Listar iosMobileAppConfigurations
description: Lista propriedades e relações dos objetos iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dab23ce2fa663f47befa30d60d92a337b20e94f7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921155"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="94dfe-103">Listar iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="94dfe-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="94dfe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94dfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94dfe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94dfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94dfe-106">Lista propriedades e relações dos objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94dfe-106">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94dfe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94dfe-107">Prerequisites</span></span>
<span data-ttu-id="94dfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94dfe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94dfe-110">Permission type</span></span>|<span data-ttu-id="94dfe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94dfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94dfe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94dfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94dfe-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94dfe-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94dfe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94dfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94dfe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94dfe-115">Not supported.</span></span>|
|<span data-ttu-id="94dfe-116">Application</span><span class="sxs-lookup"><span data-stu-id="94dfe-116">Application</span></span>|<span data-ttu-id="94dfe-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94dfe-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94dfe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94dfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="94dfe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94dfe-119">Request headers</span></span>
|<span data-ttu-id="94dfe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94dfe-120">Header</span></span>|<span data-ttu-id="94dfe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94dfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94dfe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94dfe-122">Authorization</span></span>|<span data-ttu-id="94dfe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94dfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94dfe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94dfe-124">Accept</span></span>|<span data-ttu-id="94dfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94dfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94dfe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94dfe-126">Request body</span></span>
<span data-ttu-id="94dfe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94dfe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94dfe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94dfe-128">Response</span></span>
<span data-ttu-id="94dfe-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94dfe-129">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94dfe-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94dfe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="94dfe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94dfe-131">Request</span></span>
<span data-ttu-id="94dfe-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94dfe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="94dfe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="94dfe-133">Response</span></span>
<span data-ttu-id="94dfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94dfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





