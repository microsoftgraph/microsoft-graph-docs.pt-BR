---
title: Acessar windowsPhone81CustomConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7a5112468dd9fe7afca6a49c8f4fadc8fb13a71
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178973"
---
# <a name="get-windowsphone81customconfiguration"></a><span data-ttu-id="96825-103">Acessar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="96825-103">Get windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="96825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96825-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96825-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96825-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96825-107">Leia as propriedades e as relações do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96825-107">Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96825-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96825-108">Prerequisites</span></span>
<span data-ttu-id="96825-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96825-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96825-111">Permission type</span></span>|<span data-ttu-id="96825-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96825-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96825-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96825-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96825-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96825-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96825-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96825-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96825-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96825-116">Not supported.</span></span>|
|<span data-ttu-id="96825-117">Application</span><span class="sxs-lookup"><span data-stu-id="96825-117">Application</span></span>|<span data-ttu-id="96825-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96825-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96825-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96825-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96825-120">Optional query parameters</span></span>
<span data-ttu-id="96825-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96825-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96825-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-122">Request headers</span></span>
|<span data-ttu-id="96825-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96825-123">Header</span></span>|<span data-ttu-id="96825-124">Valor</span><span class="sxs-lookup"><span data-stu-id="96825-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96825-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="96825-125">Authorization</span></span>|<span data-ttu-id="96825-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96825-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96825-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96825-127">Accept</span></span>|<span data-ttu-id="96825-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96825-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96825-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-129">Request body</span></span>
<span data-ttu-id="96825-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96825-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96825-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-131">Response</span></span>
<span data-ttu-id="96825-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96825-132">If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96825-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96825-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="96825-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-134">Request</span></span>
<span data-ttu-id="96825-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96825-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="96825-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-136">Response</span></span>
<span data-ttu-id="96825-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1519

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSetting",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value"
      }
    ]
  }
}
```



