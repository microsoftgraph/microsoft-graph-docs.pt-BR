---
title: Listar deviceManagementCollectionSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f719ced3546dd9c235f7a54959c503cdb1ccbc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054459"
---
# <a name="list-devicemanagementcollectionsettingdefinitions"></a><span data-ttu-id="3903b-103">Listar deviceManagementCollectionSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="3903b-103">List deviceManagementCollectionSettingDefinitions</span></span>

<span data-ttu-id="3903b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3903b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3903b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3903b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3903b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3903b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3903b-107">Listar Propriedades e relações dos objetos [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3903b-107">List properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3903b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3903b-108">Prerequisites</span></span>
<span data-ttu-id="3903b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3903b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3903b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3903b-111">Permission type</span></span>|<span data-ttu-id="3903b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3903b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3903b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3903b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3903b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3903b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3903b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3903b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3903b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3903b-116">Not supported.</span></span>|
|<span data-ttu-id="3903b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3903b-117">Application</span></span>|<span data-ttu-id="3903b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3903b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3903b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3903b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3903b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3903b-120">Request headers</span></span>
|<span data-ttu-id="3903b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3903b-121">Header</span></span>|<span data-ttu-id="3903b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3903b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3903b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3903b-123">Authorization</span></span>|<span data-ttu-id="3903b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3903b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3903b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3903b-125">Accept</span></span>|<span data-ttu-id="3903b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3903b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3903b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3903b-127">Request body</span></span>
<span data-ttu-id="3903b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3903b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3903b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3903b-129">Response</span></span>
<span data-ttu-id="3903b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3903b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3903b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3903b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3903b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3903b-132">Request</span></span>
<span data-ttu-id="3903b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3903b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="3903b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3903b-134">Response</span></span>
<span data-ttu-id="3903b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3903b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1213

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
      "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
      "elementDefinitionId": "Element Definition Id value"
    }
  ]
}
```






