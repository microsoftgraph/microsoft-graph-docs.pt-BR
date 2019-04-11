---
title: Criar deviceManagementSettingDefinition
description: Criar um novo objeto deviceManagementSettingDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66dc71a6e95f9838788a0aac22341a5a3881a5e9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803448"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="442a9-103">Criar deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="442a9-103">Create deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="442a9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="442a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="442a9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="442a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="442a9-106">Criar um novo objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="442a9-106">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="442a9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="442a9-107">Prerequisites</span></span>
<span data-ttu-id="442a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="442a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="442a9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="442a9-110">Permission type</span></span>|<span data-ttu-id="442a9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="442a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="442a9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="442a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="442a9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="442a9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="442a9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="442a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="442a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="442a9-115">Not supported.</span></span>|
|<span data-ttu-id="442a9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="442a9-116">Application</span></span>|<span data-ttu-id="442a9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="442a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="442a9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="442a9-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="442a9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="442a9-119">Request headers</span></span>
|<span data-ttu-id="442a9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="442a9-120">Header</span></span>|<span data-ttu-id="442a9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="442a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="442a9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="442a9-122">Authorization</span></span>|<span data-ttu-id="442a9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="442a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="442a9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="442a9-124">Accept</span></span>|<span data-ttu-id="442a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="442a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="442a9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="442a9-126">Request body</span></span>
<span data-ttu-id="442a9-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="442a9-127">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="442a9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="442a9-128">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="442a9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="442a9-129">Property</span></span>|<span data-ttu-id="442a9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="442a9-130">Type</span></span>|<span data-ttu-id="442a9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="442a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="442a9-132">id</span><span class="sxs-lookup"><span data-stu-id="442a9-132">id</span></span>|<span data-ttu-id="442a9-133">String</span><span class="sxs-lookup"><span data-stu-id="442a9-133">String</span></span>|<span data-ttu-id="442a9-134">A ID da definição de configuração</span><span class="sxs-lookup"><span data-stu-id="442a9-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="442a9-135">valueType</span><span class="sxs-lookup"><span data-stu-id="442a9-135">valueType</span></span>|[<span data-ttu-id="442a9-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="442a9-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="442a9-137">O tipo de dados do valor.</span><span class="sxs-lookup"><span data-stu-id="442a9-137">The data type of the value.</span></span> <span data-ttu-id="442a9-138">Os valores possíveis são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span><span class="sxs-lookup"><span data-stu-id="442a9-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="442a9-139">displayName</span><span class="sxs-lookup"><span data-stu-id="442a9-139">displayName</span></span>|<span data-ttu-id="442a9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="442a9-140">String</span></span>|<span data-ttu-id="442a9-141">O nome de exibição da configuração</span><span class="sxs-lookup"><span data-stu-id="442a9-141">The setting's display name</span></span>|
|<span data-ttu-id="442a9-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="442a9-142">isTopLevel</span></span>|<span data-ttu-id="442a9-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="442a9-143">Boolean</span></span>|<span data-ttu-id="442a9-144">Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa</span><span class="sxs-lookup"><span data-stu-id="442a9-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="442a9-145">description</span><span class="sxs-lookup"><span data-stu-id="442a9-145">description</span></span>|<span data-ttu-id="442a9-146">String</span><span class="sxs-lookup"><span data-stu-id="442a9-146">String</span></span>|<span data-ttu-id="442a9-147">A descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="442a9-147">The setting's description</span></span>|
|<span data-ttu-id="442a9-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="442a9-148">documentationUrl</span></span>|<span data-ttu-id="442a9-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="442a9-149">String</span></span>|<span data-ttu-id="442a9-150">URL para configurar a documentação</span><span class="sxs-lookup"><span data-stu-id="442a9-150">Url to setting documentation</span></span>|
|<span data-ttu-id="442a9-151">palavras-chave</span><span class="sxs-lookup"><span data-stu-id="442a9-151">keywords</span></span>|<span data-ttu-id="442a9-152">Coleção String</span><span class="sxs-lookup"><span data-stu-id="442a9-152">String collection</span></span>|<span data-ttu-id="442a9-153">Palavras-chave associadas à configuração</span><span class="sxs-lookup"><span data-stu-id="442a9-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="442a9-154">as</span><span class="sxs-lookup"><span data-stu-id="442a9-154">constraints</span></span>|<span data-ttu-id="442a9-155">coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="442a9-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="442a9-156">Conjunto de restrições para o valor de configuração</span><span class="sxs-lookup"><span data-stu-id="442a9-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="442a9-157">relação</span><span class="sxs-lookup"><span data-stu-id="442a9-157">dependencies</span></span>|<span data-ttu-id="442a9-158">coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)</span><span class="sxs-lookup"><span data-stu-id="442a9-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="442a9-159">Coleção de dependências em outras configurações</span><span class="sxs-lookup"><span data-stu-id="442a9-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="442a9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="442a9-160">Response</span></span>
<span data-ttu-id="442a9-161">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="442a9-161">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="442a9-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="442a9-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="442a9-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="442a9-163">Request</span></span>
<span data-ttu-id="442a9-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="442a9-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="442a9-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="442a9-165">Response</span></span>
<span data-ttu-id="442a9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="442a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```





