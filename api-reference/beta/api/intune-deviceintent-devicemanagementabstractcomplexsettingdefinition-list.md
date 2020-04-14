---
title: Listar deviceManagementAbstractComplexSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementAbstractComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8680c56b79102f30fdb36e3c0db01b04e17d6cc8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43331472"
---
# <a name="list-devicemanagementabstractcomplexsettingdefinitions"></a><span data-ttu-id="6c3bc-103">Listar deviceManagementAbstractComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="6c3bc-103">List deviceManagementAbstractComplexSettingDefinitions</span></span>

<span data-ttu-id="6c3bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c3bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c3bc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c3bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3bc-107">Listar Propriedades e relações dos objetos [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6c3bc-107">List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c3bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c3bc-108">Prerequisites</span></span>
<span data-ttu-id="6c3bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c3bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c3bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c3bc-111">Permission type</span></span>|<span data-ttu-id="6c3bc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c3bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c3bc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c3bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c3bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c3bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c3bc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c3bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c3bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-116">Not supported.</span></span>|
|<span data-ttu-id="6c3bc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c3bc-117">Application</span></span>|<span data-ttu-id="6c3bc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c3bc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c3bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c3bc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6c3bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3bc-120">Request headers</span></span>
|<span data-ttu-id="6c3bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c3bc-121">Header</span></span>|<span data-ttu-id="6c3bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c3bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c3bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c3bc-123">Authorization</span></span>|<span data-ttu-id="6c3bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c3bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c3bc-125">Accept</span></span>|<span data-ttu-id="6c3bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c3bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c3bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3bc-127">Request body</span></span>
<span data-ttu-id="6c3bc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c3bc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c3bc-129">Response</span></span>
<span data-ttu-id="6c3bc-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c3bc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c3bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c3bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3bc-132">Request</span></span>
<span data-ttu-id="6c3bc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="6c3bc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c3bc-134">Response</span></span>
<span data-ttu-id="6c3bc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c3bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



