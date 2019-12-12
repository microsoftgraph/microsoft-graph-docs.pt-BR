---
title: Listar androidForWorkWiFiConfigurations
description: Listar Propriedades e relações dos objetos androidForWorkWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 240405e49fb4c82890bc525c31b1b103148751f0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954507"
---
# <a name="list-androidforworkwificonfigurations"></a><span data-ttu-id="81fe3-103">Listar androidForWorkWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="81fe3-103">List androidForWorkWiFiConfigurations</span></span>

> <span data-ttu-id="81fe3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81fe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81fe3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81fe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81fe3-106">Listar Propriedades e relações dos objetos [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81fe3-106">List properties and relationships of the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81fe3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81fe3-107">Prerequisites</span></span>
<span data-ttu-id="81fe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81fe3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81fe3-110">Permission type</span></span>|<span data-ttu-id="81fe3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81fe3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81fe3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81fe3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81fe3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81fe3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81fe3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81fe3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81fe3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81fe3-115">Not supported.</span></span>|
|<span data-ttu-id="81fe3-116">Application</span><span class="sxs-lookup"><span data-stu-id="81fe3-116">Application</span></span>|<span data-ttu-id="81fe3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81fe3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81fe3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81fe3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="81fe3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81fe3-119">Request headers</span></span>
|<span data-ttu-id="81fe3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81fe3-120">Header</span></span>|<span data-ttu-id="81fe3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81fe3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81fe3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81fe3-122">Authorization</span></span>|<span data-ttu-id="81fe3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81fe3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81fe3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81fe3-124">Accept</span></span>|<span data-ttu-id="81fe3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81fe3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81fe3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81fe3-126">Request body</span></span>
<span data-ttu-id="81fe3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81fe3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81fe3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fe3-128">Response</span></span>
<span data-ttu-id="81fe3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81fe3-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81fe3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81fe3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="81fe3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81fe3-131">Request</span></span>
<span data-ttu-id="81fe3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81fe3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="81fe3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fe3-133">Response</span></span>
<span data-ttu-id="81fe3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81fe3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1568

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
      "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaEnterprise"
    }
  ]
}
```





