---
title: Criar deviceManagementSettingDefinition
description: Crie um novo objeto deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e93bd4424d4e09fb27528d719898067f192aa345
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154578"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="9655a-103">Criar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="9655a-103">Create deviceManagementSettingDefinition</span></span>

<span data-ttu-id="9655a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9655a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9655a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9655a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9655a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9655a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9655a-107">Crie um novo [objeto deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9655a-107">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9655a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9655a-108">Prerequisites</span></span>
<span data-ttu-id="9655a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9655a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9655a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9655a-111">Permission type</span></span>|<span data-ttu-id="9655a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9655a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9655a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9655a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9655a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9655a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9655a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9655a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9655a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9655a-116">Not supported.</span></span>|
|<span data-ttu-id="9655a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9655a-117">Application</span></span>|<span data-ttu-id="9655a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9655a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9655a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9655a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9655a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9655a-120">Request headers</span></span>
|<span data-ttu-id="9655a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9655a-121">Header</span></span>|<span data-ttu-id="9655a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9655a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9655a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9655a-123">Authorization</span></span>|<span data-ttu-id="9655a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9655a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9655a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9655a-125">Accept</span></span>|<span data-ttu-id="9655a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9655a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9655a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9655a-127">Request body</span></span>
<span data-ttu-id="9655a-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="9655a-128">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="9655a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="9655a-129">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="9655a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9655a-130">Property</span></span>|<span data-ttu-id="9655a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9655a-131">Type</span></span>|<span data-ttu-id="9655a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9655a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9655a-133">id</span><span class="sxs-lookup"><span data-stu-id="9655a-133">id</span></span>|<span data-ttu-id="9655a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-134">String</span></span>|<span data-ttu-id="9655a-135">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="9655a-136">valueType</span><span class="sxs-lookup"><span data-stu-id="9655a-136">valueType</span></span>|[<span data-ttu-id="9655a-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="9655a-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="9655a-138">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="9655a-138">The data type of the value.</span></span> <span data-ttu-id="9655a-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="9655a-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="9655a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9655a-140">displayName</span></span>|<span data-ttu-id="9655a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-141">String</span></span>|<span data-ttu-id="9655a-142">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-142">The setting's display name</span></span>|
|<span data-ttu-id="9655a-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="9655a-143">isTopLevel</span></span>|<span data-ttu-id="9655a-144">Booleano</span><span class="sxs-lookup"><span data-stu-id="9655a-144">Boolean</span></span>|<span data-ttu-id="9655a-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser empacotada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="9655a-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="9655a-146">descrição</span><span class="sxs-lookup"><span data-stu-id="9655a-146">description</span></span>|<span data-ttu-id="9655a-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-147">String</span></span>|<span data-ttu-id="9655a-148">Descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-148">The setting's description</span></span>|
|<span data-ttu-id="9655a-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="9655a-149">placeholderText</span></span>|<span data-ttu-id="9655a-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-150">String</span></span>|<span data-ttu-id="9655a-151">Texto de espaço reservado como exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="9655a-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="9655a-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="9655a-152">documentationUrl</span></span>|<span data-ttu-id="9655a-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-153">String</span></span>|<span data-ttu-id="9655a-154">Url para a documentação de configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-154">Url to setting documentation</span></span>|
|<span data-ttu-id="9655a-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="9655a-155">headerTitle</span></span>|<span data-ttu-id="9655a-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-156">String</span></span>|<span data-ttu-id="9655a-157">título do header de configuração representa uma categoria/seção de uma configuração/configurações</span><span class="sxs-lookup"><span data-stu-id="9655a-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="9655a-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="9655a-158">headerSubtitle</span></span>|<span data-ttu-id="9655a-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-159">String</span></span>|<span data-ttu-id="9655a-160">subtítulo do header de configuração para obter mais detalhes sobre a categoria/seção</span><span class="sxs-lookup"><span data-stu-id="9655a-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="9655a-161">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="9655a-161">keywords</span></span>|<span data-ttu-id="9655a-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9655a-162">String collection</span></span>|<span data-ttu-id="9655a-163">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="9655a-164">restrições</span><span class="sxs-lookup"><span data-stu-id="9655a-164">constraints</span></span>|<span data-ttu-id="9655a-165">[Coleção deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9655a-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="9655a-166">Coleção de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="9655a-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="9655a-167">dependencies</span><span class="sxs-lookup"><span data-stu-id="9655a-167">dependencies</span></span>|<span data-ttu-id="9655a-168">[Coleção deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="9655a-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="9655a-169">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="9655a-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="9655a-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="9655a-170">Response</span></span>
<span data-ttu-id="9655a-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9655a-171">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9655a-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9655a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9655a-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9655a-173">Request</span></span>
<span data-ttu-id="9655a-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9655a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1014

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
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

### <a name="response"></a><span data-ttu-id="9655a-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="9655a-175">Response</span></span>
<span data-ttu-id="9655a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9655a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1063

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
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




