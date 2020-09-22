---
title: Criar deviceManagementComplexSettingDefinition
description: Criar um novo objeto deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f067d4e5b846a3e10f88014da1b1894effc4bff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040865"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="f6303-103">Criar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="f6303-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="f6303-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6303-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6303-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6303-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6303-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6303-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6303-107">Criar um novo objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f6303-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6303-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6303-108">Prerequisites</span></span>
<span data-ttu-id="f6303-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6303-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6303-111">Permission type</span></span>|<span data-ttu-id="f6303-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6303-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6303-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6303-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6303-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6303-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6303-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6303-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6303-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6303-116">Not supported.</span></span>|
|<span data-ttu-id="f6303-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6303-117">Application</span></span>|<span data-ttu-id="f6303-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6303-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6303-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6303-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/settingDefinitions
POST /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="f6303-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6303-120">Request headers</span></span>
|<span data-ttu-id="f6303-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6303-121">Header</span></span>|<span data-ttu-id="f6303-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6303-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6303-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6303-123">Authorization</span></span>|<span data-ttu-id="f6303-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6303-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6303-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6303-125">Accept</span></span>|<span data-ttu-id="f6303-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6303-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6303-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6303-127">Request body</span></span>
<span data-ttu-id="f6303-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="f6303-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="f6303-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="f6303-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="f6303-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6303-130">Property</span></span>|<span data-ttu-id="f6303-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6303-131">Type</span></span>|<span data-ttu-id="f6303-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6303-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6303-133">id</span><span class="sxs-lookup"><span data-stu-id="f6303-133">id</span></span>|<span data-ttu-id="f6303-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-134">String</span></span>|<span data-ttu-id="f6303-135">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-136">valueType</span><span class="sxs-lookup"><span data-stu-id="f6303-136">valueType</span></span>|[<span data-ttu-id="f6303-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="f6303-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="f6303-138">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f6303-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="f6303-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="f6303-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="f6303-140">displayName</span><span class="sxs-lookup"><span data-stu-id="f6303-140">displayName</span></span>|<span data-ttu-id="f6303-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-141">String</span></span>|<span data-ttu-id="f6303-142">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="f6303-143">isTopLevel</span></span>|<span data-ttu-id="f6303-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6303-144">Boolean</span></span>|<span data-ttu-id="f6303-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-146">description</span><span class="sxs-lookup"><span data-stu-id="f6303-146">description</span></span>|<span data-ttu-id="f6303-147">String</span><span class="sxs-lookup"><span data-stu-id="f6303-147">String</span></span>|<span data-ttu-id="f6303-148">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="f6303-149">placeholderText</span></span>|<span data-ttu-id="f6303-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-150">String</span></span>|<span data-ttu-id="f6303-151">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="f6303-152">documentationUrl</span></span>|<span data-ttu-id="f6303-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-153">String</span></span>|<span data-ttu-id="f6303-154">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="f6303-155">keywords</span></span>|<span data-ttu-id="f6303-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-156">String collection</span></span>|<span data-ttu-id="f6303-157">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-158">as</span><span class="sxs-lookup"><span data-stu-id="f6303-158">constraints</span></span>|<span data-ttu-id="f6303-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="f6303-160">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-161">relação</span><span class="sxs-lookup"><span data-stu-id="f6303-161">dependencies</span></span>|<span data-ttu-id="f6303-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="f6303-163">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f6303-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="f6303-164">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="f6303-164">propertyDefinitionIds</span></span>|<span data-ttu-id="f6303-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6303-165">String collection</span></span>|<span data-ttu-id="f6303-166">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="f6303-166">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="f6303-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6303-167">Response</span></span>
<span data-ttu-id="f6303-168">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6303-168">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6303-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6303-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6303-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6303-170">Request</span></span>
<span data-ttu-id="f6303-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6303-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1008

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
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
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f6303-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6303-172">Response</span></span>
<span data-ttu-id="f6303-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6303-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1057

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
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
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```






