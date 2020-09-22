---
title: Criar deviceManagementSettingDefinition
description: Criar um novo objeto deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c92467d3ad05422da91e5da5eccaf1df3b2a709
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074675"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="f4f67-103">Criar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="f4f67-103">Create deviceManagementSettingDefinition</span></span>

<span data-ttu-id="f4f67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4f67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4f67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4f67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f67-107">Criar um novo objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f4f67-107">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4f67-108">Prerequisites</span></span>
<span data-ttu-id="f4f67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4f67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4f67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4f67-111">Permission type</span></span>|<span data-ttu-id="f4f67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4f67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4f67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4f67-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4f67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4f67-116">Not supported.</span></span>|
|<span data-ttu-id="f4f67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4f67-117">Application</span></span>|<span data-ttu-id="f4f67-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f67-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4f67-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f4f67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f67-120">Request headers</span></span>
|<span data-ttu-id="f4f67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4f67-121">Header</span></span>|<span data-ttu-id="f4f67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4f67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4f67-123">Authorization</span></span>|<span data-ttu-id="f4f67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4f67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4f67-125">Accept</span></span>|<span data-ttu-id="f4f67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f67-127">Request body</span></span>
<span data-ttu-id="f4f67-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="f4f67-128">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="f4f67-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="f4f67-129">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="f4f67-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4f67-130">Property</span></span>|<span data-ttu-id="f4f67-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4f67-131">Type</span></span>|<span data-ttu-id="f4f67-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4f67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f67-133">id</span><span class="sxs-lookup"><span data-stu-id="f4f67-133">id</span></span>|<span data-ttu-id="f4f67-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4f67-134">String</span></span>|<span data-ttu-id="f4f67-135">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="f4f67-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="f4f67-136">valueType</span><span class="sxs-lookup"><span data-stu-id="f4f67-136">valueType</span></span>|[<span data-ttu-id="f4f67-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="f4f67-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="f4f67-138">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="f4f67-138">The data type of the value.</span></span> <span data-ttu-id="f4f67-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="f4f67-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="f4f67-140">displayName</span><span class="sxs-lookup"><span data-stu-id="f4f67-140">displayName</span></span>|<span data-ttu-id="f4f67-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4f67-141">String</span></span>|<span data-ttu-id="f4f67-142">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="f4f67-142">The setting's display name</span></span>|
|<span data-ttu-id="f4f67-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="f4f67-143">isTopLevel</span></span>|<span data-ttu-id="f4f67-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4f67-144">Boolean</span></span>|<span data-ttu-id="f4f67-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="f4f67-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="f4f67-146">description</span><span class="sxs-lookup"><span data-stu-id="f4f67-146">description</span></span>|<span data-ttu-id="f4f67-147">String</span><span class="sxs-lookup"><span data-stu-id="f4f67-147">String</span></span>|<span data-ttu-id="f4f67-148">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="f4f67-148">The setting's description</span></span>|
|<span data-ttu-id="f4f67-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="f4f67-149">placeholderText</span></span>|<span data-ttu-id="f4f67-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4f67-150">String</span></span>|<span data-ttu-id="f4f67-151">Texto do espaço reservado como um exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="f4f67-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="f4f67-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="f4f67-152">documentationUrl</span></span>|<span data-ttu-id="f4f67-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4f67-153">String</span></span>|<span data-ttu-id="f4f67-154">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="f4f67-154">Url to setting documentation</span></span>|
|<span data-ttu-id="f4f67-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="f4f67-155">keywords</span></span>|<span data-ttu-id="f4f67-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4f67-156">String collection</span></span>|<span data-ttu-id="f4f67-157">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="f4f67-157">Keywords associated with the setting</span></span>|
|<span data-ttu-id="f4f67-158">as</span><span class="sxs-lookup"><span data-stu-id="f4f67-158">constraints</span></span>|<span data-ttu-id="f4f67-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f4f67-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="f4f67-160">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="f4f67-160">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="f4f67-161">relação</span><span class="sxs-lookup"><span data-stu-id="f4f67-161">dependencies</span></span>|<span data-ttu-id="f4f67-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="f4f67-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="f4f67-163">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="f4f67-163">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="f4f67-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4f67-164">Response</span></span>
<span data-ttu-id="f4f67-165">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4f67-165">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f67-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4f67-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f67-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f67-167">Request</span></span>
<span data-ttu-id="f4f67-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4f67-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4f67-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4f67-169">Response</span></span>
<span data-ttu-id="f4f67-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4f67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






