---
title: Get androidForWorkAppConfigurationSchema
description: Ler propriedades e relações do objeto androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e5c6e60a34632dccb95b2ad66473ec9f143b89d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32499842"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="d9bd5-103">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="d9bd5-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="d9bd5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9bd5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9bd5-106">Ler propriedades e relações do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="d9bd5-106">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9bd5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9bd5-107">Prerequisites</span></span>
<span data-ttu-id="d9bd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9bd5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9bd5-110">Permission type</span></span>|<span data-ttu-id="d9bd5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9bd5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9bd5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9bd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9bd5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9bd5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9bd5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9bd5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9bd5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-115">Not supported.</span></span>|
|<span data-ttu-id="d9bd5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9bd5-116">Application</span></span>|<span data-ttu-id="d9bd5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9bd5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9bd5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9bd5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9bd5-119">Optional query parameters</span></span>
<span data-ttu-id="d9bd5-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9bd5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9bd5-121">Request headers</span></span>
|<span data-ttu-id="d9bd5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9bd5-122">Header</span></span>|<span data-ttu-id="d9bd5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d9bd5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9bd5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9bd5-124">Authorization</span></span>|<span data-ttu-id="d9bd5-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9bd5-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9bd5-126">Accept</span></span>|<span data-ttu-id="d9bd5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d9bd5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9bd5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9bd5-128">Request body</span></span>
<span data-ttu-id="d9bd5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9bd5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9bd5-130">Response</span></span>
<span data-ttu-id="d9bd5-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-131">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9bd5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9bd5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9bd5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9bd5-133">Request</span></span>
<span data-ttu-id="d9bd5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="d9bd5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9bd5-135">Response</span></span>
<span data-ttu-id="d9bd5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9bd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





