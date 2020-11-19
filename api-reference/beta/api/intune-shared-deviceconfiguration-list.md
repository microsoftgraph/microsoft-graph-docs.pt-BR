---
title: Listar deviceConfigurations
description: Listar propriedades e relações dos objetos deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af62e5d846eeff0d1aabe878b9dc6f82aa34c643
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295898"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="50982-103">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="50982-103">List deviceConfigurations</span></span>

<span data-ttu-id="50982-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50982-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50982-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50982-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50982-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50982-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50982-107">Listar propriedades e relações dos objetos [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50982-107">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50982-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50982-108">Prerequisites</span></span>
<span data-ttu-id="50982-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50982-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50982-111">Permission type</span></span>|<span data-ttu-id="50982-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50982-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50982-113">Delegado (conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="50982-113">Delegated (work or school account</span></span>||
| <span data-ttu-id="50982-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50982-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50982-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50982-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="50982-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="50982-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="50982-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50982-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50982-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50982-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50982-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50982-119">Not supported.</span></span>|
|<span data-ttu-id="50982-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50982-120">Application</span></span>||
| <span data-ttu-id="50982-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50982-121">&nbsp; &nbsp; **Device configuration**</span></span> |<span data-ttu-id="50982-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50982-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="50982-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="50982-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="50982-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50982-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50982-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50982-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50982-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50982-126">Request headers</span></span>
|<span data-ttu-id="50982-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50982-127">Header</span></span>|<span data-ttu-id="50982-128">Valor</span><span class="sxs-lookup"><span data-stu-id="50982-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50982-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="50982-129">Authorization</span></span>|<span data-ttu-id="50982-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50982-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50982-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50982-131">Accept</span></span>|<span data-ttu-id="50982-132">application/json</span><span class="sxs-lookup"><span data-stu-id="50982-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50982-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50982-133">Request body</span></span>
<span data-ttu-id="50982-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50982-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50982-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50982-135">Response</span></span>
<span data-ttu-id="50982-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50982-136">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50982-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50982-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="50982-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50982-138">Request</span></span>
<span data-ttu-id="50982-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50982-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="50982-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50982-140">Response</span></span>
<span data-ttu-id="50982-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50982-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







