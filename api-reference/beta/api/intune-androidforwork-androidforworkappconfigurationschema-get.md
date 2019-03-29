---
title: Get androidForWorkAppConfigurationSchema
description: Ler propriedades e relações do objeto androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4028244c487aaecbb9ab53a18800ee7769239f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977342"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="ae2d6-103">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ae2d6-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="ae2d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae2d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae2d6-106">Ler propriedades e relações do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="ae2d6-106">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae2d6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae2d6-107">Prerequisites</span></span>
<span data-ttu-id="ae2d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae2d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae2d6-110">Permission type</span></span>|<span data-ttu-id="ae2d6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae2d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae2d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae2d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae2d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae2d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae2d6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae2d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae2d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-115">Not supported.</span></span>|
|<span data-ttu-id="ae2d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae2d6-116">Application</span></span>|<span data-ttu-id="ae2d6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae2d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae2d6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae2d6-119">Optional query parameters</span></span>
<span data-ttu-id="ae2d6-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae2d6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2d6-121">Request headers</span></span>
|<span data-ttu-id="ae2d6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae2d6-122">Header</span></span>|<span data-ttu-id="ae2d6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ae2d6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae2d6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae2d6-124">Authorization</span></span>|<span data-ttu-id="ae2d6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae2d6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae2d6-126">Accept</span></span>|<span data-ttu-id="ae2d6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae2d6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae2d6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2d6-128">Request body</span></span>
<span data-ttu-id="ae2d6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae2d6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae2d6-130">Response</span></span>
<span data-ttu-id="ae2d6-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-131">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2d6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae2d6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae2d6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2d6-133">Request</span></span>
<span data-ttu-id="ae2d6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="ae2d6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae2d6-135">Response</span></span>
<span data-ttu-id="ae2d6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae2d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
    "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
    "exampleJson": "ZXhhbXBsZUpzb24=",
    "schemaItems": [
      {
        "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
        "schemaItemKey": "Schema Item Key value",
        "displayName": "Display Name value",
        "description": "Description value",
        "defaultBoolValue": true,
        "defaultIntValue": 15,
        "defaultStringValue": "Default String Value value",
        "defaultStringArrayValue": [
          "Default String Array Value value"
        ],
        "dataType": "integer",
        "selections": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ]
      }
    ]
  }
}
```




