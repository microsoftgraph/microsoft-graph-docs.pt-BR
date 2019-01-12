---
title: Atualizar androidManagedStoreAppConfigurationSchema
description: Atualize as propriedades de um objeto androidManagedStoreAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f45a7d831c9db3b94a2cc8812e900ac20faf8887
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956651"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="85375-103">Atualizar androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="85375-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="85375-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85375-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85375-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85375-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85375-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85375-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85375-107">Atualize as propriedades de um objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="85375-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85375-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85375-108">Prerequisites</span></span>
<span data-ttu-id="85375-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85375-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85375-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85375-111">Permission type</span></span>|<span data-ttu-id="85375-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85375-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85375-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85375-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85375-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85375-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85375-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85375-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85375-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85375-116">Not supported.</span></span>|
|<span data-ttu-id="85375-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85375-117">Application</span></span>|<span data-ttu-id="85375-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85375-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85375-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85375-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="85375-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85375-120">Request headers</span></span>
|<span data-ttu-id="85375-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85375-121">Header</span></span>|<span data-ttu-id="85375-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85375-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85375-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85375-123">Authorization</span></span>|<span data-ttu-id="85375-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85375-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85375-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85375-125">Accept</span></span>|<span data-ttu-id="85375-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85375-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85375-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85375-127">Request body</span></span>
<span data-ttu-id="85375-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="85375-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="85375-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="85375-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="85375-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85375-130">Property</span></span>|<span data-ttu-id="85375-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="85375-131">Type</span></span>|<span data-ttu-id="85375-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="85375-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85375-133">id</span><span class="sxs-lookup"><span data-stu-id="85375-133">id</span></span>|<span data-ttu-id="85375-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85375-134">String</span></span>|<span data-ttu-id="85375-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="85375-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="85375-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="85375-136">exampleJson</span></span>|<span data-ttu-id="85375-137">Binária</span><span class="sxs-lookup"><span data-stu-id="85375-137">Binary</span></span>|<span data-ttu-id="85375-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="85375-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="85375-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="85375-139">schemaItems</span></span>|<span data-ttu-id="85375-140">coleção [androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="85375-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="85375-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="85375-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="85375-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="85375-142">Response</span></span>
<span data-ttu-id="85375-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85375-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85375-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85375-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="85375-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85375-145">Request</span></span>
<span data-ttu-id="85375-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85375-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 725

{
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

### <a name="response"></a><span data-ttu-id="85375-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="85375-147">Response</span></span>
<span data-ttu-id="85375-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85375-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





