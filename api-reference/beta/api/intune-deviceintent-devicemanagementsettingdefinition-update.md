---
title: Atualizar deviceManagementSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementSettingDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f1b0540aa1696459c70783b5c31788276e71558
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771485"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="abe30-103">Atualizar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="abe30-103">Update deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="abe30-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abe30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abe30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abe30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abe30-106">Atualiza as propriedades de um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="abe30-106">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abe30-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abe30-107">Prerequisites</span></span>
<span data-ttu-id="abe30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abe30-110">Permission type</span></span>|<span data-ttu-id="abe30-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abe30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abe30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abe30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abe30-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abe30-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abe30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abe30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abe30-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abe30-115">Not supported.</span></span>|
|<span data-ttu-id="abe30-116">Application</span><span class="sxs-lookup"><span data-stu-id="abe30-116">Application</span></span>|<span data-ttu-id="abe30-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abe30-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abe30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abe30-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="abe30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abe30-119">Request headers</span></span>
|<span data-ttu-id="abe30-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abe30-120">Header</span></span>|<span data-ttu-id="abe30-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abe30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abe30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abe30-122">Authorization</span></span>|<span data-ttu-id="abe30-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abe30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abe30-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abe30-124">Accept</span></span>|<span data-ttu-id="abe30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abe30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abe30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abe30-126">Request body</span></span>
<span data-ttu-id="abe30-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="abe30-127">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="abe30-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="abe30-128">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="abe30-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abe30-129">Property</span></span>|<span data-ttu-id="abe30-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abe30-130">Type</span></span>|<span data-ttu-id="abe30-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abe30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abe30-132">id</span><span class="sxs-lookup"><span data-stu-id="abe30-132">id</span></span>|<span data-ttu-id="abe30-133">String</span><span class="sxs-lookup"><span data-stu-id="abe30-133">String</span></span>|<span data-ttu-id="abe30-134">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="abe30-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="abe30-135">valueType</span><span class="sxs-lookup"><span data-stu-id="abe30-135">valueType</span></span>|[<span data-ttu-id="abe30-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="abe30-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="abe30-137">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="abe30-137">The data type of the value.</span></span> <span data-ttu-id="abe30-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="abe30-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="abe30-139">displayName</span><span class="sxs-lookup"><span data-stu-id="abe30-139">displayName</span></span>|<span data-ttu-id="abe30-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abe30-140">String</span></span>|<span data-ttu-id="abe30-141">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="abe30-141">The setting's display name</span></span>|
|<span data-ttu-id="abe30-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="abe30-142">isTopLevel</span></span>|<span data-ttu-id="abe30-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="abe30-143">Boolean</span></span>|<span data-ttu-id="abe30-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="abe30-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="abe30-145">description</span><span class="sxs-lookup"><span data-stu-id="abe30-145">description</span></span>|<span data-ttu-id="abe30-146">String</span><span class="sxs-lookup"><span data-stu-id="abe30-146">String</span></span>|<span data-ttu-id="abe30-147">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="abe30-147">The setting's description</span></span>|
|<span data-ttu-id="abe30-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="abe30-148">placeholderText</span></span>|<span data-ttu-id="abe30-149">String</span><span class="sxs-lookup"><span data-stu-id="abe30-149">String</span></span>|<span data-ttu-id="abe30-150">Texto do espaço reservado como um exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="abe30-150">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="abe30-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="abe30-151">documentationUrl</span></span>|<span data-ttu-id="abe30-152">String</span><span class="sxs-lookup"><span data-stu-id="abe30-152">String</span></span>|<span data-ttu-id="abe30-153">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="abe30-153">Url to setting documentation</span></span>|
|<span data-ttu-id="abe30-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="abe30-154">keywords</span></span>|<span data-ttu-id="abe30-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abe30-155">String collection</span></span>|<span data-ttu-id="abe30-156">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="abe30-156">Keywords associated with the setting</span></span>|
|<span data-ttu-id="abe30-157">as</span><span class="sxs-lookup"><span data-stu-id="abe30-157">constraints</span></span>|<span data-ttu-id="abe30-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="abe30-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="abe30-159">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="abe30-159">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="abe30-160">relação</span><span class="sxs-lookup"><span data-stu-id="abe30-160">dependencies</span></span>|<span data-ttu-id="abe30-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="abe30-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="abe30-162">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="abe30-162">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="abe30-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe30-163">Response</span></span>
<span data-ttu-id="abe30-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abe30-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abe30-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abe30-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="abe30-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abe30-166">Request</span></span>
<span data-ttu-id="abe30-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abe30-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="abe30-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="abe30-168">Response</span></span>
<span data-ttu-id="abe30-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abe30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




