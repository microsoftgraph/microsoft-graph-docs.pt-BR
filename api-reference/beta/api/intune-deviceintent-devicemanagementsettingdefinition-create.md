---
title: Criar deviceManagementSettingDefinition
description: Criar um novo objeto deviceManagementSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b818d2acdae8f3388c5f70fc16f921feb87c67e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636004"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="aec5b-103">Criar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="aec5b-103">Create deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="aec5b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aec5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aec5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec5b-106">Criar um novo objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="aec5b-106">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aec5b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aec5b-107">Prerequisites</span></span>
<span data-ttu-id="aec5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec5b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aec5b-110">Permission type</span></span>|<span data-ttu-id="aec5b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aec5b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec5b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aec5b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aec5b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec5b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aec5b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aec5b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec5b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aec5b-115">Not supported.</span></span>|
|<span data-ttu-id="aec5b-116">Application</span><span class="sxs-lookup"><span data-stu-id="aec5b-116">Application</span></span>|<span data-ttu-id="aec5b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec5b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aec5b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aec5b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="aec5b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aec5b-119">Request headers</span></span>
|<span data-ttu-id="aec5b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aec5b-120">Header</span></span>|<span data-ttu-id="aec5b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aec5b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aec5b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aec5b-122">Authorization</span></span>|<span data-ttu-id="aec5b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aec5b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aec5b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aec5b-124">Accept</span></span>|<span data-ttu-id="aec5b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aec5b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec5b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aec5b-126">Request body</span></span>
<span data-ttu-id="aec5b-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="aec5b-127">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="aec5b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="aec5b-128">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="aec5b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aec5b-129">Property</span></span>|<span data-ttu-id="aec5b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aec5b-130">Type</span></span>|<span data-ttu-id="aec5b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aec5b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec5b-132">id</span><span class="sxs-lookup"><span data-stu-id="aec5b-132">id</span></span>|<span data-ttu-id="aec5b-133">String</span><span class="sxs-lookup"><span data-stu-id="aec5b-133">String</span></span>|<span data-ttu-id="aec5b-134">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="aec5b-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="aec5b-135">valueType</span><span class="sxs-lookup"><span data-stu-id="aec5b-135">valueType</span></span>|[<span data-ttu-id="aec5b-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="aec5b-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="aec5b-137">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="aec5b-137">The data type of the value.</span></span> <span data-ttu-id="aec5b-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="aec5b-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="aec5b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="aec5b-139">displayName</span></span>|<span data-ttu-id="aec5b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aec5b-140">String</span></span>|<span data-ttu-id="aec5b-141">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="aec5b-141">The setting's display name</span></span>|
|<span data-ttu-id="aec5b-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="aec5b-142">isTopLevel</span></span>|<span data-ttu-id="aec5b-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="aec5b-143">Boolean</span></span>|<span data-ttu-id="aec5b-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="aec5b-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="aec5b-145">description</span><span class="sxs-lookup"><span data-stu-id="aec5b-145">description</span></span>|<span data-ttu-id="aec5b-146">String</span><span class="sxs-lookup"><span data-stu-id="aec5b-146">String</span></span>|<span data-ttu-id="aec5b-147">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="aec5b-147">The setting's description</span></span>|
|<span data-ttu-id="aec5b-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="aec5b-148">placeholderText</span></span>|<span data-ttu-id="aec5b-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aec5b-149">String</span></span>|<span data-ttu-id="aec5b-150">Texto do espaço reservado como um exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="aec5b-150">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="aec5b-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="aec5b-151">documentationUrl</span></span>|<span data-ttu-id="aec5b-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aec5b-152">String</span></span>|<span data-ttu-id="aec5b-153">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="aec5b-153">Url to setting documentation</span></span>|
|<span data-ttu-id="aec5b-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="aec5b-154">keywords</span></span>|<span data-ttu-id="aec5b-155">String collection</span><span class="sxs-lookup"><span data-stu-id="aec5b-155">String collection</span></span>|<span data-ttu-id="aec5b-156">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="aec5b-156">Keywords associated with the setting</span></span>|
|<span data-ttu-id="aec5b-157">as</span><span class="sxs-lookup"><span data-stu-id="aec5b-157">constraints</span></span>|<span data-ttu-id="aec5b-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="aec5b-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="aec5b-159">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="aec5b-159">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="aec5b-160">relação</span><span class="sxs-lookup"><span data-stu-id="aec5b-160">dependencies</span></span>|<span data-ttu-id="aec5b-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="aec5b-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="aec5b-162">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="aec5b-162">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="aec5b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec5b-163">Response</span></span>
<span data-ttu-id="aec5b-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aec5b-164">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aec5b-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aec5b-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="aec5b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec5b-166">Request</span></span>
<span data-ttu-id="aec5b-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aec5b-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="aec5b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec5b-168">Response</span></span>
<span data-ttu-id="aec5b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aec5b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```





