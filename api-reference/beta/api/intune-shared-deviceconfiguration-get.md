---
title: Get deviceConfiguration
description: Ler propriedades e relações do objeto deviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 897a17c3ba095980f16da01ad7478c5834b051fa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536165"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="55425-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="55425-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="55425-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55425-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55425-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55425-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55425-106">Ler propriedades e relações do objeto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55425-106">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55425-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55425-107">Prerequisites</span></span>
<span data-ttu-id="55425-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55425-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55425-110">Permission type</span></span>|<span data-ttu-id="55425-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55425-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55425-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55425-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="55425-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="55425-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="55425-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55425-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="55425-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="55425-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="55425-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55425-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55425-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55425-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55425-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55425-118">Not supported.</span></span>|
|<span data-ttu-id="55425-119">Application</span><span class="sxs-lookup"><span data-stu-id="55425-119">Application</span></span>||
| <span data-ttu-id="55425-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="55425-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="55425-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55425-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="55425-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="55425-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="55425-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55425-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55425-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55425-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55425-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55425-125">Optional query parameters</span></span>
<span data-ttu-id="55425-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55425-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55425-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55425-127">Request headers</span></span>
|<span data-ttu-id="55425-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55425-128">Header</span></span>|<span data-ttu-id="55425-129">Valor</span><span class="sxs-lookup"><span data-stu-id="55425-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55425-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="55425-130">Authorization</span></span>|<span data-ttu-id="55425-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55425-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55425-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55425-132">Accept</span></span>|<span data-ttu-id="55425-133">application/json</span><span class="sxs-lookup"><span data-stu-id="55425-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55425-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55425-134">Request body</span></span>
<span data-ttu-id="55425-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55425-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55425-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55425-136">Response</span></span>
<span data-ttu-id="55425-137">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55425-137">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55425-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55425-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="55425-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55425-139">Request</span></span>
<span data-ttu-id="55425-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55425-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="55425-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55425-141">Response</span></span>
<span data-ttu-id="55425-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55425-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
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
    "version": 7
  }
}
```






