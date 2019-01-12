---
title: Atualizar androidForWorkAppConfigurationSchema
description: Atualizar as propriedades de um objeto androidForWorkAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09393062a4d23622c10bf87f3fec420fc51c6650
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946515"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="fce02-103">Atualizar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="fce02-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="fce02-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fce02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fce02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fce02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fce02-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fce02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fce02-107">Atualizar as propriedades de um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fce02-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fce02-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fce02-108">Prerequisites</span></span>
<span data-ttu-id="fce02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce02-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fce02-111">Permission type</span></span>|<span data-ttu-id="fce02-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fce02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fce02-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fce02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fce02-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce02-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fce02-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fce02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fce02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fce02-116">Not supported.</span></span>|
|<span data-ttu-id="fce02-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fce02-117">Application</span></span>|<span data-ttu-id="fce02-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fce02-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fce02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fce02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="fce02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fce02-120">Request headers</span></span>
|<span data-ttu-id="fce02-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fce02-121">Header</span></span>|<span data-ttu-id="fce02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fce02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fce02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fce02-123">Authorization</span></span>|<span data-ttu-id="fce02-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fce02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fce02-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fce02-125">Accept</span></span>|<span data-ttu-id="fce02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fce02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fce02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fce02-127">Request body</span></span>
<span data-ttu-id="fce02-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fce02-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="fce02-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fce02-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="fce02-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fce02-130">Property</span></span>|<span data-ttu-id="fce02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fce02-131">Type</span></span>|<span data-ttu-id="fce02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fce02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce02-133">id</span><span class="sxs-lookup"><span data-stu-id="fce02-133">id</span></span>|<span data-ttu-id="fce02-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce02-134">String</span></span>|<span data-ttu-id="fce02-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="fce02-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="fce02-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="fce02-136">exampleJson</span></span>|<span data-ttu-id="fce02-137">Binária</span><span class="sxs-lookup"><span data-stu-id="fce02-137">Binary</span></span>|<span data-ttu-id="fce02-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="fce02-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="fce02-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="fce02-139">schemaItems</span></span>|<span data-ttu-id="fce02-140">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="fce02-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="fce02-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="fce02-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="fce02-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce02-142">Response</span></span>
<span data-ttu-id="fce02-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fce02-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce02-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fce02-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="fce02-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fce02-145">Request</span></span>
<span data-ttu-id="fce02-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fce02-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
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

### <a name="response"></a><span data-ttu-id="fce02-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce02-147">Response</span></span>
<span data-ttu-id="fce02-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fce02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





