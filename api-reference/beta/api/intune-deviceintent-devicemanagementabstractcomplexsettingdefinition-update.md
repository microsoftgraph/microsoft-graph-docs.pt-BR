---
title: Atualizar deviceManagementAbstractComplexSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementAbstractComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f0eb96e5da1c73714dd28dac71a282dd5240e69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472986"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="11336-103">Atualizar deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="11336-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="11336-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11336-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11336-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11336-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11336-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11336-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11336-107">Atualiza as propriedades de um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="11336-107">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11336-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11336-108">Prerequisites</span></span>
<span data-ttu-id="11336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11336-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11336-111">Permission type</span></span>|<span data-ttu-id="11336-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11336-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11336-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11336-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11336-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11336-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11336-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11336-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11336-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11336-116">Not supported.</span></span>|
|<span data-ttu-id="11336-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11336-117">Application</span></span>|<span data-ttu-id="11336-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11336-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11336-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11336-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="11336-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11336-120">Request headers</span></span>
|<span data-ttu-id="11336-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11336-121">Header</span></span>|<span data-ttu-id="11336-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11336-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11336-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11336-123">Authorization</span></span>|<span data-ttu-id="11336-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11336-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11336-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11336-125">Accept</span></span>|<span data-ttu-id="11336-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11336-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11336-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11336-127">Request body</span></span>
<span data-ttu-id="11336-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="11336-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="11336-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11336-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="11336-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11336-130">Property</span></span>|<span data-ttu-id="11336-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11336-131">Type</span></span>|<span data-ttu-id="11336-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11336-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11336-133">id</span><span class="sxs-lookup"><span data-stu-id="11336-133">id</span></span>|<span data-ttu-id="11336-134">String</span><span class="sxs-lookup"><span data-stu-id="11336-134">String</span></span>|<span data-ttu-id="11336-135">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-136">valueType</span><span class="sxs-lookup"><span data-stu-id="11336-136">valueType</span></span>|[<span data-ttu-id="11336-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="11336-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="11336-138">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11336-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="11336-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="11336-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="11336-140">displayName</span><span class="sxs-lookup"><span data-stu-id="11336-140">displayName</span></span>|<span data-ttu-id="11336-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11336-141">String</span></span>|<span data-ttu-id="11336-142">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="11336-143">isTopLevel</span></span>|<span data-ttu-id="11336-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="11336-144">Boolean</span></span>|<span data-ttu-id="11336-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-146">description</span><span class="sxs-lookup"><span data-stu-id="11336-146">description</span></span>|<span data-ttu-id="11336-147">String</span><span class="sxs-lookup"><span data-stu-id="11336-147">String</span></span>|<span data-ttu-id="11336-148">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="11336-149">placeholderText</span></span>|<span data-ttu-id="11336-150">String</span><span class="sxs-lookup"><span data-stu-id="11336-150">String</span></span>|<span data-ttu-id="11336-151">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="11336-152">documentationUrl</span></span>|<span data-ttu-id="11336-153">String</span><span class="sxs-lookup"><span data-stu-id="11336-153">String</span></span>|<span data-ttu-id="11336-154">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="11336-155">keywords</span></span>|<span data-ttu-id="11336-156">String collection</span><span class="sxs-lookup"><span data-stu-id="11336-156">String collection</span></span>|<span data-ttu-id="11336-157">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-158">as</span><span class="sxs-lookup"><span data-stu-id="11336-158">constraints</span></span>|<span data-ttu-id="11336-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="11336-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="11336-160">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-161">relação</span><span class="sxs-lookup"><span data-stu-id="11336-161">dependencies</span></span>|<span data-ttu-id="11336-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="11336-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="11336-163">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11336-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="11336-164">implementações</span><span class="sxs-lookup"><span data-stu-id="11336-164">implementations</span></span>|<span data-ttu-id="11336-165">String collection</span><span class="sxs-lookup"><span data-stu-id="11336-165">String collection</span></span>|<span data-ttu-id="11336-166">Lista de IDs de definição para todas as implementações possíveis dessa configuração complexa abstrata</span><span class="sxs-lookup"><span data-stu-id="11336-166">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="11336-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="11336-167">Response</span></span>
<span data-ttu-id="11336-168">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11336-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11336-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11336-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="11336-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11336-170">Request</span></span>
<span data-ttu-id="11336-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11336-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="11336-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="11336-172">Response</span></span>
<span data-ttu-id="11336-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11336-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "implementations": [
    "Implementations value"
  ]
}
```





