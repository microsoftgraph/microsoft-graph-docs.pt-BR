---
title: Atualizar deviceManagementCollectionSettingDefinition
description: Atualize as propriedades de um objeto deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bfd9fc6e84ba6c11d6941e87a7acac9237c3562
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132125"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="77fc4-103">Atualizar deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="77fc4-103">Update deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="77fc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77fc4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77fc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77fc4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77fc4-107">Atualize as propriedades de [um objeto deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-107">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77fc4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77fc4-108">Prerequisites</span></span>
<span data-ttu-id="77fc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77fc4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77fc4-111">Permission type</span></span>|<span data-ttu-id="77fc4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77fc4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77fc4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77fc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77fc4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77fc4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77fc4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77fc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77fc4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77fc4-116">Not supported.</span></span>|
|<span data-ttu-id="77fc4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77fc4-117">Application</span></span>|<span data-ttu-id="77fc4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77fc4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77fc4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77fc4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="77fc4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77fc4-120">Request headers</span></span>
|<span data-ttu-id="77fc4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77fc4-121">Header</span></span>|<span data-ttu-id="77fc4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77fc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77fc4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77fc4-123">Authorization</span></span>|<span data-ttu-id="77fc4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77fc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77fc4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77fc4-125">Accept</span></span>|<span data-ttu-id="77fc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77fc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77fc4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77fc4-127">Request body</span></span>
<span data-ttu-id="77fc4-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementCollectionSettingDefinition.](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="77fc4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="77fc4-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="77fc4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77fc4-130">Property</span></span>|<span data-ttu-id="77fc4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77fc4-131">Type</span></span>|<span data-ttu-id="77fc4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77fc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77fc4-133">id</span><span class="sxs-lookup"><span data-stu-id="77fc4-133">id</span></span>|<span data-ttu-id="77fc4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-134">String</span></span>|<span data-ttu-id="77fc4-135">A ID da definição de configuração Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-136">valueType</span><span class="sxs-lookup"><span data-stu-id="77fc4-136">valueType</span></span>|[<span data-ttu-id="77fc4-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="77fc4-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="77fc4-138">O tipo de dados do valor Herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="77fc4-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="77fc4-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="77fc4-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="77fc4-140">displayName</span><span class="sxs-lookup"><span data-stu-id="77fc4-140">displayName</span></span>|<span data-ttu-id="77fc4-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-141">String</span></span>|<span data-ttu-id="77fc4-142">Nome de exibição da configuração Herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="77fc4-143">isTopLevel</span></span>|<span data-ttu-id="77fc4-144">Booleano</span><span class="sxs-lookup"><span data-stu-id="77fc4-144">Boolean</span></span>|<span data-ttu-id="77fc4-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser empacotada em uma coleção ou configuração complexa Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-146">descrição</span><span class="sxs-lookup"><span data-stu-id="77fc4-146">description</span></span>|<span data-ttu-id="77fc4-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-147">String</span></span>|<span data-ttu-id="77fc4-148">Descrição da configuração Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="77fc4-149">placeholderText</span></span>|<span data-ttu-id="77fc4-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-150">String</span></span>|<span data-ttu-id="77fc4-151">Texto de espaço reservado como um exemplo de entrada válida Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="77fc4-152">documentationUrl</span></span>|<span data-ttu-id="77fc4-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-153">String</span></span>|<span data-ttu-id="77fc4-154">Url para a documentação de configuração Herdada [de deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="77fc4-155">headerTitle</span></span>|<span data-ttu-id="77fc4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-156">String</span></span>|<span data-ttu-id="77fc4-157">título do header de configuração representa uma categoria/seção de uma configuração/configurações Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="77fc4-158">headerSubtitle</span></span>|<span data-ttu-id="77fc4-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-159">String</span></span>|<span data-ttu-id="77fc4-160">subtítulo do header de configuração para obter mais detalhes sobre a categoria/seção Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-161">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="77fc4-161">keywords</span></span>|<span data-ttu-id="77fc4-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-162">String collection</span></span>|<span data-ttu-id="77fc4-163">Palavras-chave associadas à configuração Herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-164">restrições</span><span class="sxs-lookup"><span data-stu-id="77fc4-164">constraints</span></span>|<span data-ttu-id="77fc4-165">[Coleção deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="77fc4-166">Coleção de restrições para o valor de configuração Herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-167">dependencies</span><span class="sxs-lookup"><span data-stu-id="77fc4-167">dependencies</span></span>|<span data-ttu-id="77fc4-168">[Coleção deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="77fc4-169">Coleção de dependências em outras configurações Herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77fc4-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="77fc4-170">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="77fc4-170">elementDefinitionId</span></span>|<span data-ttu-id="77fc4-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77fc4-171">String</span></span>|<span data-ttu-id="77fc4-172">A ID de Definição de Definição que descreve a aparência de cada elemento da coleção</span><span class="sxs-lookup"><span data-stu-id="77fc4-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="77fc4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="77fc4-173">Response</span></span>
<span data-ttu-id="77fc4-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77fc4-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77fc4-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77fc4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="77fc4-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77fc4-176">Request</span></span>
<span data-ttu-id="77fc4-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77fc4-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1081

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="77fc4-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="77fc4-178">Response</span></span>
<span data-ttu-id="77fc4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77fc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```




