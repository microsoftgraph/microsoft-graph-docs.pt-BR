---
title: Listar deviceManagementConfigurationSettingGroupCollectionDefinitions
description: Listar propriedades e relações dos objetos deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3f54b474b8152449e8c1e3b7c06e5788d91c661
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665151"
---
# <a name="list-devicemanagementconfigurationsettinggroupcollectiondefinitions"></a><span data-ttu-id="b2852-103">Listar deviceManagementConfigurationSettingGroupCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="b2852-103">List deviceManagementConfigurationSettingGroupCollectionDefinitions</span></span>

<span data-ttu-id="b2852-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2852-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2852-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2852-107">Listar propriedades e relações [dos objetos deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2852-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2852-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2852-108">Prerequisites</span></span>
<span data-ttu-id="b2852-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2852-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2852-111">Permission type</span></span>|<span data-ttu-id="b2852-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2852-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2852-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2852-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2852-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2852-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2852-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2852-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2852-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2852-116">Not supported.</span></span>|
|<span data-ttu-id="b2852-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2852-117">Application</span></span>|<span data-ttu-id="b2852-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2852-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2852-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2852-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b2852-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2852-120">Request headers</span></span>
|<span data-ttu-id="b2852-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2852-121">Header</span></span>|<span data-ttu-id="b2852-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2852-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2852-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2852-123">Authorization</span></span>|<span data-ttu-id="b2852-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2852-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2852-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2852-125">Accept</span></span>|<span data-ttu-id="b2852-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2852-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2852-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2852-127">Request body</span></span>
<span data-ttu-id="b2852-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2852-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2852-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2852-129">Response</span></span>
<span data-ttu-id="b2852-130">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [de objetos deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2852-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2852-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2852-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2852-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2852-132">Request</span></span>
<span data-ttu-id="b2852-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2852-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="b2852-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2852-134">Response</span></span>
<span data-ttu-id="b2852-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2852-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2099

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
      "referredSettingInformationList": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
          "settingDefinitionId": "Setting Definition Id value"
        }
      ],
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




