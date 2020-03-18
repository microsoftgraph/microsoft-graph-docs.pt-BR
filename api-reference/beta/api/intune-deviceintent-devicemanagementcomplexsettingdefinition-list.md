---
title: Listar deviceManagementComplexSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementComplexSettingDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a250f58f71c19ceee26f036ea043e09d6afa8ef4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730176"
---
# <a name="list-devicemanagementcomplexsettingdefinitions"></a><span data-ttu-id="0aafb-103">Listar deviceManagementComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="0aafb-103">List deviceManagementComplexSettingDefinitions</span></span>

> <span data-ttu-id="0aafb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0aafb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aafb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0aafb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aafb-106">Listar Propriedades e relações dos objetos [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0aafb-106">List properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aafb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0aafb-107">Prerequisites</span></span>
<span data-ttu-id="0aafb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aafb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aafb-110">Permission type</span></span>|<span data-ttu-id="0aafb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0aafb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aafb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aafb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0aafb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aafb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0aafb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aafb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aafb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aafb-115">Not supported.</span></span>|
|<span data-ttu-id="0aafb-116">Application</span><span class="sxs-lookup"><span data-stu-id="0aafb-116">Application</span></span>|<span data-ttu-id="0aafb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aafb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aafb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aafb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0aafb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aafb-119">Request headers</span></span>
|<span data-ttu-id="0aafb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0aafb-120">Header</span></span>|<span data-ttu-id="0aafb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0aafb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aafb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aafb-122">Authorization</span></span>|<span data-ttu-id="0aafb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aafb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aafb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0aafb-124">Accept</span></span>|<span data-ttu-id="0aafb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0aafb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aafb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aafb-126">Request body</span></span>
<span data-ttu-id="0aafb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0aafb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aafb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aafb-128">Response</span></span>
<span data-ttu-id="0aafb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aafb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aafb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aafb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aafb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aafb-131">Request</span></span>
<span data-ttu-id="0aafb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aafb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="0aafb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aafb-133">Response</span></span>
<span data-ttu-id="0aafb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0aafb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1234

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




