---
title: Obter deviceManagementConfigurationSettingDefinition
description: Leia propriedades e relações do objeto deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93b1726861e6a77f64661d8ef8d252cd4c9bcf30
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862831"
---
# <a name="get-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="e78ae-103">Obter deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e78ae-103">Get deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="e78ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e78ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e78ae-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e78ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e78ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e78ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e78ae-107">Leia propriedades e relações do [objeto deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e78ae-107">Read properties and relationships of the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e78ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e78ae-108">Prerequisites</span></span>
<span data-ttu-id="e78ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e78ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e78ae-111">Permission type</span></span>|<span data-ttu-id="e78ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e78ae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e78ae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e78ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e78ae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78ae-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e78ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e78ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e78ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e78ae-116">Not supported.</span></span>|
|<span data-ttu-id="e78ae-117">Application</span><span class="sxs-lookup"><span data-stu-id="e78ae-117">Application</span></span>|<span data-ttu-id="e78ae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78ae-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e78ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e78ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e78ae-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e78ae-120">Optional query parameters</span></span>
<span data-ttu-id="e78ae-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e78ae-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e78ae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ae-122">Request headers</span></span>
|<span data-ttu-id="e78ae-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e78ae-123">Header</span></span>|<span data-ttu-id="e78ae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e78ae-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e78ae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e78ae-125">Authorization</span></span>|<span data-ttu-id="e78ae-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e78ae-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e78ae-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e78ae-127">Accept</span></span>|<span data-ttu-id="e78ae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e78ae-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78ae-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ae-129">Request body</span></span>
<span data-ttu-id="e78ae-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e78ae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e78ae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78ae-131">Response</span></span>
<span data-ttu-id="e78ae-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e78ae-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78ae-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e78ae-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e78ae-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ae-134">Request</span></span>
<span data-ttu-id="e78ae-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e78ae-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="e78ae-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78ae-136">Response</span></span>
<span data-ttu-id="e78ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e78ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1404

{
  "value": {
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
    "uxBehavior": "dropdown",
    "visibility": "settingsCatalog",
    "referredSettingInformationList": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
        "settingDefinitionId": "Setting Definition Id value"
      }
    ],
    "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
    "description": "Description value",
    "helpText": "Help Text value",
    "name": "Name value",
    "displayName": "Display Name value",
    "version": "Version value"
  }
}
```




