---
title: Obter deviceManagementComplexSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4dc630c906f18624939a0f2ff1848c0fa3d5b514
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428231"
---
# <a name="get-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="7b1a4-103">Obter deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="7b1a4-103">Get deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="7b1a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b1a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b1a4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b1a4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b1a4-107">Leia as propriedades e as relações do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="7b1a4-107">Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b1a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b1a4-108">Prerequisites</span></span>
<span data-ttu-id="7b1a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b1a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b1a4-111">Permission type</span></span>|<span data-ttu-id="7b1a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b1a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b1a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b1a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b1a4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b1a4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b1a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b1a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b1a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-116">Not supported.</span></span>|
|<span data-ttu-id="7b1a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b1a4-117">Application</span></span>|<span data-ttu-id="7b1a4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b1a4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b1a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b1a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b1a4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b1a4-120">Optional query parameters</span></span>
<span data-ttu-id="7b1a4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b1a4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1a4-122">Request headers</span></span>
|<span data-ttu-id="7b1a4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b1a4-123">Header</span></span>|<span data-ttu-id="7b1a4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7b1a4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b1a4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b1a4-125">Authorization</span></span>|<span data-ttu-id="7b1a4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b1a4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b1a4-127">Accept</span></span>|<span data-ttu-id="7b1a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7b1a4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b1a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1a4-129">Request body</span></span>
<span data-ttu-id="7b1a4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b1a4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b1a4-131">Response</span></span>
<span data-ttu-id="7b1a4-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-132">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b1a4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b1a4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b1a4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b1a4-134">Request</span></span>
<span data-ttu-id="7b1a4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="7b1a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b1a4-136">Response</span></span>
<span data-ttu-id="7b1a4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1148

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
    "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
    "valueType": "boolean",
    "displayName": "Display Name value",
    "isTopLevel": true,
    "description": "Description value",
    "placeholderText": "Placeholder Text value",
    "documentationUrl": "https://example.com/documentationUrl/",
    "keywords": [
      "Keywords value"
    ],
    "constraints": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
        "supportedTypes": [
          "Supported Types value"
        ]
      }
    ],
    "dependencies": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
        "definitionId": "Definition Id value",
        "constraints": [
          {
            "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
            "supportedTypes": [
              "Supported Types value"
            ]
          }
        ]
      }
    ],
    "propertyDefinitionIds": [
      "Property Definition Ids value"
    ]
  }
}
```



