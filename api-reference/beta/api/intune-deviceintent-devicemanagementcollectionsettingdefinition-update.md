---
title: Atualizar deviceManagementCollectionSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementCollectionSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32f9c7b1f6c56c2b1e53393019a935220ba03051
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000767"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="14d39-103">Atualizar deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="14d39-103">Update deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="14d39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14d39-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14d39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14d39-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14d39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14d39-107">Atualiza as propriedades de um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="14d39-107">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14d39-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14d39-108">Prerequisites</span></span>
<span data-ttu-id="14d39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d39-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14d39-111">Permission type</span></span>|<span data-ttu-id="14d39-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14d39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14d39-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14d39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14d39-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d39-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14d39-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14d39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14d39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14d39-116">Not supported.</span></span>|
|<span data-ttu-id="14d39-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14d39-117">Application</span></span>|<span data-ttu-id="14d39-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d39-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14d39-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14d39-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="14d39-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14d39-120">Request headers</span></span>
|<span data-ttu-id="14d39-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14d39-121">Header</span></span>|<span data-ttu-id="14d39-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14d39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14d39-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14d39-123">Authorization</span></span>|<span data-ttu-id="14d39-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14d39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14d39-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14d39-125">Accept</span></span>|<span data-ttu-id="14d39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14d39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14d39-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14d39-127">Request body</span></span>
<span data-ttu-id="14d39-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="14d39-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="14d39-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="14d39-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="14d39-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14d39-130">Property</span></span>|<span data-ttu-id="14d39-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="14d39-131">Type</span></span>|<span data-ttu-id="14d39-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d39-133">id</span><span class="sxs-lookup"><span data-stu-id="14d39-133">id</span></span>|<span data-ttu-id="14d39-134">String</span><span class="sxs-lookup"><span data-stu-id="14d39-134">String</span></span>|<span data-ttu-id="14d39-135">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-136">valueType</span><span class="sxs-lookup"><span data-stu-id="14d39-136">valueType</span></span>|[<span data-ttu-id="14d39-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="14d39-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="14d39-138">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="14d39-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="14d39-139">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="14d39-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="14d39-140">displayName</span><span class="sxs-lookup"><span data-stu-id="14d39-140">displayName</span></span>|<span data-ttu-id="14d39-141">String</span><span class="sxs-lookup"><span data-stu-id="14d39-141">String</span></span>|<span data-ttu-id="14d39-142">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="14d39-143">isTopLevel</span></span>|<span data-ttu-id="14d39-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="14d39-144">Boolean</span></span>|<span data-ttu-id="14d39-145">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-146">description</span><span class="sxs-lookup"><span data-stu-id="14d39-146">description</span></span>|<span data-ttu-id="14d39-147">String</span><span class="sxs-lookup"><span data-stu-id="14d39-147">String</span></span>|<span data-ttu-id="14d39-148">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="14d39-149">placeholderText</span></span>|<span data-ttu-id="14d39-150">String</span><span class="sxs-lookup"><span data-stu-id="14d39-150">String</span></span>|<span data-ttu-id="14d39-151">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="14d39-152">documentationUrl</span></span>|<span data-ttu-id="14d39-153">String</span><span class="sxs-lookup"><span data-stu-id="14d39-153">String</span></span>|<span data-ttu-id="14d39-154">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-155">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="14d39-155">keywords</span></span>|<span data-ttu-id="14d39-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14d39-156">String collection</span></span>|<span data-ttu-id="14d39-157">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-158">as</span><span class="sxs-lookup"><span data-stu-id="14d39-158">constraints</span></span>|<span data-ttu-id="14d39-159">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="14d39-160">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-161">relação</span><span class="sxs-lookup"><span data-stu-id="14d39-161">dependencies</span></span>|<span data-ttu-id="14d39-162">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="14d39-163">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14d39-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="14d39-164">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="14d39-164">elementDefinitionId</span></span>|<span data-ttu-id="14d39-165">String</span><span class="sxs-lookup"><span data-stu-id="14d39-165">String</span></span>|<span data-ttu-id="14d39-166">A ID de definição de configuração que descreve a aparência de cada elemento da coleção</span><span class="sxs-lookup"><span data-stu-id="14d39-166">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="14d39-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="14d39-167">Response</span></span>
<span data-ttu-id="14d39-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14d39-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d39-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14d39-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="14d39-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14d39-170">Request</span></span>
<span data-ttu-id="14d39-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14d39-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 995

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="14d39-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="14d39-172">Response</span></span>
<span data-ttu-id="14d39-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14d39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1044

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```






