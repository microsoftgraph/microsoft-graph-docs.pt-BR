---
title: Listar androidManagedStoreAppConfigurationSchemas
description: Listar Propriedades e relações dos objetos androidManagedStoreAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 150912f43cfeaaf90378d21ca7e90040fbfd8d4a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966429"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="5e2f5-103">Listar androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="5e2f5-103">List androidManagedStoreAppConfigurationSchemas</span></span>

> <span data-ttu-id="5e2f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e2f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e2f5-106">Listar Propriedades e relações dos objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="5e2f5-106">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e2f5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e2f5-107">Prerequisites</span></span>
<span data-ttu-id="5e2f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e2f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e2f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e2f5-110">Permission type</span></span>|<span data-ttu-id="5e2f5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e2f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e2f5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e2f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e2f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e2f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e2f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e2f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e2f5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-115">Not supported.</span></span>|
|<span data-ttu-id="5e2f5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e2f5-116">Application</span></span>|<span data-ttu-id="5e2f5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e2f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="5e2f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2f5-119">Request headers</span></span>
|<span data-ttu-id="5e2f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e2f5-120">Header</span></span>|<span data-ttu-id="5e2f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5e2f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e2f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e2f5-122">Authorization</span></span>|<span data-ttu-id="5e2f5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e2f5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e2f5-124">Accept</span></span>|<span data-ttu-id="5e2f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e2f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e2f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2f5-126">Request body</span></span>
<span data-ttu-id="5e2f5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e2f5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2f5-128">Response</span></span>
<span data-ttu-id="5e2f5-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e2f5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e2f5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e2f5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2f5-131">Request</span></span>
<span data-ttu-id="5e2f5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="5e2f5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2f5-133">Response</span></span>
<span data-ttu-id="5e2f5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e2f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 987

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
      "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





