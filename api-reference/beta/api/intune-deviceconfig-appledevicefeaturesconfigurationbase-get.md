---
title: Acessar appleDeviceFeaturesConfigurationBase
description: Leia as propriedades e as relações do objeto appleDeviceFeaturesConfigurationBase.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a40186a2572d410a5f218254657d794685f978de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155908"
---
# <a name="get-appledevicefeaturesconfigurationbase"></a><span data-ttu-id="194f3-103">Acessar appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="194f3-103">Get appleDeviceFeaturesConfigurationBase</span></span>

<span data-ttu-id="194f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="194f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="194f3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="194f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="194f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194f3-107">Leia as propriedades e as relações do objeto [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="194f3-107">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="194f3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="194f3-108">Prerequisites</span></span>
<span data-ttu-id="194f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="194f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="194f3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="194f3-111">Permission type</span></span>|<span data-ttu-id="194f3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="194f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="194f3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="194f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="194f3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194f3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="194f3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="194f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="194f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="194f3-116">Not supported.</span></span>|
|<span data-ttu-id="194f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="194f3-117">Application</span></span>|<span data-ttu-id="194f3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194f3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="194f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="194f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="194f3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="194f3-120">Optional query parameters</span></span>
<span data-ttu-id="194f3-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="194f3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="194f3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="194f3-122">Request headers</span></span>
|<span data-ttu-id="194f3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="194f3-123">Header</span></span>|<span data-ttu-id="194f3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="194f3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="194f3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="194f3-125">Authorization</span></span>|<span data-ttu-id="194f3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="194f3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="194f3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="194f3-127">Accept</span></span>|<span data-ttu-id="194f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="194f3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="194f3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="194f3-129">Request body</span></span>
<span data-ttu-id="194f3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="194f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="194f3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="194f3-131">Response</span></span>
<span data-ttu-id="194f3-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="194f3-132">If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="194f3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="194f3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="194f3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="194f3-134">Request</span></span>
<span data-ttu-id="194f3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="194f3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="194f3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="194f3-136">Response</span></span>
<span data-ttu-id="194f3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="194f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1550

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
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
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ]
  }
}
```




