---
title: Criar deviceManagementCollectionSettingDefinition
description: Criar um novo objeto deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 623b0678ad1f3f4653d542fb7553e53168b19cb5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306307"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="0aecb-103">Criar deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="0aecb-103">Create deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="0aecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aecb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aecb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0aecb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aecb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0aecb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aecb-107">Criar um novo objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0aecb-107">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aecb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0aecb-108">Prerequisites</span></span>
<span data-ttu-id="0aecb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aecb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aecb-111">Permission type</span></span>|<span data-ttu-id="0aecb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0aecb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aecb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aecb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0aecb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aecb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0aecb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aecb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aecb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aecb-116">Not supported.</span></span>|
|<span data-ttu-id="0aecb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0aecb-117">Application</span></span>|<span data-ttu-id="0aecb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aecb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aecb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aecb-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0aecb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aecb-120">Request headers</span></span>
|<span data-ttu-id="0aecb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0aecb-121">Header</span></span>|<span data-ttu-id="0aecb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0aecb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aecb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aecb-123">Authorization</span></span>|<span data-ttu-id="0aecb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aecb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aecb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0aecb-125">Accept</span></span>|<span data-ttu-id="0aecb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0aecb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aecb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aecb-127">Request body</span></span>
<span data-ttu-id="0aecb-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementCollectionSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="0aecb-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="0aecb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementCollectionSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="0aecb-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="0aecb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0aecb-130">Property</span></span>|<span data-ttu-id="0aecb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0aecb-131">Type</span></span>|<span data-ttu-id="0aecb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0aecb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aecb-133">id</span><span class="sxs-lookup"><span data-stu-id="0aecb-133">id</span></span>|<span data-ttu-id="0aecb-134">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-134">String</span></span>|<span data-ttu-id="0aecb-135">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-136">valueType</span><span class="sxs-lookup"><span data-stu-id="0aecb-136">valueType</span></span>|[<span data-ttu-id="0aecb-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="0aecb-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="0aecb-138">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0aecb-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="0aecb-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="0aecb-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="0aecb-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0aecb-140">displayName</span></span>|<span data-ttu-id="0aecb-141">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-141">String</span></span>|<span data-ttu-id="0aecb-142">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="0aecb-143">isTopLevel</span></span>|<span data-ttu-id="0aecb-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="0aecb-144">Boolean</span></span>|<span data-ttu-id="0aecb-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-146">description</span><span class="sxs-lookup"><span data-stu-id="0aecb-146">description</span></span>|<span data-ttu-id="0aecb-147">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-147">String</span></span>|<span data-ttu-id="0aecb-148">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="0aecb-149">placeholderText</span></span>|<span data-ttu-id="0aecb-150">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-150">String</span></span>|<span data-ttu-id="0aecb-151">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="0aecb-152">documentationUrl</span></span>|<span data-ttu-id="0aecb-153">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-153">String</span></span>|<span data-ttu-id="0aecb-154">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="0aecb-155">headerTitle</span></span>|<span data-ttu-id="0aecb-156">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-156">String</span></span>|<span data-ttu-id="0aecb-157">título do cabeçalho da configuração representa uma categoria/seção de uma configuração/definições herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="0aecb-158">headerSubtitle</span></span>|<span data-ttu-id="0aecb-159">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-159">String</span></span>|<span data-ttu-id="0aecb-160">subtítulo do cabeçalho da configuração para obter mais detalhes sobre a categoria/seção herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-161">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="0aecb-161">keywords</span></span>|<span data-ttu-id="0aecb-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aecb-162">String collection</span></span>|<span data-ttu-id="0aecb-163">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-164">as</span><span class="sxs-lookup"><span data-stu-id="0aecb-164">constraints</span></span>|<span data-ttu-id="0aecb-165">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="0aecb-166">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-167">relação</span><span class="sxs-lookup"><span data-stu-id="0aecb-167">dependencies</span></span>|<span data-ttu-id="0aecb-168">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="0aecb-169">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0aecb-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="0aecb-170">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0aecb-170">elementDefinitionId</span></span>|<span data-ttu-id="0aecb-171">String</span><span class="sxs-lookup"><span data-stu-id="0aecb-171">String</span></span>|<span data-ttu-id="0aecb-172">A ID de definição de configuração que descreve a aparência de cada elemento da coleção</span><span class="sxs-lookup"><span data-stu-id="0aecb-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="0aecb-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aecb-173">Response</span></span>
<span data-ttu-id="0aecb-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aecb-174">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aecb-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aecb-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aecb-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aecb-176">Request</span></span>
<span data-ttu-id="0aecb-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aecb-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="0aecb-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aecb-178">Response</span></span>
<span data-ttu-id="0aecb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0aecb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




