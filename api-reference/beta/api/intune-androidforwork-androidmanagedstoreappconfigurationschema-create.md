---
title: Criar androidManagedStoreAppConfigurationSchema
description: Crie um novo objeto de androidManagedStoreAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c3cf700bb835df981c419fc15b56ef5fbc905fea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874540"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="b3144-103">Criar androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="b3144-103">Create androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="b3144-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3144-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3144-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3144-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3144-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3144-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3144-107">Crie um novo objeto de [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="b3144-107">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3144-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3144-108">Prerequisites</span></span>
<span data-ttu-id="b3144-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3144-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3144-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3144-111">Permission type</span></span>|<span data-ttu-id="b3144-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3144-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3144-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3144-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3144-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3144-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3144-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3144-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3144-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3144-116">Not supported.</span></span>|
|<span data-ttu-id="b3144-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3144-117">Application</span></span>|<span data-ttu-id="b3144-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3144-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3144-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3144-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="b3144-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3144-120">Request headers</span></span>
|<span data-ttu-id="b3144-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3144-121">Header</span></span>|<span data-ttu-id="b3144-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3144-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3144-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3144-123">Authorization</span></span>|<span data-ttu-id="b3144-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3144-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3144-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3144-125">Accept</span></span>|<span data-ttu-id="b3144-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3144-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3144-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3144-127">Request body</span></span>
<span data-ttu-id="b3144-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidManagedStoreAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="b3144-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="b3144-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidManagedStoreAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="b3144-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="b3144-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3144-130">Property</span></span>|<span data-ttu-id="b3144-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3144-131">Type</span></span>|<span data-ttu-id="b3144-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3144-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3144-133">id</span><span class="sxs-lookup"><span data-stu-id="b3144-133">id</span></span>|<span data-ttu-id="b3144-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3144-134">String</span></span>|<span data-ttu-id="b3144-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="b3144-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="b3144-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="b3144-136">exampleJson</span></span>|<span data-ttu-id="b3144-137">Binária</span><span class="sxs-lookup"><span data-stu-id="b3144-137">Binary</span></span>|<span data-ttu-id="b3144-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3144-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="b3144-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="b3144-139">schemaItems</span></span>|<span data-ttu-id="b3144-140">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="b3144-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="b3144-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="b3144-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="b3144-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3144-142">Response</span></span>
<span data-ttu-id="b3144-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3144-143">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3144-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3144-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3144-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3144-145">Request</span></span>
<span data-ttu-id="b3144-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3144-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="b3144-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3144-147">Response</span></span>
<span data-ttu-id="b3144-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3144-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





