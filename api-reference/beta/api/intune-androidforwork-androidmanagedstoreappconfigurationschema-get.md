---
title: Obter androidManagedStoreAppConfigurationSchema
description: Leia as propriedades e os relacionamentos do objeto androidManagedStoreAppConfigurationSchema.
ms.openlocfilehash: dc0da9d8cf92a6c346178e44ee8fe08b81ce9f4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035895"
---
# <a name="get-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="f3d61-103">Obter androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="f3d61-103">Get androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="f3d61-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3d61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3d61-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3d61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3d61-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f3d61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3d61-107">Leia as propriedades e os relacionamentos do objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="f3d61-107">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3d61-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3d61-108">Prerequisites</span></span>
<span data-ttu-id="f3d61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3d61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3d61-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3d61-111">Permission type</span></span>|<span data-ttu-id="f3d61-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3d61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3d61-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3d61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3d61-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3d61-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f3d61-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3d61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3d61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3d61-116">Not supported.</span></span>|
|<span data-ttu-id="f3d61-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3d61-117">Application</span></span>|<span data-ttu-id="f3d61-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3d61-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3d61-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3d61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3d61-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3d61-120">Optional query parameters</span></span>
<span data-ttu-id="f3d61-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3d61-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f3d61-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-122">Request headers</span></span>
|<span data-ttu-id="f3d61-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3d61-123">Header</span></span>|<span data-ttu-id="f3d61-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f3d61-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3d61-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3d61-125">Authorization</span></span>|<span data-ttu-id="f3d61-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3d61-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3d61-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f3d61-127">Accept</span></span>|<span data-ttu-id="f3d61-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f3d61-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3d61-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-129">Request body</span></span>
<span data-ttu-id="f3d61-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3d61-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3d61-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d61-131">Response</span></span>
<span data-ttu-id="f3d61-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3d61-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3d61-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3d61-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3d61-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d61-134">Request</span></span>
<span data-ttu-id="f3d61-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3d61-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="f3d61-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d61-136">Response</span></span>
<span data-ttu-id="f3d61-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3d61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 923

{
  "value": {
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
}
```





