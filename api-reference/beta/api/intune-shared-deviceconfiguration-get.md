---
title: Get deviceConfiguration
description: Ler propriedades e relações do objeto deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38f28cf631dfd5b6ad9bb5ed382c94eb6d592409
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390632"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="50aee-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="50aee-103">Get deviceConfiguration</span></span>

<span data-ttu-id="50aee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50aee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50aee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50aee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50aee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50aee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50aee-107">Ler propriedades e relações do objeto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50aee-107">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50aee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50aee-108">Prerequisites</span></span>
<span data-ttu-id="50aee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50aee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50aee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50aee-111">Permission type</span></span>|<span data-ttu-id="50aee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50aee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50aee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50aee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="50aee-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50aee-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50aee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50aee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="50aee-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="50aee-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="50aee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50aee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50aee-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50aee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50aee-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50aee-119">Not supported.</span></span>|
|<span data-ttu-id="50aee-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50aee-120">Application</span></span>||
| <span data-ttu-id="50aee-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50aee-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50aee-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50aee-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="50aee-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="50aee-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="50aee-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50aee-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50aee-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50aee-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50aee-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50aee-126">Optional query parameters</span></span>
<span data-ttu-id="50aee-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50aee-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50aee-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50aee-128">Request headers</span></span>
|<span data-ttu-id="50aee-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50aee-129">Header</span></span>|<span data-ttu-id="50aee-130">Valor</span><span class="sxs-lookup"><span data-stu-id="50aee-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50aee-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="50aee-131">Authorization</span></span>|<span data-ttu-id="50aee-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50aee-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50aee-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50aee-133">Accept</span></span>|<span data-ttu-id="50aee-134">application/json</span><span class="sxs-lookup"><span data-stu-id="50aee-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50aee-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50aee-135">Request body</span></span>
<span data-ttu-id="50aee-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50aee-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50aee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50aee-137">Response</span></span>
<span data-ttu-id="50aee-138">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50aee-138">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50aee-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50aee-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="50aee-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50aee-140">Request</span></span>
<span data-ttu-id="50aee-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50aee-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50aee-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="50aee-142">Response</span></span>
<span data-ttu-id="50aee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50aee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






