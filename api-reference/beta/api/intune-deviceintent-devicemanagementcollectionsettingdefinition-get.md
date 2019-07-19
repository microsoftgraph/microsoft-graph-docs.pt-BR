---
title: Obter deviceManagementCollectionSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementCollectionSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f0fac6df34410f2df86f1e6622e2d89a1080d6d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960857"
---
# <a name="get-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="fedbf-103">Obter deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="fedbf-103">Get deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="fedbf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fedbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fedbf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fedbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fedbf-106">Leia as propriedades e as relações do objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="fedbf-106">Read properties and relationships of the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fedbf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fedbf-107">Prerequisites</span></span>
<span data-ttu-id="fedbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fedbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fedbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fedbf-110">Permission type</span></span>|<span data-ttu-id="fedbf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fedbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fedbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fedbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fedbf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fedbf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fedbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fedbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fedbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fedbf-115">Not supported.</span></span>|
|<span data-ttu-id="fedbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fedbf-116">Application</span></span>|<span data-ttu-id="fedbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fedbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fedbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fedbf-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="fedbf-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fedbf-119">Optional query parameters</span></span>
<span data-ttu-id="fedbf-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fedbf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fedbf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fedbf-121">Request headers</span></span>
|<span data-ttu-id="fedbf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fedbf-122">Header</span></span>|<span data-ttu-id="fedbf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fedbf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fedbf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fedbf-124">Authorization</span></span>|<span data-ttu-id="fedbf-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fedbf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fedbf-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fedbf-126">Accept</span></span>|<span data-ttu-id="fedbf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fedbf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fedbf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fedbf-128">Request body</span></span>
<span data-ttu-id="fedbf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fedbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fedbf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fedbf-130">Response</span></span>
<span data-ttu-id="fedbf-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fedbf-131">If successful, this method returns a `200 OK` response code and [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fedbf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fedbf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fedbf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fedbf-133">Request</span></span>
<span data-ttu-id="fedbf-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fedbf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="fedbf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fedbf-135">Response</span></span>
<span data-ttu-id="fedbf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fedbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "value": {
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
}
```





