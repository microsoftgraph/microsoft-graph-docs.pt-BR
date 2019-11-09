---
title: Listar deviceConfigurations
description: Listar propriedades e relações dos objetos deviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3929fc02d08ff280503ad713d5276109afa62c5f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086127"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="372f2-103">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="372f2-103">List deviceConfigurations</span></span>

> <span data-ttu-id="372f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="372f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="372f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="372f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="372f2-106">Listar propriedades e relações dos objetos [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="372f2-106">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="372f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="372f2-107">Prerequisites</span></span>
<span data-ttu-id="372f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="372f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="372f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="372f2-110">Permission type</span></span>|<span data-ttu-id="372f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="372f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="372f2-112">Delegado (conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="372f2-112">Delegated (work or school account</span></span>||
| <span data-ttu-id="372f2-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="372f2-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="372f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="372f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="372f2-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="372f2-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="372f2-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="372f2-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="372f2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="372f2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="372f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="372f2-118">Not supported.</span></span>|
|<span data-ttu-id="372f2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="372f2-119">Application</span></span>||
| <span data-ttu-id="372f2-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="372f2-120">&nbsp; &nbsp; **Device configuration**</span></span> |<span data-ttu-id="372f2-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="372f2-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="372f2-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="372f2-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="372f2-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="372f2-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="372f2-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="372f2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="372f2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="372f2-125">Request headers</span></span>
|<span data-ttu-id="372f2-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="372f2-126">Header</span></span>|<span data-ttu-id="372f2-127">Valor</span><span class="sxs-lookup"><span data-stu-id="372f2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="372f2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="372f2-128">Authorization</span></span>|<span data-ttu-id="372f2-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="372f2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="372f2-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="372f2-130">Accept</span></span>|<span data-ttu-id="372f2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="372f2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="372f2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="372f2-132">Request body</span></span>
<span data-ttu-id="372f2-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="372f2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="372f2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="372f2-134">Response</span></span>
<span data-ttu-id="372f2-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="372f2-135">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="372f2-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="372f2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="372f2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="372f2-137">Request</span></span>
<span data-ttu-id="372f2-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="372f2-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="372f2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="372f2-139">Response</span></span>
<span data-ttu-id="372f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="372f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1355

{
  "value": [
    {
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
  ]
}
```









