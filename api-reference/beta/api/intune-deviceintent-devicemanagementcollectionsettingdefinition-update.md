---
title: Atualizar deviceManagementCollectionSettingDefinition
description: Atualiza as propriedades de um objeto deviceManagementCollectionSettingDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4240dd4f9b1d26aff07aebd46fb9a9376c6e98e7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730652"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="b356f-103">Atualizar deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="b356f-103">Update deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="b356f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b356f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b356f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b356f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b356f-106">Atualiza as propriedades de um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b356f-106">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b356f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b356f-107">Prerequisites</span></span>
<span data-ttu-id="b356f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b356f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b356f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b356f-110">Permission type</span></span>|<span data-ttu-id="b356f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b356f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b356f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b356f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b356f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b356f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b356f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b356f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b356f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b356f-115">Not supported.</span></span>|
|<span data-ttu-id="b356f-116">Application</span><span class="sxs-lookup"><span data-stu-id="b356f-116">Application</span></span>|<span data-ttu-id="b356f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b356f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b356f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b356f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b356f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b356f-119">Request headers</span></span>
|<span data-ttu-id="b356f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b356f-120">Header</span></span>|<span data-ttu-id="b356f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b356f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b356f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b356f-122">Authorization</span></span>|<span data-ttu-id="b356f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b356f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b356f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b356f-124">Accept</span></span>|<span data-ttu-id="b356f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b356f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b356f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b356f-126">Request body</span></span>
<span data-ttu-id="b356f-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b356f-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="b356f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b356f-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="b356f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b356f-129">Property</span></span>|<span data-ttu-id="b356f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b356f-130">Type</span></span>|<span data-ttu-id="b356f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b356f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b356f-132">id</span><span class="sxs-lookup"><span data-stu-id="b356f-132">id</span></span>|<span data-ttu-id="b356f-133">String</span><span class="sxs-lookup"><span data-stu-id="b356f-133">String</span></span>|<span data-ttu-id="b356f-134">A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-135">valueType</span><span class="sxs-lookup"><span data-stu-id="b356f-135">valueType</span></span>|[<span data-ttu-id="b356f-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="b356f-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="b356f-137">O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b356f-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="b356f-138">Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="b356f-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="b356f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b356f-139">displayName</span></span>|<span data-ttu-id="b356f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b356f-140">String</span></span>|<span data-ttu-id="b356f-141">O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="b356f-142">isTopLevel</span></span>|<span data-ttu-id="b356f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b356f-143">Boolean</span></span>|<span data-ttu-id="b356f-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-145">description</span><span class="sxs-lookup"><span data-stu-id="b356f-145">description</span></span>|<span data-ttu-id="b356f-146">String</span><span class="sxs-lookup"><span data-stu-id="b356f-146">String</span></span>|<span data-ttu-id="b356f-147">A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-148">placeholderText</span><span class="sxs-lookup"><span data-stu-id="b356f-148">placeholderText</span></span>|<span data-ttu-id="b356f-149">String</span><span class="sxs-lookup"><span data-stu-id="b356f-149">String</span></span>|<span data-ttu-id="b356f-150">Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-150">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-151">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="b356f-151">documentationUrl</span></span>|<span data-ttu-id="b356f-152">String</span><span class="sxs-lookup"><span data-stu-id="b356f-152">String</span></span>|<span data-ttu-id="b356f-153">URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-153">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-154">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="b356f-154">keywords</span></span>|<span data-ttu-id="b356f-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b356f-155">String collection</span></span>|<span data-ttu-id="b356f-156">Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-156">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-157">as</span><span class="sxs-lookup"><span data-stu-id="b356f-157">constraints</span></span>|<span data-ttu-id="b356f-158">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-158">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="b356f-159">Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-159">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-160">relação</span><span class="sxs-lookup"><span data-stu-id="b356f-160">dependencies</span></span>|<span data-ttu-id="b356f-161">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-161">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="b356f-162">Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b356f-162">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="b356f-163">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b356f-163">elementDefinitionId</span></span>|<span data-ttu-id="b356f-164">String</span><span class="sxs-lookup"><span data-stu-id="b356f-164">String</span></span>|<span data-ttu-id="b356f-165">A ID de definição de configuração que descreve a aparência de cada elemento da coleção</span><span class="sxs-lookup"><span data-stu-id="b356f-165">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="b356f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b356f-166">Response</span></span>
<span data-ttu-id="b356f-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b356f-167">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b356f-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b356f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b356f-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b356f-169">Request</span></span>
<span data-ttu-id="b356f-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b356f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b356f-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b356f-171">Response</span></span>
<span data-ttu-id="b356f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b356f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




