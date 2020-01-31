---
title: Atualizar deviceManagementCollectionSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementCollectionSettingDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3417eaa470b181e0ba1b77f87c3048232e0ae4c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636431"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="b7999-103">Atualizar deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="b7999-103">Update deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="b7999-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7999-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7999-106">Atualiza as propriedades de um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b7999-106">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7999-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7999-107">Prerequisites</span></span>
<span data-ttu-id="b7999-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7999-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7999-110">Permission type</span></span>|<span data-ttu-id="b7999-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7999-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7999-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7999-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7999-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7999-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7999-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7999-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7999-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7999-115">Not supported.</span></span>|
|<span data-ttu-id="b7999-116">Application</span><span class="sxs-lookup"><span data-stu-id="b7999-116">Application</span></span>|<span data-ttu-id="b7999-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7999-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7999-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7999-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b7999-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7999-119">Request headers</span></span>
|<span data-ttu-id="b7999-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7999-120">Header</span></span>|<span data-ttu-id="b7999-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7999-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7999-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7999-122">Authorization</span></span>|<span data-ttu-id="b7999-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7999-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7999-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7999-124">Accept</span></span>|<span data-ttu-id="b7999-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7999-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7999-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7999-126">Request body</span></span>
<span data-ttu-id="b7999-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b7999-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="b7999-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b7999-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="b7999-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7999-129">Property</span></span>|<span data-ttu-id="b7999-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7999-130">Type</span></span>|<span data-ttu-id="b7999-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7999-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7999-132">id</span><span class="sxs-lookup"><span data-stu-id="b7999-132">id</span></span>|<span data-ttu-id="b7999-133">String</span><span class="sxs-lookup"><span data-stu-id="b7999-133">String</span></span>|<span data-ttu-id="b7999-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-135">valueType</span><span class="sxs-lookup"><span data-stu-id="b7999-135">valueType</span></span>|[<span data-ttu-id="b7999-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="b7999-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="b7999-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b7999-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="b7999-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="b7999-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="b7999-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b7999-139">displayName</span></span>|<span data-ttu-id="b7999-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7999-140">String</span></span>|<span data-ttu-id="b7999-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="b7999-142">isTopLevel</span></span>|<span data-ttu-id="b7999-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7999-143">Boolean</span></span>|<span data-ttu-id="b7999-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-145">description</span><span class="sxs-lookup"><span data-stu-id="b7999-145">description</span></span>|<span data-ttu-id="b7999-146">String</span><span class="sxs-lookup"><span data-stu-id="b7999-146">String</span></span>|<span data-ttu-id="b7999-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="b7999-148">placeholderText</span></span>|<span data-ttu-id="b7999-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7999-149">String</span></span>|<span data-ttu-id="b7999-150">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="b7999-151">documentationUrl</span></span>|<span data-ttu-id="b7999-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7999-152">String</span></span>|<span data-ttu-id="b7999-153">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="b7999-154">keywords</span></span>|<span data-ttu-id="b7999-155">String collection</span><span class="sxs-lookup"><span data-stu-id="b7999-155">String collection</span></span>|<span data-ttu-id="b7999-156">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-157">as</span><span class="sxs-lookup"><span data-stu-id="b7999-157">constraints</span></span>|<span data-ttu-id="b7999-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="b7999-159">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-160">relação</span><span class="sxs-lookup"><span data-stu-id="b7999-160">dependencies</span></span>|<span data-ttu-id="b7999-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="b7999-162">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b7999-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b7999-163">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7999-163">elementDefinitionId</span></span>|<span data-ttu-id="b7999-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7999-164">String</span></span>|<span data-ttu-id="b7999-165">A ID de definição de configuração que descreve a aparência de cada elemento da coleção</span><span class="sxs-lookup"><span data-stu-id="b7999-165">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="b7999-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7999-166">Response</span></span>
<span data-ttu-id="b7999-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7999-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7999-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7999-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7999-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7999-169">Request</span></span>
<span data-ttu-id="b7999-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7999-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7999-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7999-171">Response</span></span>
<span data-ttu-id="b7999-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7999-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





