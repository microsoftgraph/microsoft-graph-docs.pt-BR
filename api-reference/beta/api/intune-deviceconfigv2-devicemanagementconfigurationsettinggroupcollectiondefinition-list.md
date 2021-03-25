---
title: Listar deviceManagementConfigurationSettingGroupCollectionDefinitions
description: Listar propriedades e relações dos objetos deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35ef5ad9d1f8a24a3e709a36971a5b09f3d40b2c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150847"
---
# <a name="list-devicemanagementconfigurationsettinggroupcollectiondefinitions"></a><span data-ttu-id="cab7f-103">Listar deviceManagementConfigurationSettingGroupCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="cab7f-103">List deviceManagementConfigurationSettingGroupCollectionDefinitions</span></span>

<span data-ttu-id="cab7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cab7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cab7f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cab7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cab7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cab7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cab7f-107">Listar propriedades e relações [dos objetos deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cab7f-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cab7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cab7f-108">Prerequisites</span></span>
<span data-ttu-id="cab7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cab7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cab7f-111">Permission type</span></span>|<span data-ttu-id="cab7f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cab7f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cab7f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cab7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cab7f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab7f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cab7f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cab7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cab7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab7f-116">Not supported.</span></span>|
|<span data-ttu-id="cab7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cab7f-117">Application</span></span>|<span data-ttu-id="cab7f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab7f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cab7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cab7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cab7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cab7f-120">Request headers</span></span>
|<span data-ttu-id="cab7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cab7f-121">Header</span></span>|<span data-ttu-id="cab7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cab7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cab7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cab7f-123">Authorization</span></span>|<span data-ttu-id="cab7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cab7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cab7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cab7f-125">Accept</span></span>|<span data-ttu-id="cab7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cab7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cab7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cab7f-127">Request body</span></span>
<span data-ttu-id="cab7f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cab7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cab7f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab7f-129">Response</span></span>
<span data-ttu-id="cab7f-130">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [de objetos deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cab7f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cab7f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cab7f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cab7f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab7f-132">Request</span></span>
<span data-ttu-id="cab7f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab7f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="cab7f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab7f-134">Response</span></span>
<span data-ttu-id="cab7f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cab7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1859

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
      "uxBehavior": "dropdown",
      "visibility": "settingsCatalog",
      "id": "739da194-a194-739d-94a1-9d7394a19d73",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "childIds": [
        "Child Ids value"
      ],
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ],
      "maximumCount": 12,
      "minimumCount": 12
    }
  ]
}
```




