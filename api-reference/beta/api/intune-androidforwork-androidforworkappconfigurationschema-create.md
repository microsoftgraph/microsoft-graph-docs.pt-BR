---
title: Criar androidForWorkAppConfigurationSchema
description: Criar um novo objeto androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ebbe17ab43740e389da432f69866b8f7a37fa88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446272"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="69bd9-103">Criar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="69bd9-103">Create androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="69bd9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69bd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69bd9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69bd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69bd9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69bd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69bd9-107">Criar um novo objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="69bd9-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69bd9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69bd9-108">Prerequisites</span></span>
<span data-ttu-id="69bd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69bd9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69bd9-111">Permission type</span></span>|<span data-ttu-id="69bd9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69bd9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69bd9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69bd9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69bd9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69bd9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69bd9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69bd9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69bd9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69bd9-116">Not supported.</span></span>|
|<span data-ttu-id="69bd9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69bd9-117">Application</span></span>|<span data-ttu-id="69bd9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69bd9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69bd9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69bd9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="69bd9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69bd9-120">Request headers</span></span>
|<span data-ttu-id="69bd9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69bd9-121">Header</span></span>|<span data-ttu-id="69bd9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="69bd9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69bd9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69bd9-123">Authorization</span></span>|<span data-ttu-id="69bd9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69bd9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69bd9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69bd9-125">Accept</span></span>|<span data-ttu-id="69bd9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69bd9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69bd9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69bd9-127">Request body</span></span>
<span data-ttu-id="69bd9-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="69bd9-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="69bd9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkAppConfigurationSchema.</span><span class="sxs-lookup"><span data-stu-id="69bd9-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="69bd9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69bd9-130">Property</span></span>|<span data-ttu-id="69bd9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69bd9-131">Type</span></span>|<span data-ttu-id="69bd9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69bd9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69bd9-133">id</span><span class="sxs-lookup"><span data-stu-id="69bd9-133">id</span></span>|<span data-ttu-id="69bd9-134">String</span><span class="sxs-lookup"><span data-stu-id="69bd9-134">String</span></span>|<span data-ttu-id="69bd9-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="69bd9-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="69bd9-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="69bd9-136">exampleJson</span></span>|<span data-ttu-id="69bd9-137">Binária</span><span class="sxs-lookup"><span data-stu-id="69bd9-137">Binary</span></span>|<span data-ttu-id="69bd9-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="69bd9-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="69bd9-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="69bd9-139">schemaItems</span></span>|<span data-ttu-id="69bd9-140">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="69bd9-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="69bd9-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="69bd9-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="69bd9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="69bd9-142">Response</span></span>
<span data-ttu-id="69bd9-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69bd9-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69bd9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69bd9-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="69bd9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69bd9-145">Request</span></span>
<span data-ttu-id="69bd9-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69bd9-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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

### <a name="response"></a><span data-ttu-id="69bd9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="69bd9-147">Response</span></span>
<span data-ttu-id="69bd9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69bd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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





