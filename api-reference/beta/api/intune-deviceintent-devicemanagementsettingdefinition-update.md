---
title: Atualizar deviceManagementSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0931fe68689fdcb0c57531a74124dda46f84133c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724280"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="def50-103">Atualizar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="def50-103">Update deviceManagementSettingDefinition</span></span>

<span data-ttu-id="def50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="def50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="def50-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="def50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="def50-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="def50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def50-107">Atualiza as propriedades de um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="def50-107">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="def50-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="def50-108">Prerequisites</span></span>
<span data-ttu-id="def50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def50-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="def50-111">Permission type</span></span>|<span data-ttu-id="def50-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="def50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="def50-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="def50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="def50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="def50-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="def50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="def50-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def50-116">Not supported.</span></span>|
|<span data-ttu-id="def50-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="def50-117">Application</span></span>|<span data-ttu-id="def50-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def50-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="def50-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="def50-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="def50-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="def50-120">Request headers</span></span>
|<span data-ttu-id="def50-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="def50-121">Header</span></span>|<span data-ttu-id="def50-122">Valor</span><span class="sxs-lookup"><span data-stu-id="def50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="def50-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="def50-123">Authorization</span></span>|<span data-ttu-id="def50-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="def50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="def50-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="def50-125">Accept</span></span>|<span data-ttu-id="def50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="def50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="def50-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="def50-127">Request body</span></span>
<span data-ttu-id="def50-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="def50-128">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="def50-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="def50-129">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="def50-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="def50-130">Property</span></span>|<span data-ttu-id="def50-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="def50-131">Type</span></span>|<span data-ttu-id="def50-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="def50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def50-133">id</span><span class="sxs-lookup"><span data-stu-id="def50-133">id</span></span>|<span data-ttu-id="def50-134">String</span><span class="sxs-lookup"><span data-stu-id="def50-134">String</span></span>|<span data-ttu-id="def50-135">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="def50-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="def50-136">valueType</span><span class="sxs-lookup"><span data-stu-id="def50-136">valueType</span></span>|[<span data-ttu-id="def50-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="def50-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="def50-138">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="def50-138">The data type of the value.</span></span> <span data-ttu-id="def50-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="def50-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="def50-140">displayName</span><span class="sxs-lookup"><span data-stu-id="def50-140">displayName</span></span>|<span data-ttu-id="def50-141">String</span><span class="sxs-lookup"><span data-stu-id="def50-141">String</span></span>|<span data-ttu-id="def50-142">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="def50-142">The setting's display name</span></span>|
|<span data-ttu-id="def50-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="def50-143">isTopLevel</span></span>|<span data-ttu-id="def50-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="def50-144">Boolean</span></span>|<span data-ttu-id="def50-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="def50-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="def50-146">description</span><span class="sxs-lookup"><span data-stu-id="def50-146">description</span></span>|<span data-ttu-id="def50-147">String</span><span class="sxs-lookup"><span data-stu-id="def50-147">String</span></span>|<span data-ttu-id="def50-148">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="def50-148">The setting's description</span></span>|
|<span data-ttu-id="def50-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="def50-149">placeholderText</span></span>|<span data-ttu-id="def50-150">String</span><span class="sxs-lookup"><span data-stu-id="def50-150">String</span></span>|<span data-ttu-id="def50-151">Texto do espaço reservado como um exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="def50-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="def50-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="def50-152">documentationUrl</span></span>|<span data-ttu-id="def50-153">String</span><span class="sxs-lookup"><span data-stu-id="def50-153">String</span></span>|<span data-ttu-id="def50-154">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="def50-154">Url to setting documentation</span></span>|
|<span data-ttu-id="def50-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="def50-155">headerTitle</span></span>|<span data-ttu-id="def50-156">String</span><span class="sxs-lookup"><span data-stu-id="def50-156">String</span></span>|<span data-ttu-id="def50-157">título do cabeçalho da configuração representa uma categoria/seção de uma configuração/configurações</span><span class="sxs-lookup"><span data-stu-id="def50-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="def50-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="def50-158">headerSubtitle</span></span>|<span data-ttu-id="def50-159">String</span><span class="sxs-lookup"><span data-stu-id="def50-159">String</span></span>|<span data-ttu-id="def50-160">subtítulo do cabeçalho da configuração para obter mais detalhes sobre a categoria/seção</span><span class="sxs-lookup"><span data-stu-id="def50-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="def50-161">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="def50-161">keywords</span></span>|<span data-ttu-id="def50-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="def50-162">String collection</span></span>|<span data-ttu-id="def50-163">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="def50-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="def50-164">as</span><span class="sxs-lookup"><span data-stu-id="def50-164">constraints</span></span>|<span data-ttu-id="def50-165">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="def50-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="def50-166">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="def50-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="def50-167">relação</span><span class="sxs-lookup"><span data-stu-id="def50-167">dependencies</span></span>|<span data-ttu-id="def50-168">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="def50-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="def50-169">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="def50-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="def50-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="def50-170">Response</span></span>
<span data-ttu-id="def50-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="def50-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="def50-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="def50-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="def50-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="def50-173">Request</span></span>
<span data-ttu-id="def50-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="def50-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="def50-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="def50-175">Response</span></span>
<span data-ttu-id="def50-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="def50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





