---
title: Listar iosCustomConfigurations
description: Listar propriedades e relações dos objetos iosCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 857ea93aa27065c26479c43a2cf3d33a18c58346
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949114"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="cb74d-103">Listar iosCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="cb74d-103">List iosCustomConfigurations</span></span>

> <span data-ttu-id="cb74d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb74d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb74d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb74d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb74d-106">Listar propriedades e relações dos objetos [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb74d-106">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb74d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb74d-107">Prerequisites</span></span>
<span data-ttu-id="cb74d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb74d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb74d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb74d-110">Permission type</span></span>|<span data-ttu-id="cb74d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb74d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb74d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb74d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb74d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb74d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cb74d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb74d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb74d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb74d-115">Not supported.</span></span>|
|<span data-ttu-id="cb74d-116">Application</span><span class="sxs-lookup"><span data-stu-id="cb74d-116">Application</span></span>|<span data-ttu-id="cb74d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb74d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb74d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb74d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cb74d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb74d-119">Request headers</span></span>
|<span data-ttu-id="cb74d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb74d-120">Header</span></span>|<span data-ttu-id="cb74d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb74d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb74d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb74d-122">Authorization</span></span>|<span data-ttu-id="cb74d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb74d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb74d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb74d-124">Accept</span></span>|<span data-ttu-id="cb74d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb74d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb74d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb74d-126">Request body</span></span>
<span data-ttu-id="cb74d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb74d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb74d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb74d-128">Response</span></span>
<span data-ttu-id="cb74d-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb74d-129">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb74d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb74d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb74d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb74d-131">Request</span></span>
<span data-ttu-id="cb74d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb74d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="cb74d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb74d-133">Response</span></span>
<span data-ttu-id="cb74d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb74d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1489

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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





