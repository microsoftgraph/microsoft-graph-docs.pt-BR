---
title: Obter androidManagedStoreAppConfigurationSchema
description: Leia as propriedades e as relações do objeto androidManagedStoreAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e813b1fe5bef2f13db8867eb41baaff98009418b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395511"
---
# <a name="get-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="524b1-103">Obter androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="524b1-103">Get androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="524b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="524b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="524b1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="524b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="524b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="524b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="524b1-107">Leia as propriedades e as relações do objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="524b1-107">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="524b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="524b1-108">Prerequisites</span></span>
<span data-ttu-id="524b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="524b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="524b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="524b1-111">Permission type</span></span>|<span data-ttu-id="524b1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="524b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="524b1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="524b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="524b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="524b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="524b1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="524b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="524b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="524b1-116">Not supported.</span></span>|
|<span data-ttu-id="524b1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="524b1-117">Application</span></span>|<span data-ttu-id="524b1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="524b1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="524b1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="524b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="524b1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="524b1-120">Optional query parameters</span></span>
<span data-ttu-id="524b1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="524b1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="524b1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="524b1-122">Request headers</span></span>
|<span data-ttu-id="524b1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="524b1-123">Header</span></span>|<span data-ttu-id="524b1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="524b1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="524b1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="524b1-125">Authorization</span></span>|<span data-ttu-id="524b1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="524b1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="524b1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="524b1-127">Accept</span></span>|<span data-ttu-id="524b1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="524b1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="524b1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="524b1-129">Request body</span></span>
<span data-ttu-id="524b1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="524b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="524b1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="524b1-131">Response</span></span>
<span data-ttu-id="524b1-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="524b1-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="524b1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="524b1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="524b1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="524b1-134">Request</span></span>
<span data-ttu-id="524b1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="524b1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="524b1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="524b1-136">Response</span></span>
<span data-ttu-id="524b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="524b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "value": {
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
}
```



