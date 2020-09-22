---
title: Listar androidManagedStoreAppConfigurationSchemas
description: Listar Propriedades e relações dos objetos androidManagedStoreAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 923819bf4850243510a2dc1e499d42b0a054dcc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001271"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="617f6-103">Listar androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="617f6-103">List androidManagedStoreAppConfigurationSchemas</span></span>

<span data-ttu-id="617f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="617f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="617f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="617f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="617f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="617f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="617f6-107">Listar Propriedades e relações dos objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="617f6-107">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="617f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="617f6-108">Prerequisites</span></span>
<span data-ttu-id="617f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="617f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="617f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="617f6-111">Permission type</span></span>|<span data-ttu-id="617f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="617f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="617f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="617f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="617f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="617f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="617f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="617f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="617f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="617f6-116">Not supported.</span></span>|
|<span data-ttu-id="617f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="617f6-117">Application</span></span>|<span data-ttu-id="617f6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="617f6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="617f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="617f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="617f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="617f6-120">Request headers</span></span>
|<span data-ttu-id="617f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="617f6-121">Header</span></span>|<span data-ttu-id="617f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="617f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="617f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="617f6-123">Authorization</span></span>|<span data-ttu-id="617f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="617f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="617f6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="617f6-125">Accept</span></span>|<span data-ttu-id="617f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="617f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="617f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="617f6-127">Request body</span></span>
<span data-ttu-id="617f6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="617f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="617f6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="617f6-129">Response</span></span>
<span data-ttu-id="617f6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="617f6-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="617f6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="617f6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="617f6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="617f6-132">Request</span></span>
<span data-ttu-id="617f6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="617f6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="617f6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="617f6-134">Response</span></span>
<span data-ttu-id="617f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="617f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1871

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
      "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
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
      ],
      "nestedSchemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
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






