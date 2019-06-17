---
title: Atualizar androidForWorkAppConfigurationSchema
description: Atualizar as propriedades de um objeto androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c417c07ae2b3d4b6f3282adc4a3c66d4a849b72
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965624"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="eb822-103">Atualizar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="eb822-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="eb822-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb822-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb822-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb822-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb822-106">Atualizar as propriedades de um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="eb822-106">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb822-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb822-107">Prerequisites</span></span>
<span data-ttu-id="eb822-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb822-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb822-110">Permission type</span></span>|<span data-ttu-id="eb822-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb822-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb822-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb822-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb822-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb822-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb822-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb822-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb822-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb822-115">Not supported.</span></span>|
|<span data-ttu-id="eb822-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb822-116">Application</span></span>|<span data-ttu-id="eb822-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb822-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb822-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb822-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="eb822-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb822-119">Request headers</span></span>
|<span data-ttu-id="eb822-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb822-120">Header</span></span>|<span data-ttu-id="eb822-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb822-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb822-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb822-122">Authorization</span></span>|<span data-ttu-id="eb822-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb822-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb822-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb822-124">Accept</span></span>|<span data-ttu-id="eb822-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb822-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb822-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb822-126">Request body</span></span>
<span data-ttu-id="eb822-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="eb822-127">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="eb822-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="eb822-128">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="eb822-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb822-129">Property</span></span>|<span data-ttu-id="eb822-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb822-130">Type</span></span>|<span data-ttu-id="eb822-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb822-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb822-132">id</span><span class="sxs-lookup"><span data-stu-id="eb822-132">id</span></span>|<span data-ttu-id="eb822-133">String</span><span class="sxs-lookup"><span data-stu-id="eb822-133">String</span></span>|<span data-ttu-id="eb822-134">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="eb822-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="eb822-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="eb822-135">exampleJson</span></span>|<span data-ttu-id="eb822-136">Binária</span><span class="sxs-lookup"><span data-stu-id="eb822-136">Binary</span></span>|<span data-ttu-id="eb822-137">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb822-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="eb822-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="eb822-138">schemaItems</span></span>|<span data-ttu-id="eb822-139">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="eb822-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="eb822-140">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="eb822-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="eb822-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb822-141">Response</span></span>
<span data-ttu-id="eb822-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb822-142">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb822-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb822-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb822-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb822-144">Request</span></span>
<span data-ttu-id="eb822-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb822-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb822-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb822-146">Response</span></span>
<span data-ttu-id="eb822-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb822-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





