---
title: Listar macOSCustomConfigurations
description: Listar propriedades e relações dos objetos macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 241bd8a436c26822725a91491f64fd3b3fdab351
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948435"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="8c077-103">Listar macOSCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="8c077-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="8c077-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c077-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c077-106">Listar propriedades e relações dos objetos [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c077-106">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c077-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c077-107">Prerequisites</span></span>
<span data-ttu-id="8c077-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c077-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c077-110">Permission type</span></span>|<span data-ttu-id="8c077-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c077-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c077-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c077-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c077-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c077-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c077-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c077-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c077-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c077-115">Not supported.</span></span>|
|<span data-ttu-id="8c077-116">Application</span><span class="sxs-lookup"><span data-stu-id="8c077-116">Application</span></span>|<span data-ttu-id="8c077-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c077-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c077-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c077-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8c077-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c077-119">Request headers</span></span>
|<span data-ttu-id="8c077-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c077-120">Header</span></span>|<span data-ttu-id="8c077-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8c077-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c077-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c077-122">Authorization</span></span>|<span data-ttu-id="8c077-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c077-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c077-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c077-124">Accept</span></span>|<span data-ttu-id="8c077-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c077-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c077-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c077-126">Request body</span></span>
<span data-ttu-id="8c077-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c077-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c077-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c077-128">Response</span></span>
<span data-ttu-id="8c077-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c077-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c077-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c077-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c077-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c077-131">Request</span></span>
<span data-ttu-id="8c077-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c077-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8c077-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c077-133">Response</span></span>
<span data-ttu-id="8c077-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c077-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1491

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```





