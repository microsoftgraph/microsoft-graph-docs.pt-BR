---
title: Atualizar androidForWorkAppConfigurationSchema
description: Atualizar as propriedades de um objeto androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dac55baada3bc4e2254aea9b2279588a137ac172
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141306"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="8228f-103">Atualizar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="8228f-103">Update androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="8228f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8228f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8228f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8228f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8228f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8228f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8228f-107">Atualizar as propriedades de um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8228f-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8228f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8228f-108">Prerequisites</span></span>
<span data-ttu-id="8228f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8228f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8228f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8228f-111">Permission type</span></span>|<span data-ttu-id="8228f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8228f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8228f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8228f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8228f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8228f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8228f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8228f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8228f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8228f-116">Not supported.</span></span>|
|<span data-ttu-id="8228f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8228f-117">Application</span></span>|<span data-ttu-id="8228f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8228f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8228f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8228f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="8228f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8228f-120">Request headers</span></span>
|<span data-ttu-id="8228f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8228f-121">Header</span></span>|<span data-ttu-id="8228f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8228f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8228f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8228f-123">Authorization</span></span>|<span data-ttu-id="8228f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8228f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8228f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8228f-125">Accept</span></span>|<span data-ttu-id="8228f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8228f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8228f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8228f-127">Request body</span></span>
<span data-ttu-id="8228f-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8228f-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="8228f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8228f-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="8228f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8228f-130">Property</span></span>|<span data-ttu-id="8228f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8228f-131">Type</span></span>|<span data-ttu-id="8228f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8228f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8228f-133">id</span><span class="sxs-lookup"><span data-stu-id="8228f-133">id</span></span>|<span data-ttu-id="8228f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8228f-134">String</span></span>|<span data-ttu-id="8228f-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="8228f-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="8228f-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="8228f-136">exampleJson</span></span>|<span data-ttu-id="8228f-137">Binária</span><span class="sxs-lookup"><span data-stu-id="8228f-137">Binary</span></span>|<span data-ttu-id="8228f-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="8228f-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="8228f-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="8228f-139">schemaItems</span></span>|<span data-ttu-id="8228f-140">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="8228f-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="8228f-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="8228f-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="8228f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8228f-142">Response</span></span>
<span data-ttu-id="8228f-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8228f-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8228f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8228f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8228f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8228f-145">Request</span></span>
<span data-ttu-id="8228f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8228f-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
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

### <a name="response"></a><span data-ttu-id="8228f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8228f-147">Response</span></span>
<span data-ttu-id="8228f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8228f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




