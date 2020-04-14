---
title: Atualizar androidManagedStoreAppConfigurationSchema
description: Atualiza as propriedades de um objeto androidManagedStoreAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 399ebecdbed9942ebb5ca828c815aa6ad03befea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395496"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="03240-103">Atualizar androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="03240-103">Update androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="03240-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03240-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03240-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03240-107">Atualiza as propriedades de um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="03240-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03240-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03240-108">Prerequisites</span></span>
<span data-ttu-id="03240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03240-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03240-111">Permission type</span></span>|<span data-ttu-id="03240-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03240-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03240-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03240-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03240-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03240-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03240-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03240-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03240-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03240-116">Not supported.</span></span>|
|<span data-ttu-id="03240-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03240-117">Application</span></span>|<span data-ttu-id="03240-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03240-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03240-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03240-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="03240-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03240-120">Request headers</span></span>
|<span data-ttu-id="03240-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03240-121">Header</span></span>|<span data-ttu-id="03240-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03240-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03240-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03240-123">Authorization</span></span>|<span data-ttu-id="03240-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03240-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03240-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03240-125">Accept</span></span>|<span data-ttu-id="03240-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03240-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03240-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03240-127">Request body</span></span>
<span data-ttu-id="03240-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="03240-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="03240-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="03240-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="03240-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03240-130">Property</span></span>|<span data-ttu-id="03240-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03240-131">Type</span></span>|<span data-ttu-id="03240-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03240-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03240-133">id</span><span class="sxs-lookup"><span data-stu-id="03240-133">id</span></span>|<span data-ttu-id="03240-134">String</span><span class="sxs-lookup"><span data-stu-id="03240-134">String</span></span>|<span data-ttu-id="03240-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="03240-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="03240-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="03240-136">exampleJson</span></span>|<span data-ttu-id="03240-137">Binária</span><span class="sxs-lookup"><span data-stu-id="03240-137">Binary</span></span>|<span data-ttu-id="03240-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="03240-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="03240-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="03240-139">schemaItems</span></span>|<span data-ttu-id="03240-140">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="03240-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="03240-141">Coleção de itens que representa uma opção de configuração nomeada no esquema.</span><span class="sxs-lookup"><span data-stu-id="03240-141">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="03240-142">Ele contém apenas a configuração de nível de raiz.</span><span class="sxs-lookup"><span data-stu-id="03240-142">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="03240-143">nestedSchemaItems</span><span class="sxs-lookup"><span data-stu-id="03240-143">nestedSchemaItems</span></span>|<span data-ttu-id="03240-144">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="03240-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="03240-145">Coleção de itens que representa uma opção de configuração nomeada no esquema.</span><span class="sxs-lookup"><span data-stu-id="03240-145">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="03240-146">Ele contém uma lista simples de todas as configurações.</span><span class="sxs-lookup"><span data-stu-id="03240-146">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="03240-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="03240-147">Response</span></span>
<span data-ttu-id="03240-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03240-148">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03240-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03240-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="03240-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03240-150">Request</span></span>
<span data-ttu-id="03240-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03240-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
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
```

### <a name="response"></a><span data-ttu-id="03240-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="03240-152">Response</span></span>
<span data-ttu-id="03240-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03240-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

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
```



