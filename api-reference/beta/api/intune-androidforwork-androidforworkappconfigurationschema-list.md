---
title: Listar androidForWorkAppConfigurationSchemas
description: Listar propriedades e relações dos objetos androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8fc68b90da5144453066d3c46028fc2d916152f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813927"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="20499-103">Listar androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="20499-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="20499-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20499-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20499-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20499-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20499-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20499-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20499-107">Listar propriedades e relações dos objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="20499-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20499-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20499-108">Prerequisites</span></span>
<span data-ttu-id="20499-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20499-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20499-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20499-111">Permission type</span></span>|<span data-ttu-id="20499-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20499-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20499-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20499-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20499-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20499-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="20499-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20499-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20499-116">Not supported.</span></span>|
|<span data-ttu-id="20499-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20499-117">Application</span></span>|<span data-ttu-id="20499-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20499-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20499-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="20499-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20499-120">Request headers</span></span>
|<span data-ttu-id="20499-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20499-121">Header</span></span>|<span data-ttu-id="20499-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20499-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20499-123">Authorization</span></span>|<span data-ttu-id="20499-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20499-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20499-125">Accept</span></span>|<span data-ttu-id="20499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20499-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20499-127">Request body</span></span>
<span data-ttu-id="20499-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20499-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20499-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20499-129">Response</span></span>
<span data-ttu-id="20499-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20499-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20499-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20499-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="20499-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20499-132">Request</span></span>
<span data-ttu-id="20499-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20499-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="20499-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="20499-134">Response</span></span>
<span data-ttu-id="20499-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20499-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





