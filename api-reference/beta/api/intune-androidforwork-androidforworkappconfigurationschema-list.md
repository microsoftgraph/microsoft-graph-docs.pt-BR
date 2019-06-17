---
title: Listar androidForWorkAppConfigurationSchemas
description: Listar propriedades e relações dos objetos androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6cd8f76142983b42be24632c4ca79371423c322
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966569"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="94358-103">Listar androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="94358-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="94358-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94358-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94358-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94358-106">Listar propriedades e relações dos objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="94358-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94358-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94358-107">Prerequisites</span></span>
<span data-ttu-id="94358-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94358-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94358-110">Permission type</span></span>|<span data-ttu-id="94358-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94358-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94358-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94358-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94358-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94358-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94358-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94358-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94358-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94358-115">Not supported.</span></span>|
|<span data-ttu-id="94358-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94358-116">Application</span></span>|<span data-ttu-id="94358-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94358-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94358-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94358-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="94358-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94358-119">Request headers</span></span>
|<span data-ttu-id="94358-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94358-120">Header</span></span>|<span data-ttu-id="94358-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94358-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94358-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94358-122">Authorization</span></span>|<span data-ttu-id="94358-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94358-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94358-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94358-124">Accept</span></span>|<span data-ttu-id="94358-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94358-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94358-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94358-126">Request body</span></span>
<span data-ttu-id="94358-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94358-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94358-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94358-128">Response</span></span>
<span data-ttu-id="94358-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94358-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94358-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94358-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="94358-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94358-131">Request</span></span>
<span data-ttu-id="94358-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94358-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="94358-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="94358-133">Response</span></span>
<span data-ttu-id="94358-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94358-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





