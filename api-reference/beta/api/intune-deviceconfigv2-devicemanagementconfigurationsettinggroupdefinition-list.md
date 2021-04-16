---
title: Listar deviceManagementConfigurationSettingGroupDefinitions
description: Listar propriedades e relações dos objetos deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba7265e12a55a691b3f439113ba72e5ee6f17308
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864295"
---
# <a name="list-devicemanagementconfigurationsettinggroupdefinitions"></a><span data-ttu-id="27067-103">Listar deviceManagementConfigurationSettingGroupDefinitions</span><span class="sxs-lookup"><span data-stu-id="27067-103">List deviceManagementConfigurationSettingGroupDefinitions</span></span>

<span data-ttu-id="27067-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27067-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27067-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27067-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27067-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27067-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27067-107">Listar propriedades e relações dos [objetos deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="27067-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27067-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27067-108">Prerequisites</span></span>
<span data-ttu-id="27067-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27067-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27067-111">Permission type</span></span>|<span data-ttu-id="27067-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27067-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27067-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27067-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27067-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27067-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27067-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27067-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27067-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27067-116">Not supported.</span></span>|
|<span data-ttu-id="27067-117">Application</span><span class="sxs-lookup"><span data-stu-id="27067-117">Application</span></span>|<span data-ttu-id="27067-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27067-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27067-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27067-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="27067-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27067-120">Request headers</span></span>
|<span data-ttu-id="27067-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27067-121">Header</span></span>|<span data-ttu-id="27067-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27067-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27067-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27067-123">Authorization</span></span>|<span data-ttu-id="27067-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27067-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27067-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27067-125">Accept</span></span>|<span data-ttu-id="27067-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27067-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27067-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27067-127">Request body</span></span>
<span data-ttu-id="27067-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27067-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27067-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="27067-129">Response</span></span>
<span data-ttu-id="27067-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27067-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27067-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27067-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="27067-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27067-132">Request</span></span>
<span data-ttu-id="27067-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27067-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="27067-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27067-134">Response</span></span>
<span data-ttu-id="27067-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27067-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2035

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
      "id": "95dc9604-9604-95dc-0496-dc950496dc95",
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
      ]
    }
  ]
}
```




