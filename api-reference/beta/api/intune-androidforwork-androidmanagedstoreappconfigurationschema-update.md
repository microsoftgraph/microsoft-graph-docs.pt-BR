---
title: Atualizar androidManagedStoreAppConfigurationSchema
description: Atualiza as propriedades de um objeto androidManagedStoreAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95b01edae05234c1e6bd9c801d3f5c5f83287195
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32497567"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="60e58-103">Atualizar androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="60e58-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="60e58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60e58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60e58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e58-106">Atualiza as propriedades de um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="60e58-106">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60e58-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60e58-107">Prerequisites</span></span>
<span data-ttu-id="60e58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60e58-110">Permission type</span></span>|<span data-ttu-id="60e58-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60e58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60e58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60e58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60e58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60e58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60e58-115">Not supported.</span></span>|
|<span data-ttu-id="60e58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60e58-116">Application</span></span>|<span data-ttu-id="60e58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60e58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60e58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="60e58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60e58-119">Request headers</span></span>
|<span data-ttu-id="60e58-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60e58-120">Header</span></span>|<span data-ttu-id="60e58-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60e58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60e58-122">Authorization</span></span>|<span data-ttu-id="60e58-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60e58-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60e58-124">Accept</span></span>|<span data-ttu-id="60e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60e58-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60e58-126">Request body</span></span>
<span data-ttu-id="60e58-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="60e58-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="60e58-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="60e58-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="60e58-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60e58-129">Property</span></span>|<span data-ttu-id="60e58-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="60e58-130">Type</span></span>|<span data-ttu-id="60e58-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="60e58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e58-132">id</span><span class="sxs-lookup"><span data-stu-id="60e58-132">id</span></span>|<span data-ttu-id="60e58-133">String</span><span class="sxs-lookup"><span data-stu-id="60e58-133">String</span></span>|<span data-ttu-id="60e58-134">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="60e58-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="60e58-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="60e58-135">exampleJson</span></span>|<span data-ttu-id="60e58-136">Binária</span><span class="sxs-lookup"><span data-stu-id="60e58-136">Binary</span></span>|<span data-ttu-id="60e58-137">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="60e58-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="60e58-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="60e58-138">schemaItems</span></span>|<span data-ttu-id="60e58-139">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="60e58-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="60e58-140">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="60e58-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="60e58-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="60e58-141">Response</span></span>
<span data-ttu-id="60e58-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60e58-142">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e58-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60e58-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="60e58-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60e58-144">Request</span></span>
<span data-ttu-id="60e58-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60e58-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
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
```

### <a name="response"></a><span data-ttu-id="60e58-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="60e58-146">Response</span></span>
<span data-ttu-id="60e58-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60e58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

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
```





