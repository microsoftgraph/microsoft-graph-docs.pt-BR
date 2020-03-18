---
title: Atualizar deviceManagementComplexSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementComplexSettingDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac2d8e047a59012f6c62674d97a50451bf7b2909
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730106"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="5daa6-103">Atualizar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="5daa6-103">Update deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="5daa6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5daa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5daa6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5daa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5daa6-106">Atualiza as propriedades de um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="5daa6-106">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5daa6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5daa6-107">Prerequisites</span></span>
<span data-ttu-id="5daa6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5daa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5daa6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5daa6-110">Permission type</span></span>|<span data-ttu-id="5daa6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5daa6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5daa6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5daa6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5daa6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5daa6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5daa6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5daa6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5daa6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5daa6-115">Not supported.</span></span>|
|<span data-ttu-id="5daa6-116">Application</span><span class="sxs-lookup"><span data-stu-id="5daa6-116">Application</span></span>|<span data-ttu-id="5daa6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5daa6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5daa6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5daa6-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5daa6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5daa6-119">Request headers</span></span>
|<span data-ttu-id="5daa6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5daa6-120">Header</span></span>|<span data-ttu-id="5daa6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5daa6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5daa6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5daa6-122">Authorization</span></span>|<span data-ttu-id="5daa6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5daa6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5daa6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5daa6-124">Accept</span></span>|<span data-ttu-id="5daa6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5daa6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5daa6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5daa6-126">Request body</span></span>
<span data-ttu-id="5daa6-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="5daa6-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="5daa6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5daa6-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="5daa6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5daa6-129">Property</span></span>|<span data-ttu-id="5daa6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5daa6-130">Type</span></span>|<span data-ttu-id="5daa6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5daa6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5daa6-132">id</span><span class="sxs-lookup"><span data-stu-id="5daa6-132">id</span></span>|<span data-ttu-id="5daa6-133">String</span><span class="sxs-lookup"><span data-stu-id="5daa6-133">String</span></span>|<span data-ttu-id="5daa6-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-135">valueType</span><span class="sxs-lookup"><span data-stu-id="5daa6-135">valueType</span></span>|[<span data-ttu-id="5daa6-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="5daa6-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="5daa6-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5daa6-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="5daa6-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="5daa6-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="5daa6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5daa6-139">displayName</span></span>|<span data-ttu-id="5daa6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5daa6-140">String</span></span>|<span data-ttu-id="5daa6-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="5daa6-142">isTopLevel</span></span>|<span data-ttu-id="5daa6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5daa6-143">Boolean</span></span>|<span data-ttu-id="5daa6-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-145">description</span><span class="sxs-lookup"><span data-stu-id="5daa6-145">description</span></span>|<span data-ttu-id="5daa6-146">String</span><span class="sxs-lookup"><span data-stu-id="5daa6-146">String</span></span>|<span data-ttu-id="5daa6-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="5daa6-148">placeholderText</span></span>|<span data-ttu-id="5daa6-149">String</span><span class="sxs-lookup"><span data-stu-id="5daa6-149">String</span></span>|<span data-ttu-id="5daa6-150">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="5daa6-151">documentationUrl</span></span>|<span data-ttu-id="5daa6-152">String</span><span class="sxs-lookup"><span data-stu-id="5daa6-152">String</span></span>|<span data-ttu-id="5daa6-153">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="5daa6-154">keywords</span></span>|<span data-ttu-id="5daa6-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5daa6-155">String collection</span></span>|<span data-ttu-id="5daa6-156">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-157">as</span><span class="sxs-lookup"><span data-stu-id="5daa6-157">constraints</span></span>|<span data-ttu-id="5daa6-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="5daa6-159">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-160">relação</span><span class="sxs-lookup"><span data-stu-id="5daa6-160">dependencies</span></span>|<span data-ttu-id="5daa6-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="5daa6-162">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5daa6-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5daa6-163">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="5daa6-163">propertyDefinitionIds</span></span>|<span data-ttu-id="5daa6-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5daa6-164">String collection</span></span>|<span data-ttu-id="5daa6-165">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="5daa6-165">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="5daa6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5daa6-166">Response</span></span>
<span data-ttu-id="5daa6-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5daa6-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5daa6-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5daa6-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5daa6-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5daa6-169">Request</span></span>
<span data-ttu-id="5daa6-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5daa6-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="5daa6-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5daa6-171">Response</span></span>
<span data-ttu-id="5daa6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5daa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




