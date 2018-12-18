---
title: Atualizar androidForWorkAppConfigurationSchema
description: Atualizar as propriedades de um objeto androidForWorkAppConfigurationSchema.
author: tfitzmac
ms.openlocfilehash: ba4050ce741e1fdcfd3158e7f9e9d9e47f422882
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333898"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="239eb-103">Atualizar androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="239eb-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="239eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="239eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="239eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="239eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="239eb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="239eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="239eb-107">Atualizar as propriedades de um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="239eb-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="239eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="239eb-108">Prerequisites</span></span>
<span data-ttu-id="239eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="239eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="239eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="239eb-111">Permission type</span></span>|<span data-ttu-id="239eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="239eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="239eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="239eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="239eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="239eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="239eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="239eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="239eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="239eb-116">Not supported.</span></span>|
|<span data-ttu-id="239eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="239eb-117">Application</span></span>|<span data-ttu-id="239eb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="239eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="239eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="239eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="239eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="239eb-120">Request headers</span></span>
|<span data-ttu-id="239eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="239eb-121">Header</span></span>|<span data-ttu-id="239eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="239eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="239eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="239eb-123">Authorization</span></span>|<span data-ttu-id="239eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="239eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="239eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="239eb-125">Accept</span></span>|<span data-ttu-id="239eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="239eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="239eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="239eb-127">Request body</span></span>
<span data-ttu-id="239eb-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="239eb-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="239eb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="239eb-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="239eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="239eb-130">Property</span></span>|<span data-ttu-id="239eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="239eb-131">Type</span></span>|<span data-ttu-id="239eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="239eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="239eb-133">id</span><span class="sxs-lookup"><span data-stu-id="239eb-133">id</span></span>|<span data-ttu-id="239eb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="239eb-134">String</span></span>|<span data-ttu-id="239eb-135">A chave da entidade ao qual o nome do pacote Android para o aplicativo cujo esquema corresponde a</span><span class="sxs-lookup"><span data-stu-id="239eb-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="239eb-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="239eb-136">exampleJson</span></span>|<span data-ttu-id="239eb-137">Binária</span><span class="sxs-lookup"><span data-stu-id="239eb-137">Binary</span></span>|<span data-ttu-id="239eb-138">A matriz de bytes codificados de UTF8 que contém exemplo de cadeia JSON em conformidade com esse esquema que demonstra como definir a configuração para esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="239eb-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="239eb-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="239eb-139">schemaItems</span></span>|<span data-ttu-id="239eb-140">Coleção [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="239eb-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="239eb-141">Coleção de itens que representa uma opção de configuração nomeada no esquema</span><span class="sxs-lookup"><span data-stu-id="239eb-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="239eb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="239eb-142">Response</span></span>
<span data-ttu-id="239eb-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="239eb-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239eb-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="239eb-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="239eb-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="239eb-145">Request</span></span>
<span data-ttu-id="239eb-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="239eb-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="239eb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="239eb-147">Response</span></span>
<span data-ttu-id="239eb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="239eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





