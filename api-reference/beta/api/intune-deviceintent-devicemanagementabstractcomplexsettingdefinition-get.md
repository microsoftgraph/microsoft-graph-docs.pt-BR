---
title: Obter deviceManagementAbstractComplexSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementAbstractComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b3776041773ba7461031b5feea33456179d481a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961067"
---
# <a name="get-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="78ede-103">Obter deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="78ede-103">Get deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="78ede-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78ede-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ede-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78ede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ede-106">Leia as propriedades e as relações do objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="78ede-106">Read properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78ede-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78ede-107">Prerequisites</span></span>
<span data-ttu-id="78ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78ede-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78ede-110">Permission type</span></span>|<span data-ttu-id="78ede-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78ede-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78ede-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78ede-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78ede-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78ede-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78ede-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78ede-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ede-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ede-115">Not supported.</span></span>|
|<span data-ttu-id="78ede-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78ede-116">Application</span></span>|<span data-ttu-id="78ede-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ede-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ede-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78ede-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="78ede-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78ede-119">Optional query parameters</span></span>
<span data-ttu-id="78ede-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78ede-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78ede-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78ede-121">Request headers</span></span>
|<span data-ttu-id="78ede-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78ede-122">Header</span></span>|<span data-ttu-id="78ede-123">Valor</span><span class="sxs-lookup"><span data-stu-id="78ede-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78ede-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="78ede-124">Authorization</span></span>|<span data-ttu-id="78ede-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78ede-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78ede-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78ede-126">Accept</span></span>|<span data-ttu-id="78ede-127">application/json</span><span class="sxs-lookup"><span data-stu-id="78ede-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78ede-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78ede-128">Request body</span></span>
<span data-ttu-id="78ede-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78ede-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78ede-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ede-130">Response</span></span>
<span data-ttu-id="78ede-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ede-131">If successful, this method returns a `200 OK` response code and [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78ede-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78ede-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="78ede-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78ede-133">Request</span></span>
<span data-ttu-id="78ede-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ede-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="78ede-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ede-135">Response</span></span>
<span data-ttu-id="78ede-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78ede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 928

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
    "id": "1b703309-3309-1b70-0933-701b0933701b",
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
    "implementations": [
      "Implementations value"
    ]
  }
}
```





