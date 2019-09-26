---
title: Atualizar deviceManagementAbstractComplexSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementAbstractComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6454da2e051cb068c3f0f66f5889bddff6a0e2c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181256"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="b3836-103">Atualizar deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="b3836-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="b3836-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3836-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3836-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3836-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3836-106">Atualiza as propriedades de um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b3836-106">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3836-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3836-107">Prerequisites</span></span>
<span data-ttu-id="b3836-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3836-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3836-110">Permission type</span></span>|<span data-ttu-id="b3836-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3836-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3836-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3836-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3836-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3836-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3836-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3836-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3836-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3836-115">Not supported.</span></span>|
|<span data-ttu-id="b3836-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3836-116">Application</span></span>|<span data-ttu-id="b3836-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3836-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3836-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3836-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b3836-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3836-119">Request headers</span></span>
|<span data-ttu-id="b3836-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3836-120">Header</span></span>|<span data-ttu-id="b3836-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3836-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3836-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3836-122">Authorization</span></span>|<span data-ttu-id="b3836-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3836-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3836-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3836-124">Accept</span></span>|<span data-ttu-id="b3836-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3836-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3836-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3836-126">Request body</span></span>
<span data-ttu-id="b3836-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b3836-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="b3836-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b3836-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="b3836-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3836-129">Property</span></span>|<span data-ttu-id="b3836-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3836-130">Type</span></span>|<span data-ttu-id="b3836-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3836-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3836-132">id</span><span class="sxs-lookup"><span data-stu-id="b3836-132">id</span></span>|<span data-ttu-id="b3836-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3836-133">String</span></span>|<span data-ttu-id="b3836-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-135">valueType</span><span class="sxs-lookup"><span data-stu-id="b3836-135">valueType</span></span>|[<span data-ttu-id="b3836-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="b3836-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="b3836-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b3836-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="b3836-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="b3836-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="b3836-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b3836-139">displayName</span></span>|<span data-ttu-id="b3836-140">String</span><span class="sxs-lookup"><span data-stu-id="b3836-140">String</span></span>|<span data-ttu-id="b3836-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="b3836-142">isTopLevel</span></span>|<span data-ttu-id="b3836-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3836-143">Boolean</span></span>|<span data-ttu-id="b3836-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-145">descrição</span><span class="sxs-lookup"><span data-stu-id="b3836-145">description</span></span>|<span data-ttu-id="b3836-146">String</span><span class="sxs-lookup"><span data-stu-id="b3836-146">String</span></span>|<span data-ttu-id="b3836-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="b3836-148">documentationUrl</span></span>|<span data-ttu-id="b3836-149">String</span><span class="sxs-lookup"><span data-stu-id="b3836-149">String</span></span>|<span data-ttu-id="b3836-150">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="b3836-151">keywords</span></span>|<span data-ttu-id="b3836-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3836-152">String collection</span></span>|<span data-ttu-id="b3836-153">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-154">as</span><span class="sxs-lookup"><span data-stu-id="b3836-154">constraints</span></span>|<span data-ttu-id="b3836-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="b3836-156">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-157">relação</span><span class="sxs-lookup"><span data-stu-id="b3836-157">dependencies</span></span>|<span data-ttu-id="b3836-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="b3836-159">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b3836-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b3836-160">implementações</span><span class="sxs-lookup"><span data-stu-id="b3836-160">implementations</span></span>|<span data-ttu-id="b3836-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3836-161">String collection</span></span>|<span data-ttu-id="b3836-162">Lista de IDs de definição para todas as implementações possíveis dessa configuração complexa abstrata</span><span class="sxs-lookup"><span data-stu-id="b3836-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="b3836-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3836-163">Response</span></span>
<span data-ttu-id="b3836-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3836-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3836-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3836-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3836-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3836-166">Request</span></span>
<span data-ttu-id="b3836-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3836-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 802

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b3836-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3836-168">Response</span></span>
<span data-ttu-id="b3836-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3836-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 851

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




