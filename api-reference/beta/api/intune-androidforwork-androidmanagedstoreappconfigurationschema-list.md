---
title: Lista androidManagedStoreAppConfigurationSchemas
description: Lista as propriedades e os relacionamentos dos objetos androidManagedStoreAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c655795b05dba448508001585d5ef2baa24e7da3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401779"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="87a7f-103">Lista androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="87a7f-103">List androidManagedStoreAppConfigurationSchemas</span></span>

> <span data-ttu-id="87a7f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="87a7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87a7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87a7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87a7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="87a7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a7f-107">Lista as propriedades e os relacionamentos dos objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="87a7f-107">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87a7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87a7f-108">Prerequisites</span></span>
<span data-ttu-id="87a7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87a7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87a7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87a7f-111">Permission type</span></span>|<span data-ttu-id="87a7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87a7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87a7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87a7f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87a7f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87a7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87a7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a7f-116">Not supported.</span></span>|
|<span data-ttu-id="87a7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87a7f-117">Application</span></span>|<span data-ttu-id="87a7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87a7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="87a7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87a7f-120">Request headers</span></span>
|<span data-ttu-id="87a7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87a7f-121">Header</span></span>|<span data-ttu-id="87a7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87a7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87a7f-123">Authorization</span></span>|<span data-ttu-id="87a7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87a7f-125">Accept</span></span>|<span data-ttu-id="87a7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87a7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87a7f-127">Request body</span></span>
<span data-ttu-id="87a7f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87a7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87a7f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a7f-129">Response</span></span>
<span data-ttu-id="87a7f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a7f-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a7f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87a7f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87a7f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87a7f-132">Request</span></span>
<span data-ttu-id="87a7f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87a7f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="87a7f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a7f-134">Response</span></span>
<span data-ttu-id="87a7f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87a7f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




