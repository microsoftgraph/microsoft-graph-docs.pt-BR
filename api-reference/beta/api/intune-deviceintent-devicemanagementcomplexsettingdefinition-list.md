---
title: Listar deviceManagementComplexSettingDefinitions
description: Listar propriedades e relações dos objetos deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8819bd0a8fd60af316c4cb1aff88d05d7b7f3f94
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128954"
---
# <a name="list-devicemanagementcomplexsettingdefinitions"></a><span data-ttu-id="9656f-103">Listar deviceManagementComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="9656f-103">List deviceManagementComplexSettingDefinitions</span></span>

<span data-ttu-id="9656f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9656f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9656f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9656f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9656f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9656f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9656f-107">Listar propriedades e relações dos [objetos deviceManagementComplexSettingDefinition.](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9656f-107">List properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9656f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9656f-108">Prerequisites</span></span>
<span data-ttu-id="9656f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9656f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9656f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9656f-111">Permission type</span></span>|<span data-ttu-id="9656f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9656f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9656f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9656f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9656f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9656f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9656f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9656f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9656f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9656f-116">Not supported.</span></span>|
|<span data-ttu-id="9656f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9656f-117">Application</span></span>|<span data-ttu-id="9656f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9656f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9656f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9656f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="9656f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9656f-120">Request headers</span></span>
|<span data-ttu-id="9656f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9656f-121">Header</span></span>|<span data-ttu-id="9656f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9656f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9656f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9656f-123">Authorization</span></span>|<span data-ttu-id="9656f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9656f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9656f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9656f-125">Accept</span></span>|<span data-ttu-id="9656f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9656f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9656f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9656f-127">Request body</span></span>
<span data-ttu-id="9656f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9656f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9656f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9656f-129">Response</span></span>
<span data-ttu-id="9656f-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9656f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9656f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9656f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9656f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9656f-132">Request</span></span>
<span data-ttu-id="9656f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9656f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="9656f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9656f-134">Response</span></span>
<span data-ttu-id="9656f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9656f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1328

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
      "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
      "valueType": "boolean",
      "displayName": "Display Name value",
      "isTopLevel": true,
      "description": "Description value",
      "placeholderText": "Placeholder Text value",
      "documentationUrl": "https://example.com/documentationUrl/",
      "headerTitle": "Header Title value",
      "headerSubtitle": "Header Subtitle value",
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
  ]
}
```




