---
title: Listar deviceManagementConfigurationSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c4991676759af002232d0dfcd51067cd247ffa5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241352"
---
# <a name="list-devicemanagementconfigurationsettingdefinitions"></a><span data-ttu-id="8ee3f-103">Listar deviceManagementConfigurationSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="8ee3f-103">List deviceManagementConfigurationSettingDefinitions</span></span>

<span data-ttu-id="8ee3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ee3f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ee3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee3f-107">Listar Propriedades e relações dos objetos [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8ee3f-107">List properties and relationships of the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ee3f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ee3f-108">Prerequisites</span></span>
<span data-ttu-id="8ee3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ee3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ee3f-111">Permission type</span></span>|<span data-ttu-id="8ee3f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ee3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee3f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ee3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee3f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ee3f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8ee3f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ee3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-116">Not supported.</span></span>|
|<span data-ttu-id="8ee3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ee3f-117">Application</span></span>|<span data-ttu-id="8ee3f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ee3f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ee3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8ee3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ee3f-120">Request headers</span></span>
|<span data-ttu-id="8ee3f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ee3f-121">Header</span></span>|<span data-ttu-id="8ee3f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ee3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ee3f-123">Authorization</span></span>|<span data-ttu-id="8ee3f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee3f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ee3f-125">Accept</span></span>|<span data-ttu-id="8ee3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ee3f-127">Request body</span></span>
<span data-ttu-id="8ee3f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ee3f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ee3f-129">Response</span></span>
<span data-ttu-id="8ee3f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee3f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ee3f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ee3f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ee3f-132">Request</span></span>
<span data-ttu-id="8ee3f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="8ee3f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ee3f-134">Response</span></span>
<span data-ttu-id="8ee3f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ee3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1183

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
      "applicability": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
        "description": "Description value",
        "platform": "macOS",
        "deviceMode": "kiosk",
        "technologies": "mdm"
      },
      "accessTypes": "add",
      "keywords": [
        "Keywords value"
      ],
      "infoUrls": [
        "Info Urls value"
      ],
      "occurrence": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
        "minDeviceOccurrence": 3,
        "maxDeviceOccurrence": 3
      },
      "baseUri": "Base Uri value",
      "offsetUri": "Offset Uri value",
      "rootDefinitionId": "Root Definition Id value",
      "categoryId": "Category Id value",
      "settingUsage": "configuration",
      "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value"
    }
  ]
}
```




