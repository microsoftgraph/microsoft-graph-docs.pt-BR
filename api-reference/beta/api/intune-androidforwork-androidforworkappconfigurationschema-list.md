---
title: Listar androidForWorkAppConfigurationSchemas
description: Listar propriedades e relações dos objetos androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44f03b848e54b29e44049fc87014ccaf556a6908
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178379"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="5dadf-103">Listar androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="5dadf-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="5dadf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dadf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dadf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dadf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dadf-106">Listar propriedades e relações dos objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="5dadf-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dadf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dadf-107">Prerequisites</span></span>
<span data-ttu-id="5dadf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dadf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dadf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dadf-110">Permission type</span></span>|<span data-ttu-id="5dadf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dadf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dadf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dadf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5dadf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5dadf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5dadf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dadf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dadf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dadf-115">Not supported.</span></span>|
|<span data-ttu-id="5dadf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dadf-116">Application</span></span>|<span data-ttu-id="5dadf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5dadf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dadf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dadf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="5dadf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dadf-119">Request headers</span></span>
|<span data-ttu-id="5dadf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dadf-120">Header</span></span>|<span data-ttu-id="5dadf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5dadf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dadf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dadf-122">Authorization</span></span>|<span data-ttu-id="5dadf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dadf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dadf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dadf-124">Accept</span></span>|<span data-ttu-id="5dadf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5dadf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dadf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dadf-126">Request body</span></span>
<span data-ttu-id="5dadf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dadf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dadf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dadf-128">Response</span></span>
<span data-ttu-id="5dadf-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dadf-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dadf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dadf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dadf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dadf-131">Request</span></span>
<span data-ttu-id="5dadf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dadf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="5dadf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dadf-133">Response</span></span>
<span data-ttu-id="5dadf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dadf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
    {
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
  ]
}
```




