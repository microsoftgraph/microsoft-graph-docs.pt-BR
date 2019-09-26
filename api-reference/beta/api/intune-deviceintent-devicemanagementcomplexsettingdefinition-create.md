---
title: Criar deviceManagementComplexSettingDefinition
description: Criar um novo objeto deviceManagementComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e2a758cc7f5892ecf8f02f3e85cf26260b9870d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181102"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="eef69-103">Criar deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="eef69-103">Create deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="eef69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eef69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eef69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eef69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef69-106">Criar um novo objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="eef69-106">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eef69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eef69-107">Prerequisites</span></span>
<span data-ttu-id="eef69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eef69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eef69-110">Permission type</span></span>|<span data-ttu-id="eef69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eef69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eef69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eef69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eef69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eef69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eef69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eef69-115">Not supported.</span></span>|
|<span data-ttu-id="eef69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eef69-116">Application</span></span>|<span data-ttu-id="eef69-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef69-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eef69-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="eef69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eef69-119">Request headers</span></span>
|<span data-ttu-id="eef69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eef69-120">Header</span></span>|<span data-ttu-id="eef69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eef69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eef69-122">Authorization</span></span>|<span data-ttu-id="eef69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eef69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eef69-124">Accept</span></span>|<span data-ttu-id="eef69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eef69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eef69-126">Request body</span></span>
<span data-ttu-id="eef69-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="eef69-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="eef69-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="eef69-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="eef69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eef69-129">Property</span></span>|<span data-ttu-id="eef69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eef69-130">Type</span></span>|<span data-ttu-id="eef69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eef69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef69-132">id</span><span class="sxs-lookup"><span data-stu-id="eef69-132">id</span></span>|<span data-ttu-id="eef69-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eef69-133">String</span></span>|<span data-ttu-id="eef69-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-135">valueType</span><span class="sxs-lookup"><span data-stu-id="eef69-135">valueType</span></span>|[<span data-ttu-id="eef69-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="eef69-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="eef69-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eef69-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="eef69-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="eef69-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="eef69-139">displayName</span><span class="sxs-lookup"><span data-stu-id="eef69-139">displayName</span></span>|<span data-ttu-id="eef69-140">String</span><span class="sxs-lookup"><span data-stu-id="eef69-140">String</span></span>|<span data-ttu-id="eef69-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="eef69-142">isTopLevel</span></span>|<span data-ttu-id="eef69-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="eef69-143">Boolean</span></span>|<span data-ttu-id="eef69-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-145">descrição</span><span class="sxs-lookup"><span data-stu-id="eef69-145">description</span></span>|<span data-ttu-id="eef69-146">String</span><span class="sxs-lookup"><span data-stu-id="eef69-146">String</span></span>|<span data-ttu-id="eef69-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="eef69-148">documentationUrl</span></span>|<span data-ttu-id="eef69-149">String</span><span class="sxs-lookup"><span data-stu-id="eef69-149">String</span></span>|<span data-ttu-id="eef69-150">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="eef69-151">keywords</span></span>|<span data-ttu-id="eef69-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eef69-152">String collection</span></span>|<span data-ttu-id="eef69-153">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-154">as</span><span class="sxs-lookup"><span data-stu-id="eef69-154">constraints</span></span>|<span data-ttu-id="eef69-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="eef69-156">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-157">relação</span><span class="sxs-lookup"><span data-stu-id="eef69-157">dependencies</span></span>|<span data-ttu-id="eef69-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="eef69-159">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eef69-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="eef69-160">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="eef69-160">propertyDefinitionIds</span></span>|<span data-ttu-id="eef69-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eef69-161">String collection</span></span>|<span data-ttu-id="eef69-162">As definições de cada propriedade da configuração complexa</span><span class="sxs-lookup"><span data-stu-id="eef69-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="eef69-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef69-163">Response</span></span>
<span data-ttu-id="eef69-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eef69-164">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef69-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eef69-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="eef69-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eef69-166">Request</span></span>
<span data-ttu-id="eef69-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eef69-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="eef69-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="eef69-168">Response</span></span>
<span data-ttu-id="eef69-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eef69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




