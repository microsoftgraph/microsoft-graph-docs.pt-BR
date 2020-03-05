---
title: Obter unsupportedDeviceConfiguration
description: Leia as propriedades e as relações do objeto unsupportedDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7fd79204ac1cd087e65c97dbaa744ac8bc742a6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42482507"
---
# <a name="get-unsupporteddeviceconfiguration"></a><span data-ttu-id="58057-103">Obter unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="58057-103">Get unsupportedDeviceConfiguration</span></span>

<span data-ttu-id="58057-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="58057-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58057-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58057-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58057-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58057-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58057-107">Leia as propriedades e as relações do objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58057-107">Read properties and relationships of the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58057-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58057-108">Prerequisites</span></span>
<span data-ttu-id="58057-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58057-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58057-111">Permission type</span></span>|<span data-ttu-id="58057-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58057-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58057-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58057-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58057-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58057-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="58057-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58057-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58057-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58057-116">Not supported.</span></span>|
|<span data-ttu-id="58057-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58057-117">Application</span></span>|<span data-ttu-id="58057-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58057-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58057-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58057-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58057-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58057-120">Optional query parameters</span></span>
<span data-ttu-id="58057-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58057-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58057-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58057-122">Request headers</span></span>
|<span data-ttu-id="58057-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58057-123">Header</span></span>|<span data-ttu-id="58057-124">Valor</span><span class="sxs-lookup"><span data-stu-id="58057-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58057-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="58057-125">Authorization</span></span>|<span data-ttu-id="58057-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58057-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58057-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58057-127">Accept</span></span>|<span data-ttu-id="58057-128">application/json</span><span class="sxs-lookup"><span data-stu-id="58057-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58057-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58057-129">Request body</span></span>
<span data-ttu-id="58057-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58057-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58057-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="58057-131">Response</span></span>
<span data-ttu-id="58057-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58057-132">If successful, this method returns a `200 OK` response code and [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58057-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58057-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="58057-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58057-134">Request</span></span>
<span data-ttu-id="58057-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58057-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="58057-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="58057-136">Response</span></span>
<span data-ttu-id="58057-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58057-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

{
  "value": {
    "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
    "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
    "originalEntityTypeName": "Original Entity Type Name value",
    "details": [
      {
        "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
        "message": "Message value",
        "propertyName": "Property Name value"
      }
    ]
  }
}
```





