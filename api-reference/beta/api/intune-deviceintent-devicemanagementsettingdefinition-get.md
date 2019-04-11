---
title: Obter deviceManagementSettingDefinition
description: Leia as propriedades e as relações do objeto deviceManagementSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7655e46fc8ac5e24e970760b2d926aa8c0cd81d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789833"
---
# <a name="get-devicemanagementsettingdefinition"></a><span data-ttu-id="04704-103">Obter deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="04704-103">Get deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="04704-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04704-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04704-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04704-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04704-106">Leia as propriedades e as relações do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="04704-106">Read properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04704-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04704-107">Prerequisites</span></span>
<span data-ttu-id="04704-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04704-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04704-110">Permission type</span></span>|<span data-ttu-id="04704-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04704-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04704-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04704-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04704-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="04704-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="04704-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04704-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04704-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04704-115">Not supported.</span></span>|
|<span data-ttu-id="04704-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04704-116">Application</span></span>|<span data-ttu-id="04704-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04704-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04704-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04704-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="04704-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04704-119">Optional query parameters</span></span>
<span data-ttu-id="04704-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04704-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04704-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04704-121">Request headers</span></span>
|<span data-ttu-id="04704-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04704-122">Header</span></span>|<span data-ttu-id="04704-123">Valor</span><span class="sxs-lookup"><span data-stu-id="04704-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04704-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="04704-124">Authorization</span></span>|<span data-ttu-id="04704-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04704-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04704-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04704-126">Accept</span></span>|<span data-ttu-id="04704-127">application/json</span><span class="sxs-lookup"><span data-stu-id="04704-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04704-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04704-128">Request body</span></span>
<span data-ttu-id="04704-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04704-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04704-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="04704-130">Response</span></span>
<span data-ttu-id="04704-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04704-131">If successful, this method returns a `200 OK` response code and [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04704-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04704-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="04704-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04704-133">Request</span></span>
<span data-ttu-id="04704-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04704-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="04704-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="04704-135">Response</span></span>
<span data-ttu-id="04704-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04704-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





