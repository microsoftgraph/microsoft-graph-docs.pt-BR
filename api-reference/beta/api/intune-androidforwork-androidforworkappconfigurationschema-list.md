---
title: Listar androidForWorkAppConfigurationSchemas
description: Listar propriedades e relações dos objetos androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10da106f50a6c7bf95b13e3a9fc241b96a797d16
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254997"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="b79fd-103">Listar androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="b79fd-103">List androidForWorkAppConfigurationSchemas</span></span>

<span data-ttu-id="b79fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b79fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b79fd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b79fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b79fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b79fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b79fd-107">Listar propriedades e relações dos objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="b79fd-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b79fd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b79fd-108">Prerequisites</span></span>
<span data-ttu-id="b79fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b79fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b79fd-111">Permission type</span></span>|<span data-ttu-id="b79fd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b79fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b79fd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b79fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b79fd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79fd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b79fd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b79fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b79fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b79fd-116">Not supported.</span></span>|
|<span data-ttu-id="b79fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b79fd-117">Application</span></span>|<span data-ttu-id="b79fd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79fd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b79fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b79fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="b79fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b79fd-120">Request headers</span></span>
|<span data-ttu-id="b79fd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b79fd-121">Header</span></span>|<span data-ttu-id="b79fd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b79fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b79fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b79fd-123">Authorization</span></span>|<span data-ttu-id="b79fd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b79fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b79fd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b79fd-125">Accept</span></span>|<span data-ttu-id="b79fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b79fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b79fd-127">Request body</span></span>
<span data-ttu-id="b79fd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b79fd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b79fd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b79fd-129">Response</span></span>
<span data-ttu-id="b79fd-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b79fd-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b79fd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b79fd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b79fd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b79fd-132">Request</span></span>
<span data-ttu-id="b79fd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b79fd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="b79fd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b79fd-134">Response</span></span>
<span data-ttu-id="b79fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b79fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




