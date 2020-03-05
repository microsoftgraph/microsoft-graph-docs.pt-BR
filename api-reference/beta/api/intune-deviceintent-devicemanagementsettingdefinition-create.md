---
title: Criar deviceManagementSettingDefinition
description: Criar um novo objeto deviceManagementSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cae21343cde9fcb248d81d4e7a80764ed017a23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470613"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="d6c8e-103">Criar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="d6c8e-103">Create deviceManagementSettingDefinition</span></span>

<span data-ttu-id="d6c8e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6c8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6c8e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6c8e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c8e-107">Criar um novo objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c8e-107">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6c8e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6c8e-108">Prerequisites</span></span>
<span data-ttu-id="d6c8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6c8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c8e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6c8e-111">Permission type</span></span>|<span data-ttu-id="d6c8e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6c8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c8e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6c8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c8e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c8e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6c8e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6c8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c8e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-116">Not supported.</span></span>|
|<span data-ttu-id="d6c8e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6c8e-117">Application</span></span>|<span data-ttu-id="d6c8e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c8e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c8e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c8e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d6c8e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c8e-120">Request headers</span></span>
|<span data-ttu-id="d6c8e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6c8e-121">Header</span></span>|<span data-ttu-id="d6c8e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6c8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6c8e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6c8e-123">Authorization</span></span>|<span data-ttu-id="d6c8e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6c8e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6c8e-125">Accept</span></span>|<span data-ttu-id="d6c8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c8e-127">Request body</span></span>
<span data-ttu-id="d6c8e-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-128">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="d6c8e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-129">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="d6c8e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6c8e-130">Property</span></span>|<span data-ttu-id="d6c8e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6c8e-131">Type</span></span>|<span data-ttu-id="d6c8e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6c8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c8e-133">id</span><span class="sxs-lookup"><span data-stu-id="d6c8e-133">id</span></span>|<span data-ttu-id="d6c8e-134">String</span><span class="sxs-lookup"><span data-stu-id="d6c8e-134">String</span></span>|<span data-ttu-id="d6c8e-135">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="d6c8e-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="d6c8e-136">valueType</span><span class="sxs-lookup"><span data-stu-id="d6c8e-136">valueType</span></span>|[<span data-ttu-id="d6c8e-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="d6c8e-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="d6c8e-138">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-138">The data type of the value.</span></span> <span data-ttu-id="d6c8e-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="d6c8e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d6c8e-140">displayName</span></span>|<span data-ttu-id="d6c8e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6c8e-141">String</span></span>|<span data-ttu-id="d6c8e-142">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="d6c8e-142">The setting's display name</span></span>|
|<span data-ttu-id="d6c8e-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="d6c8e-143">isTopLevel</span></span>|<span data-ttu-id="d6c8e-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6c8e-144">Boolean</span></span>|<span data-ttu-id="d6c8e-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="d6c8e-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="d6c8e-146">description</span><span class="sxs-lookup"><span data-stu-id="d6c8e-146">description</span></span>|<span data-ttu-id="d6c8e-147">String</span><span class="sxs-lookup"><span data-stu-id="d6c8e-147">String</span></span>|<span data-ttu-id="d6c8e-148">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="d6c8e-148">The setting's description</span></span>|
|<span data-ttu-id="d6c8e-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="d6c8e-149">placeholderText</span></span>|<span data-ttu-id="d6c8e-150">String</span><span class="sxs-lookup"><span data-stu-id="d6c8e-150">String</span></span>|<span data-ttu-id="d6c8e-151">Texto do espaço reservado como um exemplo de entrada válida</span><span class="sxs-lookup"><span data-stu-id="d6c8e-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="d6c8e-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="d6c8e-152">documentationUrl</span></span>|<span data-ttu-id="d6c8e-153">String</span><span class="sxs-lookup"><span data-stu-id="d6c8e-153">String</span></span>|<span data-ttu-id="d6c8e-154">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="d6c8e-154">Url to setting documentation</span></span>|
|<span data-ttu-id="d6c8e-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="d6c8e-155">keywords</span></span>|<span data-ttu-id="d6c8e-156">String collection</span><span class="sxs-lookup"><span data-stu-id="d6c8e-156">String collection</span></span>|<span data-ttu-id="d6c8e-157">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="d6c8e-157">Keywords associated with the setting</span></span>|
|<span data-ttu-id="d6c8e-158">as</span><span class="sxs-lookup"><span data-stu-id="d6c8e-158">constraints</span></span>|<span data-ttu-id="d6c8e-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d6c8e-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="d6c8e-160">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="d6c8e-160">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="d6c8e-161">relação</span><span class="sxs-lookup"><span data-stu-id="d6c8e-161">dependencies</span></span>|<span data-ttu-id="d6c8e-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="d6c8e-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="d6c8e-163">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="d6c8e-163">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="d6c8e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6c8e-164">Response</span></span>
<span data-ttu-id="d6c8e-165">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-165">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6c8e-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6c8e-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6c8e-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c8e-167">Request</span></span>
<span data-ttu-id="d6c8e-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6c8e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6c8e-169">Response</span></span>
<span data-ttu-id="d6c8e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6c8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





