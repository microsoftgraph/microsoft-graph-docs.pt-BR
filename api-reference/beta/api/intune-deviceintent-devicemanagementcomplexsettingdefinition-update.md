---
title: Atualizar deviceManagementComplexSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementComplexSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9084ba536f4911ce5d2e5d31e9cfa3cbce3d759
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771132"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="bfa60-103">Atualizar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="bfa60-103">Update deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="bfa60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bfa60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfa60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bfa60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa60-106">Atualiza as propriedades de um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="bfa60-106">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfa60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bfa60-107">Prerequisites</span></span>
<span data-ttu-id="bfa60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfa60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfa60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfa60-110">Permission type</span></span>|<span data-ttu-id="bfa60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bfa60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfa60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfa60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bfa60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfa60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfa60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfa60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfa60-115">Not supported.</span></span>|
|<span data-ttu-id="bfa60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfa60-116">Application</span></span>|<span data-ttu-id="bfa60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfa60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfa60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfa60-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bfa60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfa60-119">Request headers</span></span>
|<span data-ttu-id="bfa60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bfa60-120">Header</span></span>|<span data-ttu-id="bfa60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bfa60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfa60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfa60-122">Authorization</span></span>|<span data-ttu-id="bfa60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfa60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfa60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bfa60-124">Accept</span></span>|<span data-ttu-id="bfa60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bfa60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfa60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfa60-126">Request body</span></span>
<span data-ttu-id="bfa60-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="bfa60-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="bfa60-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="bfa60-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="bfa60-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfa60-129">Property</span></span>|<span data-ttu-id="bfa60-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfa60-130">Type</span></span>|<span data-ttu-id="bfa60-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfa60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa60-132">id</span><span class="sxs-lookup"><span data-stu-id="bfa60-132">id</span></span>|<span data-ttu-id="bfa60-133">String</span><span class="sxs-lookup"><span data-stu-id="bfa60-133">String</span></span>|<span data-ttu-id="bfa60-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-135">valueType</span><span class="sxs-lookup"><span data-stu-id="bfa60-135">valueType</span></span>|[<span data-ttu-id="bfa60-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="bfa60-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="bfa60-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="bfa60-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="bfa60-138">Os valores possíveis são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="bfa60-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="bfa60-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bfa60-139">displayName</span></span>|<span data-ttu-id="bfa60-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfa60-140">String</span></span>|<span data-ttu-id="bfa60-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="bfa60-142">isTopLevel</span></span>|<span data-ttu-id="bfa60-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="bfa60-143">Boolean</span></span>|<span data-ttu-id="bfa60-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-145">description</span><span class="sxs-lookup"><span data-stu-id="bfa60-145">description</span></span>|<span data-ttu-id="bfa60-146">String</span><span class="sxs-lookup"><span data-stu-id="bfa60-146">String</span></span>|<span data-ttu-id="bfa60-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="bfa60-148">documentationUrl</span></span>|<span data-ttu-id="bfa60-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfa60-149">String</span></span>|<span data-ttu-id="bfa60-150">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="bfa60-151">keywords</span></span>|<span data-ttu-id="bfa60-152">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bfa60-152">String collection</span></span>|<span data-ttu-id="bfa60-153">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-154">as</span><span class="sxs-lookup"><span data-stu-id="bfa60-154">constraints</span></span>|<span data-ttu-id="bfa60-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="bfa60-156">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-157">relação</span><span class="sxs-lookup"><span data-stu-id="bfa60-157">dependencies</span></span>|<span data-ttu-id="bfa60-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="bfa60-159">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bfa60-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bfa60-160">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="bfa60-160">propertyDefinitionIds</span></span>|<span data-ttu-id="bfa60-161">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bfa60-161">String collection</span></span>|<span data-ttu-id="bfa60-162">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="bfa60-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="bfa60-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfa60-163">Response</span></span>
<span data-ttu-id="bfa60-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfa60-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfa60-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfa60-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfa60-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfa60-166">Request</span></span>
<span data-ttu-id="bfa60-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfa60-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 808

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="bfa60-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfa60-168">Response</span></span>
<span data-ttu-id="bfa60-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfa60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```





