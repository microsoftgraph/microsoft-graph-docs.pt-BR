---
title: Criar deviceManagementAbstractComplexSettingDefinition
description: Criar um novo objeto deviceManagementAbstractComplexSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4505d0e672d55ef42ba2aa5633e997f196c95f1e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946263"
---
# <a name="create-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="4a808-103">Criar deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="4a808-103">Create deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="4a808-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a808-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a808-106">Criar um novo objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="4a808-106">Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a808-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a808-107">Prerequisites</span></span>
<span data-ttu-id="4a808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a808-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a808-110">Permission type</span></span>|<span data-ttu-id="4a808-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a808-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a808-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a808-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a808-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a808-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a808-115">Not supported.</span></span>|
|<span data-ttu-id="4a808-116">Application</span><span class="sxs-lookup"><span data-stu-id="4a808-116">Application</span></span>|<span data-ttu-id="4a808-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a808-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a808-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a808-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4a808-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a808-119">Request headers</span></span>
|<span data-ttu-id="4a808-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a808-120">Header</span></span>|<span data-ttu-id="4a808-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4a808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a808-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a808-122">Authorization</span></span>|<span data-ttu-id="4a808-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a808-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a808-124">Accept</span></span>|<span data-ttu-id="4a808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a808-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a808-126">Request body</span></span>
<span data-ttu-id="4a808-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAbstractComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="4a808-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingDefinition object.</span></span>

<span data-ttu-id="4a808-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAbstractComplexSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="4a808-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingDefinition.</span></span>

|<span data-ttu-id="4a808-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a808-129">Property</span></span>|<span data-ttu-id="4a808-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a808-130">Type</span></span>|<span data-ttu-id="4a808-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a808-132">id</span><span class="sxs-lookup"><span data-stu-id="4a808-132">id</span></span>|<span data-ttu-id="4a808-133">String</span><span class="sxs-lookup"><span data-stu-id="4a808-133">String</span></span>|<span data-ttu-id="4a808-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-135">valueType</span><span class="sxs-lookup"><span data-stu-id="4a808-135">valueType</span></span>|[<span data-ttu-id="4a808-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="4a808-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="4a808-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4a808-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="4a808-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="4a808-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="4a808-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4a808-139">displayName</span></span>|<span data-ttu-id="4a808-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a808-140">String</span></span>|<span data-ttu-id="4a808-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="4a808-142">isTopLevel</span></span>|<span data-ttu-id="4a808-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a808-143">Boolean</span></span>|<span data-ttu-id="4a808-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-145">description</span><span class="sxs-lookup"><span data-stu-id="4a808-145">description</span></span>|<span data-ttu-id="4a808-146">String</span><span class="sxs-lookup"><span data-stu-id="4a808-146">String</span></span>|<span data-ttu-id="4a808-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="4a808-148">documentationUrl</span></span>|<span data-ttu-id="4a808-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4a808-149">String</span></span>|<span data-ttu-id="4a808-150">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="4a808-151">keywords</span></span>|<span data-ttu-id="4a808-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a808-152">String collection</span></span>|<span data-ttu-id="4a808-153">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-154">as</span><span class="sxs-lookup"><span data-stu-id="4a808-154">constraints</span></span>|<span data-ttu-id="4a808-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="4a808-156">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-157">relação</span><span class="sxs-lookup"><span data-stu-id="4a808-157">dependencies</span></span>|<span data-ttu-id="4a808-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="4a808-159">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4a808-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="4a808-160">implementações</span><span class="sxs-lookup"><span data-stu-id="4a808-160">implementations</span></span>|<span data-ttu-id="4a808-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a808-161">String collection</span></span>|<span data-ttu-id="4a808-162">Lista de IDs de definição para todas as implementações possíveis dessa configuração complexa abstrata</span><span class="sxs-lookup"><span data-stu-id="4a808-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="4a808-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a808-163">Response</span></span>
<span data-ttu-id="4a808-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a808-164">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a808-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a808-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a808-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a808-166">Request</span></span>
<span data-ttu-id="4a808-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a808-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="4a808-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a808-168">Response</span></span>
<span data-ttu-id="4a808-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a808-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





