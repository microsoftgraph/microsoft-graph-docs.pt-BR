---
title: Obter deviceManagementSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ad8396bf8822bf438a1bd9219c2f18f569f4ceb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343248"
---
# <a name="get-devicemanagementsettingdefinition"></a><span data-ttu-id="64b88-103">Obter deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="64b88-103">Get deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="64b88-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64b88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64b88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64b88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b88-106">Leia as propriedades e as relações do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="64b88-106">Read properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64b88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64b88-107">Prerequisites</span></span>
<span data-ttu-id="64b88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b88-110">Permission type</span></span>|<span data-ttu-id="64b88-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64b88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64b88-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64b88-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64b88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b88-115">Not supported.</span></span>|
|<span data-ttu-id="64b88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64b88-116">Application</span></span>|<span data-ttu-id="64b88-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64b88-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b88-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="64b88-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64b88-119">Optional query parameters</span></span>
<span data-ttu-id="64b88-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64b88-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64b88-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b88-121">Request headers</span></span>
|<span data-ttu-id="64b88-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64b88-122">Header</span></span>|<span data-ttu-id="64b88-123">Valor</span><span class="sxs-lookup"><span data-stu-id="64b88-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64b88-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b88-124">Authorization</span></span>|<span data-ttu-id="64b88-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b88-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64b88-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64b88-126">Accept</span></span>|<span data-ttu-id="64b88-127">application/json</span><span class="sxs-lookup"><span data-stu-id="64b88-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b88-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b88-128">Request body</span></span>
<span data-ttu-id="64b88-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64b88-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b88-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b88-130">Response</span></span>
<span data-ttu-id="64b88-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b88-131">If successful, this method returns a `200 OK` response code and [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b88-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64b88-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="64b88-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b88-133">Request</span></span>
<span data-ttu-id="64b88-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64b88-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="64b88-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b88-135">Response</span></span>
<span data-ttu-id="64b88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64b88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 848

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
    "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
    ]
  }
}
```






