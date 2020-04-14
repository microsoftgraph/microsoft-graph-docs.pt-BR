---
title: Listar deviceManagementSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04c2797f19b5a9c901c458b24029d43be9aa2684
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325593"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="167a7-103">Listar deviceManagementSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="167a7-103">List deviceManagementSettingDefinitions</span></span>

<span data-ttu-id="167a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="167a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="167a7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="167a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="167a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="167a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="167a7-107">Listar Propriedades e relações dos objetos [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="167a7-107">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="167a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="167a7-108">Prerequisites</span></span>
<span data-ttu-id="167a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="167a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="167a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="167a7-111">Permission type</span></span>|<span data-ttu-id="167a7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="167a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="167a7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="167a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="167a7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="167a7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="167a7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="167a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="167a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="167a7-116">Not supported.</span></span>|
|<span data-ttu-id="167a7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="167a7-117">Application</span></span>|<span data-ttu-id="167a7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="167a7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="167a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="167a7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="167a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="167a7-120">Request headers</span></span>
|<span data-ttu-id="167a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="167a7-121">Header</span></span>|<span data-ttu-id="167a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="167a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="167a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="167a7-123">Authorization</span></span>|<span data-ttu-id="167a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="167a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="167a7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="167a7-125">Accept</span></span>|<span data-ttu-id="167a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="167a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="167a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="167a7-127">Request body</span></span>
<span data-ttu-id="167a7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="167a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="167a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="167a7-129">Response</span></span>
<span data-ttu-id="167a7-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="167a7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="167a7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="167a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="167a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="167a7-132">Request</span></span>
<span data-ttu-id="167a7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="167a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="167a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="167a7-134">Response</span></span>
<span data-ttu-id="167a7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="167a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1142

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
      "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
      ]
    }
  ]
}
```



