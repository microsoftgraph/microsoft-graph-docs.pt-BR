---
title: Atualizar deviceManagementComplexSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementComplexSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a8bfc2181bb2e6f7585e48c412a789b118fe95f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428208"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="24cde-103">Atualizar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="24cde-103">Update deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="24cde-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24cde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24cde-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24cde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24cde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24cde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cde-107">Atualiza as propriedades de um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="24cde-107">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24cde-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24cde-108">Prerequisites</span></span>
<span data-ttu-id="24cde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cde-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24cde-111">Permission type</span></span>|<span data-ttu-id="24cde-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24cde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24cde-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24cde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24cde-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cde-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24cde-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24cde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24cde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24cde-116">Not supported.</span></span>|
|<span data-ttu-id="24cde-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24cde-117">Application</span></span>|<span data-ttu-id="24cde-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cde-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24cde-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24cde-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="24cde-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24cde-120">Request headers</span></span>
|<span data-ttu-id="24cde-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24cde-121">Header</span></span>|<span data-ttu-id="24cde-122">Valor</span><span class="sxs-lookup"><span data-stu-id="24cde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24cde-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24cde-123">Authorization</span></span>|<span data-ttu-id="24cde-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24cde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24cde-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24cde-125">Accept</span></span>|<span data-ttu-id="24cde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24cde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24cde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24cde-127">Request body</span></span>
<span data-ttu-id="24cde-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="24cde-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="24cde-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="24cde-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="24cde-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24cde-130">Property</span></span>|<span data-ttu-id="24cde-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="24cde-131">Type</span></span>|<span data-ttu-id="24cde-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="24cde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24cde-133">id</span><span class="sxs-lookup"><span data-stu-id="24cde-133">id</span></span>|<span data-ttu-id="24cde-134">String</span><span class="sxs-lookup"><span data-stu-id="24cde-134">String</span></span>|<span data-ttu-id="24cde-135">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-136">valueType</span><span class="sxs-lookup"><span data-stu-id="24cde-136">valueType</span></span>|[<span data-ttu-id="24cde-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="24cde-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="24cde-138">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="24cde-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="24cde-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="24cde-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="24cde-140">displayName</span><span class="sxs-lookup"><span data-stu-id="24cde-140">displayName</span></span>|<span data-ttu-id="24cde-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24cde-141">String</span></span>|<span data-ttu-id="24cde-142">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="24cde-143">isTopLevel</span></span>|<span data-ttu-id="24cde-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="24cde-144">Boolean</span></span>|<span data-ttu-id="24cde-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-146">description</span><span class="sxs-lookup"><span data-stu-id="24cde-146">description</span></span>|<span data-ttu-id="24cde-147">String</span><span class="sxs-lookup"><span data-stu-id="24cde-147">String</span></span>|<span data-ttu-id="24cde-148">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="24cde-149">placeholderText</span></span>|<span data-ttu-id="24cde-150">String</span><span class="sxs-lookup"><span data-stu-id="24cde-150">String</span></span>|<span data-ttu-id="24cde-151">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="24cde-152">documentationUrl</span></span>|<span data-ttu-id="24cde-153">String</span><span class="sxs-lookup"><span data-stu-id="24cde-153">String</span></span>|<span data-ttu-id="24cde-154">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="24cde-155">keywords</span></span>|<span data-ttu-id="24cde-156">Coleção String</span><span class="sxs-lookup"><span data-stu-id="24cde-156">String collection</span></span>|<span data-ttu-id="24cde-157">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-158">as</span><span class="sxs-lookup"><span data-stu-id="24cde-158">constraints</span></span>|<span data-ttu-id="24cde-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="24cde-160">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-161">relação</span><span class="sxs-lookup"><span data-stu-id="24cde-161">dependencies</span></span>|<span data-ttu-id="24cde-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="24cde-163">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24cde-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="24cde-164">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="24cde-164">propertyDefinitionIds</span></span>|<span data-ttu-id="24cde-165">Coleção String</span><span class="sxs-lookup"><span data-stu-id="24cde-165">String collection</span></span>|<span data-ttu-id="24cde-166">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="24cde-166">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="24cde-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="24cde-167">Response</span></span>
<span data-ttu-id="24cde-168">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24cde-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24cde-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24cde-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="24cde-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24cde-170">Request</span></span>
<span data-ttu-id="24cde-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24cde-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24cde-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="24cde-172">Response</span></span>
<span data-ttu-id="24cde-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24cde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



