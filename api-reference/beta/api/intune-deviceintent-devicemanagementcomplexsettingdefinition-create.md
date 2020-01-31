---
title: Criar deviceManagementComplexSettingDefinition
description: Criar um novo objeto deviceManagementComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2217c21a111d1668d225183ec2db4163cc4dc8cd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636424"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="e474f-103">Criar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e474f-103">Create deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="e474f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e474f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e474f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e474f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e474f-106">Criar um novo objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e474f-106">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e474f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e474f-107">Prerequisites</span></span>
<span data-ttu-id="e474f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e474f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e474f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e474f-110">Permission type</span></span>|<span data-ttu-id="e474f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e474f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e474f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e474f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e474f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e474f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e474f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e474f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e474f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e474f-115">Not supported.</span></span>|
|<span data-ttu-id="e474f-116">Application</span><span class="sxs-lookup"><span data-stu-id="e474f-116">Application</span></span>|<span data-ttu-id="e474f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e474f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e474f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e474f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e474f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e474f-119">Request headers</span></span>
|<span data-ttu-id="e474f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e474f-120">Header</span></span>|<span data-ttu-id="e474f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e474f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e474f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e474f-122">Authorization</span></span>|<span data-ttu-id="e474f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e474f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e474f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e474f-124">Accept</span></span>|<span data-ttu-id="e474f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e474f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e474f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e474f-126">Request body</span></span>
<span data-ttu-id="e474f-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="e474f-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="e474f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="e474f-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="e474f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e474f-129">Property</span></span>|<span data-ttu-id="e474f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e474f-130">Type</span></span>|<span data-ttu-id="e474f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e474f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e474f-132">id</span><span class="sxs-lookup"><span data-stu-id="e474f-132">id</span></span>|<span data-ttu-id="e474f-133">String</span><span class="sxs-lookup"><span data-stu-id="e474f-133">String</span></span>|<span data-ttu-id="e474f-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-135">valueType</span><span class="sxs-lookup"><span data-stu-id="e474f-135">valueType</span></span>|[<span data-ttu-id="e474f-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="e474f-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="e474f-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e474f-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="e474f-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="e474f-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="e474f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e474f-139">displayName</span></span>|<span data-ttu-id="e474f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e474f-140">String</span></span>|<span data-ttu-id="e474f-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="e474f-142">isTopLevel</span></span>|<span data-ttu-id="e474f-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="e474f-143">Boolean</span></span>|<span data-ttu-id="e474f-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-145">description</span><span class="sxs-lookup"><span data-stu-id="e474f-145">description</span></span>|<span data-ttu-id="e474f-146">String</span><span class="sxs-lookup"><span data-stu-id="e474f-146">String</span></span>|<span data-ttu-id="e474f-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="e474f-148">placeholderText</span></span>|<span data-ttu-id="e474f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e474f-149">String</span></span>|<span data-ttu-id="e474f-150">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="e474f-151">documentationUrl</span></span>|<span data-ttu-id="e474f-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e474f-152">String</span></span>|<span data-ttu-id="e474f-153">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="e474f-154">keywords</span></span>|<span data-ttu-id="e474f-155">String collection</span><span class="sxs-lookup"><span data-stu-id="e474f-155">String collection</span></span>|<span data-ttu-id="e474f-156">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-157">as</span><span class="sxs-lookup"><span data-stu-id="e474f-157">constraints</span></span>|<span data-ttu-id="e474f-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e474f-159">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-160">relação</span><span class="sxs-lookup"><span data-stu-id="e474f-160">dependencies</span></span>|<span data-ttu-id="e474f-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="e474f-162">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e474f-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e474f-163">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="e474f-163">propertyDefinitionIds</span></span>|<span data-ttu-id="e474f-164">String collection</span><span class="sxs-lookup"><span data-stu-id="e474f-164">String collection</span></span>|<span data-ttu-id="e474f-165">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="e474f-165">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="e474f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e474f-166">Response</span></span>
<span data-ttu-id="e474f-167">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e474f-167">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e474f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e474f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="e474f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e474f-169">Request</span></span>
<span data-ttu-id="e474f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e474f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e474f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e474f-171">Response</span></span>
<span data-ttu-id="e474f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e474f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





