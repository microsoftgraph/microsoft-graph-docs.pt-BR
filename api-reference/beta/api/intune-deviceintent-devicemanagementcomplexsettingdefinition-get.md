---
title: Obter deviceManagementComplexSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 643c86bb1e748a2f3e6bc7978196b5534241259d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960717"
---
# <a name="get-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="689cd-103">Obter deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="689cd-103">Get deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="689cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="689cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="689cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689cd-106">Leia as propriedades e as relações do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="689cd-106">Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="689cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="689cd-107">Prerequisites</span></span>
<span data-ttu-id="689cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="689cd-110">Permission type</span></span>|<span data-ttu-id="689cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="689cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="689cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="689cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="689cd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="689cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="689cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="689cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="689cd-115">Not supported.</span></span>|
|<span data-ttu-id="689cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="689cd-116">Application</span></span>|<span data-ttu-id="689cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="689cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="689cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="689cd-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="689cd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="689cd-119">Optional query parameters</span></span>
<span data-ttu-id="689cd-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="689cd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="689cd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="689cd-121">Request headers</span></span>
|<span data-ttu-id="689cd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="689cd-122">Header</span></span>|<span data-ttu-id="689cd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="689cd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="689cd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="689cd-124">Authorization</span></span>|<span data-ttu-id="689cd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="689cd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="689cd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="689cd-126">Accept</span></span>|<span data-ttu-id="689cd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="689cd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="689cd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="689cd-128">Request body</span></span>
<span data-ttu-id="689cd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="689cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="689cd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="689cd-130">Response</span></span>
<span data-ttu-id="689cd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="689cd-131">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689cd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="689cd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="689cd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="689cd-133">Request</span></span>
<span data-ttu-id="689cd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="689cd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="689cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="689cd-135">Response</span></span>
<span data-ttu-id="689cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="689cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
    "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
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
    "propertyDefinitionIds": [
      "Property Definition Ids value"
    ]
  }
}
```





