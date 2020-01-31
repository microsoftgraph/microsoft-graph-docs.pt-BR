---
title: Listar deviceManagementAbstractComplexSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementAbstractComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac7278a02037a957f9801199dc9d76759c7593af
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636459"
---
# <a name="list-devicemanagementabstractcomplexsettingdefinitions"></a><span data-ttu-id="f8e60-103">Listar deviceManagementAbstractComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="f8e60-103">List deviceManagementAbstractComplexSettingDefinitions</span></span>

> <span data-ttu-id="f8e60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8e60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8e60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8e60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e60-106">Listar Propriedades e relações dos objetos [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f8e60-106">List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8e60-107">Prerequisites</span></span>
<span data-ttu-id="f8e60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8e60-110">Permission type</span></span>|<span data-ttu-id="f8e60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8e60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8e60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f8e60-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8e60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8e60-115">Not supported.</span></span>|
|<span data-ttu-id="f8e60-116">Application</span><span class="sxs-lookup"><span data-stu-id="f8e60-116">Application</span></span>|<span data-ttu-id="f8e60-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e60-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8e60-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f8e60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e60-119">Request headers</span></span>
|<span data-ttu-id="f8e60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8e60-120">Header</span></span>|<span data-ttu-id="f8e60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8e60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8e60-122">Authorization</span></span>|<span data-ttu-id="f8e60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8e60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8e60-124">Accept</span></span>|<span data-ttu-id="f8e60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e60-126">Request body</span></span>
<span data-ttu-id="f8e60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8e60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8e60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e60-128">Response</span></span>
<span data-ttu-id="f8e60-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8e60-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8e60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8e60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e60-131">Request</span></span>
<span data-ttu-id="f8e60-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8e60-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="f8e60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e60-133">Response</span></span>
<span data-ttu-id="f8e60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8e60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1228

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
      "id": "1b703309-3309-1b70-0933-701b0933701b",
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
      "implementations": [
        "Implementations value"
      ]
    }
  ]
}
```





