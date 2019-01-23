---
title: Atualizar androidManagedStoreAppConfigurationSchema
description: Atualize as propriedades de um objeto androidManagedStoreAppConfigurationSchema.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 326f56f497f1086ccc6e37d0171261c50dfb9c77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410130"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="62a9b-103">Atualizar androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="62a9b-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="62a9b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="62a9b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62a9b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62a9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62a9b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="62a9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a9b-107">Atualize as propriedades de um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="62a9b-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a9b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62a9b-108">Prerequisites</span></span>
<span data-ttu-id="62a9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62a9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62a9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62a9b-111">Permission type</span></span>|<span data-ttu-id="62a9b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62a9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a9b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62a9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a9b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a9b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62a9b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62a9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a9b-116">Not supported.</span></span>|
|<span data-ttu-id="62a9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a9b-117">Application</span></span>|<span data-ttu-id="62a9b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a9b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62a9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="62a9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62a9b-120">Request headers</span></span>
|<span data-ttu-id="62a9b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62a9b-121">Header</span></span>|<span data-ttu-id="62a9b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62a9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a9b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62a9b-123">Authorization</span></span>|<span data-ttu-id="62a9b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62a9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a9b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62a9b-125">Accept</span></span>|<span data-ttu-id="62a9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62a9b-127">Request body</span></span>
<span data-ttu-id="62a9b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="62a9b-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="62a9b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="62a9b-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="62a9b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a9b-130">Property</span></span>|<span data-ttu-id="62a9b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a9b-131">Type</span></span>|<span data-ttu-id="62a9b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a9b-133">id</span><span class="sxs-lookup"><span data-stu-id="62a9b-133">id</span></span>|<span data-ttu-id="62a9b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62a9b-134">String</span></span>|<span data-ttu-id="62a9b-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="62a9b-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="62a9b-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="62a9b-136">exampleJson</span></span>|<span data-ttu-id="62a9b-137">Binária</span><span class="sxs-lookup"><span data-stu-id="62a9b-137">Binary</span></span>|<span data-ttu-id="62a9b-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a9b-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="62a9b-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="62a9b-139">schemaItems</span></span>|<span data-ttu-id="62a9b-140">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="62a9b-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="62a9b-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="62a9b-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="62a9b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a9b-142">Response</span></span>
<span data-ttu-id="62a9b-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62a9b-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a9b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62a9b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a9b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62a9b-145">Request</span></span>
<span data-ttu-id="62a9b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62a9b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62a9b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a9b-147">Response</span></span>
<span data-ttu-id="62a9b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62a9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




