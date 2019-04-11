---
title: Listar deviceManagementCollectionSettingDefinitions
description: Listar Propriedades e relações dos objetos deviceManagementCollectionSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac00acf1aab35bb4fde0159f396788c5557af851
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777141"
---
# <a name="list-devicemanagementcollectionsettingdefinitions"></a><span data-ttu-id="5e5c2-103">Listar deviceManagementCollectionSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="5e5c2-103">List deviceManagementCollectionSettingDefinitions</span></span>

> <span data-ttu-id="5e5c2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e5c2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e5c2-106">Listar Propriedades e relações dos objetos [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="5e5c2-106">List properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e5c2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e5c2-107">Prerequisites</span></span>
<span data-ttu-id="5e5c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e5c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e5c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e5c2-110">Permission type</span></span>|<span data-ttu-id="5e5c2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e5c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e5c2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e5c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e5c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e5c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e5c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e5c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e5c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-115">Not supported.</span></span>|
|<span data-ttu-id="5e5c2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e5c2-116">Application</span></span>|<span data-ttu-id="5e5c2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e5c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e5c2-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5e5c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e5c2-119">Request headers</span></span>
|<span data-ttu-id="5e5c2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e5c2-120">Header</span></span>|<span data-ttu-id="5e5c2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5e5c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e5c2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e5c2-122">Authorization</span></span>|<span data-ttu-id="5e5c2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e5c2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e5c2-124">Accept</span></span>|<span data-ttu-id="5e5c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e5c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e5c2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e5c2-126">Request body</span></span>
<span data-ttu-id="5e5c2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e5c2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e5c2-128">Response</span></span>
<span data-ttu-id="5e5c2-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e5c2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e5c2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e5c2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e5c2-131">Request</span></span>
<span data-ttu-id="5e5c2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="5e5c2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e5c2-133">Response</span></span>
<span data-ttu-id="5e5c2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 985

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
      "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
      "valueType": "boolean",
      "displayName": "Display Name value",
      "isTopLevel": true,
      "description": "Description value",
      "documentationUrl": "https://example.com/documentationUrl/",
      "keywords": [
        "Keywords value"
      ],
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ],
      "dependencies": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
          "definitionId": "Definition Id value",
          "constraints": [
            {
              "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
            }
          ]
        }
      ],
      "elementDefinitionId": "Element Definition Id value"
    }
  ]
}
```





